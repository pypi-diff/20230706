# Comparing `tmp/iamlistening-0.2.6.tar.gz` & `tmp/iamlistening-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.2.6.tar", max compression
+gzip compressed data, was "iamlistening-0.2.7.tar", max compression
```

## Comparing `iamlistening-0.2.6.tar` & `iamlistening-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-04 07:03:56.563760 iamlistening-0.2.6/LICENSE
--rw-r--r--   0        0        0     1857 2023-07-04 07:03:56.563760 iamlistening-0.2.6/README.md
--rw-r--r--   0        0        0       99 2023-07-04 07:03:57.299777 iamlistening-0.2.6/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-04 07:03:56.563760 iamlistening-0.2.6/iamlistening/config.py
--rw-r--r--   0        0        0      805 2023-07-04 07:03:56.563760 iamlistening-0.2.6/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3961 2023-07-04 07:03:56.563760 iamlistening-0.2.6/iamlistening/main.py
--rw-r--r--   0        0        0     2163 2023-07-04 07:03:57.299777 iamlistening-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 iamlistening-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-06 13:18:14.182083 iamlistening-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3065 2023-07-06 13:18:14.182083 iamlistening-0.2.7/README.md
+-rw-r--r--   0        0        0       99 2023-07-06 13:18:14.862084 iamlistening-0.2.7/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-06 13:18:14.186083 iamlistening-0.2.7/iamlistening/config.py
+-rw-r--r--   0        0        0      805 2023-07-06 13:18:14.186083 iamlistening-0.2.7/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3961 2023-07-06 13:18:14.186083 iamlistening-0.2.7/iamlistening/main.py
+-rw-r--r--   0        0        0     2163 2023-07-06 13:18:14.858085 iamlistening-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 iamlistening-0.2.7/PKG-INFO
```

### Comparing `iamlistening-0.2.6/LICENSE` & `iamlistening-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.6/iamlistening/config.py` & `iamlistening-0.2.7/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.6/iamlistening/default_settings.toml` & `iamlistening-0.2.7/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.6/iamlistening/main.py` & `iamlistening-0.2.7/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.6/pyproject.toml` & `iamlistening-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.2.6"
+version = "0.2.7"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

