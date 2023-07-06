# Comparing `tmp/IAMPASS-0.0.31.tar.gz` & `tmp/IAMPASS-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/IAMPASS-0.0.31.tar", last modified: Mon Oct 31 17:30:29 2022, max compression
+gzip compressed data, was "dist/IAMPASS-0.0.32.tar", last modified: Thu Jul  6 15:19:28 2023, max compression
```

## Comparing `IAMPASS-0.0.31.tar` & `IAMPASS-0.0.32.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jasonmullings   (501) staff       (20)        0 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/
-drwxr-xr-x   0 jasonmullings   (501) staff       (20)        0 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/IAMPASS/
--rw-r--r--   0 jasonmullings   (501) staff       (20)        0 2020-03-30 19:52:48.000000 IAMPASS-0.0.31/IAMPASS/__init__.py
--rw-r--r--   0 jasonmullings   (501) staff       (20)     4314 2022-10-31 17:21:11.000000 IAMPASS-0.0.31/IAMPASS/authentication_api.py
--rw-r--r--   0 jasonmullings   (501) staff       (20)      187 2020-03-30 14:53:42.000000 IAMPASS-0.0.31/IAMPASS/authentication_method.py
--rw-r--r--   0 jasonmullings   (501) staff       (20)      120 2022-10-31 16:50:39.000000 IAMPASS-0.0.31/IAMPASS/config.py
--rw-r--r--   0 jasonmullings   (501) staff       (20)     1429 2022-02-18 20:00:04.000000 IAMPASS-0.0.31/IAMPASS/hmac.py
--rw-r--r--   0 jasonmullings   (501) staff       (20)    12909 2022-02-18 19:43:26.000000 IAMPASS-0.0.31/IAMPASS/management_api.py
--rw-r--r--   0 jasonmullings   (501) staff       (20)     6421 2022-02-18 19:39:43.000000 IAMPASS-0.0.31/IAMPASS/session.py
--rw-r--r--   0 jasonmullings   (501) staff       (20)      175 2020-03-25 03:15:59.000000 IAMPASS-0.0.31/IAMPASS/status.py
-drwxr-xr-x   0 jasonmullings   (501) staff       (20)        0 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/IAMPASS.egg-info/
--rw-r--r--   0 jasonmullings   (501) staff       (20)     8436 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/IAMPASS.egg-info/PKG-INFO
--rw-r--r--   0 jasonmullings   (501) staff       (20)      352 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/IAMPASS.egg-info/SOURCES.txt
--rw-r--r--   0 jasonmullings   (501) staff       (20)        1 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/IAMPASS.egg-info/dependency_links.txt
--rw-r--r--   0 jasonmullings   (501) staff       (20)       39 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/IAMPASS.egg-info/requires.txt
--rw-r--r--   0 jasonmullings   (501) staff       (20)        8 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/IAMPASS.egg-info/top_level.txt
--rw-r--r--   0 jasonmullings   (501) staff       (20)     8436 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/PKG-INFO
--rw-r--r--   0 jasonmullings   (501) staff       (20)     6643 2022-10-31 16:42:11.000000 IAMPASS-0.0.31/README.md
--rw-r--r--   0 jasonmullings   (501) staff       (20)       38 2022-10-31 17:30:29.000000 IAMPASS-0.0.31/setup.cfg
--rw-r--r--   0 jasonmullings   (501) staff       (20)      691 2022-10-31 17:30:21.000000 IAMPASS-0.0.31/setup.py
+drwxr-xr-x   0 jasonmullings   (501) staff       (20)        0 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/
+drwxr-xr-x   0 jasonmullings   (501) staff       (20)        0 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/IAMPASS/
+-rw-r--r--   0 jasonmullings   (501) staff       (20)        0 2022-10-31 17:41:53.000000 IAMPASS-0.0.32/IAMPASS/__init__.py
+-rw-r--r--   0 jasonmullings   (501) staff       (20)     4314 2022-10-31 17:41:53.000000 IAMPASS-0.0.32/IAMPASS/authentication_api.py
+-rw-r--r--   0 jasonmullings   (501) staff       (20)      187 2022-10-31 17:41:53.000000 IAMPASS-0.0.32/IAMPASS/authentication_method.py
+-rw-r--r--   0 jasonmullings   (501) staff       (20)      115 2023-07-06 15:16:56.000000 IAMPASS-0.0.32/IAMPASS/config.py
+-rw-r--r--   0 jasonmullings   (501) staff       (20)     1429 2022-10-31 17:41:53.000000 IAMPASS-0.0.32/IAMPASS/hmac.py
+-rw-r--r--   0 jasonmullings   (501) staff       (20)    12909 2022-10-31 17:41:53.000000 IAMPASS-0.0.32/IAMPASS/management_api.py
+-rw-r--r--   0 jasonmullings   (501) staff       (20)     6421 2022-10-31 17:43:54.000000 IAMPASS-0.0.32/IAMPASS/session.py
+-rw-r--r--   0 jasonmullings   (501) staff       (20)      175 2022-10-31 17:41:53.000000 IAMPASS-0.0.32/IAMPASS/status.py
+drwxr-xr-x   0 jasonmullings   (501) staff       (20)        0 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/IAMPASS.egg-info/
+-rw-r--r--   0 jasonmullings   (501) staff       (20)     8421 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/IAMPASS.egg-info/PKG-INFO
+-rw-r--r--   0 jasonmullings   (501) staff       (20)      352 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/IAMPASS.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonmullings   (501) staff       (20)        1 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/IAMPASS.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonmullings   (501) staff       (20)       39 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/IAMPASS.egg-info/requires.txt
+-rw-r--r--   0 jasonmullings   (501) staff       (20)        8 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/IAMPASS.egg-info/top_level.txt
+-rw-r--r--   0 jasonmullings   (501) staff       (20)     8421 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/PKG-INFO
+-rw-r--r--   0 jasonmullings   (501) staff       (20)     6628 2023-07-06 15:16:56.000000 IAMPASS-0.0.32/README.md
+-rw-r--r--   0 jasonmullings   (501) staff       (20)       38 2023-07-06 15:19:28.000000 IAMPASS-0.0.32/setup.cfg
+-rw-r--r--   0 jasonmullings   (501) staff       (20)      691 2023-07-06 15:16:56.000000 IAMPASS-0.0.32/setup.py
```

### Comparing `IAMPASS-0.0.31/IAMPASS/authentication_api.py` & `IAMPASS-0.0.32/IAMPASS/authentication_api.py`

 * *Files identical despite different names*

### Comparing `IAMPASS-0.0.31/IAMPASS/hmac.py` & `IAMPASS-0.0.32/IAMPASS/hmac.py`

 * *Files identical despite different names*

### Comparing `IAMPASS-0.0.31/IAMPASS/management_api.py` & `IAMPASS-0.0.32/IAMPASS/management_api.py`

 * *Files identical despite different names*

### Comparing `IAMPASS-0.0.31/IAMPASS/session.py` & `IAMPASS-0.0.32/IAMPASS/session.py`

 * *Files identical despite different names*

### Comparing `IAMPASS-0.0.31/IAMPASS.egg-info/PKG-INFO` & `IAMPASS-0.0.32/IAMPASS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: IAMPASS
-Version: 0.0.31
+Version: 0.0.32
 Summary: Python package to access IAMPASS API
 Home-page: UNKNOWN
 Author: IAMPASS
 Author-email: support@iampass.com
 License: UNKNOWN
 Description: # IAMPASS
         
-        [IAMPASS](https://main.iampass.com) provides multifactor identity and presence verification.
+        [IAMPASS](https://iampass.com) provides multifactor identity and presence verification.
         
         
         This library provides a Python wrapper for the IAMPASS API.
         
         ## Getting Started
         ### Create an IAMPASS Account
-        To begin visit [IAMPASS Developer Portal](https://main.iam-api.com/register) to register.
+        To begin visit [IAMPASS Developer Portal](https://iam-api.com/register) to register.
         ### Create an IAMPASS Application
-        Once you have registered [create a new IAMPASS application](https://main.iam-api.com/create_application).
+        Once you have registered [create a new IAMPASS application](https://iam-api.com/create_application).
         Save the Application ID and Application Secret in a safe place as you will need this to authenticate calls to the IAMPASS API.
         ### Register Users
         IAMPASS identifies application users using a token supplied by the application developer.
         You can use your existing user IDs or create a lookup table that maps your user ID to a value you provide to IAMPASS.
         
         Users are registered using the IAMPASS ManagementAPI.
         Create an instance of IAMPASS.ManagementAPI using your application ID and secret.
```

### Comparing `IAMPASS-0.0.31/PKG-INFO` & `IAMPASS-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: IAMPASS
-Version: 0.0.31
+Version: 0.0.32
 Summary: Python package to access IAMPASS API
 Home-page: UNKNOWN
 Author: IAMPASS
 Author-email: support@iampass.com
 License: UNKNOWN
 Description: # IAMPASS
         
-        [IAMPASS](https://main.iampass.com) provides multifactor identity and presence verification.
+        [IAMPASS](https://iampass.com) provides multifactor identity and presence verification.
         
         
         This library provides a Python wrapper for the IAMPASS API.
         
         ## Getting Started
         ### Create an IAMPASS Account
-        To begin visit [IAMPASS Developer Portal](https://main.iam-api.com/register) to register.
+        To begin visit [IAMPASS Developer Portal](https://iam-api.com/register) to register.
         ### Create an IAMPASS Application
-        Once you have registered [create a new IAMPASS application](https://main.iam-api.com/create_application).
+        Once you have registered [create a new IAMPASS application](https://iam-api.com/create_application).
         Save the Application ID and Application Secret in a safe place as you will need this to authenticate calls to the IAMPASS API.
         ### Register Users
         IAMPASS identifies application users using a token supplied by the application developer.
         You can use your existing user IDs or create a lookup table that maps your user ID to a value you provide to IAMPASS.
         
         Users are registered using the IAMPASS ManagementAPI.
         Create an instance of IAMPASS.ManagementAPI using your application ID and secret.
```

### Comparing `IAMPASS-0.0.31/README.md` & `IAMPASS-0.0.32/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # IAMPASS
 
-[IAMPASS](https://main.iampass.com) provides multifactor identity and presence verification.
+[IAMPASS](https://iampass.com) provides multifactor identity and presence verification.
 
 
 This library provides a Python wrapper for the IAMPASS API.
 
 ## Getting Started
 ### Create an IAMPASS Account
-To begin visit [IAMPASS Developer Portal](https://main.iam-api.com/register) to register.
+To begin visit [IAMPASS Developer Portal](https://iam-api.com/register) to register.
 ### Create an IAMPASS Application
-Once you have registered [create a new IAMPASS application](https://main.iam-api.com/create_application).
+Once you have registered [create a new IAMPASS application](https://iam-api.com/create_application).
 Save the Application ID and Application Secret in a safe place as you will need this to authenticate calls to the IAMPASS API.
 ### Register Users
 IAMPASS identifies application users using a token supplied by the application developer.
 You can use your existing user IDs or create a lookup table that maps your user ID to a value you provide to IAMPASS.
 
 Users are registered using the IAMPASS ManagementAPI.
 Create an instance of IAMPASS.ManagementAPI using your application ID and secret.
```

### Comparing `IAMPASS-0.0.31/setup.py` & `IAMPASS-0.0.32/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="IAMPASS",
-    version="0.0.31",
+    version="0.0.32",
     author="IAMPASS",
     author_email="support@iampass.com",
     description="Python package to access IAMPASS API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
```

