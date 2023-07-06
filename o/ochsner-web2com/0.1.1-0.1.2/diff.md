# Comparing `tmp/ochsner_web2com-0.1.1.tar.gz` & `tmp/ochsner_web2com-0.1.2.tar.gz`

## Comparing `ochsner_web2com-0.1.1.tar` & `ochsner_web2com-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/build.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/src/__init__.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/src/web2com.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/LICENSE
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/README.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/.gitattributes
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/build.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/ochsner_web2com/__init__.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/ochsner_web2com/web2com.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/README.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.2/PKG-INFO
```

### Comparing `ochsner_web2com-0.1.1/src/web2com.py` & `ochsner_web2com-0.1.2/ochsner_web2com/web2com.py`

 * *Files identical despite different names*

### Comparing `ochsner_web2com-0.1.1/LICENSE` & `ochsner_web2com-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ochsner_web2com-0.1.1/README.md` & `ochsner_web2com-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ochsner_web2com-0.1.1/pyproject.toml` & `ochsner_web2com-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ochsner_web2com"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Alexander Hackl", email="pypi@eccoz.de" },
 ]
 description = "Access to the ochsner web2com interface"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ochsner_web2com-0.1.1/PKG-INFO` & `ochsner_web2com-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ochsner_web2com
-Version: 0.1.1
+Version: 0.1.2
 Summary: Access to the ochsner web2com interface
 Project-URL: Homepage, https://github.com/ahackl/pypi_ochsner_web2com
 Project-URL: Bug Tracker, https://github.com/ahackl/pypi_ochsner_web2com/issues
 Author-email: Alexander Hackl <pypi@eccoz.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

