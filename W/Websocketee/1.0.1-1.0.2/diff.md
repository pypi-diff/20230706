# Comparing `tmp/Websocketee-1.0.1.tar.gz` & `tmp/Websocketee-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Websocketee-1.0.1.tar", last modified: Thu Jul  6 10:08:49 2023, max compression
+gzip compressed data, was "Websocketee-1.0.2.tar", last modified: Thu Jul  6 10:14:53 2023, max compression
```

## Comparing `Websocketee-1.0.1.tar` & `Websocketee-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:08:49.077747 Websocketee-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-05 10:45:18.000000 Websocketee-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1290 2023-07-06 10:08:49.077747 Websocketee-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-07-05 10:55:31.000000 Websocketee-1.0.1/README.md
--rw-rw-rw-   0        0        0      110 2023-07-06 06:11:35.000000 Websocketee-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      826 2023-07-06 10:08:49.082744 Websocketee-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 10:08:49.035774 Websocketee-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 10:08:49.076747 Websocketee-1.0.1/src/Websocketee.egg-info/
--rw-rw-rw-   0        0        0     1290 2023-07-06 10:08:48.000000 Websocketee-1.0.1/src/Websocketee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-06 10:08:49.000000 Websocketee-1.0.1/src/Websocketee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:08:48.000000 Websocketee-1.0.1/src/Websocketee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-06 10:08:48.000000 Websocketee-1.0.1/src/Websocketee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:08:48.000000 Websocketee-1.0.1/src/Websocketee.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 10:14:53.632736 Websocketee-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-05 10:45:18.000000 Websocketee-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1290 2023-07-06 10:14:53.633736 Websocketee-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-07-05 10:55:31.000000 Websocketee-1.0.2/README.md
+-rw-rw-rw-   0        0        0      110 2023-07-06 06:11:35.000000 Websocketee-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      826 2023-07-06 10:14:53.636734 Websocketee-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 10:14:53.590762 Websocketee-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 10:14:53.631737 Websocketee-1.0.2/src/Websocketee.egg-info/
+-rw-rw-rw-   0        0        0     1290 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/top_level.txt
```

### Comparing `Websocketee-1.0.1/LICENSE` & `Websocketee-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Websocketee-1.0.1/PKG-INFO` & `Websocketee-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Websocketee
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Isnta-Bot for spaming
 Home-page: https://github.com/pypa/Insta-Spam
 Author: sm02present , SM02
 Author-email: rajnikantmahato@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/Insta-Spam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `Websocketee-1.0.1/README.md` & `Websocketee-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Websocketee-1.0.1/setup.cfg` & `Websocketee-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2057 6562 736f 636b 6574 6565 0d0a   = Websocketee..
-00000020: 7665 7273 696f 6e20 3d20 312e 302e 310d  version = 1.0.1.
+00000020: 7665 7273 696f 6e20 3d20 312e 302e 320d  version = 1.0.2.
 00000030: 0a64 6174 6520 3d20 3132 2f30 322f 3230  .date = 12/02/20
 00000040: 3232 0d0a 6175 7468 6f72 203d 2073 6d30  22..author = sm0
 00000050: 3270 7265 7365 6e74 202c 2053 4d30 320d  2present , SM02.
 00000060: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000070: 7261 6a6e 696b 616e 746d 6168 6174 6f40  rajnikantmahato@
 00000080: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000090: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python
```

### Comparing `Websocketee-1.0.1/src/Websocketee.egg-info/PKG-INFO` & `Websocketee-1.0.2/src/Websocketee.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Websocketee
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Isnta-Bot for spaming
 Home-page: https://github.com/pypa/Insta-Spam
 Author: sm02present , SM02
 Author-email: rajnikantmahato@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/Insta-Spam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
```

