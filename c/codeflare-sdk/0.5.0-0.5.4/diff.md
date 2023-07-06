# Comparing `tmp/codeflare_sdk-0.5.0.tar.gz` & `tmp/codeflare_sdk-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflare_sdk-0.5.0.tar", max compression
+gzip compressed data, was "codeflare_sdk-0.5.4.tar", max compression
```

## Comparing `codeflare_sdk-0.5.0.tar` & `codeflare_sdk-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-06 19:46:30.609866 codeflare_sdk-0.5.0/LICENSE
--rw-r--r--   0        0        0     3488 2023-07-06 19:46:30.609866 codeflare_sdk-0.5.0/README.md
--rw-r--r--   0        0        0      859 2023-07-06 19:46:45.658588 codeflare_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/__init__.py
--rw-r--r--   0        0        0     4434 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/auth.py
--rw-r--r--   0        0        0     3931 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/awload.py
--rw-r--r--   0        0        0    18065 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/cluster.py
--rw-r--r--   0        0        0     1802 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/config.py
--rw-r--r--   0        0        0     2141 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/model.py
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/job/__init__.py
--rw-r--r--   0        0        0     6618 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/job/jobs.py
--rw-r--r--   0        0        0    15130 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/templates/base-template.yaml
--rw-r--r--   0        0        0        0 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/__init__.py
--rw-r--r--   0        0        0     5697 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_cert.py
--rwxr-xr-x   0        0        0    15433 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_yaml.py
--rw-r--r--   0        0        0     6778 2023-07-06 19:46:30.625867 codeflare_sdk-0.5.0/src/codeflare_sdk/utils/pretty_print.py
--rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 codeflare_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 19:42:09.512284 codeflare_sdk-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3488 2023-07-06 19:42:09.512284 codeflare_sdk-0.5.4/README.md
+-rw-r--r--   0        0        0      860 2023-07-06 19:42:24.621338 codeflare_sdk-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/__init__.py
+-rw-r--r--   0        0        0     4434 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/auth.py
+-rw-r--r--   0        0        0     3931 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/awload.py
+-rw-r--r--   0        0        0    18065 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/cluster.py
+-rw-r--r--   0        0        0     1802 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/config.py
+-rw-r--r--   0        0        0     2141 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/model.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/job/__init__.py
+-rw-r--r--   0        0        0     6618 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/job/jobs.py
+-rw-r--r--   0        0        0    15130 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/templates/base-template.yaml
+-rw-r--r--   0        0        0        0 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     5697 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/utils/generate_cert.py
+-rwxr-xr-x   0        0        0    15433 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/utils/generate_yaml.py
+-rw-r--r--   0        0        0     6778 2023-07-06 19:42:09.524285 codeflare_sdk-0.5.4/src/codeflare_sdk/utils/pretty_print.py
+-rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 codeflare_sdk-0.5.4/PKG-INFO
```

### Comparing `codeflare_sdk-0.5.0/LICENSE` & `codeflare_sdk-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/README.md` & `codeflare_sdk-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/pyproject.toml` & `codeflare_sdk-0.5.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeflare-sdk"
-version = "0.5.0"
+version = "v0.5.4"
 description = "Python SDK for codeflare client"
 
 license = "Apache-2.0"
 
 authors = [
     "Michael Clifford <mcliffor@redhat.com>",
     "Mustafa Eyceoz <meyceoz@redhat.com>",
```

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/auth.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/auth.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/awload.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/awload.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/cluster.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/config.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/config.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/cluster/model.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/cluster/model.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/job/jobs.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/job/jobs.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/templates/base-template.yaml` & `codeflare_sdk-0.5.4/src/codeflare_sdk/templates/base-template.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_cert.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/utils/generate_cert.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/utils/generate_yaml.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/utils/generate_yaml.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/src/codeflare_sdk/utils/pretty_print.py` & `codeflare_sdk-0.5.4/src/codeflare_sdk/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.5.0/PKG-INFO` & `codeflare_sdk-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflare-sdk
-Version: 0.5.0
+Version: 0.5.4
 Summary: Python SDK for codeflare client
 Home-page: https://github.com/project-codeflare/codeflare-sdk
 License: Apache-2.0
 Keywords: codeflare,python,sdk,client,batch,scale
 Author: Michael Clifford
 Author-email: mcliffor@redhat.com
 Requires-Python: >=3.7,<4.0
```

