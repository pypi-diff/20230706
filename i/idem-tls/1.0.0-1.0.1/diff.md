# Comparing `tmp/idem-tls-1.0.0.tar.gz` & `tmp/idem-tls-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-tls-1.0.0.tar", last modified: Mon Jun 26 15:46:15 2023, max compression
+gzip compressed data, was "idem-tls-1.0.1.tar", last modified: Wed Jul  5 23:52:13 2023, max compression
```

## Comparing `idem-tls-1.0.0.tar` & `idem-tls-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-06-26 15:46:02.000000 idem-tls-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5173 2023-06-26 15:46:15.721062 idem-tls-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4370 2023-06-26 15:46:02.000000 idem-tls-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/acct/tls/
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-26 15:46:02.000000 idem-tls-1.0.0/idem_tls/acct/tls/init.py
--rw-r--r--   0 root         (0) root         (0)     1319 2023-06-26 15:46:02.000000 idem-tls-1.0.0/idem_tls/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/exec/tls/
--rw-r--r--   0 root         (0) root         (0)     5305 2023-06-26 15:46:02.000000 idem-tls-1.0.0/idem_tls/exec/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-26 15:46:02.000000 idem-tls-1.0.0/idem_tls/exec/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/states/tls/
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-26 15:46:02.000000 idem-tls-1.0.0/idem_tls/states/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls/tool/tls/
--rw-r--r--   0 root         (0) root         (0)     2356 2023-06-26 15:46:02.000000 idem-tls-1.0.0/idem_tls/tool/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:46:15.000000 idem-tls-1.0.0/idem_tls/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:46:15.717062 idem-tls-1.0.0/idem_tls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5173 2023-06-26 15:46:15.000000 idem-tls-1.0.0/idem_tls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2023-06-26 15:46:15.000000 idem-tls-1.0.0/idem_tls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:46:15.000000 idem-tls-1.0.0/idem_tls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:46:15.000000 idem-tls-1.0.0/idem_tls.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-26 15:46:15.000000 idem-tls-1.0.0/idem_tls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-26 15:46:15.000000 idem-tls-1.0.0/idem_tls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:46:15.721062 idem-tls-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2716 2023-06-26 15:46:02.000000 idem-tls-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-07-05 23:51:58.000000 idem-tls-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5173 2023-07-05 23:52:13.618877 idem-tls-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-07-05 23:51:58.000000 idem-tls-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/acct/tls/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/acct/tls/init.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/exec/tls/
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/exec/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/exec/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/states/tls/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/states/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls/tool/tls/
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 23:51:58.000000 idem-tls-1.0.1/idem_tls/tool/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 23:52:13.618877 idem-tls-1.0.1/idem_tls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5173 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 23:52:13.000000 idem-tls-1.0.1/idem_tls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 23:52:13.618877 idem-tls-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-05 23:51:58.000000 idem-tls-1.0.1/setup.py
```

### Comparing `idem-tls-1.0.0/LICENSE` & `idem-tls-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.0/PKG-INFO` & `idem-tls-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-tls
-Version: 1.0.0
+Version: 1.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-tls-1.0.0/README.rst` & `idem-tls-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.0/idem_tls/conf.py` & `idem-tls-1.0.1/idem_tls/conf.py`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.0/idem_tls/exec/tls/certificate.py` & `idem-tls-1.0.1/idem_tls/exec/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.0/idem_tls/tool/tls/certificate.py` & `idem-tls-1.0.1/idem_tls/tool/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.0/idem_tls.egg-info/PKG-INFO` & `idem-tls-1.0.1/idem_tls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-tls
-Version: 1.0.0
+Version: 1.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-tls-1.0.0/setup.py` & `idem-tls-1.0.1/setup.py`

 * *Files identical despite different names*

