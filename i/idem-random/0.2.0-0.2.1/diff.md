# Comparing `tmp/idem-random-0.2.0.tar.gz` & `tmp/idem-random-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-random-0.2.0.tar", last modified: Fri Jun  2 18:46:15 2023, max compression
+gzip compressed data, was "idem-random-0.2.1.tar", last modified: Thu Jul  6 02:24:42 2023, max compression
```

## Comparing `idem-random-0.2.0.tar` & `idem-random-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    11329 2023-06-02 18:46:01.000000 idem-random-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3713 2023-06-02 18:46:15.323582 idem-random-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-02 18:46:01.000000 idem-random-0.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/
--rw-r--r--   0 root         (0) root         (0)     1293 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/exec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/exec/random/
--rw-r--r--   0 root         (0) root         (0)     2049 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/exec/random/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/idem_random/
--rw-r--r--   0 root         (0) root         (0)      836 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/idem_random/init.py
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/states/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/states/random/
--rw-r--r--   0 root         (0) root         (0)     4968 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/states/random/id.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/states/random/integer.py
--rw-r--r--   0 root         (0) root         (0)     7323 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/states/random/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/tool/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random/tool/random/
--rw-r--r--   0 root         (0) root         (0)      864 2023-06-02 18:46:01.000000 idem-random-0.2.0/idem_random/tool/random/id.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-02 18:46:14.000000 idem-random-0.2.0/idem_random/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 18:46:15.323582 idem-random-0.2.0/idem_random.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3713 2023-06-02 18:46:15.000000 idem-random-0.2.0/idem_random.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-02 18:46:15.000000 idem-random-0.2.0/idem_random.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 18:46:15.000000 idem-random-0.2.0/idem_random.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-02 18:46:15.000000 idem-random-0.2.0/idem_random.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-02 18:46:15.000000 idem-random-0.2.0/idem_random.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-02 18:46:15.000000 idem-random-0.2.0/idem_random.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-02 18:46:15.323582 idem-random-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2766 2023-06-02 18:46:01.000000 idem-random-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-07-06 02:24:27.000000 idem-random-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-06 02:24:42.512631 idem-random-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-06 02:24:27.000000 idem-random-0.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/exec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/exec/random/
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/exec/random/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/idem_random/
+-rw-r--r--   0 root         (0) root         (0)      836 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/idem_random/init.py
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/states/random/
+-rw-r--r--   0 root         (0) root         (0)     4968 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/random/id.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/random/integer.py
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/states/random/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/tool/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random/tool/random/
+-rw-r--r--   0 root         (0) root         (0)      864 2023-07-06 02:24:27.000000 idem-random-0.2.1/idem_random/tool/random/id.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 02:24:41.000000 idem-random-0.2.1/idem_random/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:24:42.512631 idem-random-0.2.1/idem_random.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-06 02:24:42.000000 idem-random-0.2.1/idem_random.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 02:24:42.512631 idem-random-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-07-06 02:24:27.000000 idem-random-0.2.1/setup.py
```

### Comparing `idem-random-0.2.0/LICENSE` & `idem-random-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/PKG-INFO` & `idem-random-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-random
-Version: 0.2.0
+Version: 0.2.1
 Summary: Idem plugin for providing randomness
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-random-0.2.0/README.rst` & `idem-random-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random/conf.py` & `idem-random-0.2.1/idem_random/conf.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random/exec/random/password.py` & `idem-random-0.2.1/idem_random/exec/random/password.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random/idem_random/init.py` & `idem-random-0.2.1/idem_random/idem_random/init.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random/states/random/id.py` & `idem-random-0.2.1/idem_random/states/random/id.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random/states/random/integer.py` & `idem-random-0.2.1/idem_random/states/random/integer.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random/states/random/password.py` & `idem-random-0.2.1/idem_random/states/random/password.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random/tool/random/id.py` & `idem-random-0.2.1/idem_random/tool/random/id.py`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/idem_random.egg-info/PKG-INFO` & `idem-random-0.2.1/idem_random.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-random
-Version: 0.2.0
+Version: 0.2.1
 Summary: Idem plugin for providing randomness
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-random-0.2.0/idem_random.egg-info/SOURCES.txt` & `idem-random-0.2.1/idem_random.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-random-0.2.0/setup.py` & `idem-random-0.2.1/setup.py`

 * *Files identical despite different names*

