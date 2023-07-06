# Comparing `tmp/collei-0.1.2.tar.gz` & `tmp/collei-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collei-0.1.2.tar", max compression
+gzip compressed data, was "collei-1.0.0.tar", max compression
```

## Comparing `collei-0.1.2.tar` & `collei-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 collei-0.1.2/LICENSE
--rw-r--r--   0        0        0      893 2023-07-06 13:49:11.629535 collei-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      687 2023-07-06 13:49:07.539646 collei-0.1.2/README.md
--rw-r--r--   0        0        0      335 2023-07-06 06:43:30.608088 collei-0.1.2/src/collei/__init__.py
--rw-r--r--   0        0        0      412 2023-07-06 06:43:43.225123 collei-0.1.2/src/collei/clients.py
--rw-r--r--   0        0        0        6 2023-07-06 06:42:51.138083 collei-0.1.2/src/collei/managers/__init__.py
--rw-r--r--   0        0        0      433 2023-07-06 06:42:20.980352 collei-0.1.2/src/collei/managers/nsfw.py
--rw-r--r--   0        0        0      426 2023-07-06 06:42:23.243536 collei-0.1.2/src/collei/managers/sfw.py
--rw-r--r--   0        0        0        6 2023-07-06 06:43:22.637155 collei-0.1.2/src/collei/models/__init__.py
--rw-r--r--   0        0        0        6 2023-07-06 06:43:19.639228 collei-0.1.2/src/collei/models/enums/__init__.py
--rw-r--r--   0        0        0        6 2023-07-06 06:42:47.792143 collei-0.1.2/src/collei/models/enums/categories/__init__.py
--rw-r--r--   0        0        0      168 2023-07-06 06:42:35.909192 collei-0.1.2/src/collei/models/enums/categories/nsfw.py
--rw-r--r--   0        0        0      714 2023-07-06 06:42:42.136063 collei-0.1.2/src/collei/models/enums/categories/sfw.py
--rw-r--r--   0        0        0       61 2023-07-06 06:43:28.650121 collei-0.1.2/src/collei/models/images.py
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 collei-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 collei-1.0.0/LICENSE
+-rw-r--r--   0        0        0      893 2023-07-06 13:51:46.340984 collei-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      689 2023-07-06 13:51:27.424093 collei-1.0.0/README.md
+-rw-r--r--   0        0        0      335 2023-07-06 06:43:30.608088 collei-1.0.0/src/collei/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-06 06:43:43.225123 collei-1.0.0/src/collei/clients.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:42:51.138083 collei-1.0.0/src/collei/managers/__init__.py
+-rw-r--r--   0        0        0      433 2023-07-06 06:42:20.980352 collei-1.0.0/src/collei/managers/nsfw.py
+-rw-r--r--   0        0        0      426 2023-07-06 06:42:23.243536 collei-1.0.0/src/collei/managers/sfw.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:43:22.637155 collei-1.0.0/src/collei/models/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:43:19.639228 collei-1.0.0/src/collei/models/enums/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:42:47.792143 collei-1.0.0/src/collei/models/enums/categories/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-06 06:42:35.909192 collei-1.0.0/src/collei/models/enums/categories/nsfw.py
+-rw-r--r--   0        0        0      714 2023-07-06 06:42:42.136063 collei-1.0.0/src/collei/models/enums/categories/sfw.py
+-rw-r--r--   0        0        0       61 2023-07-06 06:43:28.650121 collei-1.0.0/src/collei/models/images.py
+-rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 collei-1.0.0/PKG-INFO
```

### Comparing `collei-0.1.2/LICENSE` & `collei-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `collei-0.1.2/pyproject.toml` & `collei-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "collei"
-version = "0.1.2"
+version = "1.0.0"
 description = "🍂 An unofficial Waifu.pics API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/collei"
 repository = "https://github.com/elaresai/collei"
```

### Comparing `collei-0.1.2/README.md` & `collei-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# xycu
+# collei
 🍂 An unofficial [*Waifu.pics*](https://waifu.pics) API wrapper for Python
 
 # 📦 Packages
 ## 🐍 PyPi
 ```sh
 pip install collei
 ```
```

### Comparing `collei-0.1.2/src/collei/models/enums/categories/sfw.py` & `collei-1.0.0/src/collei/models/enums/categories/sfw.py`

 * *Files identical despite different names*

### Comparing `collei-0.1.2/PKG-INFO` & `collei-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collei
-Version: 0.1.2
+Version: 1.0.0
 Summary: 🍂 An unofficial Waifu.pics API wrapper for Python
 Home-page: https://github.com/elaresai/collei
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/elaresai/collei
 Description-Content-Type: text/markdown
 
-# xycu
+# collei
 🍂 An unofficial [*Waifu.pics*](https://waifu.pics) API wrapper for Python
 
 # 📦 Packages
 ## 🐍 PyPi
 ```sh
 pip install collei
 ```
```

