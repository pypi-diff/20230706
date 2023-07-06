# Comparing `tmp/flowdump-0.1.0.tar.gz` & `tmp/flowdump-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowdump-0.1.0.tar", max compression
+gzip compressed data, was "flowdump-0.1.1.tar", max compression
```

## Comparing `flowdump-0.1.0.tar` & `flowdump-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    26190 2023-06-28 20:21:40.097306 flowdump-0.1.0/LICENSE
--rw-r--r--   0        0        0      613 2023-06-29 18:37:30.770298 flowdump-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3153 2023-06-30 18:36:10.002401 flowdump-0.1.0/README.md
--rw-r--r--   0        0        0      359 2023-06-30 18:37:52.616783 flowdump-0.1.0/src/flowdump/__init__.py
--rw-r--r--   0        0        0      819 2023-06-30 18:31:43.203049 flowdump-0.1.0/src/flowdump/core.py
--rw-r--r--   0        0        0     4685 2023-06-30 19:40:07.076618 flowdump-0.1.0/src/flowdump/nipype_report_parser.py
--rw-r--r--   0        0        0     1614 2023-06-30 19:40:06.996616 flowdump-0.1.0/src/flowdump/utils.py
--rw-r--r--   0        0        0     8786 2023-06-30 18:31:34.846695 flowdump-0.1.0/src/flowdump/workflow_json.py
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 flowdump-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    26190 2023-06-28 20:21:40.097306 flowdump-0.1.1/LICENSE
+-rw-r--r--   0        0        0      623 2023-07-05 20:28:37.573259 flowdump-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3153 2023-06-30 18:36:10.002401 flowdump-0.1.1/README.md
+-rw-r--r--   0        0        0      359 2023-06-30 18:37:52.616783 flowdump-0.1.1/src/flowdump/__init__.py
+-rw-r--r--   0        0        0      819 2023-06-30 18:31:43.203049 flowdump-0.1.1/src/flowdump/core.py
+-rw-r--r--   0        0        0     4685 2023-06-30 19:40:07.076618 flowdump-0.1.1/src/flowdump/nipype_report_parser.py
+-rw-r--r--   0        0        0     1614 2023-06-30 19:40:06.996616 flowdump-0.1.1/src/flowdump/utils.py
+-rw-r--r--   0        0        0     8786 2023-06-30 18:31:34.846695 flowdump-0.1.1/src/flowdump/workflow_json.py
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 flowdump-0.1.1/PKG-INFO
```

### Comparing `flowdump-0.1.0/LICENSE` & `flowdump-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flowdump-0.1.0/pyproject.toml` & `flowdump-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "flowdump"
-version = "0.1.0"
+version = "0.1.1"
 description = "NiPype-1 workflow serializer."
 authors = ["Florian Rupprecht <floruppr@gmail.com>"]
 license = "LGPL-2.1"
 readme = "README.md"
-packages = [{include = "src/flowdump"}]
+packages = [{include = "flowdump", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 nipype = ">=1.0.0, <2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
```

### Comparing `flowdump-0.1.0/README.md` & `flowdump-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flowdump-0.1.0/src/flowdump/core.py` & `flowdump-0.1.1/src/flowdump/core.py`

 * *Files identical despite different names*

### Comparing `flowdump-0.1.0/src/flowdump/nipype_report_parser.py` & `flowdump-0.1.1/src/flowdump/nipype_report_parser.py`

 * *Files identical despite different names*

### Comparing `flowdump-0.1.0/src/flowdump/utils.py` & `flowdump-0.1.1/src/flowdump/utils.py`

 * *Files identical despite different names*

### Comparing `flowdump-0.1.0/src/flowdump/workflow_json.py` & `flowdump-0.1.1/src/flowdump/workflow_json.py`

 * *Files identical despite different names*

### Comparing `flowdump-0.1.0/PKG-INFO` & `flowdump-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdump
-Version: 0.1.0
+Version: 0.1.1
 Summary: NiPype-1 workflow serializer.
 License: LGPL-2.1
 Author: Florian Rupprecht
 Author-email: floruppr@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

