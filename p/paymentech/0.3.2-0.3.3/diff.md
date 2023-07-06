# Comparing `tmp/paymentech-0.3.2.tar.gz` & `tmp/paymentech-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paymentech-0.3.2.tar", last modified: Thu Jul  6 17:24:08 2023, max compression
+gzip compressed data, was "paymentech-0.3.3.tar", last modified: Thu Jul  6 17:38:52 2023, max compression
```

## Comparing `paymentech-0.3.2.tar` & `paymentech-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:24:08.371419 paymentech-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-06 17:24:07.000000 paymentech-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 17:24:08.371419 paymentech-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 17:24:07.000000 paymentech-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:24:08.371419 paymentech-0.3.2/paymentech/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:24:08.371419 paymentech-0.3.2/paymentech/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/resources/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/resources/inquiry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/resources/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/service.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 17:24:07.000000 paymentech-0.3.2/paymentech/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:24:08.371419 paymentech-0.3.2/paymentech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 17:24:08.000000 paymentech-0.3.2/paymentech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 17:24:08.000000 paymentech-0.3.2/paymentech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:24:08.000000 paymentech-0.3.2/paymentech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 17:24:08.000000 paymentech-0.3.2/paymentech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 17:24:08.000000 paymentech-0.3.2/paymentech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 17:24:08.371419 paymentech-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-06 17:24:07.000000 paymentech-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:24:08.371419 paymentech-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:24:07.000000 paymentech-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 17:24:07.000000 paymentech-0.3.2/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 17:24:07.000000 paymentech-0.3.2/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:38:52.485790 paymentech-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-06 17:38:49.000000 paymentech-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 17:38:52.485790 paymentech-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 17:38:49.000000 paymentech-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:38:52.481790 paymentech-0.3.3/paymentech/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:38:52.485790 paymentech-0.3.3/paymentech/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/resources/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/resources/inquiry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/resources/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 17:38:49.000000 paymentech-0.3.3/paymentech/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:38:52.481790 paymentech-0.3.3/paymentech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 17:38:52.000000 paymentech-0.3.3/paymentech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 17:38:52.000000 paymentech-0.3.3/paymentech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:38:52.000000 paymentech-0.3.3/paymentech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 17:38:52.000000 paymentech-0.3.3/paymentech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 17:38:52.000000 paymentech-0.3.3/paymentech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 17:38:52.485790 paymentech-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-06 17:38:49.000000 paymentech-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:38:52.485790 paymentech-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:38:49.000000 paymentech-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 17:38:49.000000 paymentech-0.3.3/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 17:38:49.000000 paymentech-0.3.3/tests/test_sanity.py
```

### Comparing `paymentech-0.3.2/LICENSE` & `paymentech-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/PKG-INFO` & `paymentech-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paymentech
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python SDK for Chase Paymentech
 Home-page: https://github.com/SerenitySoftware/paymentech
 Author: Jordan Ambra
 Author-email: jordan@serenity.software
 License: UNKNOWN
 Description: # Chase Paymentech SDK
         Python SDK for Chase Paymentech
```

### Comparing `paymentech-0.3.2/paymentech/__init__.py` & `paymentech-0.3.3/paymentech/__init__.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech/resources/authorization.py` & `paymentech-0.3.3/paymentech/resources/authorization.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech/resources/base.py` & `paymentech-0.3.3/paymentech/resources/base.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech/resources/inquiry.py` & `paymentech-0.3.3/paymentech/resources/inquiry.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech/resources/order.py` & `paymentech-0.3.3/paymentech/resources/order.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech/resources/profile.py` & `paymentech-0.3.3/paymentech/resources/profile.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech/resources/reversal.py` & `paymentech-0.3.3/paymentech/resources/reversal.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech/service.py` & `paymentech-0.3.3/paymentech/service.py`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/paymentech.egg-info/PKG-INFO` & `paymentech-0.3.3/paymentech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paymentech
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python SDK for Chase Paymentech
 Home-page: https://github.com/SerenitySoftware/paymentech
 Author: Jordan Ambra
 Author-email: jordan@serenity.software
 License: UNKNOWN
 Description: # Chase Paymentech SDK
         Python SDK for Chase Paymentech
```

### Comparing `paymentech-0.3.2/paymentech.egg-info/SOURCES.txt` & `paymentech-0.3.3/paymentech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paymentech-0.3.2/setup.py` & `paymentech-0.3.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 
 version_path = os.path.join(base_path, "paymentech/version.py")
 with open(version_path, "r") as version_file:
     version = ""
     # Execute the code in version.py.
     exec(compile(version_file.read(), version_path, 'exec'))
 
-requirements_path = os.path.join(base_path, "requirements.txt")
-with open(requirements_path, "r") as requirements_file:
-    install_requires = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="paymentech",
     version=version,
     author="Jordan Ambra",
     author_email="jordan@serenity.software",
     description="Python SDK for Chase Paymentech",
@@ -33,10 +30,10 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
         "License :: Freely Distributable"
     ],
     keywords=['chase', 'paymentech', 'e-commerce', 'payments'],
-    install_requires=install_requires,
+    install_requires=["pydantic==1.6.2", "requests==2.24.0"],
     package_data={'paymentech': ['templates/*.xml']}
 )
```

### Comparing `paymentech-0.3.2/tests/test_configuration.py` & `paymentech-0.3.3/tests/test_configuration.py`

 * *Files identical despite different names*

