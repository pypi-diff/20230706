# Comparing `tmp/neosctl-0.8.8.tar.gz` & `tmp/neosctl-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.8.tar", max compression
+gzip compressed data, was "neosctl-0.8.9.tar", max compression
```

## Comparing `neosctl-0.8.8.tar` & `neosctl-0.8.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-07-05 11:53:12.771864 neosctl-0.8.8/README.md
--rw-r--r--   0        0        0       22 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/constant.py
--rw-r--r--   0        0        0     4528 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14331 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     5491 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     4556 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3564 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1409 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     5684 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3243 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      122 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     7686 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12904 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/util.py
--rw-r--r--   0        0        0     3050 2023-07-05 11:53:12.773864 neosctl-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-07-06 12:44:12.933411 neosctl-0.8.9/README.md
+-rw-r--r--   0        0        0       22 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/constant.py
+-rw-r--r--   0        0        0     4528 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-07-06 12:44:12.933411 neosctl-0.8.9/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5491 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3564 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     5684 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-07-06 12:44:12.934411 neosctl-0.8.9/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3243 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      122 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     7848 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12904 2023-07-06 12:44:12.935411 neosctl-0.8.9/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-07-06 12:44:12.935411 neosctl-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.9/PKG-INFO
```

### Comparing `neosctl-0.8.8/README.md` & `neosctl-0.8.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.8
+# Core CLI v0.8.9
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.8.8/neosctl/auth.py` & `neosctl-0.8.9/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/cli.py` & `neosctl-0.8.9/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/profile.py` & `neosctl-0.8.9/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/schema.py` & `neosctl-0.8.9/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/__init__.py` & `neosctl-0.8.9/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/data_product.py` & `neosctl-0.8.9/neosctl/services/gateway/data_product.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/data_source.py` & `neosctl-0.8.9/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/data_system.py` & `neosctl-0.8.9/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/data_unit.py` & `neosctl-0.8.9/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/entity.py` & `neosctl-0.8.9/neosctl/services/gateway/entity.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/link.py` & `neosctl-0.8.9/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/output.py` & `neosctl-0.8.9/neosctl/services/gateway/output.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/schema.py` & `neosctl-0.8.9/neosctl/services/gateway/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/secret.py` & `neosctl-0.8.9/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/spark.py` & `neosctl-0.8.9/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/gateway/tag.py` & `neosctl-0.8.9/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/iam/iam.py` & `neosctl-0.8.9/neosctl/services/iam/iam.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/iam/schema.py` & `neosctl-0.8.9/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/registry/registry.py` & `neosctl-0.8.9/neosctl/services/registry/registry.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/neosctl/services/storage/storage.py` & `neosctl-0.8.9/neosctl/services/storage/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 
 BUCKET_NAME_ARGUMENT = typer.Argument(
     ...,
     help="Bucket name",
     callback=util.validate_regex(BUCKET_NAME_PATTERN),
 )
 
+# Don't use regex as OBJECT_NAME can be `path/to/my/file.txt` etc. which could easily exceed 255 and break allowed chars
+# minio just checks that object_name is not empty.
 OBJECT_NAME_ARGUMENT = typer.Argument(
     ...,
     help="Object name",
-    callback=util.validate_regex(OBJECT_NAME_PATTERN),
+    callback=util.validate_string_not_empty,
 )
 
 app.add_typer(bucket_app, name="bucket", help="Manage object buckets.")
 app.add_typer(object_app, name="object", help="Manage objects.")
 object_app.add_typer(tagging_app, name="tags", help="Manage object tags.")
```

### Comparing `neosctl-0.8.8/neosctl/util.py` & `neosctl-0.8.9/neosctl/util.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.8/pyproject.toml` & `neosctl-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.8"
+version = "0.8.9"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.8.8/PKG-INFO` & `neosctl-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.8
+Version: 0.8.9
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.8
+# Core CLI v0.8.9
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

