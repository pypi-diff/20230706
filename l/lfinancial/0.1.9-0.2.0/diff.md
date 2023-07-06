# Comparing `tmp/lfinancial-0.1.9.tar.gz` & `tmp/lfinancial-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.1.9.tar", last modified: Wed Jul  5 13:23:49 2023, max compression
+gzip compressed data, was "lfinancial-0.2.0.tar", last modified: Thu Jul  6 09:22:29 2023, max compression
```

## Comparing `lfinancial-0.1.9.tar` & `lfinancial-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-05 13:23:25.000000 lfinancial-0.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-05 13:23:49.309429 lfinancial-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-05 13:23:25.000000 lfinancial-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 13:23:25.000000 lfinancial-0.1.9/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-05 13:23:25.000000 lfinancial-0.1.9/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 13:23:25.000000 lfinancial-0.1.9/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 13:23:49.000000 lfinancial-0.1.9/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:23:49.309429 lfinancial-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-05 13:23:25.000000 lfinancial-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:23:49.309429 lfinancial-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 13:23:25.000000 lfinancial-0.1.9/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-06 09:22:11.000000 lfinancial-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 09:22:29.607624 lfinancial-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-06 09:22:11.000000 lfinancial-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-06 09:22:11.000000 lfinancial-0.2.0/lfinancial/generators/phone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 09:22:29.000000 lfinancial-0.2.0/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:22:29.607624 lfinancial-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-06 09:22:11.000000 lfinancial-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:22:29.607624 lfinancial-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 09:22:11.000000 lfinancial-0.2.0/tests/test_document.py
```

### Comparing `lfinancial-0.1.9/LICENSE.txt` & `lfinancial-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.9/PKG-INFO` & `lfinancial-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.9
+Version: 0.2.0
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lfinancial-0.1.9/README.md` & `lfinancial-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.9/lfinancial/factory.py` & `lfinancial-0.2.0/lfinancial/factory.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.9/lfinancial/financial.py` & `lfinancial-0.2.0/lfinancial/financial.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.9/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.2.0/lfinancial.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.9
+Version: 0.2.0
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

