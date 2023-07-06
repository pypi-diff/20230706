# Comparing `tmp/talkytrend-1.5.8.tar.gz` & `tmp/talkytrend-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.5.8.tar", max compression
+gzip compressed data, was "talkytrend-1.5.9.tar", max compression
```

## Comparing `talkytrend-1.5.8.tar` & `talkytrend-1.5.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-03 20:45:45.007926 talkytrend-1.5.8/LICENSE
--rw-r--r--   0        0        0     2247 2023-07-03 20:45:45.007926 talkytrend-1.5.8/README.md
--rw-r--r--   0        0        0     2178 2023-07-03 20:45:45.727937 talkytrend-1.5.8/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-03 20:45:45.727937 talkytrend-1.5.8/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-07-03 20:45:45.007926 talkytrend-1.5.8/talkytrend/config.py
--rw-r--r--   0        0        0     2087 2023-07-03 20:45:45.007926 talkytrend-1.5.8/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6551 2023-07-03 20:45:45.007926 talkytrend-1.5.8/talkytrend/main.py
--rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 talkytrend-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-06 13:13:33.559704 talkytrend-1.5.9/LICENSE
+-rw-r--r--   0        0        0     3444 2023-07-06 13:13:33.559704 talkytrend-1.5.9/README.md
+-rw-r--r--   0        0        0     2178 2023-07-06 13:13:34.511702 talkytrend-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-06 13:13:34.511702 talkytrend-1.5.9/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-06 13:13:33.559704 talkytrend-1.5.9/talkytrend/config.py
+-rw-r--r--   0        0        0     2087 2023-07-06 13:13:33.559704 talkytrend-1.5.9/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6551 2023-07-06 13:13:33.559704 talkytrend-1.5.9/talkytrend/main.py
+-rw-r--r--   0        0        0     4387 1970-01-01 00:00:00.000000 talkytrend-1.5.9/PKG-INFO
```

### Comparing `talkytrend-1.5.8/LICENSE` & `talkytrend-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.8/pyproject.toml` & `talkytrend-1.5.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.5.8"
+version = "1.5.9"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.5.8/talkytrend/config.py` & `talkytrend-1.5.9/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.8/talkytrend/default_settings.toml` & `talkytrend-1.5.9/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.8/talkytrend/main.py` & `talkytrend-1.5.9/talkytrend/main.py`

 * *Files identical despite different names*

