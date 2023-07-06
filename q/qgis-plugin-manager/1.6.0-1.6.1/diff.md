# Comparing `tmp/qgis-plugin-manager-1.6.0.tar.gz` & `tmp/qgis-plugin-manager-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis-plugin-manager-1.6.0.tar", last modified: Mon Jun 12 09:55:21 2023, max compression
+gzip compressed data, was "qgis-plugin-manager-1.6.1.tar", last modified: Thu Jul  6 12:10:26 2023, max compression
```

## Comparing `qgis-plugin-manager-1.6.0.tar` & `qgis-plugin-manager-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10853 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.739742 qgis-plugin-manager-1.6.0/qgis_plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-06-12 09:55:19.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6784 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/definitions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11958 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (122)    18787 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.739742 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10853 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-06-12 09:55:19.000000 qgis-plugin-manager-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_full_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    10902 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9507 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/qgis_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-07-06 12:10:24.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6664 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11958 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18787 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10902 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-06 12:10:26.000000 qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-07-06 12:10:24.000000 qgis-plugin-manager-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:10:26.938125 qgis-plugin-manager-1.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_full_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-07-06 12:10:17.000000 qgis-plugin-manager-1.6.1/test/test_utils.py
```

### Comparing `qgis-plugin-manager-1.6.0/PKG-INFO` & `qgis-plugin-manager-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.6.0
+Version: 1.6.1
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.0.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.1.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
@@ -159,18 +159,18 @@
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
 #### Basic authentication
 
-It's possible to add a login and password in the remote URL :
+It's possible to add a login and password in the remote URL, with `username` and `password` in the query string :
 
 ```bash
-https://docs.3liz.org/private/repo.xml?username=loginwpd&password=pass
+https://docs.3liz.org/private/repo.xml?username=login&password=pass
 ```
 
 Every URL is parsed, and if some credentials are found, the URL is cleaned and the request is done using the
 basic authentication.
 
 ### Update
```

### Comparing `qgis-plugin-manager-1.6.0/README.md` & `qgis-plugin-manager-1.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -130,18 +130,18 @@
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
 #### Basic authentication
 
-It's possible to add a login and password in the remote URL :
+It's possible to add a login and password in the remote URL, with `username` and `password` in the query string :
 
 ```bash
-https://docs.3liz.org/private/repo.xml?username=loginwpd&password=pass
+https://docs.3liz.org/private/repo.xml?username=login&password=pass
 ```
 
 Every URL is parsed, and if some credentials are found, the URL is cleaned and the request is done using the
 basic authentication.
 
 ### Update
```

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager/__about__.py` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 __license__ = "GNU General Public License v3.0"
 __summary__ = "Tool for downloading/managing QGIS plugins from CLI."
 __title__ = "QGIS Plugin Manager"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri__ = "https://github.com/3liz/qgis-plugin-manager"
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 if "." not in __version__:
     # If __version__ is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     __version__ = "0.0.0"
 
 __version_info__ = tuple(
```

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager/__main__.py` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,34 +85,30 @@
     plugin_path = Path('.')
     qgis_plugin_path = os.environ.get('QGIS_PLUGINPATH')
     if qgis_plugin_path:
         current_directory = False
         # Except if the QGIS_PLUGINPATH is set
         plugin_path = Path(qgis_plugin_path)
 
-    if args.command in ("remote", "cache", "search"):
-        # Remote only needed, no QGIS version needed
-        remote = Remote(plugin_path)
+    if args.command in ("remote", "cache", "search", "update"):
+        # Remote only needed, with QGIS version
+        remote = Remote(plugin_path, qgis_server_version())
         if args.command == "remote":
             remote.print_list()
         elif args.command == "cache":
             latest = remote.latest(args.plugin_name)
             if latest is None:
                 print(f"{Level.Alert}Plugin not found{Level.End}")
             else:
                 print(f"Plugin {args.plugin_name} : {latest} available")
         elif args.command == "search":
             results = remote.search(args.plugin_name)
             for result in results:
                 print(result)
-
-    elif args.command in ("update", ):
-        # Remote only needed, QGIS version needed
-        remote = Remote(plugin_path, qgis_server_version())
-        if args.command == "update":
+        elif args.command == "update":
             exit_val = remote.update()
 
     elif args.command in ("remove", ):
         # Local needed only, without QGIS version
         plugins = LocalDirectory(plugin_path)
         exit_val = plugins.remove(args.plugin_name)
```

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager/definitions.py` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager/definitions.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager/local_directory.py` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager/local_directory.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager/remote.py` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager/remote.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager/utils.py` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager/utils.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/PKG-INFO` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.6.0
+Version: 1.6.1
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.0.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.1.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
@@ -159,18 +159,18 @@
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
 #### Basic authentication
 
-It's possible to add a login and password in the remote URL :
+It's possible to add a login and password in the remote URL, with `username` and `password` in the query string :
 
 ```bash
-https://docs.3liz.org/private/repo.xml?username=loginwpd&password=pass
+https://docs.3liz.org/private/repo.xml?username=login&password=pass
 ```
 
 Every URL is parsed, and if some credentials are found, the URL is cleaned and the request is done using the
 basic authentication.
 
 ### Update
```

### Comparing `qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/SOURCES.txt` & `qgis-plugin-manager-1.6.1/qgis_plugin_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/setup.py` & `qgis-plugin-manager-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     sys.exit(
         "qgis-plugin-manager requires at least Python version "
         f"{python_min_version[0]}.{python_min_version[1]}.\n"
         f"You are currently running this installation with\n\n{sys.version}"
     )
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-VERSION = "1.6.0"
+VERSION = "1.6.1"
 
 if "." not in VERSION:
     # If VERSION is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     VERSION = "0.0.0"
 
 read_me = Path(__file__).parent.joinpath("README.md").read_text(encoding='utf8')
```

### Comparing `qgis-plugin-manager-1.6.0/test/test_full_install.py` & `qgis-plugin-manager-1.6.1/test/test_full_install.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/test/test_local.py` & `qgis-plugin-manager-1.6.1/test/test_local.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/test/test_remote.py` & `qgis-plugin-manager-1.6.1/test/test_remote.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.0/test/test_utils.py` & `qgis-plugin-manager-1.6.1/test/test_utils.py`

 * *Files identical despite different names*

