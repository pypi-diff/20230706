# Comparing `tmp/findmyorder-1.5.3.tar.gz` & `tmp/findmyorder-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.5.3.tar", max compression
+gzip compressed data, was "findmyorder-1.5.4.tar", max compression
```

## Comparing `findmyorder-1.5.3.tar` & `findmyorder-1.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-03 19:54:31.818702 findmyorder-1.5.3/LICENSE
--rw-r--r--   0        0        0     2262 2023-07-03 19:54:31.818702 findmyorder-1.5.3/README.md
--rw-r--r--   0        0        0      113 2023-07-03 19:54:32.682752 findmyorder-1.5.3/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-03 19:54:31.818702 findmyorder-1.5.3/findmyorder/config.py
--rw-r--r--   0        0        0     2848 2023-07-03 19:54:31.818702 findmyorder-1.5.3/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5780 2023-07-03 19:54:31.818702 findmyorder-1.5.3/findmyorder/main.py
--rw-r--r--   0        0        0     2132 2023-07-03 19:54:32.682752 findmyorder-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 findmyorder-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-06 13:19:58.174734 findmyorder-1.5.4/LICENSE
+-rw-r--r--   0        0        0     3046 2023-07-06 13:19:58.174734 findmyorder-1.5.4/README.md
+-rw-r--r--   0        0        0      113 2023-07-06 13:19:58.998758 findmyorder-1.5.4/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-06 13:19:58.174734 findmyorder-1.5.4/findmyorder/config.py
+-rw-r--r--   0        0        0     2848 2023-07-06 13:19:58.174734 findmyorder-1.5.4/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5780 2023-07-06 13:19:58.174734 findmyorder-1.5.4/findmyorder/main.py
+-rw-r--r--   0        0        0     2132 2023-07-06 13:19:58.998758 findmyorder-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 findmyorder-1.5.4/PKG-INFO
```

### Comparing `findmyorder-1.5.3/LICENSE` & `findmyorder-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.3/findmyorder/config.py` & `findmyorder-1.5.4/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.3/findmyorder/default_settings.toml` & `findmyorder-1.5.4/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.3/findmyorder/main.py` & `findmyorder-1.5.4/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.3/pyproject.toml` & `findmyorder-1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.5.3"
+version = "1.5.4"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

