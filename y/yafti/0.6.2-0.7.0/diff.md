# Comparing `tmp/yafti-0.6.2.tar.gz` & `tmp/yafti-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafti-0.6.2.tar", max compression
+gzip compressed data, was "yafti-0.7.0.tar", max compression
```

## Comparing `yafti-0.6.2.tar` & `yafti-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-05-30 13:34:16.949961 yafti-0.6.2/LICENSE
--rw-r--r--   0        0        0    10051 2023-05-30 13:34:16.949961 yafti-0.6.2/README.md
--rw-r--r--   0        0        0     1533 2023-05-30 13:34:16.949961 yafti-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      560 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/__init__.py
--rw-r--r--   0        0        0     1087 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/__main__.py
--rw-r--r--   0        0        0     2081 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/abc.py
--rw-r--r--   0        0        0     2455 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/app.py
--rw-r--r--   0        0        0     1813 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/events.py
--rw-r--r--   0        0        0      532 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/log.py
--rw-r--r--   0        0        0     1571 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/parser.py
--rw-r--r--   0        0        0     6823 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/plugin/flatpak.py
--rw-r--r--   0        0        0     2760 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/plugin/run.py
--rw-r--r--   0        0        0      302 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/registry.py
--rw-r--r--   0        0        0     3278 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/consent.py
--rw-r--r--   0        0        0     2227 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/console.py
--rw-r--r--   0        0        0     1817 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/dialog.py
--rw-r--r--   0        0        0       50 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/__init__.py
--rw-r--r--   0        0        0      317 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/models.py
--rw-r--r--   0        0        0       98 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/__init__.py
--rw-r--r--   0        0        0     5232 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/install.py
--rw-r--r--   0        0        0     4021 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/package.py
--rw-r--r--   0        0        0     5522 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/picker.py
--rw-r--r--   0        0        0     1368 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/state.py
--rw-r--r--   0        0        0      509 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/utils.py
--rw-r--r--   0        0        0     3413 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/title.py
--rw-r--r--   0        0        0     1214 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/utils.py
--rw-r--r--   0        0        0     5216 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/window.py
--rw-r--r--   0        0        0      448 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/setup.py
--rw-r--r--   0        0        0       32 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/share.py
--rw-r--r--   0        0        0    10948 1970-01-01 00:00:00.000000 yafti-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-05 23:37:24.939910 yafti-0.7.0/LICENSE
+-rw-r--r--   0        0        0    10051 2023-07-05 23:37:24.939910 yafti-0.7.0/README.md
+-rw-r--r--   0        0        0     1533 2023-07-05 23:37:24.939910 yafti-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/__init__.py
+-rw-r--r--   0        0        0     1087 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/__main__.py
+-rw-r--r--   0        0        0     2081 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/abc.py
+-rw-r--r--   0        0        0     2455 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/app.py
+-rw-r--r--   0        0        0     1813 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/events.py
+-rw-r--r--   0        0        0      532 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/log.py
+-rw-r--r--   0        0        0     1571 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/parser.py
+-rw-r--r--   0        0        0     6823 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/plugin/flatpak.py
+-rw-r--r--   0        0        0     3070 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/plugin/run.py
+-rw-r--r--   0        0        0      302 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/registry.py
+-rw-r--r--   0        0        0     3278 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/consent.py
+-rw-r--r--   0        0        0     2227 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/console.py
+-rw-r--r--   0        0        0     1817 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/dialog.py
+-rw-r--r--   0        0        0       50 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/__init__.py
+-rw-r--r--   0        0        0      317 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/models.py
+-rw-r--r--   0        0        0       98 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/__init__.py
+-rw-r--r--   0        0        0     5232 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/install.py
+-rw-r--r--   0        0        0     4021 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/package.py
+-rw-r--r--   0        0        0     5522 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/picker.py
+-rw-r--r--   0        0        0     1368 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/state.py
+-rw-r--r--   0        0        0      509 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/utils.py
+-rw-r--r--   0        0        0     3413 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/title.py
+-rw-r--r--   0        0        0     1214 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/utils.py
+-rw-r--r--   0        0        0     5216 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/window.py
+-rw-r--r--   0        0        0      448 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/setup.py
+-rw-r--r--   0        0        0       32 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/share.py
+-rw-r--r--   0        0        0    10948 1970-01-01 00:00:00.000000 yafti-0.7.0/PKG-INFO
```

### Comparing `yafti-0.6.2/LICENSE` & `yafti-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/README.md` & `yafti-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/pyproject.toml` & `yafti-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yafti"
-version = "0.6.2"
+version = "0.7.0"
 description = "Yet another first time installer"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/ublue-os/yafti"
 repository = "https://github.com/ublue-os/yafti"
 classifiers = [
```

### Comparing `yafti-0.6.2/yafti/__init__.py` & `yafti-0.7.0/yafti/__init__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/__main__.py` & `yafti-0.7.0/yafti/__main__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/abc.py` & `yafti-0.7.0/yafti/abc.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/app.py` & `yafti-0.7.0/yafti/app.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/events.py` & `yafti-0.7.0/yafti/events.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/log.py` & `yafti-0.7.0/yafti/log.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/parser.py` & `yafti-0.7.0/yafti/parser.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/plugin/flatpak.py` & `yafti-0.7.0/yafti/plugin/flatpak.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/plugin/run.py` & `yafti-0.7.0/yafti/plugin/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,25 @@
             stderr=stderr,
         )
 
         return subprocess.CompletedProcess(
             cmd, returncode=proc.returncode, stdout=stdout, stderr=stderr
         )
 
+    async def install(self, package: str) -> YaftiPluginReturn:
+        """Execute a command on the host system
+
+        Args:
+          package: The command to execute
+
+        Returns:
+          An object containing the stdout and stderr from the command
+        """
+        return await self.exec(package)
+
     @validate_arguments
     async def __call__(self, cmd: list[str] | str) -> YaftiPluginReturn:
         log.debug("run called", cmd=cmd)
         if isinstance(cmd, list):
             cmd = shlex.join(cmd)
 
         r = await self.exec(cmd)
```

### Comparing `yafti-0.6.2/yafti/screen/consent.py` & `yafti-0.7.0/yafti/screen/consent.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/console.py` & `yafti-0.7.0/yafti/screen/console.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/dialog.py` & `yafti-0.7.0/yafti/screen/dialog.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/package/screen/install.py` & `yafti-0.7.0/yafti/screen/package/screen/install.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/package/screen/package.py` & `yafti-0.7.0/yafti/screen/package/screen/package.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/package/screen/picker.py` & `yafti-0.7.0/yafti/screen/package/screen/picker.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/package/state.py` & `yafti-0.7.0/yafti/screen/package/state.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/title.py` & `yafti-0.7.0/yafti/screen/title.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/utils.py` & `yafti-0.7.0/yafti/screen/utils.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/yafti/screen/window.py` & `yafti-0.7.0/yafti/screen/window.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.2/PKG-INFO` & `yafti-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yafti
-Version: 0.6.2
+Version: 0.7.0
 Summary: Yet another first time installer
 Home-page: https://github.com/ublue-os/yafti
 License: Apache 2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: X11 Applications :: GTK
```

