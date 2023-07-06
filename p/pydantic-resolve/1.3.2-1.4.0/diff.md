# Comparing `tmp/pydantic_resolve-1.3.2.tar.gz` & `tmp/pydantic_resolve-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.3.2.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.4.0.tar", max compression
```

## Comparing `pydantic_resolve-1.3.2.tar` & `pydantic_resolve-1.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.3.2/LICENSE
--rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.3.2/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.3.2/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2271 2023-06-21 14:55:58.477090 pydantic_resolve-1.3.2/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.3.2/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     6117 2023-06-27 16:04:17.836316 pydantic_resolve-1.3.2/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     4811 2023-07-03 08:00:07.994871 pydantic_resolve-1.3.2/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-03 08:19:26.214453 pydantic_resolve-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.3.2/README.md
--rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.4.0/LICENSE
+-rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.4.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-06 09:03:09.289534 pydantic_resolve-1.4.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     3410 2023-07-06 10:43:29.600208 pydantic_resolve-1.4.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.4.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     6269 2023-07-06 10:42:54.099454 pydantic_resolve-1.4.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     4811 2023-07-03 08:00:07.994871 pydantic_resolve-1.4.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-06 09:59:43.049219 pydantic_resolve-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7660 2023-07-04 04:23:48.147702 pydantic_resolve-1.4.0/README.md
+-rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 pydantic_resolve-1.4.0/PKG-INFO
```

### Comparing `pydantic_resolve-1.3.2/LICENSE` & `pydantic_resolve-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.2/pydantic_resolve/__init__.py` & `pydantic_resolve-1.4.0/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.2/pydantic_resolve/resolver.py` & `pydantic_resolve-1.4.0/pydantic_resolve/resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 import contextvars
 from inspect import iscoroutine
 from typing import TypeVar, Dict
 from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
-from .constant import PREFIX, POST_PREFIX
+from .constant import PREFIX, POST_PREFIX, ATTRIBUTE, RESOLVER
 from .util import get_class_field_annotations
 from inspect import isclass
 from aiodataloader import DataLoader
 
 
 def LoaderDepend(  # noqa: N802
     dependency: Optional[Callable[..., Any]] = None,
@@ -104,42 +104,44 @@
 
                     cache_provider[cache_key] = loader
                     self.ctx.set(cache_provider)
                 params[k] = loader
         return method(**params)
 
 
-    async def resolve_obj(self, target, field):
-        item = target.__getattribute__(field)
+    async def resolve_obj(self, target, field, attr):
         target_attr_name = str(field).replace(PREFIX, '')
 
         if not hasattr(target, target_attr_name):
             raise ResolverTargetAttrNotFound(f"attribute {target_attr_name} not found")
 
         if self.ensure_type:
-            if not item.__annotations__:
+            if not attr.__annotations__:
                 raise MissingAnnotationError(f'{field}: return annotation is required')
 
-        val = self.exec_method(item)
+        val = self.exec_method(attr)
         while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
         val = await self.resolve(val)  
         target.__setattr__(target_attr_name, val)
 
 
     async def resolve(self, target: T) -> T:
         """ entry: resolve dataclass object or pydantic object / or list in place """
-
         if isinstance(target, (list, tuple)):
             await asyncio.gather(*[self.resolve(t) for t in target])
 
         if core.is_acceptable_type(target):
-            await asyncio.gather(*[self.resolve_obj(target, field) 
-                                   for field in core.iter_over_object_resolvers(target)])
+            tasks = []
+            for field, attr, _type in core.iter_over_object_resolvers_and_acceptable_fields(target):
+                if _type == ATTRIBUTE: tasks.append(self.resolve(attr))
+                if _type == RESOLVER: tasks.append(self.resolve_obj(target, field, attr))
+
+            await asyncio.gather(*tasks)
 
             # execute post methods, take no params
             for post_key in core.iter_over_object_post_methods(target):
                 post_attr_name = post_key.replace(POST_PREFIX, '')
                 if not hasattr(target, post_attr_name):
                     raise ResolverTargetAttrNotFound(f"fail to run {post_key}(), attribute {post_attr_name} not found")
```

### Comparing `pydantic_resolve-1.3.2/pydantic_resolve/util.py` & `pydantic_resolve-1.4.0/pydantic_resolve/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.3.2/pyproject.toml` & `pydantic_resolve-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.3.2"
+version = "1.4.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.3.2/PKG-INFO` & `pydantic_resolve-1.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.3.2
+Version: 1.4.0
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -31,14 +31,16 @@
 > A small yet powerful package which can run resolvers to generate deep nested datasets.
 
 [Change log](./changelog.md)
 
 **example**:
 
 ```python
+# prepare dataloader
+
 import asyncio
 from typing import List, Optional
 from pydantic import BaseModel
 from pydantic_resolve import Resolver, mapper, LoaderDepend
 
 # define dataset and loader functions
 async def friends_batch_load_fn(names):
@@ -57,16 +59,19 @@
         'trump': 2011, 'sally': 2012,
     }
     result = []
     for name in names:
         n = mock_db.get(name, None)
         result.append({'number': n} if n else None)
     return result
+```
 
+```python
 # define data schemas
+
 class Contact(BaseModel):
     number: Optional[int]
 
 class Friend(BaseModel):
     name: str
 
     contact: Optional[Contact] = None
@@ -113,14 +118,19 @@
             {"name": "tangkikodo", "age": 19},
             {"name": "john", "age": 20},
             {"name": "trump", "age": 21},
             {"name": "sally", "age": 22},
             {"name": "no man", "age": 23},
         ]
 
+```
+
+```python
+# resolve results
+
 async def main():
     import json
     root = Root()
     root = await Resolver().resolve(root)                 # 4. run it
     dct = root.dict()
     print(json.dumps(dct, indent=4))
 
@@ -178,64 +188,16 @@
             "number": 1004
           },
           "is_contact_10": true
         }
       ],
       "friend_count": 2
     },
-    {
-      "name": "trump",
-      "age": 21,
-      "greeting": "hello, i'm trump, 21 years old.",
-      "contact": {
-        "number": 2011
-      },
-      "friends": [
-        {
-          "name": "sam",
-          "contact": {
-            "number": 1005
-          },
-          "is_contact_10": true
-        },
-        {
-          "name": "jim",
-          "contact": {
-            "number": 1006
-          },
-          "is_contact_10": true
-        }
-      ],
-      "friend_count": 2
-    },
-    {
-      "name": "sally",
-      "age": 22,
-      "greeting": "hello, i'm sally, 22 years old.",
-      "contact": {
-        "number": 2012
-      },
-      "friends": [
-        {
-          "name": "sindy",
-          "contact": {
-            "number": 1007
-          },
-          "is_contact_10": true
-        },
-        {
-          "name": "lydia",
-          "contact": {
-            "number": 1008
-          },
-          "is_contact_10": true
-        }
-      ],
-      "friend_count": 2
-    },
+    ...
+    ,
     {
       "name": "no man",
       "age": 23,
       "greeting": "hello, i'm no man, 23 years old.",
       "contact": null,
       "friends": [],
       "friend_count": 0
@@ -249,21 +211,64 @@
 ```shell
 pip install pydantic-resolve
 ```
 
 - use `resolve` for simple scenario,
 - use `Resolver` and `LoaderDepend` for complicated nested batch query.
 
-```python
-from pydantic_resolve import (
-    resolve,                     # handle simple resolving task
-    Resolver, LoaderDepend,      # handle schema resolving with LoaderDepend and DataLoader
-    ResolverTargetAttrNotFound, DataloaderDependCantBeResolved, LoaderFieldNotProvidedError  # errors
-)
-```
+## API
+
+`Resolver(loader_filters, loader_instances, ensure_type)`
+
+- `loader_filters`
+
+  provide extra query filters along with loader key.
+
+  detail: `examples/6_sqlalchemy_loaderdepend_global_filter.py` L55, L59
+
+- `loader_instances`
+
+  provide pre-created loader instance, with can `prime` data into loader cache.
+
+  detail: `tests/resolver/test_20_loader_instance.py`, L62, L63
+
+- `ensure_type`
+
+  if `True`, resolve method is restricted to be annotated.
+
+  detail: `tests/resolver/test_13_check_wrong_type`
+
+`LoaderDepend(loader_fn)`
+
+- `loader_fn`: subclass of DataLoader or batch_load_fn. [detail](https://github.com/syrusakbary/aiodataloader#dataloaderbatch_load_fn-options)
+
+  declare dataloader dependency, `pydantic-resolve` will take the care of lifecycle of dataloader.
+
+`build_list(rows, keys, fn)` & `build_object(rows, keys, fn)`
+
+- `rows`: query result
+- `keys`: batch_load_fn:keys
+- `fn`: define the way to get primary key
+
+  helper function to generate return value required by `batch_load_fn`. read the code for details.
+
+`mapper(param)`
+
+- `param`: can be either a class of pydantic or dataclass, or a lambda.
+
+  `pydantic-resolve` will trigger the fn in `mapper` after inner future is resolved. it exposes an interface to change return schema even from the same dataloader.
+  if param is a class, it will try to automatically transform it.
+
+`ensure_subset(base_class)`
+
+- `base_class`: pydantic class
+
+  it can raise exception if fields of decorated class has field not existed in `base_class`.
+
+  detail: `tests/utils/test_2_ensure_subset.py`
 
 ## Run FastAPI example
 
 ```shell
 poetry shell
 cd examples
 uvicorn fastapi_demo.main:app
```

