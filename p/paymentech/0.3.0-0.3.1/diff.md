# Comparing `tmp/paymentech-0.3.0.tar.gz` & `tmp/paymentech-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paymentech-0.3.0.tar", last modified: Mon Apr 10 14:25:10 2023, max compression
+gzip compressed data, was "paymentech-0.3.1.tar", last modified: Thu Jul  6 17:15:06 2023, max compression
```

## Comparing `paymentech-0.3.0.tar` & `paymentech-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 14:25:04.000000 paymentech-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 14:25:09.990123 paymentech-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 14:25:04.000000 paymentech-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/paymentech/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/paymentech/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/inquiry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/service.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 14:25:04.000000 paymentech-0.3.0/paymentech/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/paymentech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 14:25:09.000000 paymentech-0.3.0/paymentech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 14:25:09.990123 paymentech-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-10 14:25:04.000000 paymentech-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:09.990123 paymentech-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:25:04.000000 paymentech-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-10 14:25:04.000000 paymentech-0.3.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 14:25:04.000000 paymentech-0.3.0/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:15:06.041828 paymentech-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-06 17:15:04.000000 paymentech-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 17:15:06.041828 paymentech-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 17:15:04.000000 paymentech-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:15:06.037828 paymentech-0.3.1/paymentech/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:15:06.041828 paymentech-0.3.1/paymentech/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/resources/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/resources/inquiry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/resources/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 17:15:04.000000 paymentech-0.3.1/paymentech/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:15:06.037828 paymentech-0.3.1/paymentech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 17:15:05.000000 paymentech-0.3.1/paymentech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 17:15:06.000000 paymentech-0.3.1/paymentech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:15:05.000000 paymentech-0.3.1/paymentech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 17:15:05.000000 paymentech-0.3.1/paymentech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 17:15:05.000000 paymentech-0.3.1/paymentech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 17:15:06.041828 paymentech-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 17:15:04.000000 paymentech-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:15:06.041828 paymentech-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:15:04.000000 paymentech-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 17:15:04.000000 paymentech-0.3.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 17:15:04.000000 paymentech-0.3.1/tests/test_sanity.py
```

### Comparing `paymentech-0.3.0/LICENSE` & `paymentech-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/PKG-INFO` & `paymentech-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paymentech
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for Chase Paymentech
 Home-page: https://github.com/SerenitySoftware/paymentech
 Author: Jordan Ambra
 Author-email: jordan@serenity.software
 License: UNKNOWN
 Description: # Chase Paymentech SDK
         Python SDK for Chase Paymentech
```

### Comparing `paymentech-0.3.0/paymentech/__init__.py` & `paymentech-0.3.1/paymentech/__init__.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech/resources/authorization.py` & `paymentech-0.3.1/paymentech/resources/authorization.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech/resources/base.py` & `paymentech-0.3.1/paymentech/resources/base.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech/resources/inquiry.py` & `paymentech-0.3.1/paymentech/resources/inquiry.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech/resources/order.py` & `paymentech-0.3.1/paymentech/resources/order.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech/resources/profile.py` & `paymentech-0.3.1/paymentech/resources/profile.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech/resources/reversal.py` & `paymentech-0.3.1/paymentech/resources/reversal.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech/service.py` & `paymentech-0.3.1/paymentech/service.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/paymentech.egg-info/PKG-INFO` & `paymentech-0.3.1/paymentech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paymentech
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for Chase Paymentech
 Home-page: https://github.com/SerenitySoftware/paymentech
 Author: Jordan Ambra
 Author-email: jordan@serenity.software
 License: UNKNOWN
 Description: # Chase Paymentech SDK
         Python SDK for Chase Paymentech
```

### Comparing `paymentech-0.3.0/paymentech.egg-info/SOURCES.txt` & `paymentech-0.3.1/paymentech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.0/setup.py` & `paymentech-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 version_path = os.path.join(os.path.split(__file__)[0], "paymentech/version.py")
 with open(version_path) as version_file:
     version = ""
     # Execute the code in version.py.
     exec(compile(version_file.read(), version_path, 'exec'))
 
+with open("requirements.txt", "r") as requirements_file:
+    install_requires = requirements_file.read().splitlines()
+
 setuptools.setup(
     name="paymentech",
     version=version,
     author="Jordan Ambra",
     author_email="jordan@serenity.software",
     description="Python SDK for Chase Paymentech",
     long_description=long_description,
@@ -26,10 +29,10 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
         "License :: Freely Distributable"
     ],
     keywords=['chase', 'paymentech', 'e-commerce', 'payments'],
-    install_requires=['requests', 'pydantic'],
+    install_requires=install_requires,
     package_data={'paymentech': ['templates/*.xml']}
 )
```

### Comparing `paymentech-0.3.0/tests/test_configuration.py` & `paymentech-0.3.1/tests/test_configuration.py`

 * *Files identical despite different names*

