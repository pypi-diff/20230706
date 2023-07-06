# Comparing `tmp/pojediga-3.0.1.tar.gz` & `tmp/pojediga-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pojediga-3.0.1.tar", last modified: Thu Jul  6 17:46:14 2023, max compression
+gzip compressed data, was "pojediga-3.0.3.tar", last modified: Thu Jul  6 17:53:49 2023, max compression
```

## Comparing `pojediga-3.0.1.tar` & `pojediga-3.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:46:14.963089 pojediga-3.0.1/
--rw-r--r--   0 kryox      (501) staff       (20)      943 2023-07-06 17:46:14.962898 pojediga-3.0.1/PKG-INFO
--rw-r--r--   0 kryox      (501) staff       (20)      546 2023-07-06 17:32:35.000000 pojediga-3.0.1/README.md
-drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:46:14.961722 pojediga-3.0.1/pojediga/
--rw-r--r--   0 kryox      (501) staff       (20)       54 2023-07-06 17:44:39.000000 pojediga-3.0.1/pojediga/__init__.py
--rw-r--r--   0 kryox      (501) staff       (20)      216 2023-07-06 17:21:55.000000 pojediga-3.0.1/pojediga/pojediga.py
-drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:46:14.962598 pojediga-3.0.1/pojediga.egg-info/
--rw-r--r--   0 kryox      (501) staff       (20)      943 2023-07-06 17:46:14.000000 pojediga-3.0.1/pojediga.egg-info/PKG-INFO
--rw-r--r--   0 kryox      (501) staff       (20)      188 2023-07-06 17:46:14.000000 pojediga-3.0.1/pojediga.egg-info/SOURCES.txt
--rw-r--r--   0 kryox      (501) staff       (20)        1 2023-07-06 17:46:14.000000 pojediga-3.0.1/pojediga.egg-info/dependency_links.txt
--rw-r--r--   0 kryox      (501) staff       (20)        9 2023-07-06 17:46:14.000000 pojediga-3.0.1/pojediga.egg-info/top_level.txt
--rw-r--r--   0 kryox      (501) staff       (20)       38 2023-07-06 17:46:14.963152 pojediga-3.0.1/setup.cfg
--rw-r--r--   0 kryox      (501) staff       (20)      620 2023-07-06 17:45:32.000000 pojediga-3.0.1/setup.py
+drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:53:49.125805 pojediga-3.0.3/
+-rw-r--r--   0 kryox      (501) staff       (20)      943 2023-07-06 17:53:49.125592 pojediga-3.0.3/PKG-INFO
+-rw-r--r--   0 kryox      (501) staff       (20)      546 2023-07-06 17:32:35.000000 pojediga-3.0.3/README.md
+drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:53:49.124394 pojediga-3.0.3/pojediga/
+-rw-r--r--   0 kryox      (501) staff       (20)       54 2023-07-06 17:44:39.000000 pojediga-3.0.3/pojediga/__init__.py
+-rw-r--r--   0 kryox      (501) staff       (20)      249 2023-07-06 17:53:18.000000 pojediga-3.0.3/pojediga/pojediga.py
+drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:53:49.125246 pojediga-3.0.3/pojediga.egg-info/
+-rw-r--r--   0 kryox      (501) staff       (20)      943 2023-07-06 17:53:49.000000 pojediga-3.0.3/pojediga.egg-info/PKG-INFO
+-rw-r--r--   0 kryox      (501) staff       (20)      188 2023-07-06 17:53:49.000000 pojediga-3.0.3/pojediga.egg-info/SOURCES.txt
+-rw-r--r--   0 kryox      (501) staff       (20)        1 2023-07-06 17:53:49.000000 pojediga-3.0.3/pojediga.egg-info/dependency_links.txt
+-rw-r--r--   0 kryox      (501) staff       (20)        9 2023-07-06 17:53:49.000000 pojediga-3.0.3/pojediga.egg-info/top_level.txt
+-rw-r--r--   0 kryox      (501) staff       (20)       38 2023-07-06 17:53:49.125872 pojediga-3.0.3/setup.cfg
+-rw-r--r--   0 kryox      (501) staff       (20)      620 2023-07-06 17:53:36.000000 pojediga-3.0.3/setup.py
```

### Comparing `pojediga-3.0.1/PKG-INFO` & `pojediga-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pojediga
-Version: 3.0.1
+Version: 3.0.3
 Summary: A simple pojediga package to feel good every day, every night
 Author: 🇷🇸
 Author-email: ja_sam_lekar_za_sve@pojediga.rs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `pojediga-3.0.1/README.md` & `pojediga-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pojediga-3.0.1/pojediga.egg-info/PKG-INFO` & `pojediga-3.0.3/pojediga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pojediga
-Version: 3.0.1
+Version: 3.0.3
 Summary: A simple pojediga package to feel good every day, every night
 Author: 🇷🇸
 Author-email: ja_sam_lekar_za_sve@pojediga.rs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `pojediga-3.0.1/setup.py` & `pojediga-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pojediga",
-    version="3.0.1",
+    version="3.0.3",
     author="🇷🇸",
     author_email="ja_sam_lekar_za_sve@pojediga.rs",
     description="A simple pojediga package to feel good every day, every night",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["pojediga"],
     classifiers=[
```

