# Comparing `tmp/djm8-0.1.0.tar.gz` & `tmp/djm8-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djm8-0.1.0.tar", max compression
+gzip compressed data, was "djm8-0.1.1.tar", max compression
```

## Comparing `djm8-0.1.0.tar` & `djm8-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-02 03:53:34.912071 djm8-0.1.0/m8project/djm8/__init__.py
--rw-r--r--   0        0        0     9680 2023-07-06 18:37:21.161942 djm8-0.1.0/m8project/djm8/routes.py
--rw-r--r--   0        0        0      453 2023-07-06 18:53:34.804154 djm8-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 djm8-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-02 03:53:34.912071 djm8-0.1.1/m8project/djm8/__init__.py
+-rw-r--r--   0        0        0     9560 2023-07-06 20:46:49.626861 djm8-0.1.1/m8project/djm8/routes.py
+-rw-r--r--   0        0        0      453 2023-07-06 20:47:15.499588 djm8-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 djm8-0.1.1/PKG-INFO
```

### Comparing `djm8-0.1.0/m8project/djm8/routes.py` & `djm8-0.1.1/m8project/djm8/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,20 @@
     "path",
     "uuid"
 )
 
 ThisRouteType = TypeVar("ThisRouteType", bound="Route")
 Self = TypeVar("Self", bound="Route")
 
+
 @frozen
 class RouteProtocol:
-    
+
     possible_view_methods: ClassVar[Sequence[str]] = (
-            "view", "get", "post", "put", "patch", "delete")
+        "view", "get", "post", "put", "patch", "delete")
 
     @staticmethod
     def snaky(name: str) -> str:
         """
         Turns camelCase and PascalCase names into snake_case name.
 
         - `snaky("camelCase")` -> `"camel_case"`
@@ -91,49 +92,49 @@
     @property
     def rproto(self) -> RouteProtocol | None:
         """
         Returns the parent route's protocol if it exists.
         Otherwise returns None.
         """
         return self.rroute.__proto__ if self.rroute else None
-    
+
     @property
     def is_last_root(self) -> bool:
         """Returns whether the route is the last root route."""
         return not self.rroute
 
     @property
     def children(self) -> Iterable[type[Route]]:
         """Iterates over the route's children routes."""
         return (c for c in self.route.__subclasses__() if issubclass(c, Route))
-    
+
     @property
     def attribute_annotations(self):
         if self.rroute:
             yield from self.rroute.__proto__.attribute_annotations
         yield from self.route.__annotations__.items()
 
     @property
     def url_parameters_patterns(self) -> Iterable[str]:
         """Iterates over the route's url parameters patterns."""
         return (f"<{converter}:{name}>"
                 for name, converter
                 in self.url_parameters)
-            
+
     @property
     def url_parameters(self) -> Iterable[tuple[str, str]]:
         """Iterates over the route's parameters and converters names."""
         # converter can be a type or a string (type's name)
         # depending on whether annotations are imported from __future__ or not
         # so we create a lookup of `Converter: name` and `Converter.__name__: name`
         converters = get_converters()
         converters_lookup = dict(chain(
             ((type(c), n) for n, c in converters.items()),
             ((type(c).__name__, n) for n, c in converters.items())))
-        
+
         for name, converter in self.route.__annotations__.items():
             if converter in converters:
                 yield (name, converter)
             elif getattr(converter, "__name__", None) in converters:
                 yield (name, converter.__name__)
             elif converter in converters_lookup:
                 yield (name, converters_lookup[converter])
@@ -144,101 +145,103 @@
 
     @property
     def url_patterns_parts(self) -> Iterable[str]:
         if self.rproto:
             yield from self.rproto.url_patterns_parts
             yield self.name
         yield from self.url_parameters_patterns
-        
+
     @property
     def url_parameters_parts(self) -> Iterable[str | tuple[str, str]]:
         if self.rproto:
             yield from self.rproto.url_parameters_parts
             yield self.name
         yield from self.url_parameters
-    
+
     @property
     def url(self) -> str:
         """Returns the route's absolute url."""
         return "/".join(self.url_patterns_parts)
 
     @property
     def absolute_name(self) -> str:
         return f"{self.rproto.absolute_name}.{self.name}" if self.rproto else self.name
 
-    async def view(self, request: HttpRequest, **parameters) -> HttpResponse | None:
+    def view(self, request: HttpRequest, **parameters) -> HttpResponse | None:
         """Returns the route's view."""
-        return await getattr(
+        return getattr(
             route := self.route(**parameters),
             (request.method or "get").lower(),
             getattr(route, "view"))(request)
-    
+
     @property
     def is_endpoint(self) -> bool:
         """Returns whether the route is an endpoint / has views."""
         return any(hasattr(self.route, name) for name in self.possible_view_methods)
-        
+
     @property
     def url_children_patterns(self) -> Iterable[URLPattern | URLResolver]:
         """Iterates over the route's children url patterns."""
         for child in self.children:
             yield from child.__proto__.url_patterns
         yield from ()
-        
+
     @property
     def has_children(self) -> bool:
         """Returns whether the route has children."""
         return any(self.children)
-        
+
     @property
     def url_patterns(self) -> Iterable[URLPattern | URLResolver]:
         if self.is_endpoint:
             yield urlpath(
                 self.url,
                 self.view,  # type: ignore
-                name=self.absolute_name) 
+                name=self.absolute_name)
         yield from self.url_children_patterns
 
+
 def templated_view(template_name: str, view: Callable):
     @wraps(view)
-    async def wrapper(self, request: HttpRequest):
-        match await view(self, request):
+    def wrapper(self, request: HttpRequest):
+        match view(self, request):
             case dict() as context:
                 return render(request, template_name, context)
             case HttpResponse() as response:
                 return response
             case [int() as status, dict() as context]:
                 return render(request, template_name, context, status=status)
-    wrapper.contextualised = True # type: ignore
+    wrapper.contextualised = True  # type: ignore
     return wrapper
 
+
 def apply(template: str):
     """Decorate a view to pass its return value to a template."""
-    
+
     @overload
     def decorator(view_or_route: type[Route]):
         ...
-        
+
     @overload
     def decorator(
         view_or_route: Callable[
-            [Self, HttpRequest], 
+            [Self, HttpRequest],
             dict[str, Any] | HttpResponse | tuple[int, dict[str, Any]]]):
         ...
-    
+
     def decorator(view_or_route):
         if isinstance(view_or_route, type) and issubclass(view_or_route, Route):
             for name in RouteProtocol.possible_view_methods:
                 if hasattr(view_or_route, name):
                     setattr(view_or_route, name,
-                        templated_view(template, view)
-                        if not getattr(
-                            (view:=getattr(view_or_route, name)),
-                            "contextualised", False
-                        ) else view)
+                            templated_view(template, view)
+                            if not getattr(
+                                (view := getattr(view_or_route, name)),
+                                "contextualised", False
+                            ) else view)
             return view_or_route
         if callable(view_or_route):
             return templated_view(template, view_or_route)
     return decorator
 
 
 class Route:
@@ -248,53 +251,54 @@
     This is the only modification we make to the class.
     """
 
     @classmethod
     @property
     def urlpatterns(cls) -> list[URLPattern | URLResolver]:
         return list(cls.__proto__.url_patterns)
-        
+
     def get_absolute_url(self) -> str:
         return '/'.join(
             part if isinstance(part, str)
             else getattr(
                 get_converter(part[1]),
                 'to_url', str
             )(getattr(self, part[0]))
-            for part in chain(('',), 
-                self.__proto__.url_parameters_parts))
-        
-    url: str = property(get_absolute_url) # type: ignore
-    
+            for part in chain(('',),
+                              self.__proto__.url_parameters_parts))
+
+    url: str = property(get_absolute_url)  # type: ignore
+
     @property
     def redirect(self):
         return redirect(self, permanent=False)
-    
+
     @property
     def permanent_redirect(self):
         return redirect(self, permanent=True)
 
     def __init__(self, **parameters) -> None:
         for name, value in parameters.items():
             setattr(self, name, value)
 
     def __init_subclass__(
         cls,
         app: str | None = None,
         name: str | None = None,
     ) -> None:
         """Prepares the route."""
-        cls.__proto__ = RouteProtocol(route=cls, custom_app=app, custom_name=name)
-        
-        
+        cls.__proto__ = RouteProtocol(
+            route=cls, custom_app=app, custom_name=name)
+
+
 class Parameter:
-    
+
     regex: str
-    
+
     def to_python(self, value: str) -> Any:
         return value
-    
+
     def to_url(self, value: Any) -> str:
         return str(value)
-    
+
     def __init_subclass__(cls) -> None:
-        register_converter(cls, RouteProtocol.snaky(cls.__qualname__))
+        register_converter(cls, RouteProtocol.snaky(cls.__qualname__))
```

