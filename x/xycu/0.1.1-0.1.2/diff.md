# Comparing `tmp/xycu-0.1.1.tar.gz` & `tmp/xycu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xycu-0.1.1.tar", max compression
+gzip compressed data, was "xycu-0.1.2.tar", max compression
```

## Comparing `xycu-0.1.1.tar` & `xycu-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 xycu-0.1.1/LICENSE
--rw-r--r--   0        0        0      876 2023-07-01 19:55:40.591410 xycu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      721 2023-07-01 19:54:10.975278 xycu-0.1.1/README.md
--rw-r--r--   0        0        0      304 2023-07-01 19:37:51.695752 xycu-0.1.1/src/xycu/__init__.py
--rw-r--r--   0        0        0      491 2023-07-01 19:18:53.252663 xycu-0.1.1/src/xycu/clients.py
--rw-r--r--   0        0        0       19 2023-07-01 19:10:19.351552 xycu-0.1.1/src/xycu/managers/__init__.py
--rw-r--r--   0        0        0      494 2023-07-01 19:28:13.555575 xycu-0.1.1/src/xycu/managers/nsfw.py
--rw-r--r--   0        0        0      485 2023-07-01 19:23:22.239378 xycu-0.1.1/src/xycu/managers/sfw.py
--rw-r--r--   0        0        0       19 2023-07-01 19:04:08.843430 xycu-0.1.1/src/xycu/models/__init__.py
--rw-r--r--   0        0        0       19 2023-07-01 19:09:52.336652 xycu-0.1.1/src/xycu/models/enums/__init__.py
--rw-r--r--   0        0        0       19 2023-07-01 19:10:09.772425 xycu-0.1.1/src/xycu/models/enums/categories/__init__.py
--rw-r--r--   0        0        0      211 2023-07-01 19:10:02.374449 xycu-0.1.1/src/xycu/models/enums/categories/nsfw.py
--rw-r--r--   0        0        0      755 2023-07-01 19:14:46.560219 xycu-0.1.1/src/xycu/models/enums/categories/sfw.py
--rw-r--r--   0        0        0      103 2023-07-01 19:13:02.936202 xycu-0.1.1/src/xycu/models/images.py
--rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 xycu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 xycu-0.1.2/LICENSE
+-rw-r--r--   0        0        0      885 2023-07-06 06:46:46.018736 xycu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      677 2023-07-06 06:38:55.421979 xycu-0.1.2/README.md
+-rw-r--r--   0        0        0      335 2023-07-06 06:43:30.608088 xycu-0.1.2/src/xycu/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-06 06:43:43.225123 xycu-0.1.2/src/xycu/clients.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:42:51.138083 xycu-0.1.2/src/xycu/managers/__init__.py
+-rw-r--r--   0        0        0      433 2023-07-06 06:42:20.980352 xycu-0.1.2/src/xycu/managers/nsfw.py
+-rw-r--r--   0        0        0      426 2023-07-06 06:42:23.243536 xycu-0.1.2/src/xycu/managers/sfw.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:43:22.637155 xycu-0.1.2/src/xycu/models/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:43:19.639228 xycu-0.1.2/src/xycu/models/enums/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:42:47.792143 xycu-0.1.2/src/xycu/models/enums/categories/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-06 06:42:35.909192 xycu-0.1.2/src/xycu/models/enums/categories/nsfw.py
+-rw-r--r--   0        0        0      714 2023-07-06 06:42:42.136063 xycu-0.1.2/src/xycu/models/enums/categories/sfw.py
+-rw-r--r--   0        0        0       61 2023-07-06 06:43:28.650121 xycu-0.1.2/src/xycu/models/images.py
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 xycu-0.1.2/PKG-INFO
```

### Comparing `xycu-0.1.1/LICENSE` & `xycu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xycu-0.1.1/pyproject.toml` & `xycu-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "xycu"
-version = "0.1.1"
-description = "An unofficial Python waifu.pics API wrapper"
+version = "0.1.2"
+description = "🍂 An unofficial Waifu.pics API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/xycu"
 repository = "https://github.com/elaresai/xycu"
 classifiers = [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xycu-0.1.1/README.md` & `xycu-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # xycu
-An unofficial Python [waifu.pics](https://waifu.pics) API wrapper
+🍂 An unofficial [*Waifu.pics*](https://waifu.pics) API wrapper for Python
 
-![language](https://img.shields.io/badge/language-Python-009933)
-![license](https://img.shields.io/badge/license-MIT-cafffe)
-
-# Installation
-`pip install xycu`
-
-# Examples
-`examples/basic.py`
+# 📦 Packages
+## 🐍 PyPi
+```sh
+pip install xycu
+```
+# 🔎 Examples
+[*examples/basic.py*](https://github.com/elaresai/xycu/blob/main/examples/basic.py)
 ```py
 """basic.py"""
 
 from xycu import Client, SfwCategory
 
 client = Client()
 
-print(client.sfw.get(SfwCategory.HUG).url)
-print(client.sfw.get(SfwCategory.KISS).url)
-print(client.sfw.get(SfwCategory.LICK).url)
-print(client.sfw.get(SfwCategory.BITE).url)
+print(client.sfw.get(SfwCategory.HUG))
+print(client.sfw.get(SfwCategory.KISS))
+print(client.sfw.get(SfwCategory.LICK))
+print(client.sfw.get(SfwCategory.BITE))
 ```
 
-# Links
-[🐍 **PyPi**](https://pypi.org/project/xycu/)\
-[🏠 **Homepage**](https://github.com/elaresai/xycu)\
-[🐱 **Repository**](https://github.com/elaresai/xycu)
+# ✨ Links
+[🐍 *PyPi*](https://pypi.org/project/xycu/)\
+[🏠 *Homepage*](https://github.com/elaresai/xycu)\
+[🐱 *Repository*](https://github.com/elaresai/xycu)
```

### Comparing `xycu-0.1.1/src/xycu/models/enums/categories/sfw.py` & `xycu-0.1.2/src/xycu/models/enums/categories/sfw.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-"""sfw.py"""
-
 import enum
 import typing
 
 
 @typing.final
 class SfwCategory(str, enum.Enum):
-    """SfwCategory"""
-
     WAIFU = "waifu"
     NEKO = "neko"
     SHINOBU = "shinobu"
     MEGUMIN = "megumin"
     BULLY = "bully"
     CUDDLE = "cuddle"
     CRY = "cry"
```

