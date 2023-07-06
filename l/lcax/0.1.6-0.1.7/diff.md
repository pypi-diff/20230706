# Comparing `tmp/lcax-0.1.6.tar.gz` & `tmp/lcax-0.1.7.tar.gz`

## Comparing `lcax-0.1.6.tar` & `lcax-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 lcax-0.1.6/Cargo.toml
--rw-r--r--   0     1001      123     1039 2023-07-05 13:17:25.000000 lcax-0.1.6/.github/workflows/cicd.yaml
--rw-r--r--   0     1001      123        0 2023-07-05 13:17:25.000000 lcax-0.1.6/.github/workflows/csharp.yaml
--rw-r--r--   0     1001      123     1303 2023-07-05 13:17:25.000000 lcax-0.1.6/.github/workflows/docs.yaml
--rw-r--r--   0     1001      123        0 2023-07-05 13:17:25.000000 lcax-0.1.6/.github/workflows/javascript.yaml
--rw-r--r--   0     1001      123     1363 2023-07-05 13:17:25.000000 lcax-0.1.6/.github/workflows/python.yaml
--rw-r--r--   0     1001      123      877 2023-07-05 13:17:25.000000 lcax-0.1.6/.github/workflows/release.yaml
--rw-r--r--   0     1001      123      863 2023-07-05 13:17:25.000000 lcax-0.1.6/.github/workflows/rust.yaml
--rw-r--r--   0     1001      123     3182 2023-07-05 13:17:25.000000 lcax-0.1.6/.gitignore
--rw-r--r--   0     1001      123      560 2023-07-05 13:17:25.000000 lcax-0.1.6/COPYRIGHT
--rw-r--r--   0     1001      123    12302 2023-07-05 13:17:36.000000 lcax-0.1.6/Cargo.lock
--rw-r--r--   0     1001      123    10173 2023-07-05 13:17:25.000000 lcax-0.1.6/LICENSE
--rw-r--r--   0     1001      123      516 2023-07-05 13:17:25.000000 lcax-0.1.6/README.md
--rw-r--r--   0     1001      123    59384 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/assets/benchmark.png
--rw-r--r--   0     1001      123    24746 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/assets/epdx.png
--rw-r--r--   0     1001      123   660950 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/assets/lcax project.jpeg
--rw-r--r--   0     1001      123     1342 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/data_structure.md
--rw-r--r--   0     1001      123    16040 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/examples/basic_project.json
--rw-r--r--   0     1001      123      127 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/examples.md
--rw-r--r--   0     1001      123     1859 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/index.md
--rw-r--r--   0     1001      123      127 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/overrides/partials/integrations/analytics/custom.html
--rw-r--r--   0     1001      123      335 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/overrides/stylesheets/extra.css
--rw-r--r--   0     1001      123        0 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/schemas/.gitkeep
--rw-r--r--   0     1001      123      507 2023-07-05 13:17:25.000000 lcax-0.1.6/docs/schemas.md
--rw-r--r--   0     1001      123     1073 2023-07-05 13:17:25.000000 lcax-0.1.6/mkdocs.yml
--rw-r--r--   0     1001      123      100 2023-07-05 13:17:25.000000 lcax-0.1.6/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      123      136 2023-07-05 13:18:08.000000 lcax-0.1.6/packages/python/src/lcax/lcax/__init__.py
--rw-r--r--   0     1001      123      118 2023-07-05 13:18:08.000000 lcax-0.1.6/packages/python/src/lcax/lcax/ffi.py
--rw-r--r--   0     1001      123     5916 2023-07-05 13:18:09.000000 lcax-0.1.6/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      123        0 2023-07-05 13:17:25.000000 lcax-0.1.6/packages/python/tests/.gitkeep
--rw-r--r--   0     1001      123      947 2023-07-05 13:17:25.000000 lcax-0.1.6/pyproject.toml
--rwxr-xr-x   0     1001      123      801 2023-07-05 13:18:39.000000 lcax-0.1.6/run-maturin-action.sh
--rw-r--r--   0     1001      123       16 2023-07-05 13:17:25.000000 lcax-0.1.6/src/lib.rs
--rw-r--r--   0     1001      123     3136 2023-07-05 13:17:25.000000 lcax-0.1.6/src/project.rs
--rw-r--r--   0     1001      123      201 2023-07-05 13:17:25.000000 lcax-0.1.6/src/schemars.rs
--rw-r--r--   0     1001      123        0 2023-07-05 13:17:25.000000 lcax-0.1.6/tests/.gitkeep
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 lcax-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 lcax-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      123     1039 2023-07-06 11:07:03.000000 lcax-0.1.7/.github/workflows/cicd.yaml
+-rw-r--r--   0     1001      123        0 2023-07-06 11:07:03.000000 lcax-0.1.7/.github/workflows/csharp.yaml
+-rw-r--r--   0     1001      123     1303 2023-07-06 11:07:03.000000 lcax-0.1.7/.github/workflows/docs.yaml
+-rw-r--r--   0     1001      123        0 2023-07-06 11:07:03.000000 lcax-0.1.7/.github/workflows/javascript.yaml
+-rw-r--r--   0     1001      123     1363 2023-07-06 11:07:03.000000 lcax-0.1.7/.github/workflows/python.yaml
+-rw-r--r--   0     1001      123      877 2023-07-06 11:07:03.000000 lcax-0.1.7/.github/workflows/release.yaml
+-rw-r--r--   0     1001      123      863 2023-07-06 11:07:03.000000 lcax-0.1.7/.github/workflows/rust.yaml
+-rw-r--r--   0     1001      123     3182 2023-07-06 11:07:03.000000 lcax-0.1.7/.gitignore
+-rw-r--r--   0     1001      123      560 2023-07-06 11:07:03.000000 lcax-0.1.7/COPYRIGHT
+-rw-r--r--   0     1001      123    12302 2023-07-06 11:07:17.000000 lcax-0.1.7/Cargo.lock
+-rw-r--r--   0     1001      123    10173 2023-07-06 11:07:03.000000 lcax-0.1.7/LICENSE
+-rw-r--r--   0     1001      123      516 2023-07-06 11:07:03.000000 lcax-0.1.7/README.md
+-rw-r--r--   0     1001      123    59384 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/assets/benchmark.png
+-rw-r--r--   0     1001      123    24746 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/assets/epdx.png
+-rw-r--r--   0     1001      123   660950 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/assets/lcax project.jpeg
+-rw-r--r--   0     1001      123     1342 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/data_structure.md
+-rw-r--r--   0     1001      123    16059 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/examples/basic_project.json
+-rw-r--r--   0     1001      123      127 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/examples.md
+-rw-r--r--   0     1001      123     1859 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/index.md
+-rw-r--r--   0     1001      123      127 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/overrides/partials/integrations/analytics/custom.html
+-rw-r--r--   0     1001      123      335 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/overrides/stylesheets/extra.css
+-rw-r--r--   0     1001      123        0 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/schemas/.gitkeep
+-rw-r--r--   0     1001      123      507 2023-07-06 11:07:03.000000 lcax-0.1.7/docs/schemas.md
+-rw-r--r--   0     1001      123     1073 2023-07-06 11:07:03.000000 lcax-0.1.7/mkdocs.yml
+-rw-r--r--   0     1001      123      100 2023-07-06 11:07:03.000000 lcax-0.1.7/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      123      136 2023-07-06 11:08:06.000000 lcax-0.1.7/packages/python/src/lcax/lcax/__init__.py
+-rw-r--r--   0     1001      123      118 2023-07-06 11:08:06.000000 lcax-0.1.7/packages/python/src/lcax/lcax/ffi.py
+-rw-r--r--   0     1001      123     6417 2023-07-06 11:08:08.000000 lcax-0.1.7/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      123        0 2023-07-06 11:07:03.000000 lcax-0.1.7/packages/python/tests/.gitkeep
+-rw-r--r--   0     1001      123      947 2023-07-06 11:07:03.000000 lcax-0.1.7/pyproject.toml
+-rwxr-xr-x   0     1001      123      801 2023-07-06 11:08:44.000000 lcax-0.1.7/run-maturin-action.sh
+-rw-r--r--   0     1001      123       16 2023-07-06 11:07:03.000000 lcax-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      123     3473 2023-07-06 11:07:03.000000 lcax-0.1.7/src/project.rs
+-rw-r--r--   0     1001      123      201 2023-07-06 11:07:03.000000 lcax-0.1.7/src/schemars.rs
+-rw-r--r--   0     1001      123        0 2023-07-06 11:07:03.000000 lcax-0.1.7/tests/.gitkeep
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 lcax-0.1.7/PKG-INFO
```

### Comparing `lcax-0.1.6/Cargo.toml` & `lcax-0.1.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "lcax"
 description = "LCAx is an open, machine and human-readable data format for exchanging LCA results."
-version = "0.1.6"
+version = "0.1.7"
 authors = ["Christian Kongsgaard <christian@kongsgaard.eu>"]
 edition = "2018"
 readme = "README.md"
 license-file = "LICENSE"
 homepage = "https://lcax.kongsgaard.eu"
 documentation = "https://lcax.kongsgaard.eu"
 repository = "https://github.com/ocni-dtu/lcax"
```

### Comparing `lcax-0.1.6/.github/workflows/cicd.yaml` & `lcax-0.1.7/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/.github/workflows/docs.yaml` & `lcax-0.1.7/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/.github/workflows/python.yaml` & `lcax-0.1.7/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/.github/workflows/release.yaml` & `lcax-0.1.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/.github/workflows/rust.yaml` & `lcax-0.1.7/.github/workflows/rust.yaml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/.gitignore` & `lcax-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/COPYRIGHT` & `lcax-0.1.7/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/Cargo.lock` & `lcax-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lcax"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "epdx",
  "schemars",
  "serde",
  "serde_json",
 ]
```

### Comparing `lcax-0.1.6/LICENSE` & `lcax-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/README.md` & `lcax-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/docs/assets/benchmark.png` & `lcax-0.1.7/docs/assets/benchmark.png`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/docs/assets/epdx.png` & `lcax-0.1.7/docs/assets/epdx.png`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/docs/assets/lcax project.jpeg` & `lcax-0.1.7/docs/assets/lcax project.jpeg`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/docs/data_structure.md` & `lcax-0.1.7/docs/data_structure.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/docs/examples/basic_project.json` & `lcax-0.1.7/docs/examples/basic_project.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'life_span'": '50'}*

```diff
@@ -523,10 +523,11 @@
     "lcia_method": "EN15804",
     "life_cycle_stages": [
         "A1A3",
         "C3",
         "C4",
         "D"
     ],
+    "life_span": 50,
     "location": "DK",
     "name": "Basic Project"
 }
```

### Comparing `lcax-0.1.6/docs/index.md` & `lcax-0.1.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/mkdocs.yml` & `lcax-0.1.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/packages/python/src/lcax/pydantic.py` & `lcax-0.1.7/packages/python/src/lcax/pydantic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  lcax.schema.json
-#   timestamp: 2023-07-05T13:18:09+00:00
+#   timestamp: 2023-07-06T11:08:08+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
@@ -37,14 +37,42 @@
     c1: Optional[float] = None
     c2: Optional[float] = None
     c3: Optional[float] = None
     c4: Optional[float] = None
     d: Optional[float] = None
 
 
+class ImpactCategoryKey(Enum):
+    GWP = 'GWP'
+    ODP = 'ODP'
+    AP = 'AP'
+    EP = 'EP'
+    POCP = 'POCP'
+    ADPE = 'ADPE'
+    ADPF = 'ADPF'
+    PENRE = 'PENRE'
+    PERE = 'PERE'
+    PERM = 'PERM'
+    PERT = 'PERT'
+    PENRT = 'PENRT'
+    PENRM = 'PENRM'
+    SM = 'SM'
+    RSF = 'RSF'
+    NRSF = 'NRSF'
+    FW = 'FW'
+    HWD = 'HWD'
+    NHWD = 'NHWD'
+    RWD = 'RWD'
+    CRU = 'CRU'
+    MRF = 'MRF'
+    MER = 'MER'
+    EEE = 'EEE'
+    EET = 'EET'
+
+
 class InternalEPD(BaseModel):
     path: str
 
 
 class LifeCycleStage(Enum):
     A1A3 = 'A1A3'
     A4 = 'A4'
@@ -232,14 +260,15 @@
 class LCAxProject(BaseModel):
     classification_system: Optional[str] = None
     comment: Optional[str] = None
     description: str
     emission_parts: Dict[str, Assembly]
     format_version: str
     id: str
-    impact_categories: List[ImpactCategory]
+    impact_categories: List[ImpactCategoryKey]
     lcia_method: Optional[str] = None
     life_cycle_stages: List[LifeCycleStage]
+    life_span: Optional[conint(ge=0)] = None
     location: str
     meta_data: Optional[Dict[str, Any]] = None
     name: str
     results: Optional[Results] = None
```

### Comparing `lcax-0.1.6/pyproject.toml` & `lcax-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/run-maturin-action.sh` & `lcax-0.1.7/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `lcax-0.1.6/src/project.rs` & `lcax-0.1.7/src/project.rs`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,21 @@
     id: String,
     name: String,
     description: String,
     comment: Option<String>,
     location: String,
     format_version: String,
     lcia_method: Option<String>,
-    meta_data: Option<HashMap<String, String>>,
     classification_system: Option<String>,
+    life_span: Option<u8>,
     life_cycle_stages: Vec<LifeCycleStage>,
-    impact_categories: Vec<ImpactCategory>,
+    impact_categories: Vec<ImpactCategoryKey>,
     emission_parts: HashMap<String, Assembly>,
     results: Option<Results>,
+    meta_data: Option<HashMap<String, String>>,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema)]
 enum LifeCycleStage {
     A1A3,
     A4,
     A5,
@@ -36,14 +37,42 @@
     C1,
     C2,
     C3,
     C4,
     D,
 }
 
+#[derive(Deserialize, Serialize, JsonSchema)]
+enum ImpactCategoryKey {
+    GWP,
+    ODP,
+    AP,
+    EP,
+    POCP,
+    ADPE,
+    ADPF,
+    PENRE,
+    PERE,
+    PERM,
+    PERT,
+    PENRT,
+    PENRM,
+    SM,
+    RSF,
+    NRSF,
+    FW,
+    HWD,
+    NHWD,
+    RWD,
+    CRU,
+    MRF,
+    MER,
+    EEE,
+    EET
+}
 
 #[derive(Deserialize, Serialize, JsonSchema)]
 pub struct Assembly {
     id: String,
     name: String,
     description: String,
     comment: Option<String>,
```

### Comparing `lcax-0.1.6/PKG-INFO` & `lcax-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: lcax
-Version: 0.1.6
+Version: 0.1.7
 Requires-Dist: cffi
+Requires-Dist: mkdocs-material >=8.1.4,<9.0.0; extra == 'doc'
+Requires-Dist: mdx-include >=1.4.1,<2.0.0; extra == 'doc'
 Requires-Dist: pydantic >=1.8.2,<2.0.0; extra == 'code-gen'
 Requires-Dist: datamodel-code-generator; extra == 'code-gen'
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-datafixtures; extra == 'tests'
-Requires-Dist: mkdocs-material >=8.1.4,<9.0.0; extra == 'doc'
-Requires-Dist: mdx-include >=1.4.1,<2.0.0; extra == 'doc'
+Provides-Extra: doc
 Provides-Extra: code-gen
 Provides-Extra: tests
-Provides-Extra: doc
 License-File: LICENSE
 License-File: LICENSE
 Summary: LCAx is an open, machine and human-readable data format for exchanging LCA results.
 Home-Page: https://lcax.kongsgaard.eu
 Author: Christian Kongsgaard <christian@kongsgaard.eu>
 Author-email: Christian Kongsgaard <christian@kongsgaard.eu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://lcax.kongsgaard.eu
-Project-URL: homepage, https://lcax.kongsgaard.eu
 Project-URL: repository, https://github.com/ocni-dtu/lcax
+Project-URL: homepage, https://lcax.kongsgaard.eu
+Project-URL: documentation, https://lcax.kongsgaard.eu
 
 # LCAx
 
 The goal for LCAx is to make an open, machine and human-readable data format for exchanging LCA results,
 EPD's and assemblies. 
 
 We propose a simple three level data format with information on project, assembly and EPD level,
```

