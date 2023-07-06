# Comparing `tmp/raclients-3.1.6.tar.gz` & `tmp/raclients-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raclients-3.1.6.tar", max compression
+gzip compressed data, was "raclients-3.1.7.tar", max compression
```

## Comparing `raclients-3.1.6.tar` & `raclients-3.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0        0        0        0 2023-07-06 10:05:47.227628 raclients-3.1.6/LICENSES/
--rw-r--r--   0        0        0     1039 2023-07-06 10:05:47.228628 raclients-3.1.6/README.md
--rw-r--r--   0        0        0     1063 2023-07-06 10:05:49.646799 raclients-3.1.6/pyproject.toml
--rw-r--r--   0        0        0      300 2023-07-06 10:05:47.230628 raclients-3.1.6/raclients/__init__.py
--rw-r--r--   0        0        0     6858 2023-07-06 10:05:47.230628 raclients-3.1.6/raclients/auth.py
--rw-r--r--   0        0        0       99 2023-07-06 10:05:47.231628 raclients-3.1.6/raclients/graph/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-06 10:05:47.231628 raclients-3.1.6/raclients/graph/client.py
--rw-r--r--   0        0        0     9291 2023-07-06 10:05:47.231628 raclients-3.1.6/raclients/graph/transport.py
--rw-r--r--   0        0        0     3105 2023-07-06 10:05:47.231628 raclients-3.1.6/raclients/graph/util.py
--rw-r--r--   0        0        0       99 2023-07-06 10:05:47.231628 raclients-3.1.6/raclients/modelclient/__init__.py
--rw-r--r--   0        0        0     4356 2023-07-06 10:05:47.232628 raclients-3.1.6/raclients/modelclient/base.py
--rw-r--r--   0        0        0     1940 2023-07-06 10:05:47.232628 raclients-3.1.6/raclients/modelclient/lora.py
--rw-r--r--   0        0        0     5320 2023-07-06 10:05:47.232628 raclients-3.1.6/raclients/modelclient/mo.py
--rw-r--r--   0        0        0        0 2023-07-06 10:05:47.467645 raclients-3.1.6/raclients/py.typed
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 raclients-3.1.6/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-06 10:07:58.494928 raclients-3.1.7/LICENSES/
+-rw-r--r--   0        0        0     1039 2023-07-06 10:07:58.495928 raclients-3.1.7/README.md
+-rw-r--r--   0        0        0     1063 2023-07-06 10:08:00.414064 raclients-3.1.7/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-07-06 10:07:58.499929 raclients-3.1.7/raclients/__init__.py
+-rw-r--r--   0        0        0     6858 2023-07-06 10:07:58.499929 raclients-3.1.7/raclients/auth.py
+-rw-r--r--   0        0        0       99 2023-07-06 10:07:58.499929 raclients-3.1.7/raclients/graph/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-06 10:07:58.500928 raclients-3.1.7/raclients/graph/client.py
+-rw-r--r--   0        0        0     9291 2023-07-06 10:07:58.500928 raclients-3.1.7/raclients/graph/transport.py
+-rw-r--r--   0        0        0     3105 2023-07-06 10:07:58.500928 raclients-3.1.7/raclients/graph/util.py
+-rw-r--r--   0        0        0       99 2023-07-06 10:07:58.500928 raclients-3.1.7/raclients/modelclient/__init__.py
+-rw-r--r--   0        0        0     4356 2023-07-06 10:07:58.501929 raclients-3.1.7/raclients/modelclient/base.py
+-rw-r--r--   0        0        0     1940 2023-07-06 10:07:58.501929 raclients-3.1.7/raclients/modelclient/lora.py
+-rw-r--r--   0        0        0     5320 2023-07-06 10:07:58.501929 raclients-3.1.7/raclients/modelclient/mo.py
+-rw-r--r--   0        0        0        0 2023-07-06 10:07:58.636938 raclients-3.1.7/raclients/py.typed
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 raclients-3.1.7/PKG-INFO
```

### Comparing `raclients-3.1.6/README.md` & `raclients-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/pyproject.toml` & `raclients-3.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raclients"
-version = "3.1.6"
+version = "3.1.7"
 description = "Clients for OS2mo/LoRa"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ra-clients"
 keywords = ["os2mo", "lora"]
```

### Comparing `raclients-3.1.6/raclients/auth.py` & `raclients-3.1.7/raclients/auth.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/raclients/graph/client.py` & `raclients-3.1.7/raclients/graph/client.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/raclients/graph/transport.py` & `raclients-3.1.7/raclients/graph/transport.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/raclients/graph/util.py` & `raclients-3.1.7/raclients/graph/util.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/raclients/modelclient/base.py` & `raclients-3.1.7/raclients/modelclient/base.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/raclients/modelclient/lora.py` & `raclients-3.1.7/raclients/modelclient/lora.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/raclients/modelclient/mo.py` & `raclients-3.1.7/raclients/modelclient/mo.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.6/PKG-INFO` & `raclients-3.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raclients
-Version: 3.1.6
+Version: 3.1.7
 Summary: Clients for OS2mo/LoRa
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,lora
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

