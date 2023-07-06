# Comparing `tmp/AutoFeedback-1.2.tar.gz` & `tmp/AutoFeedback-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoFeedback-1.2.tar", last modified: Thu Jun 22 18:28:16 2023, max compression
+gzip compressed data, was "AutoFeedback-1.3.tar", last modified: Thu Jul  6 16:22:41 2023, max compression
```

## Comparing `AutoFeedback-1.2.tar` & `AutoFeedback-1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.787516 AutoFeedback-1.2/
--rw-r--r--   0 abrown41   (502) staff       (20)      162 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AUTHORS.rst
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.788144 AutoFeedback-1.2/AutoFeedback/
--rw-r--r--   0 abrown41   (502) staff       (20)      214 2023-04-25 17:16:18.000000 AutoFeedback-1.2/AutoFeedback/__init__.py
--rw-r--r--   0 abrown41   (502) staff       (20)      495 2023-06-22 18:28:16.788186 AutoFeedback-1.2/AutoFeedback/_version.py
--rw-r--r--   0 abrown41   (502) staff       (20)      283 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/bcolors.py
--rw-r--r--   0 abrown41   (502) staff       (20)     7052 2023-06-22 17:57:56.000000 AutoFeedback-1.2/AutoFeedback/funcchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4557 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/function_error_messages.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4374 2023-06-22 18:26:48.000000 AutoFeedback-1.2/AutoFeedback/plot_error_messages.py
--rw-r--r--   0 abrown41   (502) staff       (20)     9009 2023-06-22 18:26:41.000000 AutoFeedback-1.2/AutoFeedback/plotchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4391 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/plotclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)    16126 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/randomclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)      431 2023-06-22 17:57:56.000000 AutoFeedback-1.2/AutoFeedback/utils.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4119 2023-06-22 17:57:56.000000 AutoFeedback-1.2/AutoFeedback/varchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3986 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/variable_error_messages.py
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.785342 AutoFeedback-1.2/AutoFeedback.egg-info/
--rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/PKG-INFO
--rw-r--r--   0 abrown41   (502) staff       (20)      999 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/SOURCES.txt
--rw-r--r--   0 abrown41   (502) staff       (20)        1 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/dependency_links.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       20 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/entry_points.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       63 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/requires.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       18 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/top_level.txt
--rw-r--r--   0 abrown41   (502) staff       (20)     3081 2023-03-20 10:13:58.000000 AutoFeedback-1.2/CONTRIBUTING.rst
--rw-r--r--   0 abrown41   (502) staff       (20)     1520 2023-03-20 10:13:58.000000 AutoFeedback-1.2/LICENSE
--rw-r--r--   0 abrown41   (502) staff       (20)      398 2023-03-20 10:13:58.000000 AutoFeedback-1.2/MANIFEST.in
--rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-06-22 18:28:16.787627 AutoFeedback-1.2/PKG-INFO
--rw-r--r--   0 abrown41   (502) staff       (20)     2157 2023-03-20 10:13:58.000000 AutoFeedback-1.2/README.rst
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.785616 AutoFeedback-1.2/docs/
--rw-r--r--   0 abrown41   (502) staff       (20)      673 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/Makefile
--rw-r--r--   0 abrown41   (502) staff       (20)      797 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/make.bat
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.786085 AutoFeedback-1.2/docs/source/
--rw-r--r--   0 abrown41   (502) staff       (20)     6730 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/source/conf.py
--rw-r--r--   0 abrown41   (502) staff       (20)      396 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/source/index.rst
--rw-r--r--   0 abrown41   (502) staff       (20)     1083 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/source/min_versions.rst
--rw-r--r--   0 abrown41   (502) staff       (20)    30606 2023-06-22 17:57:56.000000 AutoFeedback-1.2/docs/source/usage.rst
--rw-r--r--   0 abrown41   (502) staff       (20)       29 2023-06-22 17:57:53.000000 AutoFeedback-1.2/requirements.txt
--rw-r--r--   0 abrown41   (502) staff       (20)      408 2023-06-22 18:28:16.787994 AutoFeedback-1.2/setup.cfg
--rw-r--r--   0 abrown41   (502) staff       (20)     2414 2023-03-20 10:13:58.000000 AutoFeedback-1.2/setup.py
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.787402 AutoFeedback-1.2/test/
--rw-r--r--   0 abrown41   (502) staff       (20)        0 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/__init__.py
--rw-r--r--   0 abrown41   (502) staff       (20)       32 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/printtest.py
--rw-r--r--   0 abrown41   (502) staff       (20)     9518 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testerrors.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3525 2023-06-22 17:57:56.000000 AutoFeedback-1.2/test/testfuncs.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3497 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testplot.py
--rw-r--r--   0 abrown41   (502) staff       (20)     2780 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testplotclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)      578 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testprint.py
--rw-r--r--   0 abrown41   (502) staff       (20)    11743 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testrandomclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)     1976 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testsymp.py
--rw-r--r--   0 abrown41   (502) staff       (20)      970 2023-06-22 17:57:56.000000 AutoFeedback-1.2/test/testutils.py
--rw-r--r--   0 abrown41   (502) staff       (20)     2224 2023-06-22 17:57:56.000000 AutoFeedback-1.2/test/testvars.py
--rw-r--r--   0 abrown41   (502) staff       (20)    78254 2023-03-20 10:13:58.000000 AutoFeedback-1.2/versioneer.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.735893 AutoFeedback-1.3/
+-rw-r--r--   0 abrown41   (502) staff       (20)      162 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AUTHORS.rst
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.736636 AutoFeedback-1.3/AutoFeedback/
+-rw-r--r--   0 abrown41   (502) staff       (20)      260 2023-07-06 16:17:28.000000 AutoFeedback-1.3/AutoFeedback/__init__.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      495 2023-07-06 16:22:41.736702 AutoFeedback-1.3/AutoFeedback/_version.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      283 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/bcolors.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     7052 2023-06-22 17:57:56.000000 AutoFeedback-1.3/AutoFeedback/funcchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4557 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/function_error_messages.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4374 2023-06-22 18:26:48.000000 AutoFeedback-1.3/AutoFeedback/plot_error_messages.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     9009 2023-06-22 18:35:21.000000 AutoFeedback-1.3/AutoFeedback/plotchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4391 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/plotclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    16126 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/randomclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      431 2023-06-22 17:57:56.000000 AutoFeedback-1.3/AutoFeedback/utils.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4119 2023-06-22 17:57:56.000000 AutoFeedback-1.3/AutoFeedback/varchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3986 2023-03-20 10:13:58.000000 AutoFeedback-1.3/AutoFeedback/variable_error_messages.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.732773 AutoFeedback-1.3/AutoFeedback.egg-info/
+-rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/PKG-INFO
+-rw-r--r--   0 abrown41   (502) staff       (20)      999 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/SOURCES.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)        1 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/dependency_links.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       20 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/entry_points.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       63 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/requires.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       18 2023-07-06 16:22:41.000000 AutoFeedback-1.3/AutoFeedback.egg-info/top_level.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)     3081 2023-03-20 10:13:58.000000 AutoFeedback-1.3/CONTRIBUTING.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)     1520 2023-03-20 10:13:58.000000 AutoFeedback-1.3/LICENSE
+-rw-r--r--   0 abrown41   (502) staff       (20)      398 2023-03-20 10:13:58.000000 AutoFeedback-1.3/MANIFEST.in
+-rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-07-06 16:22:41.735973 AutoFeedback-1.3/PKG-INFO
+-rw-r--r--   0 abrown41   (502) staff       (20)     2157 2023-03-20 10:13:58.000000 AutoFeedback-1.3/README.rst
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.733255 AutoFeedback-1.3/docs/
+-rw-r--r--   0 abrown41   (502) staff       (20)      673 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/Makefile
+-rw-r--r--   0 abrown41   (502) staff       (20)      797 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/make.bat
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.734021 AutoFeedback-1.3/docs/source/
+-rw-r--r--   0 abrown41   (502) staff       (20)     6730 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/source/conf.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      396 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/source/index.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)     1083 2023-03-20 10:13:58.000000 AutoFeedback-1.3/docs/source/min_versions.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)    30606 2023-06-22 17:57:56.000000 AutoFeedback-1.3/docs/source/usage.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)       29 2023-06-22 17:57:53.000000 AutoFeedback-1.3/requirements.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)      408 2023-07-06 16:22:41.736281 AutoFeedback-1.3/setup.cfg
+-rw-r--r--   0 abrown41   (502) staff       (20)     2414 2023-03-20 10:13:58.000000 AutoFeedback-1.3/setup.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-07-06 16:22:41.735767 AutoFeedback-1.3/test/
+-rw-r--r--   0 abrown41   (502) staff       (20)        0 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/__init__.py
+-rw-r--r--   0 abrown41   (502) staff       (20)       32 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/printtest.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     9518 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testerrors.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3525 2023-06-22 17:57:56.000000 AutoFeedback-1.3/test/testfuncs.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3497 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testplot.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     2780 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testplotclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      578 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testprint.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    11743 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testrandomclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     1976 2023-03-20 10:13:58.000000 AutoFeedback-1.3/test/testsymp.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      970 2023-06-22 17:57:56.000000 AutoFeedback-1.3/test/testutils.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     2224 2023-06-22 17:57:56.000000 AutoFeedback-1.3/test/testvars.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    78254 2023-03-20 10:13:58.000000 AutoFeedback-1.3/versioneer.py
```

### Comparing `AutoFeedback-1.2/AutoFeedback/funcchecks.py` & `AutoFeedback-1.3/AutoFeedback/funcchecks.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback/function_error_messages.py` & `AutoFeedback-1.3/AutoFeedback/function_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback/plot_error_messages.py` & `AutoFeedback-1.3/AutoFeedback/plot_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback/plotchecks.py` & `AutoFeedback-1.3/AutoFeedback/plotchecks.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback/plotclass.py` & `AutoFeedback-1.3/AutoFeedback/plotclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback/randomclass.py` & `AutoFeedback-1.3/AutoFeedback/randomclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback/varchecks.py` & `AutoFeedback-1.3/AutoFeedback/varchecks.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback/variable_error_messages.py` & `AutoFeedback-1.3/AutoFeedback/variable_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/AutoFeedback.egg-info/PKG-INFO` & `AutoFeedback-1.3/AutoFeedback.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoFeedback
-Version: 1.2
+Version: 1.3
 Summary: check basic python exercises with pretty feedback
 Home-page: https://github.com/abrown41/AutoFeedback
 Author: Andrew Brown
 Author-email: andrew.brown@qub.ac.uk
 License: BSD (3-clause)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AutoFeedback-1.2/AutoFeedback.egg-info/SOURCES.txt` & `AutoFeedback-1.3/AutoFeedback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/CONTRIBUTING.rst` & `AutoFeedback-1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/LICENSE` & `AutoFeedback-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/PKG-INFO` & `AutoFeedback-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoFeedback
-Version: 1.2
+Version: 1.3
 Summary: check basic python exercises with pretty feedback
 Home-page: https://github.com/abrown41/AutoFeedback
 Author: Andrew Brown
 Author-email: andrew.brown@qub.ac.uk
 License: BSD (3-clause)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AutoFeedback-1.2/README.rst` & `AutoFeedback-1.3/README.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/docs/Makefile` & `AutoFeedback-1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/docs/make.bat` & `AutoFeedback-1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/docs/source/conf.py` & `AutoFeedback-1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/docs/source/min_versions.rst` & `AutoFeedback-1.3/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/docs/source/usage.rst` & `AutoFeedback-1.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/setup.py` & `AutoFeedback-1.3/setup.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testerrors.py` & `AutoFeedback-1.3/test/testerrors.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testfuncs.py` & `AutoFeedback-1.3/test/testfuncs.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testplot.py` & `AutoFeedback-1.3/test/testplot.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testplotclass.py` & `AutoFeedback-1.3/test/testplotclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testprint.py` & `AutoFeedback-1.3/test/testprint.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testrandomclass.py` & `AutoFeedback-1.3/test/testrandomclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testsymp.py` & `AutoFeedback-1.3/test/testsymp.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testutils.py` & `AutoFeedback-1.3/test/testutils.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/test/testvars.py` & `AutoFeedback-1.3/test/testvars.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.2/versioneer.py` & `AutoFeedback-1.3/versioneer.py`

 * *Files identical despite different names*

