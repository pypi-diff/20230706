# Comparing `tmp/coopapi-0.7.tar.gz` & `tmp/coopapi-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coopapi-0.7.tar", last modified: Fri Jun  2 15:26:46 2023, max compression
+gzip compressed data, was "coopapi-1.0.tar", last modified: Thu Jul  6 15:53:45 2023, max compression
```

## Comparing `coopapi-0.7.tar` & `coopapi-1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 15:26:46.989445 coopapi-0.7/
--rw-rw-rw-   0        0        0     2838 2023-06-02 15:26:46.988444 coopapi-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 15:26:46.960482 coopapi-0.7/coopapi/
--rw-rw-rw-   0        0        0      312 2023-02-15 15:23:58.000000 coopapi-0.7/coopapi/__init__.py
--rw-rw-rw-   0        0        0     9526 2023-02-15 15:26:46.000000 coopapi-0.7/coopapi/apiShell.py
--rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-0.7/coopapi/enums.py
--rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-0.7/coopapi/errors.py
--rw-rw-rw-   0        0        0     4883 2023-04-13 18:18:49.000000 coopapi-0.7/coopapi/http_request.py
--rw-rw-rw-   0        0        0     4598 2023-02-23 20:53:41.000000 coopapi-0.7/coopapi/http_request_handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:26:46.986444 coopapi-0.7/coopapi.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-0.7/coopapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      279 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 15:26:46.989445 coopapi-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-06-02 15:26:42.000000 coopapi-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:53:45.278031 coopapi-1.0/
+-rw-rw-rw-   0        0        0     2838 2023-07-06 15:53:45.277031 coopapi-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 15:53:45.230080 coopapi-1.0/coopapi/
+-rw-rw-rw-   0        0        0      324 2023-07-06 13:56:43.000000 coopapi-1.0/coopapi/__init__.py
+-rw-rw-rw-   0        0        0    11887 2023-07-06 13:58:02.000000 coopapi-1.0/coopapi/apiShell.py
+-rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-1.0/coopapi/enums.py
+-rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-1.0/coopapi/errors.py
+-rw-rw-rw-   0        0        0     5954 2023-06-02 17:15:47.000000 coopapi-1.0/coopapi/http_request.py
+-rw-rw-rw-   0        0        0     6269 2023-07-06 15:51:17.000000 coopapi-1.0/coopapi/http_request_handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:53:45.274038 coopapi-1.0/coopapi.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-1.0/coopapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      279 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 15:53:45.000000 coopapi-1.0/coopapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:53:45.279034 coopapi-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-07-06 15:53:22.000000 coopapi-1.0/setup.py
```

### Comparing `coopapi-0.7/PKG-INFO` & `coopapi-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.7
+Version: 1.0
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.7/README.md` & `coopapi-1.0/README.md`

 * *Files identical despite different names*

### Comparing `coopapi-0.7/coopapi/apiShell.py` & `coopapi-1.0/coopapi/apiShell.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,226 +1,298 @@
+import uvicorn
 from fastapi import Body, Request, status
 from coopapi import http_request_handlers as hrh
 from typing import Any, Dict, List, Callable, Tuple
 from fastapi import APIRouter
 from pydantic.dataclasses import dataclass as pydataclass, Field
 from dataclasses import dataclass, field
 import json
 from urllib.parse import parse_qs
 import logging
+from coopapi.enums import RequestType
 
 logger = logging.getLogger('APIHandler')
 
-def post_route(create_callback: hrh.postRequestCallback,
-               schema: type):
-    def create(request: Request, item: schema = Body(...)) -> schema:
-        ret = hrh.post_request_handler(request=request,
+
+def route(callback: hrh.requestCallback,
+          schema: type):
+    def internal(request: Request, item: schema = Body(...)) -> schema:
+        ret = hrh.request_handler(request=request,
                                        item=item,
-                                       on_post_callback=create_callback
+                                       callback=callback
                                        )
 
         return ret
-    return create
-
-def put_route(update_callback: hrh.putRequestCallback,
-              schema: type):
-    def update(request: Request, id: str, update_values: Dict = Body(...)) -> schema:
-        return hrh.put_request_handler(request=request,
-                                       id=id,
-                                       obj_type=schema,
-                                       update_values=update_values,
-                                       on_put_callback=update_callback)
-    return update
-
-def delete_route(delete_callback: hrh.deleteRequestCallback,
-                 schema: type,
-                 redirect_url: str = None):
-    def delete(request: Request, id: str):
-        return hrh.delete_request_handler(id=id,
-                                          request=request,
-                                          obj_type=schema,
-                                          on_delete_callback=delete_callback,
-                                          redirect_url=redirect_url)
-    return delete
-
-def getone_route(find_callback: hrh.getOneRequestCallback,
-                 schema: type):
-    def find(request: Request, id: str) -> schema:
-        return hrh.getone_request_handler(id=id,
-                                          request=request,
-                                          obj_type=schema,
-                                          on_getone_callback=find_callback)
-    return find
-
-def getmany_route(list_callback: hrh.getManyRequestCallback,
-                  schema: type):
-    def list(request: Request, query: str = None, limit: int = 100) -> List[schema]:
-        if query is not None:
-            query = json.loads(query)
-        ret = hrh.getmany_request_handler(request,
-                                          on_getmany_callback=list_callback,
-                                          query=query,
-                                          limit=limit)
-        return ret
-    return list
+    return internal
 
 
-dirtyCleaner = Callable[[Dict], Dict]
 
-def dirty_post_route(create_callback: hrh.postRequestCallback,
-                     schema: type,
-                     cleaner: dirtyCleaner):
-    def dirty_post_route(request: Request, dirty_str: str = Body(...)) -> schema:
-        dirty_data = parse_qs(dirty_str)
-        clean_data = cleaner(dirty_data)
-        logger.info(f"Received Data: {dirty_str}\n"
-                    f"Cleaned Data: {clean_data}")
-
-        obj = schema(**clean_data)
-        ret = hrh.post_request_handler(request=request,
-                                       item=obj,
-                                       on_post_callback=create_callback
-                                       )
 
-        return ret
-    return dirty_post_route
+# def post_route(create_callback: hrh.postRequestCallback,
+#                schema: type):
+#     def create(request: Request, item: schema = Body(...)) -> schema:
+#         ret = hrh.post_request_handler(request=request,
+#                                        item=item,
+#                                        on_post_callback=create_callback
+#                                        )
+#
+#         return ret
+#     return create
+#
+# def put_route(update_callback: hrh.putRequestCallback,
+#               schema: type):
+#     def update(request: Request, id: str, update_values: Dict = Body(...)) -> schema:
+#         return hrh.put_request_handler(request=request,
+#                                        id=id,
+#                                        obj_type=schema,
+#                                        update_values=update_values,
+#                                        on_put_callback=update_callback)
+#     return update
+#
+# def delete_route(delete_callback: hrh.deleteRequestCallback,
+#                  schema: type,
+#                  redirect_url: str = None):
+#     def delete(request: Request, id: str):
+#         return hrh.delete_request_handler(id=id,
+#                                           request=request,
+#                                           obj_type=schema,
+#                                           on_delete_callback=delete_callback,
+#                                           redirect_url=redirect_url)
+#     return delete
+#
+# def getone_route(find_callback: hrh.getOneRequestCallback,
+#                  schema: type):
+#     def find(request: Request, id: str) -> schema:
+#         return hrh.getone_request_handler(id=id,
+#                                           request=request,
+#                                           obj_type=schema,
+#                                           on_getone_callback=find_callback)
+#     return find
+#
+# def getmany_route(list_callback: hrh.getManyRequestCallback,
+#                   schema: type):
+#     def list(request: Request, query: str = None, limit: int = 100) -> List[schema]:
+#         if query is not None:
+#             query = json.loads(query)
+#         ret = hrh.getmany_request_handler(request,
+#                                           on_getmany_callback=list_callback,
+#                                           query=query,
+#                                           limit=limit)
+#         return ret
+#     return list
+
+
+# dirtyCleaner = Callable[[Dict], Dict]
+#
+# def dirty_post_route(create_callback: hrh.postRequestCallback,
+#                      schema: type,
+#                      cleaner: dirtyCleaner):
+#     def dirty_post_route(request: Request, dirty_str: str = Body(...)) -> schema:
+#         dirty_data = parse_qs(dirty_str)
+#         clean_data = cleaner(dirty_data)
+#         logger.info(f"Received Data: {dirty_str}\n"
+#                     f"Cleaned Data: {clean_data}")
+#
+#         obj = schema(**clean_data)
+#         ret = hrh.post_request_handler(request=request,
+#                                        item=obj,
+#                                        on_post_callback=create_callback
+#                                        )
+#
+#         return ret
+#     return dirty_post_route
 
 # class Config:
 #     arbitrary_types_allowed = True
 
 @dataclass
+class CallbackPackage:
+    method: RequestType
+    callback: Callable
+    input_schema: type
+    response_schema: type
+
+@dataclass
 class ApiShell:
-    target_schema: type
     base_route: str
-    on_post_callback: hrh.postRequestCallback = field(default=None)
-    on_put_callback: hrh.putRequestCallback = field(default=None)
-    on_delete_callback: hrh.deleteRequestCallback = field(default=None)
-    on_getone_callback: hrh.getOneRequestCallback = field(default=None)
-    on_getmany_callback: hrh.getManyRequestCallback = field(default=None)
-    dirty_create: dirtyCleaner = field(default=None)
+    on_post_callback: CallbackPackage = field(default=None)
+    on_put_callback: CallbackPackage = field(default=None)
+    on_delete_callback: CallbackPackage = field(default=None)
+    on_getone_callback: CallbackPackage = field(default=None)
+    on_getmany_callback: CallbackPackage = field(default=None)
+    # dirty_create: dirtyCleaner = field(default=None)
     router: APIRouter = field(default_factory=APIRouter)
 
 
     def __post_init__(self):
         self.register_routes()
         print(f"{self.base_route} routes registered")
 
     # def __post_init_post_parse__(self):
     #     self.register_routes()
     #     print(f"{self.base_route} routes registered")
 
+
+    def _register_route_internal(self,
+                                 callback_package: CallbackPackage):
+        self.router.add_api_route(
+            f"{self.base_route}/api/",
+            route(callback=callback_package.callback, schema=callback_package.input_schema),
+            methods=[callback_package.method.value],
+            response_description=f"{callback_package.method.value} a new {callback_package.input_schema.__name__}",
+            response_model=callback_package.response_schema,
+            status_code=ApiShell._success_status_code(callback_package.method))
+
+    @staticmethod
+    def _success_status_code(method: RequestType):
+        switch = {
+            RequestType.POST: status.HTTP_201_CREATED,
+            RequestType.PUT: status.HTTP_202_ACCEPTED,
+            RequestType.GET: status.HTTP_200_OK,
+            RequestType.DELETE: status.HTTP_202_ACCEPTED,
+        }
+        return switch.get(method)
+
     def register_routes(self):
-        '''
-        Basic CRUD api_routers routes
-        '''
-        # create route
         if self.on_post_callback is not None:
-            self.router.add_api_route(
-                f"{self.base_route}/api/",
-                post_route(self.on_post_callback, schema=self.target_schema),
-                methods=['POST'],
-                response_description=f"POST a new {self.target_schema.__name__}",
-                response_model=self.target_schema,
-                status_code=status.HTTP_201_CREATED)
+            self._register_route_internal(self.on_post_callback)
 
-        # update route
         if self.on_put_callback is not None:
-            self.router.add_api_route(
-                f"{self.base_route}/api/{{id}}",
-                put_route(update_callback=self.on_put_callback, schema=self.target_schema),
-                methods=['PUT'],
-                response_description=f"PUT a {self.target_schema.__name__}",
-                response_model=self.target_schema,
-                status_code=status.HTTP_202_ACCEPTED
-            )
+            self._register_route_internal(self.on_put_callback)
 
-        # delete route
         if self.on_delete_callback is not None:
-            self.router.add_api_route(
-                f"{self.base_route}/api/{{id}}",
-                delete_route(delete_callback=self.on_delete_callback, schema=self.target_schema),
-                methods=['DELETE'],
-                response_description=f"DELETE a {self.target_schema.__name__}",
-                response_model=bool,
-                status_code=status.HTTP_200_OK
-            )
+            self._register_route_internal(self.on_delete_callback)
 
-        # find route
         if self.on_getone_callback is not None:
-            self.router.add_api_route(
-                f"{self.base_route}/api/{{id}}",
-                getone_route(find_callback=self.on_getone_callback, schema=self.target_schema),
-                methods=['GET'],
-                response_description=f"GET a single {self.target_schema.__name__} by id",
-                response_model=self.target_schema,
-                status_code=status.HTTP_200_OK)
+            self._register_route_internal(self.on_getone_callback)
 
-        # list route
         if self.on_getmany_callback is not None:
-            self.router.add_api_route(
-                f"{self.base_route}/api/",
-                getmany_route(list_callback=self.on_getmany_callback, schema=self.target_schema),
-                methods=['GET'],
-                response_description=f"GET all {self.target_schema.__name__}s",
-                response_model=List[self.target_schema],
-                status_code=status.HTTP_200_OK
-            )
-
-
-        '''
-        routes specific to being accessed via HTML elements. Since all hrefs assume a requirement for 'GET' requests,
-        they must be structured differently. Rather than using the /api_routers/ routes, instead, include the operation 
-        (eg, 'delete') in the url, and send it as a 'GET' route. These should include redirect_urls back to the base
-        route.
-        '''
+            self._register_route_internal(self.on_getmany_callback)
 
-        if self.on_delete_callback is not None:
-            self.router.add_api_route(
-                f"{self.base_route}/delete/{{id}}",
-                delete_route(delete_callback=self.on_delete_callback, schema=self.target_schema, redirect_url=f"{self.base_route}"),
-                methods=['GET'],
-                response_description=f"Delete a {self.target_schema.__name__}",
-                response_model=bool,
-                status_code=status.HTTP_200_OK
-            )
-
-        '''
-        Dirty route (used for taking in data in a format we know wont work directly, but can be manipulated to use
-        the endpoints
-        '''
-        if self.dirty_create is not None:
-            if self.on_post_callback is None:
-                raise NotImplementedError(f"Cannot supply a dirty create without an on_create_callback")
-
-            self.router.add_api_route(
-                f"{self.base_route}/dirty/",
-                dirty_post_route(create_callback=self.on_post_callback, schema=self.target_schema, cleaner=self.dirty_create),
-                methods=['POST'],
-                response_description=f"Create a {self.target_schema.__name__}",
-                response_model=self.target_schema,
-                status_code=status.HTTP_200_OK
-            )
+        # '''
+        # Basic CRUD api_routers routes
+        # '''
+        # # create route
+        # if self.on_post_callback is not None:
+        #     self.router.add_api_route(
+        #         f"{self.base_route}/api/",
+        #         route(callback=self.on_post_callback.callback, schema=self.on_post_callback.input_schema),
+        #         methods=['POST'],
+        #         response_description=f"POST a new {self.on_post_callback.input_schema.__name__}",
+        #         response_model=self.on_post_callback.response_schema,
+        #         status_code=status.HTTP_201_CREATED)
+        #
+        # # update route
+        # if self.on_put_callback is not None:
+        #     self.router.add_api_route(
+        #         f"{self.base_route}/api/{{id}}",
+        #         route(callback=self.on_put_callback.callback, schema=self.on_put_callback.input_schema),
+        #         methods=['PUT'],
+        #         response_description=f"PUT a {self.target_schema.__name__}",
+        #         response_model=self.target_schema,
+        #         status_code=status.HTTP_202_ACCEPTED
+        #     )
+        #
+        # # delete route
+        # if self.on_delete_callback is not None:
+        #     self.router.add_api_route(
+        #         f"{self.base_route}/api/{{id}}",
+        #         delete_route(delete_callback=self.on_delete_callback, schema=self.target_schema),
+        #         methods=['DELETE'],
+        #         response_description=f"DELETE a {self.target_schema.__name__}",
+        #         response_model=bool,
+        #         status_code=status.HTTP_200_OK
+        #     )
+        #
+        # # find route
+        # if self.on_getone_callback is not None:
+        #     self.router.add_api_route(
+        #         f"{self.base_route}/api/{{id}}",
+        #         getone_route(find_callback=self.on_getone_callback, schema=self.target_schema),
+        #         methods=['GET'],
+        #         response_description=f"GET a single {self.target_schema.__name__} by id",
+        #         response_model=self.target_schema,
+        #         status_code=status.HTTP_200_OK)
+        #
+        # # list route
+        # if self.on_getmany_callback is not None:
+        #     self.router.add_api_route(
+        #         f"{self.base_route}/api/",
+        #         getmany_route(list_callback=self.on_getmany_callback, schema=self.target_schema),
+        #         methods=['GET'],
+        #         response_description=f"GET all {self.target_schema.__name__}s",
+        #         response_model=List[self.target_schema],
+        #         status_code=status.HTTP_200_OK
+        #     )
+        #
+        #
+        # '''
+        # routes specific to being accessed via HTML elements. Since all hrefs assume a requirement for 'GET' requests,
+        # they must be structured differently. Rather than using the /api_routers/ routes, instead, include the operation
+        # (eg, 'delete') in the url, and send it as a 'GET' route. These should include redirect_urls back to the base
+        # route.
+        # '''
+        #
+        # if self.on_delete_callback is not None:
+        #     self.router.add_api_route(
+        #         f"{self.base_route}/delete/{{id}}",
+        #         delete_route(delete_callback=self.on_delete_callback, schema=self.target_schema, redirect_url=f"{self.base_route}"),
+        #         methods=['GET'],
+        #         response_description=f"Delete a {self.target_schema.__name__}",
+        #         response_model=bool,
+        #         status_code=status.HTTP_200_OK
+        #     )
+
+        # '''
+        # Dirty route (used for taking in data in a format we know wont work directly, but can be manipulated to use
+        # the endpoints
+        # '''
+        # if self.dirty_create is not None:
+        #     if self.on_post_callback is None:
+        #         raise NotImplementedError(f"Cannot supply a dirty create without an on_create_callback")
+        #
+        #     self.router.add_api_route(
+        #         f"{self.base_route}/dirty/",
+        #         dirty_post_route(create_callback=self.on_post_callback, schema=self.target_schema, cleaner=self.dirty_create),
+        #         methods=['POST'],
+        #         response_description=f"Create a {self.target_schema.__name__}",
+        #         response_model=self.target_schema,
+        #         status_code=status.HTTP_200_OK
+        #     )
 
 
 
 
 if __name__ == "__main__":
-    from models.ledger import LedgerSchema
-    from api.ledger_router import LedgerMongoCollectionHandler, LedgerFacade
-    from mongo import mongo_utils as utils
-    import config
-
-    ledger_facade_handler = utils.DocumentFacadeHandler(
-        facade_type=LedgerFacade,
-        obj_type=LedgerSchema)
-
-    ledger_collection_handler = LedgerMongoCollectionHandler(
-        db_name='testdb',
-        collection_name='ledger',
-        uri=utils.connection_string_uri(user=config.user(),
-                                        pw=config.pw(),
-                                        uri_template=config.uri_template()),
-        facade_handler=ledger_facade_handler
+    from dataclasses import dataclass
+    from fastapi import FastAPI
+    import uvicorn
+
+    @dataclass
+    class DummyIn:
+        a: str
+        b: int
+        d: Dict
+
+
+    @dataclass
+    class DummyOut:
+        c: Tuple[str, int]
+        e: Dict
+
+    def callback(req: Request, i: DummyIn) -> DummyOut:
+        return DummyOut(c=(i.a, i.b), e=i.d)
+
+    cpac = CallbackPackage(
+        method=RequestType.POST,
+        callback=callback,
+        input_schema=DummyIn,
+        response_schema=DummyOut
     )
 
-    cb: hrh.postRequestCallback = lambda req, T: next(iter(ledger_collection_handler.add_items([T])))
-    shell = ApiShell(schema=LedgerSchema, on_create_callback=cb)
+    shell = ApiShell(base_route='/dummy',
+                     on_post_callback=cpac)
+
+    app = FastAPI()
+    app.include_router(shell.router)
+
+    uvicorn.run(app)
```

### Comparing `coopapi-0.7/coopapi.egg-info/PKG-INFO` & `coopapi-1.0/coopapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.7
+Version: 1.0
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.7/setup.py` & `coopapi-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopapi',
-      version='0.07',
+      version='1.0',
       description='Tools for setting up an API. Built on the FastAPI framework',
       url='https://github.com/tylertjburns/coopapi',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

