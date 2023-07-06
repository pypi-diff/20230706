# Comparing `tmp/pickley-3.5.5.tar.gz` & `tmp/pickley-3.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickley-3.5.5.tar", last modified: Tue Jun 13 23:46:33 2023, max compression
+gzip compressed data, was "pickley-3.5.6.tar", last modified: Thu Jul  6 18:12:48 2023, max compression
```

## Comparing `pickley-3.5.5.tar` & `pickley-3.5.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 23:45:03.000000 pickley-3.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 23:45:03.000000 pickley-3.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:46:33.645017 pickley-3.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 23:45:03.000000 pickley-3.5.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 23:45:03.000000 pickley-3.5.5/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:45:03.000000 pickley-3.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:46:33.645017 pickley-3.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 23:45:03.000000 pickley-3.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.641018 pickley-3.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/src/pickley/
--rw-r--r--   0 runner    (1001) docker     (123)    36368 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/bstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31371 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/src/pickley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:48.389912 pickley-3.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 18:11:13.000000 pickley-3.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 18:11:13.000000 pickley-3.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-06 18:12:48.389912 pickley-3.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-06 18:11:13.000000 pickley-3.5.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 18:11:13.000000 pickley-3.5.6/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-06 18:11:13.000000 pickley-3.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:12:48.389912 pickley-3.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-06 18:11:13.000000 pickley-3.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:48.385912 pickley-3.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:48.385912 pickley-3.5.6/src/pickley/
+-rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-07-06 18:11:13.000000 pickley-3.5.6/src/pickley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-06 18:11:13.000000 pickley-3.5.6/src/pickley/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-06 18:11:13.000000 pickley-3.5.6/src/pickley/bstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31288 2023-07-06 18:11:13.000000 pickley-3.5.6/src/pickley/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-06 18:11:13.000000 pickley-3.5.6/src/pickley/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-06 18:11:13.000000 pickley-3.5.6/src/pickley/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:48.389912 pickley-3.5.6/src/pickley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-06 18:12:48.000000 pickley-3.5.6/src/pickley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-06 18:12:48.000000 pickley-3.5.6/src/pickley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:12:48.000000 pickley-3.5.6/src/pickley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-06 18:12:48.000000 pickley-3.5.6/src/pickley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 18:12:48.000000 pickley-3.5.6/src/pickley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 18:12:48.000000 pickley-3.5.6/src/pickley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:12:48.389912 pickley-3.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-06 18:11:13.000000 pickley-3.5.6/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-06 18:11:13.000000 pickley-3.5.6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-06 18:11:13.000000 pickley-3.5.6/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-07-06 18:11:13.000000 pickley-3.5.6/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-06 18:11:13.000000 pickley-3.5.6/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-06 18:11:13.000000 pickley-3.5.6/tests/test_venv.py
```

### Comparing `pickley-3.5.5/LICENSE` & `pickley-3.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/PKG-INFO` & `pickley-3.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.5
+Version: 3.5.6
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.5/README.rst` & `pickley-3.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/setup.py` & `pickley-3.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/src/pickley/__init__.py` & `pickley-3.5.6/src/pickley/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from datetime import datetime
 
 import runez
 from runez.pyenv import PypiStd, PythonDepot, PythonInstallationScanner, Version
 
 
-__version__ = "3.5.5"
+__version__ = "3.5.6"
 LOG = logging.getLogger(__name__)
 PICKLEY = "pickley"
 DOT_META = ".pk"
 K_CLI = {"delivery", "index", "python"}
 K_DIRECTIVES = {"include"}
 K_GROUPS = {"bundle", "pinned"}
 K_LEAVES = {
@@ -253,15 +253,15 @@
     def ping_path(self):
         """Path to .ping file (for throttle auto-upgrade checks)"""
         return self.cfg.cache.full_path(f"{self.dashed}.ping")
 
     @runez.cached_property
     def active_install_path(self):
         """Currently active installed venv (symlink)"""
-        return self.cfg.meta.full_path(self.dashed)
+        return self.cfg.meta.full_path(f"{self.dashed}-{self.desired_track}")
 
     @property
     def is_currently_installed(self):
         manifest = self.manifest
         return manifest and manifest.version
 
     @runez.cached_property
@@ -587,17 +587,16 @@
     def _wrapped_canonical(self, path):
         """(str | None): Canonical name of installed python package, if installed via pickley wrapper"""
         if runez.is_executable(path):
             for line in runez.readlines(path, first=12):
                 if line.startswith("# pypi-package:"):
                     return line[15:].strip()
 
-                # TODO: Remove once pickley 3.4 is phased out
                 m = self._wrapped_canonical_regex.search(line)
-                if m:
+                if m:  # pragma: no cover, TODO: Remove once pickley 3.4 is phased out
                     return m.group(1)
 
     def scan_installed(self):
         """Scan installed"""
         for item in self.base.iterdir():
             spec_name = self._wrapped_canonical(item)
             if spec_name:
```

### Comparing `pickley-3.5.5/src/pickley/bstrap.py` & `pickley-3.5.6/src/pickley/bstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/src/pickley/cli.py` & `pickley-3.5.6/src/pickley/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,16 +311,15 @@
     """Show pickley base folder"""
     path = CFG.base.path
     if what == "bootstrap-own-wrapper":
         # Internal: called by bootstrap script
         from pickley.delivery import DeliveryMethodWrap
 
         pspec = PackageSpec(CFG, f"{PICKLEY}=={__version__}")
-        venv = PythonVenv(CFG.meta.full_path(f"{PICKLEY}-{__version__}"), pspec, create=False)
-        runez.symlink(venv.folder, pspec.active_install_path)
+        venv = PythonVenv(pspec.active_install_path, pspec, create=False)
         wrap = DeliveryMethodWrap()
         wrap.install(venv, {PICKLEY: PICKLEY})
 
         # TODO: Remove once pickley 3.4 is phased out
         old_meta = CFG.base.full_path(".pickley")
         if os.path.isdir(old_meta):
             runez.delete(old_meta)
```

### Comparing `pickley-3.5.5/src/pickley/delivery.py` & `pickley-3.5.6/src/pickley/delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/src/pickley/package.py` & `pickley-3.5.6/src/pickley/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,20 +316,17 @@
         delivery = DeliveryMethod.delivery_method_by_name(pspec.settings.delivery)
         delivery.ping = ping
         args = []
         if no_binary:
             args.append("--no-binary")
             args.append(no_binary)
 
-        version = "dev" if pspec.dashed == PICKLEY and runez.DEV.project_folder else pspec.desired_track.version
-        venv_folder = pspec.cfg.meta.full_path(f"{pspec.dashed}-{version}")
-        venv = PythonVenv(venv_folder, pspec)
+        venv = PythonVenv(pspec.active_install_path, pspec)
         args.extend(pspec.pip_spec())
         venv.pip_install(*args)
-        runez.symlink(venv_folder, pspec.active_install_path)
         contents = PackageContents(venv)
         if not contents.entry_points:
             pspec.delete_all_files()
             abort(f"Can't install '{runez.bold(pspec.dashed)}', it is {runez.red('not a CLI')}")
 
         return delivery.install(venv, contents.entry_points)
```

### Comparing `pickley-3.5.5/src/pickley.egg-info/PKG-INFO` & `pickley-3.5.6/src/pickley.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.5
+Version: 3.5.6
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.5/src/pickley.egg-info/SOURCES.txt` & `pickley-3.5.6/src/pickley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/tests/test_bootstrap.py` & `pickley-3.5.6/tests/test_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from unittest.mock import patch
 
 import pytest
 import runez
 
-from pickley import bstrap, DOT_META
+from pickley import __version__, bstrap, DOT_META
 
 
 def mocked_expanduser(path):
     if path and path.startswith("~/"):
         path = path[2:]
 
     return path
@@ -31,15 +31,15 @@
 def test_bootstrap(cli, monkeypatch):
     runez.touch(".pickley/config.json")
     cli.run("-n base bootstrap-own-wrapper")
     assert cli.succeeded
     assert f"Would move .pickley/config.json -> {DOT_META}/config.json" in cli.logged
     assert f"Would save {DOT_META}/pickley.manifest.json" in cli.logged
     assert "Would delete .pickley" in cli.logged
-    assert f"Would run: {DOT_META}/pickley/bin/pickley auto-heal" in cli.logged
+    assert f"Would run: {DOT_META}/pickley-{__version__}/bin/pickley auto-heal" in cli.logged
 
     with patch("pickley.bstrap.which", side_effect=mocked_which):
         with patch("pickley.bstrap.os.path.expanduser", side_effect=mocked_expanduser):
             runez.write(".local/bin/pickley", "#!/bin/sh\necho 0.1")  # Pretend we have an old pickley
             runez.make_executable(".local/bin/pickley")
 
             with patch("pickley.bstrap.get_python_version", return_value=(3, 6)):  # urllib fails
```

### Comparing `pickley-3.5.5/tests/test_config.py` & `pickley-3.5.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/tests/test_delivery.py` & `pickley-3.5.6/tests/test_delivery.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     pspec = PackageSpec(cfg, "mgit==1.0.0")
     venv = MagicMock(pspec=pspec)
     entry_points = {"some-source": ""}
     cfg.set_base(".")
     d = DeliveryMethod()
     with pytest.raises(SystemExit):
         d.install(venv, entry_points)
-    assert "Can't deliver some-source -> .pk/mgit/bin/some-source: source does not exist" in logged.pop()
+    assert "Can't deliver some-source -> .pk/mgit-1.0.0/bin/some-source: source does not exist" in logged.pop()
 
-    runez.touch(".pk/mgit/bin/some-source")
+    runez.touch(".pk/mgit-1.0.0/bin/some-source")
     with pytest.raises(SystemExit):
         d.install(venv, entry_points)
     assert "Failed to deliver" in logged.pop()
 
 
 class SimulatedInstallation:
     def __init__(self, cfg, name, version):
```

### Comparing `pickley-3.5.5/tests/test_ops.py` & `pickley-3.5.6/tests/test_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,17 +170,16 @@
         cli.expect_failure("-n -dfoo install mgit", "Unknown delivery method 'foo'")
 
 
 def test_dev_mode(cli, monkeypatch):
     with patch("runez.pyenv.PypiStd.latest_pypi_version", side_effect=mock_latest_pypi_version):
         cli.run("-n install pickley")
         assert cli.succeeded
-        assert ".pk/pickley-dev/bin/pip install -e " in cli.logged
-        assert "Would symlink .pk/pickley-dev <- .pk/pickley" in cli.logged
-        assert "pickley-100.0" not in cli.logged
+        assert "Would run: .pk/pickley-100.0/bin/pip install -e " in cli.logged
+        assert "Would wrap pickley -> .pk/pickley-100.0/bin/pickley" in cli.logged
         assert "Would state: Installed pickley v100.0 in "
 
 
 def test_edge_cases(temp_cfg, logged):
     tv = TrackedVersion(version="1.2")
     assert str(tv) == "1.2"
     pspec = PackageSpec(temp_cfg, PICKLEY)
```

### Comparing `pickley-3.5.5/tests/test_run.py` & `pickley-3.5.6/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.5/tests/test_venv.py` & `pickley-3.5.6/tests/test_venv.py`

 * *Files identical despite different names*

