# Comparing `tmp/scopeton-2.5.tar.gz` & `tmp/scopeton-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scopeton-2.5.tar", last modified: Mon Jun  5 08:12:02 2023, max compression
+gzip compressed data, was "scopeton-3.0.tar", last modified: Thu Jul  6 16:36:58 2023, max compression
```

## Comparing `scopeton-2.5.tar` & `scopeton-3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-05 08:12:02.534923 scopeton-2.5/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1086 2023-04-16 07:04:25.000000 scopeton-2.5/LICENSE.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-05 08:12:02.534923 scopeton-2.5/PKG-INFO
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     2472 2023-04-16 07:49:04.000000 scopeton-2.5/README.md
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-05 08:12:02.534923 scopeton-2.5/scopeton/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       38 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/__init__.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1068 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/compat.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       67 2023-06-04 18:13:09.000000 scopeton-2.5/scopeton/constants.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1113 2023-06-04 18:58:02.000000 scopeton-2.5/scopeton/decorators.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       46 2023-06-04 18:11:40.000000 scopeton-2.5/scopeton/glob.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1110 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/objects.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     3105 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/qualifier_tree.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     5161 2023-06-05 08:01:03.000000 scopeton-2.5/scopeton/scope.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1320 2023-04-16 07:04:25.000000 scopeton-2.5/scopeton/scopeTools.py
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     4521 2023-06-05 08:10:52.000000 scopeton-2.5/scopeton/type_utils.py
-drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-06-05 08:12:02.534923 scopeton-2.5/scopeton.egg-info/
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/PKG-INFO
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      412 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/SOURCES.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        1 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/dependency_links.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        7 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/requires.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        9 2023-06-05 08:12:02.000000 scopeton-2.5/scopeton.egg-info/top_level.txt
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       79 2023-06-05 08:12:02.534923 scopeton-2.5/setup.cfg
--rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      500 2023-06-05 08:11:11.000000 scopeton-2.5/setup.py
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-07-06 16:36:58.789122 scopeton-3.0/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1086 2020-12-10 19:44:35.000000 scopeton-3.0/LICENSE.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-07-06 16:36:58.789122 scopeton-3.0/PKG-INFO
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     2940 2023-07-06 16:25:57.000000 scopeton-3.0/README.md
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-07-06 16:36:58.789122 scopeton-3.0/scopeton/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       38 2020-12-10 19:44:35.000000 scopeton-3.0/scopeton/__init__.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      772 2023-07-06 13:40:58.000000 scopeton-3.0/scopeton/annotation_tools.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1196 2023-07-06 13:40:34.000000 scopeton-3.0/scopeton/compat.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      179 2023-07-06 13:46:39.000000 scopeton-3.0/scopeton/constants.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      846 2023-07-06 13:48:35.000000 scopeton-3.0/scopeton/decorators.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       46 2023-07-06 13:06:59.000000 scopeton-3.0/scopeton/glob.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1118 2023-07-06 13:19:00.000000 scopeton-3.0/scopeton/objects.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     2972 2023-07-06 13:18:05.000000 scopeton-3.0/scopeton/qualifier_tree.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     5447 2023-07-06 13:49:26.000000 scopeton-3.0/scopeton/scope.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     1519 2023-07-06 13:25:31.000000 scopeton-3.0/scopeton/scope_tools.py
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)     4518 2023-07-06 13:06:59.000000 scopeton-3.0/scopeton/type_utils.py
+drwxrwxr-x   0 shaddy    (1000) shaddy    (1000)        0 2023-07-06 16:36:58.789122 scopeton-3.0/scopeton.egg-info/
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      314 2023-07-06 16:36:58.000000 scopeton-3.0/scopeton.egg-info/PKG-INFO
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      442 2023-07-06 16:36:58.000000 scopeton-3.0/scopeton.egg-info/SOURCES.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        1 2023-07-06 16:36:58.000000 scopeton-3.0/scopeton.egg-info/dependency_links.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        7 2023-07-06 16:36:58.000000 scopeton-3.0/scopeton.egg-info/requires.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)        9 2023-07-06 16:36:58.000000 scopeton-3.0/scopeton.egg-info/top_level.txt
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)       79 2023-07-06 16:36:58.789122 scopeton-3.0/setup.cfg
+-rw-rw-r--   0 shaddy    (1000) shaddy    (1000)      500 2023-07-06 16:35:50.000000 scopeton-3.0/setup.py
```

### Comparing `scopeton-2.5/LICENSE.txt` & `scopeton-3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scopeton-2.5/README.md` & `scopeton-3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     pass
 
 class Dependency4():
     pass
 
 class Dependency5():
     @Inject()
-    def __init__(self, dep1: Dependency1, a):
+    def __init__(self, dep1: Dependency1, dep4: Dependency4):
         pass
 
 
 class Dependency7():
     called = False
     @Inject()
     def __init__(self, dep1:Dependency1, dep4: Dependency4):
@@ -77,28 +77,40 @@
 overriding bean parameters:
 ```python
 appScope.registerBean(Bean(Dependency1, singleton = False), Dependency2, Dependency3)
 ```
 in this case Dependency1 will be non-singleton bean
 
 ## Services
-All beans can have postConstruct and preDestroy functions, these functions will be called automatically:
-postConstruct will be called for each bean after 
+All beans can have functions, annotated with @PostConstruct and/or PreDestroy decorators, these functions will be called automatically:
+@PostConstruct marked functions will be called for each bean after 
 ```python
 appScope.runServices()
 ```
-and preDestroy will be called after 
+and @PreDestroy marked will be called after 
 ```python
 appScope.stopServices()
 ```
 
 ## Inject scope
 
 Each bean can inject the scope itself (avoiding circular dependencies)
 
 ```python
+from scopeton.decorators import Inject
 class Dependency():
     @Inject()
-    def __init__(self, scope: Scope, a):
+    def __init__(self, scope: Scope):
         self
 ```
 
+## Non constructor injection
+Scopeton can inject beans not only in constructor injection:
+
+```python
+from scopeton.decorators import Inject
+class Dependency():
+    @Inject()
+    def some_method(self, dependency: DependencyBean):
+        self
+```
+In this case some_method will be called during bean creation and DependencyBean will be injected as a parameter
```

### Comparing `scopeton-2.5/scopeton/compat.py` & `scopeton-3.0/scopeton/compat.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,46 +3,54 @@
 
 from scopeton import constants
 
 
 class _Python2NativeArgs:
     args = ['self']
 
-def isPython3():
+
+def is_python3():
     return sys.version_info.major >= 3
 
-def getMethods(instance):
-    return [k for k in inspect.getmembers(instance, predicate=inspect.ismethod)]
 
-def isClass(obj):
-    if not isPython3():
+def get_methods(instance):
+    return [k[1] for k in inspect.getmembers(instance, predicate=inspect.ismethod)]
+
+
+def get_method_instance(method):
+    if not hasattr(method, "__self__"):
+        return None
+    return method.__self__
+
+
+def is_class(obj):
+    if not is_python3():
         import new
         return type(obj) is new.classobj or type(obj) is type
     else:
         import inspect
         return inspect.isclass(obj)
 
-def objectIsInstance(obj):
-    if not isPython3():
+
+def object_is_instance(obj):
+    if not is_python3():
         import new
         return type(obj) is new.instance or (hasattr(obj, "__class__") and hasattr(obj.__class__, "__name__"))
     else:
         import inspect
         return inspect.isclass(obj)
 
 
-def getMethodSignature(method):
-    if isPython3():
+def get_method_signature(method):
+    if is_python3():
         return inspect.getfullargspec(method)
     else:
         try:
             return inspect.getargspec(method)
         except TypeError:
             return _Python2NativeArgs()
 
 
-def hasInject(fn):
-    return hasattr(fn, constants.INJECT_FLAG)
-
-
-def isMethod(fn):
-    return inspect.ismethod(fn)
+def is_method(fn):
+    return inspect.ismethod(fn)
+def is_function(fn):
+    return inspect.isfunction(fn)
```

### Comparing `scopeton-2.5/scopeton/objects.py` & `scopeton-3.0/scopeton/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from scopeton import scopeTools
-from scopeton.scopeTools import getBean_qualifier
+from scopeton import scope_tools
+from scopeton.scope_tools import get_bean_qualifier
 
 
 class Bean(object):
     def __init__(self, cls, name=None, lazy = False, singleton=True, service = True, checkRegistered = True):
         self.checkRegistered = True
         self.cls = cls
-        self.qualifier_tree = scopeTools.getClassTreeQualifiers(cls)
+        self.qualifier_tree = scope_tools.get_class_tree_qualifiers(cls)
         if name:
-            name = getBean_qualifier(name)
+            name = get_bean_qualifier(name)
             if name not in self.qualifier_tree:
                 self.qualifier_tree.append(name)
         self.lazy = lazy
         self.singleton = singleton
         self.service = service
         if not singleton and service:
             raise Exception("Error, cannot initialize service as non singleton")
```

### Comparing `scopeton-2.5/scopeton/qualifier_tree.py` & `scopeton-3.0/scopeton/qualifier_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 import logging
 import typing
 from threading import RLock
 
-from scopeton.scopeTools import ScopetonException, flatten
+from scopeton.scope_tools import ScopetonException, flatten
 
 
 class QualifierTree:
     def __init__(self):
         self._qualifiers = {}  # type: dict[str, typing.List[object]]
         self._qualifiersMap = {}  # type: dict[object, typing.List[str]]
         self.lock = RLock()
 
-    def _registerObj(self, qualifier_name: str, obj):
+    def _register_obj(self, qualifier_name: str, obj):
         with self.lock:
-            self._regOBjectByQualifier(qualifier_name, obj)
-            self._regQualifierByObject(qualifier_name, obj)
+            self._reg_object_by_qualifier(qualifier_name, obj)
+            self._reg_qualifier_by_object(qualifier_name, obj)
 
-    def _regOBjectByQualifier(self, qualifier_name, obj):
+    def _reg_object_by_qualifier(self, qualifier_name, obj):
         if qualifier_name not in self._qualifiers:
             self._qualifiers[qualifier_name] = []
         if obj not in self._qualifiers[qualifier_name]:
             logging.debug("Registering: {}".format(obj))
             self._qualifiers[qualifier_name].append(obj)
 
-    def _regQualifierByObject(self, qualifier_name, obj):
+    def _reg_qualifier_by_object(self, qualifier_name, obj):
         if obj not in self._qualifiersMap:
             self._qualifiersMap[obj] = []
         if qualifier_name not in self._qualifiersMap[obj]:
             self._qualifiersMap[obj].append(qualifier_name)
 
     def register(self, names: typing.Union[typing.List[str], str], obj):
         if isinstance(names, str):
             names = [names]
         for name in names:
-            self._registerObj(name, obj)
+            self._register_obj(name, obj)
 
     def find_qualifiers(self, obj):
         return self._qualifiersMap[obj]
 
     def check_object_has_qualifier(self, qualifier, object):
         return qualifier in self._qualifiersMap[object]
 
     def get_qualifier_tree_length(self, obj):
         return len(self.find_qualifiers(obj))
 
     def find_suitable_qualifier(self, qualifier):
-        #logging.debug("self._qualifiersMap:{}".format(self._qualifiersMap))
-        #logging.debug("self._qualifiers:{}".format(self._qualifiers))
         if qualifier not in self._qualifiers:
             return qualifier
         objects = self._qualifiers[qualifier]
         if len(objects) > 1:
             raise Exception("expected 1 object for qualifier:{}, but got {}: {}".format(qualifier, len(objects), objects))
         if len(objects) == 0:
             raise Exception("No objects for qualifier:{}".format(qualifier))
```

### Comparing `scopeton-2.5/scopeton/scope.py` & `scopeton-3.0/scopeton/scope.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import logging
-from threading import RLock
-
 import typing
+from threading import RLock
 
-from scopeton import compat, glob, constants, type_utils
+from scopeton import compat, glob, constants, type_utils, scope_tools, annotation_tools
 from scopeton.objects import Bean
 from scopeton.qualifier_tree import QualifierTree
-from scopeton.scopeTools import getBean_qualifier, callMethodByName, getClassTree, flatten, ScopetonException
+from scopeton.scope_tools import get_bean_qualifier, ScopetonException
 
 T = typing.TypeVar("T")
 
 
 class Scope(object):
     '''this is servicelocator pattern implementation'''
 
-    def __init__(self, lock=False, initMethod="postConstruct", destroyMethod="preDestroy", parent=None):
+    def __init__(self, lock=False, parent=None):
         self._singletons = QualifierTree()
         self._beans = QualifierTree()
         self.lock = lock or RLock()  # type: RLock
-        self.initMethod = initMethod
-        self.destroyMethod = destroyMethod
         self.parent = parent  # type:  Scope
         self.servicesStarted = False
         self.children = []  # type: typing.List[Scope]
         self.registerInstance(self.__class__, self)
         if parent:
             parent.children.append(self)
 
     def getInstance(self, name: typing.Type[T]) -> T:
-        if type_utils._is_collection(name):
-            args = type_utils._get_type_args(name)
-            return self.getInstances(args[0])
+        if type_utils.is_collection(name):
+            args = type_utils.get_type_args(name)
+            return self.get_instances(typing.cast(typing.Type[T], args[0]))
         with self.lock:
-            return self._getInstance(getBean_qualifier(name))
+            return self._get_instance(get_bean_qualifier(name))
 
-    def getInstances(self, qualifier: typing.Type[T]) -> typing.List[T]:
+    def get_instances(self, qualifier: typing.Type[T]) -> typing.List[T]:
         with self.lock:
-            beans = self._beans.find_by_qualifier_name(getBean_qualifier(qualifier))
+            beans = self._beans.find_by_qualifier_name(get_bean_qualifier(qualifier))
             beans = map(lambda x: self.getInstance(x), beans)
             return list(beans)
 
-    def _getInstance(self, qualifier):
+    def _get_instance(self, qualifier):
 
-        suitableQualifier = self._beans.find_suitable_qualifier(qualifier)
+        suitable_qualifier = self._beans.find_suitable_qualifier(qualifier)
 
-        if self._singletons.contains(suitableQualifier):
-            return self._singletons.find_one_by_qualifier_name(suitableQualifier)
+        if self._singletons.contains(suitable_qualifier):
+            return self._singletons.find_one_by_qualifier_name(suitable_qualifier)
 
-        bean = self._beans.find_one_by_qualifier_name(suitableQualifier)
+        bean = self._beans.find_one_by_qualifier_name(suitable_qualifier)
         glob.lastScope = self
-        if compat.hasInject(bean.cls.__init__):
+
+        if hasattr(bean.cls.__init__, constants.TO_INJECT_FLAG):
+            # constructor injection
             instance = bean.cls()
-        elif len(compat.getMethodSignature(bean.cls.__init__).args) == 2:
+        elif len(compat.get_method_signature(bean.cls.__init__).args) == 2:
             instance = bean.cls(self)
-        elif len(compat.getMethodSignature(bean.cls.__init__).args) > 2:
+        elif len(compat.get_method_signature(bean.cls.__init__).args) > 2:
             raise ScopetonException(
                 "Invalid number of parameters for bean constructor, maybe @Inject() decorator forgotten: {}".format(
-                    compat.getMethodSignature(bean.cls.__init__).args))
+                    compat.get_method_signature(bean.cls.__init__).args))
         else:
             instance = bean.cls()
 
         if bean.singleton:
-            self.registerInstance(suitableQualifier, instance)
+            self.registerInstance(suitable_qualifier, instance)
 
         self._inject_injectables(instance)
 
         return instance
 
     def registerInstance(self, name, instance):
-        qualifier = getBean_qualifier(name)
+        qualifier = get_bean_qualifier(name)
         suitableQualifier = self._beans.find_suitable_qualifier(qualifier)
         logging.debug("Suitable qualifier for {} is: {}".format(qualifier, suitableQualifier))
         self._singletons.register(suitableQualifier, instance)
+        self._inject_injectables(instance)
 
     def registerBean(self, *args):
         with self.lock:
             for bean in args:
                 if not isinstance(bean, Bean):
                     bean = Bean(bean)
                 self._registerBean(bean)
@@ -97,37 +97,45 @@
             self._beans.register(name, bean)
 
     def runServices(self):
         if not self.servicesStarted:
             self.servicesStarted = True
             for bean in self._beans.get_all_objects():
                 if bean.service:
-                    callMethodByName(self.getInstance(bean), self.initMethod)
+                    instance = self.getInstance(bean)
+                    methods = annotation_tools.get_methods_with_annotation(instance, constants.POST_CONSTRUCT)
+                    for k in methods:
+                        self._inject_method_args(k)
 
             for childScope in self.children:
                 childScope.runServices()
 
     def stopServices(self):
         if self.servicesStarted:
             self.servicesStarted = False
             for bean in self._beans.get_all_objects():
                 if bean.service:
-                    callMethodByName(self.getInstance(bean), self.destroyMethod)
+                    methods = annotation_tools.get_methods_with_annotation(self.getInstance(bean), constants.PRE_DESTROY)
+                    for k in methods:
+                        self._inject_method_args(k)
             for childScope in self.children:
                 childScope.stopServices()
 
     def _inject_injectables(self, instance):
-        for fn in compat.getMethods(instance):
-            if hasattr(fn[1], constants.INJECT_BEFORE):
-                annotations_signature = compat.getMethodSignature(fn[1]).annotations
-                args_signature = compat.getMethodSignature(fn[1]).args
-                nargs = []
-                for arg_name in args_signature:
-                    if arg_name == "self":
-                        continue
-                    if arg_name not in annotations_signature:
-                        raise ScopetonException("Not annotated inject argument: {}".format(arg_name))
-                    arg_type = annotations_signature[arg_name]
-                    arg_to_inject = self.getInstance(arg_type)
-                    nargs.append(arg_to_inject)
-                fn[1](*nargs)
-
+        if hasattr(instance, constants.INJECTED):
+            return
+        for fn in scope_tools.get_injectables(instance):
+            self._inject_method_args(fn)
+        setattr(instance, constants.INJECTED, 1)
+
+    def _inject_method_args(self, fn, add_self=None):
+        signature = compat.get_method_signature(fn)
+        nargs = []
+        if add_self is not None:
+            nargs.append(add_self)
+        for arg_name in signature.args:
+            if arg_name == "self":
+                continue
+            if arg_name not in signature.annotations:
+                raise ScopetonException("Not annotated inject argument: {}".format(arg_name))
+            nargs.append(self.getInstance(signature.annotations[arg_name]))
+        return fn(*nargs)
```

### Comparing `scopeton-2.5/scopeton/scopeTools.py` & `scopeton-3.0/scopeton/scope_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,65 @@
+from scopeton import compat, constants
+
+
 def flatten(lst):
     res = []
     for el in lst:
         if type(el) is list:
             res += flatten(el)
         else:
             res.append(el)
     return res
 
-def getClassName(cls):
+
+def get_class_name(cls):
     return cls.__name__ if hasattr(cls, "__name__") else str(cls)
 
-def getClassTreeQualifiers(cls):
-    res = [getBean_qualifier(k) for k in getClassTree(cls)]
+
+def get_class_tree_qualifiers(cls):
+    res = [get_bean_qualifier(k) for k in get_class_tree(cls)]
     res.reverse()
     return res
 
-def rmDups(lst):
+
+def rm_dups(lst):
     res = []
     for k in lst:
         if k not in res:
             res.append(k)
     return res
 
 
-def getClassTree(cls):
-    return rmDups(_getClassTree(cls))
+def get_class_tree(cls):
+    return rm_dups(_get_class_tree(cls))
 
-def _getClassTree(cls):
+
+def _get_class_tree(cls):
     res = [cls]
     if type(cls) is not object and hasattr(cls, "__bases__") and cls.__bases__:
-        res += flatten([_getClassTree(parent) for parent in cls.__bases__])
+        res += flatten([_get_class_tree(parent) for parent in cls.__bases__])
     return res
 
-def getBean_qualifier(bean) -> str:
+
+def get_bean_qualifier(bean) -> str:
     if isinstance(bean, str):
         return bean
     from scopeton.objects import Bean
     if isinstance(bean, Bean):
         return bean.qualifier_tree[-1]
     if not hasattr(bean, "__name__"):
         return str(bean)
     return bean.__name__
 
-def callMethodByName(obj, name, *args, **kwargs):
+
+def call_method_by_name(obj, name, *args, **kwargs):
     if hasattr(obj, name):
         return getattr(obj, name)(*args, **kwargs)
 
 
+def get_injectables(instance):
+    return [fn for fn in compat.get_methods(instance) if hasattr(fn, constants.TO_INJECT_FLAG)]
+
+
 class ScopetonException(Exception):
     def __init__(self, *args, **kwargs):
-        super(Exception, self).__init__(*args, **kwargs)
+        super(Exception, self).__init__(*args, **kwargs)
```

### Comparing `scopeton-2.5/scopeton/type_utils.py` & `scopeton-3.0/scopeton/type_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,24 @@
     def __next__(self):
         raise StopIteration
 
 
 _NO_ARGS = _NoArgs()
 
 
-def _get_type_args(tp: Type, default: Tuple[Type, ...] = _NO_ARGS) -> \
+def get_type_args(tp: Type, default: Tuple[Type, ...] = _NO_ARGS) -> \
         Union[Tuple[Type, ...], _NoArgs]:
     if hasattr(tp, '__args__'):
         if tp.__args__ is not None:
             return tp.__args__
     return default
 
 
 def _get_type_arg_param(tp: Type, index: int) -> Union[Type, _NoArgs]:
-    _args = _get_type_args(tp)
+    _args = get_type_args(tp)
     if _args is not _NO_ARGS:
         try:
             return _args[index]
         except (TypeError, IndexError, NotImplementedError):
             pass
 
     return _NO_ARGS
@@ -110,15 +110,15 @@
             type_ is Any)
 
 
 def _is_mapping(type_):
     return _issubclass_safe(_get_type_origin(type_), Mapping)
 
 
-def _is_collection(type_):
+def is_collection(type_):
     return _issubclass_safe(_get_type_origin(type_), Collection)
 
 
 def _is_nonstr_collection(type_):
     return (_issubclass_safe(_get_type_origin(type_), Collection)
             and not _issubclass_safe(type_, str))
```

