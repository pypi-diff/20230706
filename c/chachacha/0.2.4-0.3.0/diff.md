# Comparing `tmp/chachacha-0.2.4.tar.gz` & `tmp/chachacha-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chachacha-0.2.4.tar", max compression
+gzip compressed data, was "chachacha-0.3.0.tar", max compression
```

## Comparing `chachacha-0.2.4.tar` & `chachacha-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4763 2023-06-10 11:39:23.648988 chachacha-0.2.4/README.md
--rw-r--r--   0        0        0       22 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/__init__.py
--rw-r--r--   0        0        0     1691 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/configuration.py
--rw-r--r--   0        0        0        0 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/drivers/__init__.py
--rw-r--r--   0        0        0     1629 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/drivers/git_provider.py
--rw-r--r--   0        0        0     4670 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/drivers/kac.py
--rw-r--r--   0        0        0     4250 2023-06-10 11:39:23.648988 chachacha-0.2.4/chachacha/main.py
--rw-r--r--   0        0        0     1029 2023-06-10 11:39:23.652989 chachacha-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5894 1970-01-01 00:00:00.000000 chachacha-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4763 2023-07-06 20:13:47.516147 chachacha-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-06 20:13:47.516147 chachacha-0.3.0/chachacha/__init__.py
+-rw-r--r--   0        0        0     1691 2023-07-06 20:13:47.516147 chachacha-0.3.0/chachacha/configuration.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:13:47.516147 chachacha-0.3.0/chachacha/drivers/__init__.py
+-rw-r--r--   0        0        0     1629 2023-07-06 20:13:47.516147 chachacha-0.3.0/chachacha/drivers/git_provider.py
+-rw-r--r--   0        0        0     4670 2023-07-06 20:13:47.516147 chachacha-0.3.0/chachacha/drivers/kac.py
+-rw-r--r--   0        0        0     4250 2023-07-06 20:13:47.516147 chachacha-0.3.0/chachacha/main.py
+-rw-r--r--   0        0        0     1029 2023-07-06 20:13:47.516147 chachacha-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5894 1970-01-01 00:00:00.000000 chachacha-0.3.0/PKG-INFO
```

### Comparing `chachacha-0.2.4/README.md` & `chachacha-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.4/chachacha/configuration.py` & `chachacha-0.3.0/chachacha/configuration.py`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.4/chachacha/drivers/git_provider.py` & `chachacha-0.3.0/chachacha/drivers/git_provider.py`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.4/chachacha/drivers/kac.py` & `chachacha-0.3.0/chachacha/drivers/kac.py`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.4/chachacha/main.py` & `chachacha-0.3.0/chachacha/main.py`

 * *Files identical despite different names*

### Comparing `chachacha-0.2.4/pyproject.toml` & `chachacha-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "chachacha"
 description = "Chachacha changes changelogs"
-version = "0.2.4"
+version = "0.3.0"
 authors = ["Alessandro Ogier <alessandro.ogier@gmail.com>"]
 readme = "README.md"
 license = "BSD"
 repository = "https://github.com/aogier/chachacha"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.8",
 ]
 
 [tool.poetry.scripts]
 chachacha = "chachacha.main:main"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 keepachangelog = "^0.3.1"
 click = "^8.1.0"
 jinja2 = "^3.1.0"
 semver = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
```

### Comparing `chachacha-0.2.4/PKG-INFO` & `chachacha-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: chachacha
-Version: 0.2.4
+Version: 0.3.0
 Summary: Chachacha changes changelogs
 Home-page: https://github.com/aogier/chachacha
 License: BSD
 Author: Alessandro Ogier
 Author-email: alessandro.ogier@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.0,<4.0.0)
 Requires-Dist: keepachangelog (>=0.3.1,<0.4.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/aogier/chachacha
 Description-Content-Type: text/markdown
```

