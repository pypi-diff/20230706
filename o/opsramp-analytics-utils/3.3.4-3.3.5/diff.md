# Comparing `tmp/opsramp-analytics-utils-3.3.4.tar.gz` & `tmp/opsramp-analytics-utils-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.3.4.tar", last modified: Thu Jun 22 11:33:45 2023, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.3.5.tar", last modified: Thu Jul  6 10:43:31 2023, max compression
```

## Comparing `opsramp-analytics-utils-3.3.4.tar` & `opsramp-analytics-utils-3.3.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-06-22 11:33:45.912619 opsramp-analytics-utils-3.3.4/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/LICENSE
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/MANIFEST.in
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-06-22 11:33:45.912619 opsramp-analytics-utils-3.3.4/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/README.md
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-06-22 11:33:45.388608 opsramp-analytics-utils-3.3.4/analytics_sdk/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/__init__.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-06-22 11:33:45.632613 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/main.js
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-06-22 11:33:45.868618 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/components.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/constants.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/oap_dash.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-06-22 11:33:45.896619 opsramp-analytics-utils-3.3.4/analytics_sdk/process/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/process/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     5809 2023-04-10 11:19:33.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/process/process.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/process/querybuilder.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-06-22 11:33:45.900619 opsramp-analytics-utils-3.3.4/analytics_sdk/renderer/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/renderer/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    33742 2023-06-22 07:52:39.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/renderer/excel.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/renderer/pdf.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    40655 2023-06-22 10:32:39.000000 opsramp-analytics-utils-3.3.4/analytics_sdk/utilities.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-06-22 11:33:45.908619 opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-06-22 11:33:44.000000 opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-06-22 11:33:45.000000 opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-06-22 11:33:44.000000 opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-06-22 11:33:44.000000 opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/requires.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-06-22 11:33:44.000000 opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/top_level.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-03 11:09:31.000000 opsramp-analytics-utils-3.3.4/requires-install.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-06-22 11:33:45.912619 opsramp-analytics-utils-3.3.4/setup.cfg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-06-22 10:33:34.000000 opsramp-analytics-utils-3.3.4/setup.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-07-06 10:43:31.485718 opsramp-analytics-utils-3.3.5/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/LICENSE
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/MANIFEST.in
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-07-06 10:43:31.481718 opsramp-analytics-utils-3.3.5/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/README.md
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-07-06 10:43:30.893760 opsramp-analytics-utils-3.3.5/analytics_sdk/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/__init__.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-07-06 10:43:31.165741 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/main.js
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-07-06 10:43:31.417723 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/components.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/constants.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/oap_dash.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-07-06 10:43:31.445721 opsramp-analytics-utils-3.3.5/analytics_sdk/process/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/process/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     5809 2023-04-10 11:19:33.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/process/process.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/process/querybuilder.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-07-06 10:43:31.473719 opsramp-analytics-utils-3.3.5/analytics_sdk/renderer/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/renderer/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    33742 2023-06-22 07:52:39.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/renderer/excel.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/renderer/pdf.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    40891 2023-07-06 10:42:36.000000 opsramp-analytics-utils-3.3.5/analytics_sdk/utilities.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-07-06 10:43:31.481718 opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-07-06 10:43:30.000000 opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-07-06 10:43:30.000000 opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-07-06 10:43:30.000000 opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-07-06 10:43:30.000000 opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/requires.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-07-06 10:43:30.000000 opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-03 11:09:31.000000 opsramp-analytics-utils-3.3.5/requires-install.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-07-06 10:43:31.485718 opsramp-analytics-utils-3.3.5/setup.cfg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-07-06 10:42:36.000000 opsramp-analytics-utils-3.3.5/setup.py
```

### Comparing `opsramp-analytics-utils-3.3.4/LICENSE` & `opsramp-analytics-utils-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/PKG-INFO` & `opsramp-analytics-utils-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.3.4
+Version: 3.3.5
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.3.4/README.md` & `opsramp-analytics-utils-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.3.5/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/components.py` & `opsramp-analytics-utils-3.3.5/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.3.5/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.3.5/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.3.5/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.3.5/analytics_sdk/renderer/excel.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.3.5/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.3.5/analytics_sdk/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,16 +739,14 @@
                 if add_pageNo:
                     uri = url + f'&pageNo={page_no}&pageSize={pageSize}'
                 else:
                     uri = url
                 res = get_response(uri, type)
             if res == None or not res.ok:
                 logger.error('Get %s API is failed, url %s', type, url)
-                return resp
-            elif "results" not in res.json() or len(res.json()['results'])==0 :
                 retry_count = 1
                 while (retry_count <= API_RETRY):
                     data = json.loads(data)
                     if "pageNo" in data:
                         data["pageNo"] = page_no
                         data["pageSize"] = pageSize
                     data=json.dumps(data)
@@ -769,14 +767,20 @@
                     elif "results" not in res.json() or len(res.json()['results'])==0:
                         res = None
                     else:
                         break
                 if res == None or "results" not in res.json() or len(res.json()['results'])==0:
                     logger.error('After retrying for %s times, Get %s API results are empty, url is %s', API_RETRY, type, url)
                     return None
+            elif res.ok and "results" not in res.json():
+                logger.error('Get %s API, results key not found, url is %s', type, url)
+                return None
+            elif res.ok and len(res.json()['results'])==0:
+                logger.error('Get %s API, results are empty, url is %s', type, url)
+                return None
             #else:   
             result = res.json()['results']
             resp.append(result)
     
             if "nextPage" not in res.json():
                 resp = []
                 logger.error('Get %s nextPage keyword is missing in url %s', type, url)
```

### Comparing `opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.3.4
+Version: 3.3.5
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.3.4/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.3.5/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.4/setup.py` & `opsramp-analytics-utils-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.3.4",
+    version="3.3.5",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     url="https://github.com/opsramp/analytics-sdk",
```

