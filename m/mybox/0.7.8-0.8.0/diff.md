# Comparing `tmp/mybox-0.7.8.tar.gz` & `tmp/mybox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybox-0.7.8.tar", max compression
+gzip compressed data, was "mybox-0.8.0.tar", max compression
```

## Comparing `mybox-0.7.8.tar` & `mybox-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,35 @@
--rw-r--r--   0        0        0    34916 2023-04-21 00:05:38.974069 mybox-0.7.8/LICENSE.md
--rw-r--r--   0        0        0     1463 2023-04-21 00:05:38.974069 mybox-0.7.8/README.md
--rw-r--r--   0        0        0        0 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/__init__.py
--rw-r--r--   0        0        0     2558 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/compute.py
--rw-r--r--   0        0        0      932 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/configparser.py
--rw-r--r--   0        0        0     9803 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/driver.py
--rw-r--r--   0        0        0     2406 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/filters.py
--rw-r--r--   0        0        0     1281 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/main.py
--rw-r--r--   0        0        0     3198 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/manager.py
--rw-r--r--   0        0        0     1135 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/__init__.py
--rw-r--r--   0        0        0     6797 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/archive.py
--rw-r--r--   0        0        0     2047 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/base.py
--rw-r--r--   0        0        0     2018 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/clone.py
--rw-r--r--   0        0        0      339 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/destination.py
--rw-r--r--   0        0        0     3330 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/github.py
--rw-r--r--   0        0        0     8997 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/installer.py
--rw-r--r--   0        0        0     1985 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/links.py
--rw-r--r--   0        0        0     4788 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/manual.py
--rw-r--r--   0        0        0      792 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/manual_version.py
--rw-r--r--   0        0        0     1567 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/npm.py
--rw-r--r--   0        0        0      907 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/pip.py
--rw-r--r--   0        0        0     1577 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/pip_base.py
--rw-r--r--   0        0        0      931 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/pipx.py
--rw-r--r--   0        0        0      500 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/root.py
--rw-r--r--   0        0        0     1794 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/shell.py
--rw-r--r--   0        0        0     2347 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/system.py
--rw-r--r--   0        0        0     1402 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/tracked.py
--rw-r--r--   0        0        0      621 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/url.py
--rw-r--r--   0        0        0     1634 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/yum_repo.py
--rw-r--r--   0        0        0     2602 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/parallel.py
--rw-r--r--   0        0        0      141 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/__init__.py
--rw-r--r--   0        0        0     4142 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/base.py
--rw-r--r--   0        0        0      315 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/installed.py
--rw-r--r--   0        0        0      160 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/version.py
--rw-r--r--   0        0        0     3626 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/utils.py
--rw-r--r--   0        0        0     2120 2023-04-21 00:06:00.114082 mybox-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 mybox-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-07-05 23:00:10.291915 mybox-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0     1463 2023-07-05 23:00:10.291915 mybox-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/__init__.py
+-rw-r--r--   0        0        0     2558 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/compute.py
+-rw-r--r--   0        0        0      932 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/configparser.py
+-rw-r--r--   0        0        0     9717 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/driver.py
+-rw-r--r--   0        0        0     2406 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/filters.py
+-rw-r--r--   0        0        0     1281 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/main.py
+-rw-r--r--   0        0        0     3198 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/manager.py
+-rw-r--r--   0        0        0     1082 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/__init__.py
+-rw-r--r--   0        0        0     6797 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/archive.py
+-rw-r--r--   0        0        0     2047 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/base.py
+-rw-r--r--   0        0        0     2018 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/clone.py
+-rw-r--r--   0        0        0      339 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/destination.py
+-rw-r--r--   0        0        0     3330 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/github.py
+-rw-r--r--   0        0        0     8997 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/installer.py
+-rw-r--r--   0        0        0     1985 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/links.py
+-rw-r--r--   0        0        0     4788 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/manual.py
+-rw-r--r--   0        0        0      792 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/manual_version.py
+-rw-r--r--   0        0        0     1567 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/npm.py
+-rw-r--r--   0        0        0     2249 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/pipx.py
+-rw-r--r--   0        0        0      500 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/root.py
+-rw-r--r--   0        0        0     1794 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/shell.py
+-rw-r--r--   0        0        0     2347 2023-07-05 23:00:10.291915 mybox-0.8.0/mybox/package/system.py
+-rw-r--r--   0        0        0     1402 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/package/tracked.py
+-rw-r--r--   0        0        0      621 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/package/url.py
+-rw-r--r--   0        0        0     1634 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/package/yum_repo.py
+-rw-r--r--   0        0        0     2602 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/parallel.py
+-rw-r--r--   0        0        0      141 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/state/__init__.py
+-rw-r--r--   0        0        0     4142 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/state/base.py
+-rw-r--r--   0        0        0      315 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/state/installed.py
+-rw-r--r--   0        0        0      160 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/state/version.py
+-rw-r--r--   0        0        0     3626 2023-07-05 23:00:10.295915 mybox-0.8.0/mybox/utils.py
+-rw-r--r--   0        0        0     2121 2023-07-05 23:00:31.027793 mybox-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 mybox-0.8.0/PKG-INFO
```

### Comparing `mybox-0.7.8/LICENSE.md` & `mybox-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/README.md` & `mybox-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/compute.py` & `mybox-0.8.0/mybox/compute.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/configparser.py` & `mybox-0.8.0/mybox/configparser.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/driver.py` & `mybox-0.8.0/mybox/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 from abc import ABCMeta, abstractmethod
-from contextlib import AsyncExitStack, asynccontextmanager
+from contextlib import asynccontextmanager, nullcontext
 from dataclasses import dataclass
 from os import environ
 from pathlib import Path
 from typing import (
     Any,
     AsyncContextManager,
     AsyncIterator,
@@ -242,16 +242,15 @@
             stderr = None
 
         # https://github.com/python/mypy/issues/5512
         cm: AsyncContextManager
         if show_output:
             cm = parallel_map_pause()
         else:
-            # Should be nullcontext, but it is not async-enabled in Python 3.9.
-            cm = AsyncExitStack()
+            cm = nullcontext()
         async with cm:
             result = await run_process(
                 command,
                 check=check,
                 stdin=input,
                 capture_stdout=not show_output,
                 stderr=stderr,
```

### Comparing `mybox-0.7.8/mybox/filters.py` & `mybox-0.8.0/mybox/filters.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/main.py` & `mybox-0.8.0/mybox/main.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/manager.py` & `mybox-0.8.0/mybox/manager.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/__init__.py` & `mybox-0.8.0/mybox/package/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 from ..driver import Driver
 from ..state import DB
 from .base import Package
 from .clone import Clone
 from .github import GitHubPackage
 from .links import Links
 from .npm import NpmPackage
-from .pip import PipPackage
 from .pipx import PipxPackage
 from .shell import Shell
 from .system import SystemPackage
 from .url import URLPackage
 from .yum_repo import YumRepo
 
 TYPES: list[Tuple[str, Type[Package]]] = [
     ("name", SystemPackage),
     ("repo", GitHubPackage),
     ("url", URLPackage),
     ("clone", Clone),
     ("npm", NpmPackage),
-    ("pip", PipPackage),
     ("pipx", PipxPackage),
     ("shell", Shell),
     ("links", Links),
     ("yum_name", YumRepo),
 ]
```

### Comparing `mybox-0.7.8/mybox/package/archive.py` & `mybox-0.8.0/mybox/package/archive.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/base.py` & `mybox-0.8.0/mybox/package/base.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/clone.py` & `mybox-0.8.0/mybox/package/clone.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/github.py` & `mybox-0.8.0/mybox/package/github.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/installer.py` & `mybox-0.8.0/mybox/package/installer.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/links.py` & `mybox-0.8.0/mybox/package/links.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/manual.py` & `mybox-0.8.0/mybox/package/manual.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/manual_version.py` & `mybox-0.8.0/mybox/package/manual_version.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/npm.py` & `mybox-0.8.0/mybox/package/npm.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/pip_base.py` & `mybox-0.8.0/mybox/package/pipx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,38 @@
+import json
 import re
-from abc import ABC, abstractmethod
 from typing import Optional, cast
 
 import requests
+from pydantic import Field, validator
 
 from .base import Package
 
 PIP = ["python3", "-m", "pip"]
 
 
-class PipBasePackage(Package, ABC):
-    package: str
+class PipxPackage(Package):
+    package: str = Field(..., alias="pipx")
+
+    @validator("package")
+    def package_to_lower(cls, value: str) -> str:  # pylint: disable=no-self-argument
+        return value.lower()
 
     @property
     def name(self) -> str:
         return self.package
 
-    @abstractmethod
     async def get_all_versions(self) -> dict[str, str]:
-        pass
+        pipx_list = json.loads(
+            await self.driver.run_output("pipx", "list", "--json", silent=True)
+        )
+        packages = (
+            item["metadata"]["main_package"] for item in pipx_list["venvs"].values()
+        )
+        return {package["package"]: package["package_version"] for package in packages}
 
     async def local_version(self) -> Optional[str]:
         return (await self.get_all_versions()).get(self.package)
 
     async def _get_pypi_version(self) -> Optional[str]:
         pypi_info = requests.get(f"https://pypi.org/pypi/{self.package}/json").json()
         try:
@@ -52,7 +62,12 @@
         if version := await self._get_pypi_version():
             return version
 
         if version := await self._get_index_version():
             return version
 
         raise Exception(f"Cannot find latest version of package '{self.package}'.")
+
+    async def install(self) -> None:
+        cmd = "install" if await self.local_version() is None else "upgrade"
+        await self.driver.run("pipx", cmd, self.package)
+        await super().install()
```

### Comparing `mybox-0.7.8/mybox/package/shell.py` & `mybox-0.8.0/mybox/package/shell.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/system.py` & `mybox-0.8.0/mybox/package/system.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/tracked.py` & `mybox-0.8.0/mybox/package/tracked.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/url.py` & `mybox-0.8.0/mybox/package/url.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/package/yum_repo.py` & `mybox-0.8.0/mybox/package/yum_repo.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/parallel.py` & `mybox-0.8.0/mybox/parallel.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/state/base.py` & `mybox-0.8.0/mybox/state/base.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/mybox/utils.py` & `mybox-0.8.0/mybox/utils.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.8/pyproject.toml` & `mybox-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "mybox"
-version = "v0.7.8"
+version = "v0.8.0"
 description = "Manage the configuration and tools on your workstation without bothering the OS too much"
 readme = "README.md"
 repository = "https://github.com/koterpillar/mybox"
 authors = ["Alexey Kotlyarov <a@koterpillar.com>"]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 pydantic = "^1.10.7"
-python = "^3.9"
+python = "^3.11"
 PyYAML = "^6.0"
 requests = "^2.28.2"
 trio = "^0.22.0"
 tqdm = "^4.64.1"
 typed-argparse = "^0.2.9"
 jsonpath-ng = "^1.5.3"
 beautifulsoup4 = "^4.11.2"
```

### Comparing `mybox-0.7.8/PKG-INFO` & `mybox-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: mybox
-Version: 0.7.8
+Version: 0.8.0
 Summary: Manage the configuration and tools on your workstation without bothering the OS too much
 Home-page: https://github.com/koterpillar/mybox
 License: GPL-3.0-or-later
 Author: Alexey Kotlyarov
 Author-email: a@koterpillar.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
```

