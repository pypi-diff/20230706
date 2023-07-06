# Comparing `tmp/muffin-0.98.8.tar.gz` & `tmp/muffin-0.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.98.8.tar", max compression
+gzip compressed data, was "muffin-0.99.1.tar", max compression
```

## Comparing `muffin-0.98.8.tar` & `muffin-0.99.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-06-21 08:00:37.152881 muffin-0.98.8/README.rst
--rw-r--r--   0        0        0      982 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/__init__.py
--rw-r--r--   0        0        0     5257 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/app.py
--rw-r--r--   0        0        0       71 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/errors.py
--rw-r--r--   0        0        0     3794 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/handler.py
--rw-r--r--   0        0        0     8814 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/manage.py
--rw-r--r--   0        0        0     2877 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/types.py
--rw-r--r--   0        0        0     2888 2023-06-21 08:00:37.152881 muffin-0.98.8/muffin/utils.py
--rw-r--r--   0        0        0     2990 2023-06-21 08:00:37.152881 muffin-0.98.8/pyproject.toml
--rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.98.8/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-07-06 09:15:53.036352 muffin-0.99.1/README.rst
+-rw-r--r--   0        0        0      982 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/__init__.py
+-rw-r--r--   0        0        0     5213 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/errors.py
+-rw-r--r--   0        0        0     3755 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/handler.py
+-rw-r--r--   0        0        0     8820 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/manage.py
+-rw-r--r--   0        0        0     2877 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/types.py
+-rw-r--r--   0        0        0     2905 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/utils.py
+-rw-r--r--   0        0        0     2990 2023-07-06 09:15:53.044352 muffin-0.99.1/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.99.1/PKG-INFO
```

### Comparing `muffin-0.98.8/README.rst` & `muffin-0.99.1/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.98.8/muffin/__init__.py` & `muffin-0.99.1/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.8/muffin/app.py` & `muffin-0.99.1/muffin/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     from types import ModuleType
 
     from asgi_tools.types import TASGIReceive, TASGIScope, TASGISend
 
     from muffin.plugins import BasePlugin
 
 BACKGROUND_TASK: Final["ContextVar[set[Awaitable] | None]"] = ContextVar(
-    "background_tasks",
-    default=None,
+    "background_tasks", default=None
 )
 
 
 class Application(BaseApp):
     """The Muffin Application."""
 
     # Default configuration values
@@ -97,20 +96,15 @@
             static_url_prefix=self.cfg.STATIC_URL_PREFIX,
         )
 
     def __repr__(self) -> str:
         """Human readable representation."""
         return f"<muffin.Application: { self.cfg.name }>"
 
-    async def __call__(
-        self,
-        scope: TASGIScope,
-        receive: TASGIReceive,
-        send: TASGISend,
-    ):
+    async def __call__(self, scope: TASGIScope, receive: TASGIReceive, send: TASGISend):
         """Support background tasks."""
         await self.lifespan(scope, receive, send)
         bgtasks = BACKGROUND_TASK.get()
         if bgtasks is not None:
             await aio_wait(*bgtasks)
             BACKGROUND_TASK.set(None)
```

### Comparing `muffin-0.98.8/muffin/errors.py` & `muffin-0.99.1/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.8/muffin/handler.py` & `muffin-0.99.1/muffin/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,15 @@
     from http_router import Router
     from http_router.types import TMethods, TMethodsArg
 
 
 class HandlerMeta(type):
     """Prepare handlers."""
 
-    def __new__(
-        mcs: Type[HandlerMeta],
-        name: str,
-        bases: Tuple[type],
-        params: Dict[str, Any],
-    ):
+    def __new__(mcs: Type[HandlerMeta], name: str, bases: Tuple[type], params: Dict[str, Any]):
         """Prepare a Handler Class."""
         cls = cast(Type["Handler"], super().__new__(mcs, name, bases, params))
 
         # Ensure that the class methods are exist and iterable
         if not cls.methods:
             cls.methods = [method for method in HTTP_METHODS if method.lower() in cls.__dict__]
```

### Comparing `muffin-0.98.8/muffin/manage.py` & `muffin-0.99.1/muffin/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import os
 import re
 import sys
 from contextlib import AsyncExitStack, suppress
 from importlib import metadata
 from pathlib import Path
-from typing import TYPE_CHECKING, AsyncContextManager, Callable, Mapping, Optional, overload
+from typing import TYPE_CHECKING, AsyncContextManager, Callable, Dict, Optional, overload
 
 from muffin.constants import CONFIG_ENV_VARIABLE
 from muffin.errors import AsyncRequiredError
 from muffin.utils import AIOLIB, AIOLIBS, aio_lib, aio_run, import_app
 
 if TYPE_CHECKING:
     from asgi_tools.types import TVCallable
@@ -67,15 +67,15 @@
                 type=str,
                 choices=list(AIOLIBS.keys()),
                 default=aio_lib(),
                 help="Select an asyncio library to run commands.",
             )
 
         self.subparsers = self.parser.add_subparsers(dest="subparser")
-        self.commands: Mapping[str, Callable] = {}
+        self.commands: Dict[str, Callable] = {}  # noqa: FA
 
         self.shell(
             getattr(
                 app.cfg,
                 "MANAGE_SHELL",
                 lambda: dict(
                     app=app,
```

### Comparing `muffin-0.98.8/muffin/plugins.py` & `muffin-0.99.1/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.8/muffin/pytest.py` & `muffin-0.99.1/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.98.8/muffin/utils.py` & `muffin-0.99.1/muffin/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     to_import = module_names or (name for _, name, _ in pkgutil.walk_packages(package.__path__))
     if exclude:
         to_import = (name for name in to_import if name not in exclude)
 
     for module_name in to_import:
         try:
             res[module_name] = importlib.import_module(f"{package_name}.{module_name}")
-        except ImportError:
+        except ImportError:  # noqa: PERF203
             if not silent:
                 raise
 
             logger.debug("Failed to import module: %s", f"{package_name}.{module_name}")
 
     return res
```

### Comparing `muffin-0.98.8/pyproject.toml` & `muffin-0.99.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.98.8"
+version = "0.99.1"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.98.8/PKG-INFO` & `muffin-0.99.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.98.8
+Version: 0.99.1
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

