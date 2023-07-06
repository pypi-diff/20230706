# Comparing `tmp/pojediga-1.0.1.tar.gz` & `tmp/pojediga-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pojediga-1.0.1.tar", last modified: Thu Jul  6 17:30:38 2023, max compression
+gzip compressed data, was "pojediga-3.0.0.tar", last modified: Thu Jul  6 17:32:46 2023, max compression
```

## Comparing `pojediga-1.0.1.tar` & `pojediga-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:30:38.969336 pojediga-1.0.1/
--rw-r--r--   0 kryox      (501) staff       (20)     1009 2023-07-06 17:30:38.969105 pojediga-1.0.1/PKG-INFO
--rw-r--r--   0 kryox      (501) staff       (20)      612 2023-07-06 17:17:53.000000 pojediga-1.0.1/README.md
-drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:30:38.967805 pojediga-1.0.1/pojediga/
--rw-r--r--   0 kryox      (501) staff       (20)        0 2023-07-06 16:23:57.000000 pojediga-1.0.1/pojediga/__init__.py
--rw-r--r--   0 kryox      (501) staff       (20)      216 2023-07-06 17:21:55.000000 pojediga-1.0.1/pojediga/pojediga.py
-drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:30:38.968639 pojediga-1.0.1/pojediga.egg-info/
--rw-r--r--   0 kryox      (501) staff       (20)     1009 2023-07-06 17:30:38.000000 pojediga-1.0.1/pojediga.egg-info/PKG-INFO
--rw-r--r--   0 kryox      (501) staff       (20)      188 2023-07-06 17:30:38.000000 pojediga-1.0.1/pojediga.egg-info/SOURCES.txt
--rw-r--r--   0 kryox      (501) staff       (20)        1 2023-07-06 17:30:38.000000 pojediga-1.0.1/pojediga.egg-info/dependency_links.txt
--rw-r--r--   0 kryox      (501) staff       (20)        9 2023-07-06 17:30:38.000000 pojediga-1.0.1/pojediga.egg-info/top_level.txt
--rw-r--r--   0 kryox      (501) staff       (20)       38 2023-07-06 17:30:38.969425 pojediga-1.0.1/setup.cfg
--rw-r--r--   0 kryox      (501) staff       (20)      620 2023-07-06 17:30:18.000000 pojediga-1.0.1/setup.py
+drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:32:46.620742 pojediga-3.0.0/
+-rw-r--r--   0 kryox      (501) staff       (20)      943 2023-07-06 17:32:46.620498 pojediga-3.0.0/PKG-INFO
+-rw-r--r--   0 kryox      (501) staff       (20)      546 2023-07-06 17:32:35.000000 pojediga-3.0.0/README.md
+drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:32:46.619064 pojediga-3.0.0/pojediga/
+-rw-r--r--   0 kryox      (501) staff       (20)        0 2023-07-06 16:23:57.000000 pojediga-3.0.0/pojediga/__init__.py
+-rw-r--r--   0 kryox      (501) staff       (20)      216 2023-07-06 17:21:55.000000 pojediga-3.0.0/pojediga/pojediga.py
+drwxr-xr-x   0 kryox      (501) staff       (20)        0 2023-07-06 17:32:46.620127 pojediga-3.0.0/pojediga.egg-info/
+-rw-r--r--   0 kryox      (501) staff       (20)      943 2023-07-06 17:32:46.000000 pojediga-3.0.0/pojediga.egg-info/PKG-INFO
+-rw-r--r--   0 kryox      (501) staff       (20)      188 2023-07-06 17:32:46.000000 pojediga-3.0.0/pojediga.egg-info/SOURCES.txt
+-rw-r--r--   0 kryox      (501) staff       (20)        1 2023-07-06 17:32:46.000000 pojediga-3.0.0/pojediga.egg-info/dependency_links.txt
+-rw-r--r--   0 kryox      (501) staff       (20)        9 2023-07-06 17:32:46.000000 pojediga-3.0.0/pojediga.egg-info/top_level.txt
+-rw-r--r--   0 kryox      (501) staff       (20)       38 2023-07-06 17:32:46.620810 pojediga-3.0.0/setup.cfg
+-rw-r--r--   0 kryox      (501) staff       (20)      620 2023-07-06 17:31:51.000000 pojediga-3.0.0/setup.py
```

### Comparing `pojediga-1.0.1/PKG-INFO` & `pojediga-3.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pojediga
-Version: 1.0.1
+Version: 3.0.0
 Summary: A simple pojediga package to feel good every day, every night
 Author: 🇷🇸
 Author-email: ja_sam_lekar_za_sve@pojediga.rs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -27,17 +27,12 @@
 
 
 ## Installation
 You can install the pojediga library using pip:
 `pip install pojediga`
 
 
-
 ---
-
-## Methods
-```mermaid
-graph LR
-A[Available Commands] --> B((pojedi_ga))
-A --> E((noga))
-A --> C((masala))
-```
+Available Methods:
+- pojediga
+- noga
+- masala
```

### Comparing `pojediga-1.0.1/README.md` & `pojediga-3.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -15,17 +15,12 @@
 
 
 ## Installation
 You can install the pojediga library using pip:
 `pip install pojediga`
 
 
-
 ---
-
-## Methods
-```mermaid
-graph LR
-A[Available Commands] --> B((pojedi_ga))
-A --> E((noga))
-A --> C((masala))
-```
+Available Methods:
+- pojediga
+- noga
+- masala
```

### Comparing `pojediga-1.0.1/pojediga.egg-info/PKG-INFO` & `pojediga-3.0.0/pojediga.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pojediga
-Version: 1.0.1
+Version: 3.0.0
 Summary: A simple pojediga package to feel good every day, every night
 Author: 🇷🇸
 Author-email: ja_sam_lekar_za_sve@pojediga.rs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -27,17 +27,12 @@
 
 
 ## Installation
 You can install the pojediga library using pip:
 `pip install pojediga`
 
 
-
 ---
-
-## Methods
-```mermaid
-graph LR
-A[Available Commands] --> B((pojedi_ga))
-A --> E((noga))
-A --> C((masala))
-```
+Available Methods:
+- pojediga
+- noga
+- masala
```

### Comparing `pojediga-1.0.1/setup.py` & `pojediga-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pojediga",
-    version="1.0.1",
+    version="3.0.0",
     author="🇷🇸",
     author_email="ja_sam_lekar_za_sve@pojediga.rs",
     description="A simple pojediga package to feel good every day, every night",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["pojediga"],
     classifiers=[
```

