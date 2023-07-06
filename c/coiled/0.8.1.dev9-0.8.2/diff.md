# Comparing `tmp/coiled-0.8.1.dev9.tar.gz` & `tmp/coiled-0.8.2.tar.gz`

## Comparing `coiled-0.8.1.dev9.tar` & `coiled-0.8.2.tar`

### file list

```diff
@@ -1,63 +1,62 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/analytics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/context.py
--rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    25059 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/magic.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/run.py
--rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/types.py
--rw-r--r--   0        0        0    53902 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/authenticate.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    45735 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.1.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/analytics.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/context.py
+-rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/exceptions.py
+-rw-r--r--   0        0        0    25059 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/magic.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/run.py
+-rw-r--r--   0        0        0    19853 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/types.py
+-rw-r--r--   0        0        0    54058 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    45637 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26637 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.2/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.2/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.2/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 coiled-0.8.2/PKG-INFO
```

### Comparing `coiled-0.8.1.dev9/coiled/__init__.py` & `coiled-0.8.2/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/analytics.py` & `coiled-0.8.2/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cluster.py` & `coiled-0.8.2/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/coiled.yaml` & `coiled-0.8.2/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/context.py` & `coiled-0.8.2/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/core.py` & `coiled-0.8.2/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/exceptions.py` & `coiled-0.8.2/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/magic.py` & `coiled-0.8.2/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/run.py` & `coiled-0.8.2/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/scan.py` & `coiled-0.8.2/coiled/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from base64 import urlsafe_b64encode
 from collections import defaultdict
 from logging import getLogger
 from pathlib import Path
 from typing import Dict, List, Optional, Union, cast
 from urllib.parse import urlparse
 
-from importlib_metadata import Distribution, PackagePath
+from importlib_metadata import Distribution, PackagePath, PathDistribution
 from packaging.version import InvalidVersion
 from packaging.version import parse as parse_version
 from rich.progress import Progress
 from typing_extensions import Literal
 
 from coiled.types import CondaPackage, CondaPlaceHolder, PackageInfo
 from coiled.utils import parse_file_uri
 
 logger = getLogger("coiled.package_sync")
 subdir_datas = {}
 PYTHON_VERSION = platform.python_version_tuple()
 
 
-class ResilientDistribution(Distribution):
+class ResilientDistribution(PathDistribution):
     """Subclass of Distribution that adds more resilient methods for retrieving files"""
 
     def _read_files_egginfo_installed(self):
         """
         Read installed-files.txt and return lines in a similar
         CSV-parsable format as RECORD: each file should be placed
         relative to the site-packages directory and must be
@@ -40,15 +40,15 @@
         but it might not be written for other installation methods.
         Assume the file is accurate if it exists.
         """
         text = self.read_text("installed-files.txt")
         # Prepend the .egg-info/ subdir to the lines in this file.
         # But this subdir is only available from PathDistribution's
         # self._path.
-        subdir = getattr(self, "_path", None)
+        subdir = self._path
         if not text or not subdir:
             return
 
         site_pkgs_path = cast(Path, self.locate_file("")).resolve()
         for name in text.splitlines():
             # relpath will add .. to a path to make it relative to site-packages,
             # so use that instead of Path.relative_to (which will raise an error)
@@ -114,15 +114,15 @@
     if metadata_location:
         if not metadata_location.exists():
             # a file for this package no longer exists
             # likely pip installed a new version
             # removing the conda installed version
             return None
         else:
-            dist = ResilientDistribution.at(pkg.prefix / metadata_location)
+            dist = ResilientDistribution(pkg.prefix / metadata_location)  # type: ignore
             name = dist.metadata["Name"] or pkg.name
     else:
         name = pkg.name
     return {
         "channel": pkg.channel,
         "path": None,
         "channel_url": pkg.channel_url,
@@ -287,15 +287,16 @@
                     elif line.rstrip() == ".":
                         continue
                     else:
                         p = location / Path(line.rstrip())
                         full_path = str(p.resolve())
                         if p.exists() and full_path not in paths:
                             paths.append(full_path)
-    dists: List[Distribution] = [dist for dist in ResilientDistribution.discover(path=list(paths))]
+    # can't use ResilientDistribution here properly without monkey patching it
+    dists: List[Distribution] = [dist for dist in Distribution.discover(path=list(paths))]
     packages = []
     if progress:
         for task in progress.track(
             asyncio.as_completed([handle_dist(dist, locations) for dist in dists]),
             total=len(dists),
             description=f"Scanning {len(dists)} python packages",
         ):
@@ -311,16 +312,16 @@
             # For duplicate .dist-info directories, we need to check which
             # version is actually importable
             existing_pkg = pkgs_by_name.get(pkg_name)
             if existing_pkg is None:
                 pkgs_by_name[pkg_name] = pkg
             else:
                 # Compare hashes to actual files
-                new_dist = ResilientDistribution.at(pkg["path"])
-                old_dist = ResilientDistribution.at(existing_pkg["path"])
+                new_dist = ResilientDistribution(pkg["path"])
+                old_dist = ResilientDistribution(existing_pkg["path"])
                 new_dist_path = new_dist._path  # type: ignore
                 old_dist_path = old_dist._path  # type: ignore
                 new_is_egg_info = new_dist_path.name.endswith(".egg-info")  # type: ignore
                 old_is_egg_info = old_dist_path.name.endswith(".egg-info")  # type: ignore
                 new_is_dist_info = new_dist_path.name.endswith(".dist-info")  # type: ignore
                 old_is_dist_info = old_dist_path.name.endswith(".dist-info")  # type: ignore
                 if (new_is_egg_info and not old_is_egg_info) or (new_is_dist_info and not old_is_dist_info):
```

### Comparing `coiled-0.8.1.dev9/coiled/software.py` & `coiled-0.8.2/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/types.py` & `coiled-0.8.2/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/utils.py` & `coiled-0.8.2/coiled/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,15 @@
     *,
     server: Optional[str] = None,
     token: Optional[str] = None,
     account: Optional[str] = None,
     save: Optional[bool] = None,
     use_config: bool = True,
     retry: bool = True,
+    browser: Optional[bool] = None,
 ):
     # "save" bool means always/never, None means try to do the thing that makes sense
     if save is None:
         # if token is already set in config and isn't being changed, then no need to save again
         if dask.config.get("coiled.token", None) and (not token or token == dask.config.get("coiled.token")):
             save = False
         else:
@@ -266,15 +267,15 @@
         server = server or dask.config.get("coiled.server")
         if "://" not in server:
             server = "http://" + server
         server = server.rstrip("/")
         account = account or dask.config.get("coiled.account")
 
     try:
-        await handle_credentials(server=server, token=token, account=account, save=save, retry=retry)
+        await handle_credentials(server=server, token=token, account=account, save=save, retry=retry, browser=browser)
     except ImportError as e:
         rich.print(f"[red]{e}")
 
 
 @backoff.on_exception(backoff.expo, ApiResponseStatusError, logger=logger)
 async def _fetch_data(*, session, server, endpoint):
     response = await session.request("GET", f"{server}{endpoint}")
@@ -297,14 +298,15 @@
     *,
     server: Optional[str] = None,
     token: Optional[str] = None,
     account: Optional[str] = None,
     save: Optional[bool] = None,
     retry: bool = True,
     print_invalid_token_messages: bool = True,
+    browser: Optional[bool] = None,
 ) -> Tuple[str, str, str]:
     """Validate and optionally save credentials
 
     Parameters
     ----------
     server
         Server to connect to. If not specified, will check the
@@ -335,24 +337,27 @@
     """
     if account:
         validate_account(account)
     # If testing locally with `ngrok` we need to
     # rewrite the server to localhost
     server = server or dask.config.get("coiled.server", COILED_SERVER)
     server = normalize_server(server)
-    login_url = f"{server}/profile?createTokenDialog=1"
+
+    browser = True if browser is None else browser
+
     if token is None:
-        rich.print(f"Please login to [link]{login_url}[/link] to get your token")
-        # Using click instead of getpass to make testing easier
-        token = click.prompt("Token", hide_input=True)
-        if not token:
-            raise ValueError(
-                "Token not provided, unable to login. You can create new tokens and "
-                f"managing your existing ones at {server}/profile?createTokenDialog=1 .\n"
-            )
+        from .auth import client_token_grant_flow
+
+        result = await client_token_grant_flow(server, browser)
+        if result:
+            return result
+        raise ValueError(
+            "Authorization failed. Please try to login again, and if the error persists, "
+            "please reach out to Coiled Support at support@coiled.io"
+        )
 
     # TODO: revert when we remove versioneer
     if dask.config.get("coiled.no-minimum-version-check", False):
         client_version = "coiled-frontend-js"
     else:
         client_version = COILED_VERSION
     account_usage = {}
@@ -367,21 +372,23 @@
             user_dict = await _fetch_data(
                 session=session,
                 server=server,
                 endpoint="/api/v2/user/me",
             )
         except AuthenticationError:
             if print_invalid_token_messages:
-                rich.print(
-                    "[red]Invalid Coiled token encountered. You can create new tokens and manage "
-                    f"your existing ones at {server}/profile?createTokenDialog=1 .\n"
-                )
+                rich.print("[red]Invalid Coiled token encountered[/red]")
             if retry:
                 return await handle_credentials(server=server, token=None, account=account, save=None, retry=False)
             else:
+                if print_invalid_token_messages:
+                    rich.print(
+                        "You can use [green]coiled login[/green] to authorize a new token for your Coiled client, "
+                        "or contact us at support@coiled.io if you continue to have problems."
+                    )
                 raise
         memberships = await _fetch_data(session=session, server=server, endpoint="/api/v2/user/me/memberships")
         if not isinstance(memberships, list) or not memberships:
             account_membership = None
         else:
             account_membership = get_account_membership(user_dict, memberships, account=account)
         # only validate if account arg is provided by user
```

### Comparing `coiled-0.8.1.dev9/coiled/websockets.py` & `coiled-0.8.2/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/authenticate.py` & `coiled-0.8.2/coiled/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import asyncio
 import webbrowser
 
 import aiohttp
-import click
 import dask.config
 import rich
 
-from ..exceptions import AuthenticationError
-from ..utils import COILED_SERVER, handle_credentials
-from .utils import CONTEXT_SETTINGS
-
-
-async def make_unattached_token(server, label=None) -> dict:
-    url = server + "/api/v1/api-tokens-no-user/"
-    async with aiohttp.ClientSession() as session:
-        async with session.post(url, data={"label": label}) as resp:
-            return await resp.json()
+from .exceptions import AuthenticationError
+from .utils import COILED_SERVER, handle_credentials
 
 
 def get_local_user() -> str:
     try:
         import getpass
         import socket
 
         local_user = f"{getpass.getuser()}@{socket.gethostname()}"
     except Exception:
         local_user = ""
     return local_user
 
 
-async def new_token_flow(server, browser):
+async def make_unattached_token(server, label=None) -> dict:
+    url = server + "/api/v1/api-tokens-no-user/"
+    async with aiohttp.ClientSession() as session:
+        async with session.post(url, data={"label": label}) as resp:
+            return await resp.json()
+
+
+async def client_token_grant_flow(server, browser):
     server = server or dask.config.get("coiled.server", COILED_SERVER)
 
     token_data = await make_unattached_token(server, label=get_local_user())
 
     token_identifier = token_data["identifier"]
     token_secret = token_data["token"]
 
@@ -43,24 +41,14 @@
         webbrowser.open(url, new=2)
 
     rich.print(f"\nVisit the following URL to authorize this computer:\n\n\t{url}\n")
 
     retries = 60
     while retries > 0:
         try:
-            await handle_credentials(
+            return await handle_credentials(
                 server=server, token=token_secret, save=True, retry=False, print_invalid_token_messages=False
             )
         except AuthenticationError:
-            # still waiting for user to do their their
+            # still waiting for user to authorize the token
             retries -= 1
             await asyncio.sleep(1)
-        else:
-            break
-
-
-@click.command(context_settings=CONTEXT_SETTINGS)
-@click.option("--browser/--no-browser", default=True, help="Open browser with page where you grant access")
-@click.option("-s", "--server", help="Coiled server to use", hidden=True)
-def authenticate(browser, server):
-    """Conveniently configure your Coiled account credentials"""
-    asyncio.run(new_token_flow(server, browser))
```

### Comparing `coiled-0.8.1.dev9/coiled/cli/config.py` & `coiled-0.8.2/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/core.py` & `coiled-0.8.2/coiled/cli/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import click
 
 from ..compatibility import COILED_VERSION
-from .authenticate import authenticate
 from .cluster import cluster
 from .config import config
 from .curl import curl
 from .diagnostics import diagnostics
 from .env import env
 from .login import login
 from .notebook import notebook
@@ -31,8 +30,7 @@
 cli.add_command(cluster)
 cli.add_command(notebook)
 cli.add_command(package_sync)
 cli.add_command(prefect)
 cli.add_command(curl)
 cli.add_command(config)
 cli.add_command(run)
-cli.add_command(authenticate)
```

### Comparing `coiled-0.8.1.dev9/coiled/cli/curl.py` & `coiled-0.8.2/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/env.py` & `coiled-0.8.2/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/login.py` & `coiled-0.8.2/coiled/cli/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 import click
 
 from ..utils import login_if_required
 from .utils import CONTEXT_SETTINGS
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
-@click.option("-s", "--server", help="Coiled server to use")
+@click.option("-s", "--server", help="Coiled server to use", hidden=True)
 @click.option("-t", "--token", help="Coiled user token")
 @click.option("-a", "--account", help="Coiled account")
 @click.option(
     "--retry/--no-retry",
     default=True,
     help="Whether or not to automatically ask for a new token if an invalid token is entered",
 )
-def login(server, token, account, retry):
+@click.option("--browser/--no-browser", default=True, help="Open browser with page where you grant access")
+def login(server, token, account, retry, browser):
     """Configure your Coiled account credentials"""
     asyncio.run(
-        login_if_required(server=server, token=token, account=account, save=True, use_config=False, retry=retry)
+        login_if_required(
+            server=server, token=token, account=account, save=True, use_config=False, retry=retry, browser=browser
+        )
     )
```

### Comparing `coiled-0.8.1.dev9/coiled/cli/package_sync.py` & `coiled-0.8.2/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/prefect.py` & `coiled-0.8.2/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/run.py` & `coiled-0.8.2/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/utils.py` & `coiled-0.8.2/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.8.2/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.8.2/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/cluster/logs.py` & `coiled-0.8.2/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/cluster/metrics.py` & `coiled-0.8.2/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.8.2/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/cluster/utils.py` & `coiled-0.8.2/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.8.2/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.8.2/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/setup/__init__.py` & `coiled-0.8.2/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/setup/amp.py` & `coiled-0.8.2/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/setup/aws.py` & `coiled-0.8.2/coiled/cli/setup/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import jsondiff
 from rich import print
 from rich.panel import Panel
 from rich.prompt import Confirm, IntPrompt
 
 import coiled
 
+from ...auth import get_local_user
 from ..utils import CONTEXT_SETTINGS
 from .util import setup_failure
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--iam-user",
@@ -82,15 +83,15 @@
     "--accept-delete",
     default=False,
     is_flag=True,
     hidden=True,
     help="use with --yes if you also want to accept deletes",
 )
 @click.option(
-    "--use-new",
+    "--use-shim",
     default=False,
     is_flag=True,
     hidden=True,
     help="Use new setup backend",
 )
 def aws_setup(
     iam_user: str,
@@ -873,21 +874,15 @@
     cloudshell_link=None,
     manual_final_setup=None,
     quotas=None,
     yes=False,
     accept_delete=False,
     use_shim=False,
 ) -> bool:
-    try:
-        import getpass
-        import socket
-
-        local_user = f"{getpass.getuser()}@{socket.gethostname()}"
-    except Exception:
-        local_user = ""
+    local_user = get_local_user()
 
     # TODO check for Coiled login, explain that we need this to automatically do Coiled setup, but they can do manually
     # call coiled.Cloud() here if we want to ensure/force log in -- is there way to just check?
     coiled.add_interaction(
         action="CliSetupAws",
         success=True,
         local_user=local_user,
```

### Comparing `coiled-0.8.1.dev9/coiled/cli/setup/entry.py` & `coiled-0.8.2/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/cli/setup/gcp.py` & `coiled-0.8.2/coiled/cli/setup/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from rich import print
 from rich.panel import Panel
 from rich.prompt import Confirm
 from rich.table import Table
 
 import coiled
 
+from ...auth import get_local_user
 from ..utils import CONTEXT_SETTINGS
 from .util import setup_failure
 
 # names to use when tracking actions
 ACTION_INIT = "init"
 ACTION_CREATE_GAR = "gar:create"
 ACTION_BIND_GAR = "gar:policy-binding"
@@ -376,21 +377,15 @@
     manual_final_setup=False,
     quotas=False,
     quota_link=False,
     export=None,
     iam_user="coiled",
     yes=False,
 ):
-    try:
-        import getpass
-        import socket
-
-        local_user = f"{getpass.getuser()}@{socket.gethostname()}"
-    except Exception:
-        local_user = ""
+    local_user = get_local_user()
 
     coiled.add_interaction(
         action="CliSetupGcp",
         success=True,
         local_user=local_user,
         # use keys that match the cli args
         region=region,
```

### Comparing `coiled-0.8.1.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.8.2/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/extensions/prefect/runners.py` & `coiled-0.8.2/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/extensions/prefect/workers.py` & `coiled-0.8.2/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/__init__.py` & `coiled-0.8.2/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/cluster.py` & `coiled-0.8.2/coiled/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/core.py` & `coiled-0.8.2/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/cwi_log_link.py` & `coiled-0.8.2/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/states.py` & `coiled-0.8.2/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/widgets/__init__.py` & `coiled-0.8.2/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/widgets/rich.py` & `coiled-0.8.2/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/coiled/v2/widgets/util.py` & `coiled-0.8.2/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/LICENSE` & `coiled-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/README.md` & `coiled-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/pyproject.toml` & `coiled-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.1.dev9/PKG-INFO` & `coiled-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.1.dev9
+Version: 0.8.2
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.8.1.dev9 Project-URL: Homepage,
-https://coiled.io Maintainer-email: Coiled
+Metadata-Version: 2.1 Name: coiled Version: 0.8.2 Project-URL: Homepage, https:
+//coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
 rich>=11.2.0 Requires-Dist: setuptools>=49.3.0 Requires-Dist: typing-extensions
```

