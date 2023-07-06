# Comparing `tmp/pydantic-config-0.1.1.tar.gz` & `tmp/pydantic-config-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-config-0.1.1.tar", last modified: Thu Feb 23 15:55:31 2023, max compression
+gzip compressed data, was "pydantic-config-0.1.2.tar", last modified: Thu Jul  6 21:07:46 2023, max compression
```

## Comparing `pydantic-config-0.1.1.tar` & `pydantic-config-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:55:31.902178 pydantic-config-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-02-23 15:55:31.902178 pydantic-config-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 15:55:31.902178 pydantic-config-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:55:31.898178 pydantic-config-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:55:31.898178 pydantic-config-0.1.1/src/pydantic_config/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/src/pydantic_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/src/pydantic_config/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/src/pydantic_config/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:55:31.898178 pydantic-config-0.1.1/src/pydantic_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-02-23 15:55:31.000000 pydantic-config-0.1.1/src/pydantic_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-23 15:55:31.000000 pydantic-config-0.1.1/src/pydantic_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 15:55:31.000000 pydantic-config-0.1.1/src/pydantic_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-23 15:55:31.000000 pydantic-config-0.1.1/src/pydantic_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 15:55:31.000000 pydantic-config-0.1.1/src/pydantic_config.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:55:31.898178 pydantic-config-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-23 15:55:18.000000 pydantic-config-0.1.1/tests/test_settings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:07:46.491129 pydantic-config-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-06 21:07:46.491129 pydantic-config-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:07:46.491129 pydantic-config-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:07:46.491129 pydantic-config-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:07:46.491129 pydantic-config-0.1.2/src/pydantic_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/src/pydantic_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/src/pydantic_config/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/src/pydantic_config/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:07:46.491129 pydantic-config-0.1.2/src/pydantic_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-06 21:07:46.000000 pydantic-config-0.1.2/src/pydantic_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-06 21:07:46.000000 pydantic-config-0.1.2/src/pydantic_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:07:46.000000 pydantic-config-0.1.2/src/pydantic_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 21:07:46.000000 pydantic-config-0.1.2/src/pydantic_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:07:46.000000 pydantic-config-0.1.2/src/pydantic_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:07:46.491129 pydantic-config-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-06 21:07:34.000000 pydantic-config-0.1.2/tests/test_settings_model.py
```

### Comparing `pydantic-config-0.1.1/LICENSE` & `pydantic-config-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-config-0.1.1/PKG-INFO` & `pydantic-config-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-config
-Version: 0.1.1
+Version: 0.1.2
 Summary: Support for Pydantic settings configuration file loading
 Author: Jordan Shaw
 Project-URL: Homepage, https://github.com/jordantshaw/pydantic-config
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 ```toml
 # config.toml
 app_name = "Python Application"
 description = "Test application description"
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     app_id: str = 1
     app_name: str = None
     description: str = None
     log_level: str = 'INFO'
@@ -67,15 +67,15 @@
 {
   "description": "Description from JSON file",
   "log_level": "WARNING"
 }
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     app_id: str = 1
     app_name: str = 'App Name'
     description: str = None
     log_level: str = 'INFO'
@@ -105,15 +105,15 @@
 ```toml
 # config2.toml
 [foo]
 item2 = "value2"
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     foo: dict = {}
 
     class Config:
         config_file = ['config.toml', 'config2.toml']
```

### Comparing `pydantic-config-0.1.1/README.md` & `pydantic-config-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```toml
 # config.toml
 app_name = "Python Application"
 description = "Test application description"
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     app_id: str = 1
     app_name: str = None
     description: str = None
     log_level: str = 'INFO'
@@ -49,15 +49,15 @@
 {
   "description": "Description from JSON file",
   "log_level": "WARNING"
 }
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     app_id: str = 1
     app_name: str = 'App Name'
     description: str = None
     log_level: str = 'INFO'
@@ -87,15 +87,15 @@
 ```toml
 # config2.toml
 [foo]
 item2 = "value2"
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     foo: dict = {}
 
     class Config:
         config_file = ['config.toml', 'config2.toml']
```

### Comparing `pydantic-config-0.1.1/pyproject.toml` & `pydantic-config-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pydantic-config"
 description = "Support for Pydantic settings configuration file loading"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{name="Jordan Shaw"}]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     'Natural Language :: English',
     'Intended Audience :: Developers',
     'Development Status :: 4 - Beta',
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    'pydantic>=1.10.0',
+    'pydantic<2.0.0, >=1.10.0',
     'pyyaml>=6.0',
     'python-dotenv>=0.21.0',
     'toml>=0.10.2'
 ]
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `pydantic-config-0.1.1/src/pydantic_config/loaders.py` & `pydantic-config-0.1.2/src/pydantic_config/loaders.py`

 * *Files identical despite different names*

### Comparing `pydantic-config-0.1.1/src/pydantic_config/main.py` & `pydantic-config-0.1.2/src/pydantic_config/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-config-0.1.1/src/pydantic_config.egg-info/PKG-INFO` & `pydantic-config-0.1.2/src/pydantic_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-config
-Version: 0.1.1
+Version: 0.1.2
 Summary: Support for Pydantic settings configuration file loading
 Author: Jordan Shaw
 Project-URL: Homepage, https://github.com/jordantshaw/pydantic-config
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 ```toml
 # config.toml
 app_name = "Python Application"
 description = "Test application description"
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     app_id: str = 1
     app_name: str = None
     description: str = None
     log_level: str = 'INFO'
@@ -67,15 +67,15 @@
 {
   "description": "Description from JSON file",
   "log_level": "WARNING"
 }
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     app_id: str = 1
     app_name: str = 'App Name'
     description: str = None
     log_level: str = 'INFO'
@@ -105,15 +105,15 @@
 ```toml
 # config2.toml
 [foo]
 item2 = "value2"
 ```
 
 ```python
-from src.pydantic_config import SettingsModel
+from pydantic_config import SettingsModel
 
 
 class Settings(SettingsModel):
     foo: dict = {}
 
     class Config:
         config_file = ['config.toml', 'config2.toml']
```

### Comparing `pydantic-config-0.1.1/tests/test_loaders.py` & `pydantic-config-0.1.2/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `pydantic-config-0.1.1/tests/test_settings_model.py` & `pydantic-config-0.1.2/tests/test_settings_model.py`

 * *Files identical despite different names*

