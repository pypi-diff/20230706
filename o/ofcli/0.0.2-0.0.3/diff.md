# Comparing `tmp/ofcli-0.0.2.tar.gz` & `tmp/ofcli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofcli-0.0.2.tar", last modified: Wed Jun 28 22:43:54 2023, max compression
+gzip compressed data, was "ofcli-0.0.3.tar", last modified: Wed Jul  5 23:28:18 2023, max compression
```

## Comparing `ofcli-0.0.2.tar` & `ofcli-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-28 22:43:54.687063 ofcli-0.0.2/
--rw-r--r--   0 diana     (1000) diana     (1000)     1688 2023-06-28 22:43:54.687063 ofcli-0.0.2/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)      359 2023-06-23 09:35:20.000000 ofcli-0.0.2/README.md
--rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.0.2/pyproject.toml
--rw-r--r--   0 diana     (1000) diana     (1000)     1500 2023-06-28 22:43:54.687063 ofcli-0.0.2/setup.cfg
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-28 22:43:54.683730 ofcli-0.0.2/src/
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-28 22:43:54.687063 ofcli-0.0.2/src/ofcli.egg-info/
--rw-r--r--   0 diana     (1000) diana     (1000)     1688 2023-06-28 22:43:54.000000 ofcli-0.0.2/src/ofcli.egg-info/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-06-28 22:43:54.000000 ofcli-0.0.2/src/ofcli.egg-info/SOURCES.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-06-28 22:43:54.000000 ofcli-0.0.2/src/ofcli.egg-info/dependency_links.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-06-28 22:43:54.000000 ofcli-0.0.2/src/ofcli.egg-info/entry_points.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       39 2023-06-28 22:43:54.000000 ofcli-0.0.2/src/ofcli.egg-info/requires.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-06-28 22:43:54.000000 ofcli-0.0.2/src/ofcli.egg-info/top_level.txt
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-05 23:28:18.423761 ofcli-0.0.3/
+-rw-r--r--   0 diana     (1000) diana     (1000)     1688 2023-07-05 23:28:18.423761 ofcli-0.0.3/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)      359 2023-06-23 09:35:20.000000 ofcli-0.0.3/README.md
+-rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.0.3/pyproject.toml
+-rw-r--r--   0 diana     (1000) diana     (1000)     1512 2023-07-05 23:28:18.423761 ofcli-0.0.3/setup.cfg
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-05 23:28:18.423761 ofcli-0.0.3/src/
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-05 23:28:18.423761 ofcli-0.0.3/src/ofcli.egg-info/
+-rw-r--r--   0 diana     (1000) diana     (1000)     1688 2023-07-05 23:28:17.000000 ofcli-0.0.3/src/ofcli.egg-info/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/SOURCES.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-05 23:28:17.000000 ofcli-0.0.3/src/ofcli.egg-info/dependency_links.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/entry_points.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       50 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/requires.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/top_level.txt
```

### Comparing `ofcli-0.0.2/PKG-INFO` & `ofcli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofcli
-Version: 0.0.2
+Version: 0.0.3
 Summary: helper CLI tool for OIDC federation exploration
 Home-page: https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ofcli-0.0.2/setup.cfg` & `ofcli-0.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ofcli
-version = 0.0.2
+version = 0.0.3
 summary = helper CLI tool for OIDC federation exploration
 description = helper tool for OIDC federation exploration
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Diana Gudu
 author_email = gudu@kit.edu
 home_page = https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
@@ -40,14 +40,15 @@
 
 [options]
 install_requires = 
 	click
 	click_logging
 	requests
 	cryptojwt
+	pygraphviz
 package_dir = 
 	=src
 packages = find:
 
 [bdist_wheel]
 universal = 1
```

### Comparing `ofcli-0.0.2/src/ofcli.egg-info/PKG-INFO` & `ofcli-0.0.3/src/ofcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofcli
-Version: 0.0.2
+Version: 0.0.3
 Summary: helper CLI tool for OIDC federation exploration
 Home-page: https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli/issues
 Classifier: Development Status :: 3 - Alpha
```

