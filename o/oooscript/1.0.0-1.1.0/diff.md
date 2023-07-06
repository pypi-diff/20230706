# Comparing `tmp/oooscript-1.0.0.tar.gz` & `tmp/oooscript-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooscript-1.0.0.tar", max compression
+gzip compressed data, was "oooscript-1.1.0.tar", max compression
```

## Comparing `oooscript-1.0.0.tar` & `oooscript-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rwxr-xr-x   0        0        0      316 2022-10-01 22:51:52.046019 oooscript-1.0.0/README.md
--rwxr-xr-x   0        0        0       71 2022-09-26 16:21:12.329300 oooscript-1.0.0/oooscript/.oooscript_root
--rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.0.0/oooscript/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.0.0/oooscript/build/__init__.py
--rwxr-xr-x   0        0        0     7573 2022-10-01 21:39:16.818438 oooscript-1.0.0/oooscript/build/build.py
--rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.0.0/oooscript/build/build_util.py
--rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.0.0/oooscript/build/copy_resource.py
--rwxr-xr-x   0        0        0     5271 2022-10-01 21:38:58.797077 oooscript-1.0.0/oooscript/build/embed_py_script.py
--rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.0.0/oooscript/build/manifest_script.py
--rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.0.0/oooscript/build/tmp_dir.py
--rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.0.0/oooscript/cfg/__init__.py
--rwxr-xr-x   0        0        0     2874 2022-10-01 22:51:52.056144 oooscript-1.0.0/oooscript/cfg/config.py
--rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.0.0/oooscript/cli/__init__.py
--rwxr-xr-x   0        0        0     2446 2022-10-01 21:39:16.821586 oooscript-1.0.0/oooscript/cli/main.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.0.0/oooscript/lib/__init__.py
--rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.0.0/oooscript/lib/enums.py
--rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.0.0/oooscript/lib/ex.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.0.0/oooscript/models/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.0.0/oooscript/models/script_cfg/__init__.py
--rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.0.0/oooscript/models/script_cfg/args.py
--rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.0.0/oooscript/models/script_cfg/model_script_cfg.py
--rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.0.0/oooscript/models/validators.py
--rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.0.0/oooscript/res/__init__.py
--rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.0.0/oooscript/res/docs/__init__.py
--rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.0.0/oooscript/res/docs/blank.odf
--rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.0.0/oooscript/res/docs/blank.odg
--rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.0.0/oooscript/res/docs/blank.odp
--rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.0.0/oooscript/res/docs/blank.ods
--rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.0.0/oooscript/res/docs/blank.odt
--rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.0.0/oooscript/utils/__init__.py
--rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.0.0/oooscript/utils/enum_util.py
--rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.0.0/oooscript/utils/paths.py
--rwxr-xr-x   0        0        0     1801 2022-10-01 22:51:52.056883 oooscript-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 oooscript-1.0.0/setup.py
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 oooscript-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0      316 2022-10-01 22:51:52.046019 oooscript-1.1.0/README.md
+-rwxr-xr-x   0        0        0       71 2022-09-26 16:21:12.329300 oooscript-1.1.0/oooscript/.oooscript_root
+-rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.1.0/oooscript/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.1.0/oooscript/build/__init__.py
+-rwxr-xr-x   0        0        0     7573 2022-10-01 21:39:16.818438 oooscript-1.1.0/oooscript/build/build.py
+-rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.1.0/oooscript/build/build_util.py
+-rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.1.0/oooscript/build/copy_resource.py
+-rwxr-xr-x   0        0        0     5271 2022-10-01 21:38:58.797077 oooscript-1.1.0/oooscript/build/embed_py_script.py
+-rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.1.0/oooscript/build/manifest_script.py
+-rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.1.0/oooscript/build/tmp_dir.py
+-rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.1.0/oooscript/cfg/__init__.py
+-rwxr-xr-x   0        0        0     3203 2023-07-06 20:04:39.651893 oooscript-1.1.0/oooscript/cfg/config.py
+-rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.1.0/oooscript/cli/__init__.py
+-rwxr-xr-x   0        0        0     2446 2022-10-01 21:39:16.821586 oooscript-1.1.0/oooscript/cli/main.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.1.0/oooscript/lib/__init__.py
+-rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.1.0/oooscript/lib/enums.py
+-rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.1.0/oooscript/lib/ex.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.1.0/oooscript/models/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.1.0/oooscript/models/script_cfg/__init__.py
+-rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.1.0/oooscript/models/script_cfg/args.py
+-rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.1.0/oooscript/models/script_cfg/model_script_cfg.py
+-rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.1.0/oooscript/models/validators.py
+-rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.1.0/oooscript/res/__init__.py
+-rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.1.0/oooscript/res/docs/__init__.py
+-rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.1.0/oooscript/res/docs/blank.odf
+-rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.1.0/oooscript/res/docs/blank.odg
+-rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.1.0/oooscript/res/docs/blank.odp
+-rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.1.0/oooscript/res/docs/blank.ods
+-rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.1.0/oooscript/res/docs/blank.odt
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.1.0/oooscript/utils/__init__.py
+-rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.1.0/oooscript/utils/enum_util.py
+-rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.1.0/oooscript/utils/paths.py
+-rwxr-xr-x   0        0        0     1866 2023-07-06 20:04:39.658628 oooscript-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 oooscript-1.1.0/PKG-INFO
```

### Comparing `oooscript-1.0.0/oooscript/build/build.py` & `oooscript-1.1.0/oooscript/build/build.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/build/copy_resource.py` & `oooscript-1.1.0/oooscript/build/copy_resource.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/build/embed_py_script.py` & `oooscript-1.1.0/oooscript/build/embed_py_script.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/build/manifest_script.py` & `oooscript-1.1.0/oooscript/build/manifest_script.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/cfg/config.py` & `oooscript-1.1.0/oooscript/cfg/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from typing import Any, Dict, List
 from dotenv import dotenv_values
 from ..res import __res_path__
 from ..utils import paths
 
 
 _APP_CFG = None
+
+
 @dataclass
 class AppConfig:
-
     lo_script_dir: str
     """
     Path Like structure to libre office scripts director.
     """
     app_build_dir: str
     """
     Path Like structure to build dir
@@ -44,41 +45,50 @@
         "app_build_dir": "build_script",
         "xml_manifest_namespace": "urn:oasis:names:tc:opendocument:xmlns:manifest:1.0",
         "build_exclude_modules": ["uno\\.*", "unohelper\\.*", "scriptforge\\.*", "access2base\\.*"],
         "build_include_paths": ["."],
     }
     return config
 
-def _split_list(cfg:Dict[str, str]) -> None:
+
+def _split_list(cfg: Dict[str, str]) -> None:
     args = ("build_exclude_modules", "build_include_paths")
     for arg in args:
         value = cfg.get(arg, None)
         if value is not None:
             if value == "":
                 cfg[arg] = []
             else:
-                sl = value.split(',')
+                sl = value.split(",")
                 cfg[arg] = [s.strip() for s in sl]
-    
+
+
+def _update_default_config(default_cfg: Dict[str, Any], cfg: Dict[str, Any]) -> None:
+    for key, value in cfg.items():
+        if key.lower() in default_cfg:
+            default_cfg[key.lower()] = value
+
 
 def read_config(config_name: str) -> AppConfig:
     """
     Gets config for given config file
 
     Args:
         config_file (str): Config file to load
 
     Returns:
         AppConfig: Configuration object
     """
     default_cfg = _get_default_config()
     try:
+        # config may contain values that are not in default config.
         config = dotenv_values(config_name)
         _split_list(config)
-        default_cfg.update(config)
+        # default_cfg.update(config)
+        _update_default_config(default_cfg, config)
     except Exception:
         pass
     # can override app build directory from environment.
     # this is for testing purposes
     app_build = os.environ.get("OOOSCRIPT_APP_BUILD_DIR", None)
     if app_build:
         default_cfg["app_build_dir"] = app_build
@@ -98,8 +108,8 @@
 def get_app_cfg() -> AppConfig:
     """
     Get App Config. config is cached
     """
     global _APP_CFG
     if _APP_CFG is None:
         _APP_CFG = read_config_default()
-    return _APP_CFG
+    return _APP_CFG
```

### Comparing `oooscript-1.0.0/oooscript/cli/main.py` & `oooscript-1.1.0/oooscript/cli/main.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/models/script_cfg/args.py` & `oooscript-1.1.0/oooscript/models/script_cfg/args.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/models/script_cfg/model_script_cfg.py` & `oooscript-1.1.0/oooscript/models/script_cfg/model_script_cfg.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/models/validators.py` & `oooscript-1.1.0/oooscript/models/validators.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/res/docs/blank.odf` & `oooscript-1.1.0/oooscript/res/docs/blank.odf`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/res/docs/blank.odg` & `oooscript-1.1.0/oooscript/res/docs/blank.odg`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/res/docs/blank.odp` & `oooscript-1.1.0/oooscript/res/docs/blank.odp`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/res/docs/blank.ods` & `oooscript-1.1.0/oooscript/res/docs/blank.ods`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/res/docs/blank.odt` & `oooscript-1.1.0/oooscript/res/docs/blank.odt`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/utils/enum_util.py` & `oooscript-1.1.0/oooscript/utils/enum_util.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/oooscript/utils/paths.py` & `oooscript-1.1.0/oooscript/utils/paths.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.0.0/pyproject.toml` & `oooscript-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooscript"
-version = "1.0.0"
+version = "1.1.0"
 description = "Compiles several python scripts into a single script that can be eaisly used by LibreOffice as a macro."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 homepage = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 documentation = "https://oooscript.readthedocs.io/en/latest/"
 repository = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 license = "MIT"
 readme = "README.md"
@@ -15,44 +15,50 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Office/Business",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 packages = [
     { include = "oooscript" }
 ]
 
 
 [tool.poetry.scripts]
 oooscript = 'oooscript.cli.main:main'
 
 [tool.poetry.dependencies]
-python = "^3.7"
-python-dotenv = "^0.21.0"
+python = "^3.8"
+python-dotenv = "^0.21.1"
 pydantic = "^1.10.2"
 scriptmerge = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.8.0"
-typing-extensions = "^4.3.0"
+black = "^22.12.0"
+typing-extensions = "^4.7.1"
 ooo-dev-tools = "^0.4.21"
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.1.3"
 tox-poetry = "^0.4.1"
 
 
 [tool.poetry.group.docs.dependencies]
-sphinx-toolbox = "^3.2.0"
-sphinxcontrib-spelling = "^7.6.0"
+sphinx-toolbox = "^3.4.0"
+sphinxcontrib-spelling = "^8.0.0"
 sphinx-rtd-dark-mode = "^1.2.4"
+sphinx = "^6.2.1"
+sphinx-autodoc-typehints = "1.23.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests"
+]
```

