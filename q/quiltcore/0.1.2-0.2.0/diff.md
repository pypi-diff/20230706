# Comparing `tmp/quiltcore-0.1.2.tar.gz` & `tmp/quiltcore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltcore-0.1.2.tar", max compression
+gzip compressed data, was "quiltcore-0.2.0.tar", max compression
```

## Comparing `quiltcore-0.1.2.tar` & `quiltcore-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.1.2/LICENSE
--rw-r--r--   0        0        0     1551 2023-06-29 23:49:03.946275 quiltcore-0.1.2/README.md
--rw-r--r--   0        0        0      831 2023-06-29 23:54:09.916620 quiltcore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      930 2023-06-30 00:35:03.061872 quiltcore-0.1.2/quiltcore/__init__.py
--rw-r--r--   0        0        0     1771 2023-06-30 07:59:56.000000 quiltcore-0.1.2/quiltcore/blob.py
--rw-r--r--   0        0        0      698 2023-06-30 00:30:52.256979 quiltcore-0.1.2/quiltcore/config.py
--rw-r--r--   0        0        0     2175 2023-06-30 07:59:56.000000 quiltcore-0.1.2/quiltcore/manifest.py
--rw-r--r--   0        0        0      599 2023-06-30 00:34:19.012973 quiltcore-0.1.2/quiltcore/namespace.py
--rw-r--r--   0        0        0      615 2023-06-30 00:34:48.607108 quiltcore-0.1.2/quiltcore/registry.py
--rw-r--r--   0        0        0     2457 2023-06-30 07:59:56.000000 quiltcore-0.1.2/quiltcore/resource.py
--rw-r--r--   0        0        0      610 2023-06-30 00:42:57.086957 quiltcore-0.1.2/quiltcore/yaml/quiltcore.yaml
--rw-r--r--   0        0        0      160 2023-06-27 22:10:43.161786 quiltcore-0.1.2/quiltcore/yaml/schema.yaml
--rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 quiltcore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1579 2023-07-06 04:28:48.600645 quiltcore-0.2.0/README.md
+-rw-r--r--   0        0        0      852 2023-07-06 05:21:55.381836 quiltcore-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1061 2023-07-05 18:42:27.110229 quiltcore-0.2.0/quiltcore/__init__.py
+-rw-r--r--   0        0        0     2937 2023-07-05 20:12:19.916372 quiltcore-0.2.0/quiltcore/changes.py
+-rw-r--r--   0        0        0      972 2023-07-05 20:12:59.420575 quiltcore-0.2.0/quiltcore/delta.py
+-rw-r--r--   0        0        0     3195 2023-07-06 01:48:32.771447 quiltcore-0.2.0/quiltcore/entry.py
+-rw-r--r--   0        0        0     2149 2023-07-06 03:48:54.467767 quiltcore-0.2.0/quiltcore/manifest.py
+-rw-r--r--   0        0        0      631 2023-07-06 04:20:34.805585 quiltcore-0.2.0/quiltcore/namespace.py
+-rw-r--r--   0        0        0     1621 2023-07-06 04:19:58.111513 quiltcore-0.2.0/quiltcore/registry.py
+-rw-r--r--   0        0        0     3402 2023-07-06 04:20:56.858303 quiltcore-0.2.0/quiltcore/resource.py
+-rw-r--r--   0        0        0     1937 2023-07-05 23:05:35.899259 quiltcore-0.2.0/quiltcore/resource_key.py
+-rw-r--r--   0        0        0     1520 2023-07-05 23:13:46.646052 quiltcore-0.2.0/quiltcore/resource_path.py
+-rw-r--r--   0        0        0     4708 2023-07-06 05:18:41.827854 quiltcore-0.2.0/quiltcore/volume.py
+-rw-r--r--   0        0        0      693 2023-07-03 20:20:23.166091 quiltcore-0.2.0/quiltcore/yaml/config.py
+-rw-r--r--   0        0        0      743 2023-07-06 01:15:21.327702 quiltcore-0.2.0/quiltcore/yaml/quiltcore.yaml
+-rw-r--r--   0        0        0      160 2023-06-30 01:13:50.059736 quiltcore-0.2.0/quiltcore/yaml/schema.yaml
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 quiltcore-0.2.0/PKG-INFO
```

### Comparing `quiltcore-0.1.2/LICENSE` & `quiltcore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quiltcore-0.1.2/README.md` & `quiltcore-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -36,22 +36,23 @@
 
 <!--pytest-codeblocks:cont-->
 ```python
 path = UPath(TEST_BKT)
 registry = Registry(path)
 named_package = registry.get(TEST_PKG)
 manifest = named_package.get(TEST_TAG)
-blob = manifest.get(TEST_KEY)
+entry = manifest.get(TEST_KEY)
 ```
 
 ### Get Object
 
 <!--pytest-codeblocks:cont-->
 ```python
 with TemporaryDirectory() as tmpdirname:
-  dest = UPath(tmpdirname) / TEST_KEY
-  local = blob.put(dest)
-  print(local)
-  assert local.exists()
-  local_bytes = local.read_bytes()
-  assert blob.verify(local_bytes)
+  dest = UPath(tmpdirname)
+  outfile = dest / TEST_KEY
+  entry.get(dest)
+  print(outfile.resolve())
+  assert outfile.exists()
+  local_bytes = outfile.read_bytes()
+  assert entry.verify(local_bytes)
 ```
```

### Comparing `quiltcore-0.1.2/pyproject.toml` & `quiltcore-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltcore"
-version = "0.1.2"
+version = "0.2.0"
 description = "low-level plubming to read/write Quilt packages"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typing-extensions = "^4.6.3"
@@ -14,14 +14,15 @@
 pyarrow = "^12.0.0"
 pandas = "^2.0.2"
 pytest-codeblocks = "^0.16.1"
 universal-pathlib = "^0.0.23"
 s3fs = "^2023.6.0"
 pandas-stubs = "^2.0.2.230605"
 multiformats = "^0.2.1"
+jsonlines = "^3.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 pytest-watcher = "^0.3.4"
```

### Comparing `quiltcore-0.1.2/quiltcore/__init__.py` & `quiltcore-0.2.0/quiltcore/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 
 The core Resource classes are, in order of increasing specialization:
 
 - Resource
 - Registry
 - Namespace
 - Manifest
-- Blob
+- Entry
 
 These make use of the 'Config' class which loads and
 manages the 'quiltcore.yaml' configuration file.
 
 """
 
-from .blob import Blob  # noqa: F401
-from .config import Config  # noqa: F401
+from .changes import Changes  # noqa: F401
+from .delta import Delta  # noqa: F401
+from .entry import Entry  # noqa: F401
 from .manifest import Manifest  # noqa: F401
 from .namespace import Namespace  # noqa: F401
 from .registry import Registry  # noqa: F401
 from .resource import Resource  # noqa: F401
+from .volume import Volume  # noqa: F401
+from .yaml.config import Config  # noqa: F401
```

### Comparing `quiltcore-0.1.2/quiltcore/config.py` & `quiltcore-0.2.0/quiltcore/yaml/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from un_yaml import UnYaml  # type: ignore
 
 
 class Config(UnYaml):
-    CONFIG_FILE = "yaml/quiltcore.yaml"
+    CONFIG_FILE = "quiltcore.yaml"
 
     @classmethod
     def DefaultConfig(cls) -> dict:
         return UnYaml.LoadYaml(cls.CONFIG_FILE, __package__)
 
     def __init__(self, yaml_data: dict = {}) -> None:
         data = yaml_data if len(yaml_data) > 0 else Config.DefaultConfig()
```

### Comparing `quiltcore-0.1.2/quiltcore/manifest.py` & `quiltcore-0.2.0/quiltcore/resource_path.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,55 @@
+from __future__ import annotations
+
 from pathlib import Path
+from typing import Generator
 
-import pyarrow as pa  # type: ignore
-import pyarrow.compute as pc  # type: ignore
-import pyarrow.json as pj  # type: ignore
-from typing_extensions import Self
-from upath import UPath
 
 from .resource import Resource
 
 
-class Manifest(Resource):
+class ResourcePath(Resource):
     """
-    In-memory representation of a serialized package manifest.
-    list/get returns Blob with Path to the Place data actually lives
+    Path-based list and get.
     """
 
-    # TODO: cache Blobs to avoid repeated lookups
-
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
-        with path.open(mode="rb") as fi:
-            self.table = pj.read_json(fi)
-        self.body = self.setup_table()
-        self.name_col = self.cf.get_str("schema/name", "logical_key")
-        self.place_col = self.cf.get_str("schema/place", "physical_keys")
-
-    def setup_table(self) -> pa.Table:
-        first = self.table.take([0]).to_pydict()
-        headers = self.cf.get_dict("schema/headers")
-        keys = list(headers.keys())
-        for key in keys:
-            setattr(self, key, first[key][0])
-        return self.table.drop_columns(keys).slice(1)
+        self.glob = self.param(self.KEY_GLOB, "*")
 
     #
-    # Private Methods for child resources
+    # Private Methods for Path-based child resources
     #
 
-    def child_row(self, key: str) -> dict:
-        """Return the dict for a child resource."""
-        # TODO: cache to avoid continually re-calcluating
-        rows = self.body.filter(pc.field(self.name_col) == key)
-        if rows.num_rows == 0:
-            raise KeyError(f"Key [{key}] not found in {self.name_col} of {self.path}")
-        return rows.to_pydict()
+    def child_args(self, key: str) -> dict:
+        """Return the kwargs for a child resource."""
+        return {}
+
+    def child(self, path: Path, key: str = ""):
+        """Return a child resource."""
+        args = self.child_args(key)
+        args[self.KEY_KEY] = key
+        merged = {**self.args, **args}
+        return self.klass(path, **merged)
 
     def child_path(self, key: str) -> Path:
-        """Return the Path for a child resource."""
-        row = self.child_row(key)
-        place = row[self.place_col][0][0]
-        return UPath(place)
+        """Return the path for a child resource."""
+        return self.path / key
 
-    def child_args(self, key: str) -> dict:
-        """Return the parameters for a child resource."""
-        row = self.child_row(key)
-        return {"row": row, "parent": self}
+    def child_list(self) -> Generator[Path, None, None]:
+        """List/generator of valid child paths; defaults to self.glob"""
+        return self.path.glob(self.glob)
 
     #
     # Public HTTP-like Methods
     #
 
-    def list(self) -> list[Self]:
+    def list(self, **kwargs) -> list["Resource"]:
         """List all child resources."""
-        names = self.body.column(self.name_col).to_pylist()
-        return [self.child(self.child_path(x), x) for x in names]
+        return [self.child(x) for x in self.child_list()]
+
+    def get(self, key: str, **kwargs) -> "Resource":
+        """Get a child resource by name."""
+        path = self.child_path(key)
+        if not path.exists():
+            raise KeyError(f"Key {key} not found in {self.path}")
+        return self.child(path, key)
```

### Comparing `quiltcore-0.1.2/quiltcore/namespace.py` & `quiltcore-0.2.0/quiltcore/namespace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pathlib import Path
 
-from .resource import Resource
+from .resource_path import ResourcePath
 
 
-class Namespace(Resource):
+class Namespace(ResourcePath):
     """
     Namespacespace of Manifests by Hash
     list/get returns a specific Manifest
     """
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
-        self.versions = kwargs["versions"]
+        self.manifests = kwargs["manifests"]
 
-    def hash(self, tag: str = "latest") -> str:
+    def hash(self, tag: str = ResourcePath.TAG_DEFAULT) -> str:
         hash_file = self.path / tag
         return hash_file.read_text()
 
     def child_path(self, key: str) -> Path:
         """Return the path for a child resource."""
         hash = self.hash(key)
-        return self.versions / hash
+        return self.manifests / hash
```

### Comparing `quiltcore-0.1.2/PKG-INFO` & `quiltcore-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: quiltcore
-Version: 0.1.2
+Version: 0.2.0
 Summary: low-level plubming to read/write Quilt packages
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pytest-codeblocks (>=0.16.1,<0.17.0)
 Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
@@ -58,23 +59,24 @@
 
 <!--pytest-codeblocks:cont-->
 ```python
 path = UPath(TEST_BKT)
 registry = Registry(path)
 named_package = registry.get(TEST_PKG)
 manifest = named_package.get(TEST_TAG)
-blob = manifest.get(TEST_KEY)
+entry = manifest.get(TEST_KEY)
 ```
 
 ### Get Object
 
 <!--pytest-codeblocks:cont-->
 ```python
 with TemporaryDirectory() as tmpdirname:
-  dest = UPath(tmpdirname) / TEST_KEY
-  local = blob.put(dest)
-  print(local)
-  assert local.exists()
-  local_bytes = local.read_bytes()
-  assert blob.verify(local_bytes)
+  dest = UPath(tmpdirname)
+  outfile = dest / TEST_KEY
+  entry.get(dest)
+  print(outfile.resolve())
+  assert outfile.exists()
+  local_bytes = outfile.read_bytes()
+  assert entry.verify(local_bytes)
 ```
```

