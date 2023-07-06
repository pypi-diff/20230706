# Comparing `tmp/metalogistic-0.0.8.tar.gz` & `tmp/metalogistic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalogistic-0.0.8.tar", max compression
+gzip compressed data, was "metalogistic-0.0.9.tar", max compression
```

## Comparing `metalogistic-0.0.8.tar` & `metalogistic-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    34523 2022-03-22 08:40:36.420866 metalogistic-0.0.8/LICENSE
--rw-r--r--   0        0        0       30 2022-03-22 08:40:36.421591 metalogistic-0.0.8/metalogistic/__init__.py
--rw-r--r--   0        0        0    34103 2022-03-22 15:52:06.314639 metalogistic-0.0.8/metalogistic/main.py
--rw-r--r--   0        0        0      391 2022-03-22 08:40:36.422275 metalogistic-0.0.8/metalogistic/support.py
--rw-r--r--   0        0        0      589 2022-03-29 18:19:58.257788 metalogistic-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      840 2022-03-29 18:20:05.173347 metalogistic-0.0.8/setup.py
--rw-r--r--   0        0        0      658 2022-03-29 18:20:05.173591 metalogistic-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-03-22 08:40:36.420866 metalogistic-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2917 2022-03-22 08:40:36.421126 metalogistic-0.0.9/README.md
+-rw-r--r--   0        0        0       30 2022-03-22 08:40:36.421591 metalogistic-0.0.9/metalogistic/__init__.py
+-rw-r--r--   0        0        0    34103 2022-03-22 15:52:06.314639 metalogistic-0.0.9/metalogistic/main.py
+-rw-r--r--   0        0        0      391 2022-03-22 08:40:36.422275 metalogistic-0.0.9/metalogistic/support.py
+-rw-r--r--   0        0        0      610 2022-03-29 18:28:01.362077 metalogistic-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3861 2022-03-29 18:28:04.718915 metalogistic-0.0.9/setup.py
+-rw-r--r--   0        0        0     3617 2022-03-29 18:28:04.719301 metalogistic-0.0.9/PKG-INFO
```

### Comparing `metalogistic-0.0.8/LICENSE` & `metalogistic-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metalogistic-0.0.8/metalogistic/main.py` & `metalogistic-0.0.9/metalogistic/main.py`

 * *Files identical despite different names*

### Comparing `metalogistic-0.0.8/pyproject.toml` & `metalogistic-0.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "metalogistic"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Python package for the metalogistic distribution. The metalogistic or metalog distribution is a highly flexible probability distribution that can be used to model data without traditional parameters."
 authors = ["tadamcz <tmkadamcz@gmail.com>"]
 license = "GNU Affero General Public License v3"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.8"
 numpy = "^1.22.3"
 scipy = "^1.8.0"
 matplotlib = "^3.5.1"
```

