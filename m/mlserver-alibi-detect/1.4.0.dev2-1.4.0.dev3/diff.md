# Comparing `tmp/mlserver-alibi-detect-1.4.0.dev2.tar.gz` & `tmp/mlserver_alibi_detect-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-alibi-detect-1.4.0.dev2.tar", last modified: Thu May  4 09:30:37 2023, max compression
+gzip compressed data, was "mlserver_alibi_detect-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-alibi-detect-1.4.0.dev2.tar` & `mlserver_alibi_detect-1.4.0.dev3.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:14:03.493129 mlserver_alibi_detect-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0     1575 2023-07-05 11:14:03.493129 mlserver_alibi_detect-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0       74 2023-07-05 11:14:03.493129 mlserver_alibi_detect-1.4.0.dev3/mlserver_alibi_detect/__init__.py
+-rw-r--r--   0        0        0     8244 2023-07-05 11:14:03.493129 mlserver_alibi_detect-1.4.0.dev3/mlserver_alibi_detect/runtime.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:14:03.493129 mlserver_alibi_detect-1.4.0.dev3/mlserver_alibi_detect/version.py
+-rw-r--r--   0        0        0      581 2023-07-05 11:14:03.493129 mlserver_alibi_detect-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2171 1970-01-01 00:00:00.000000 mlserver_alibi_detect-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-alibi-detect-1.4.0.dev2/LICENSE` & `mlserver_alibi_detect-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.4.0.dev2/PKG-INFO` & `mlserver_alibi_detect-1.4.0.dev3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,58 @@
-Metadata-Version: 2.1
-Name: mlserver-alibi-detect
-Version: 1.4.0.dev2
-Summary: Alibi-Detect runtime for MLServer
-Home-page: https://github.com/SeldonIO/MLServer.git
-Author: Seldon Technologies Ltd.
-Author-email: hello@seldon.io
-License: Apache 2.0
-Description: # Alibi-Detect runtime for MLServer
-        
-        This package provides a MLServer runtime compatible with
-        [alibi-detect](https://docs.seldon.io/projects/alibi-detect/en/latest/index.html)
-        models.
-        
-        ## Usage
-        
-        You can install the `mlserver-alibi-detect` runtime, alongside `mlserver`, as:
-        
-        ```bash
-        pip install mlserver mlserver-alibi-detect
-        ```
-        
-        For further information on how to use MLServer with Alibi-Detect, you can check
-        out this [worked out example](../../docs/examples/alibi-detect/README.md).
-        
-        ## Content Types
-        
-        If no [content type](../../docs/user-guide/content-type) is present on the
-        request or metadata, the Alibi-Detect runtime will try to decode the payload
-        as a [NumPy Array](../../docs/user-guide/content-type).
-        To avoid this, either send a different content type explicitly, or define the
-        correct one as part of your [model's
-        metadata](../../docs/reference/model-settings).
-        
-        ## Settings
-        
-        The Alibi Detect runtime exposes a couple setting flags which can be used to
-        customise how the runtime behaves.
-        These settings can be added under the `parameters.extra` section of your
-        `model-settings.json` file, e.g.
-        
-        ```{code-block} json
-        ---
-        emphasize-lines: 6-8
-        ---
-        {
-          "name": "drift-detector",
-          "implementation": "mlserver_alibi_detect.AlibiDetectRuntime",
-          "parameters": {
-            "uri": "./alibi-detect-artifact/",
-            "extra": {
-              "batch_size": 5
-            }
-          }
-        }
-        ```
-        
-        ### Reference
-        
-        You can find the full reference of the accepted extra settings for the Alibi
-        Detect runtime below:
-        
-        ```{eval-rst}
-        
-        .. autopydantic_settings:: mlserver_alibi_detect.runtime.AlibiDetectSettings
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Alibi-Detect runtime for MLServer
+
+This package provides a MLServer runtime compatible with
+[alibi-detect](https://docs.seldon.io/projects/alibi-detect/en/latest/index.html)
+models.
+
+## Usage
+
+You can install the `mlserver-alibi-detect` runtime, alongside `mlserver`, as:
+
+```bash
+pip install mlserver mlserver-alibi-detect
+```
+
+For further information on how to use MLServer with Alibi-Detect, you can check
+out this [worked out example](../../docs/examples/alibi-detect/README.md).
+
+## Content Types
+
+If no [content type](../../docs/user-guide/content-type) is present on the
+request or metadata, the Alibi-Detect runtime will try to decode the payload
+as a [NumPy Array](../../docs/user-guide/content-type).
+To avoid this, either send a different content type explicitly, or define the
+correct one as part of your [model's
+metadata](../../docs/reference/model-settings).
+
+## Settings
+
+The Alibi Detect runtime exposes a couple setting flags which can be used to
+customise how the runtime behaves.
+These settings can be added under the `parameters.extra` section of your
+`model-settings.json` file, e.g.
+
+```{code-block} json
+---
+emphasize-lines: 6-8
+---
+{
+  "name": "drift-detector",
+  "implementation": "mlserver_alibi_detect.AlibiDetectRuntime",
+  "parameters": {
+    "uri": "./alibi-detect-artifact/",
+    "extra": {
+      "batch_size": 5
+    }
+  }
+}
+```
+
+### Reference
+
+You can find the full reference of the accepted extra settings for the Alibi
+Detect runtime below:
+
+```{eval-rst}
+
+.. autopydantic_settings:: mlserver_alibi_detect.runtime.AlibiDetectSettings
+```
```

### Comparing `mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/runtime.py` & `mlserver_alibi_detect-1.4.0.dev3/mlserver_alibi_detect/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pydantic.error_wrappers import ValidationError
 from typing import Optional, List, Dict
 from pydantic import BaseSettings, Field
 from functools import cached_property
 
 from alibi_detect.saving import load_detector
 
+import mlserver
 from mlserver.batching import BatchedRequests
 from mlserver.types import InferenceRequest, InferenceResponse
 from mlserver.settings import ModelSettings
 from mlserver.model import MLModel
 from mlserver.codecs import NumpyCodec, NumpyRequestCodec
 from mlserver.utils import get_model_uri
 from mlserver.errors import MLServerError, InferenceError
@@ -65,14 +66,16 @@
         self._batch: List[InferenceRequest] = []
         super().__init__(settings)
 
     async def load(self) -> bool:
         self._model_uri = await get_model_uri(self._settings)
         try:
             self._model = load_detector(self._model_uri)
+            mlserver.register("seldon_model_drift", "Drift metrics")
+
             # Check whether an online drift detector (i.e. has a save_state method)
             self._online = True if hasattr(self._model, "save_state") else False
         except (
             ValueError,
             FileNotFoundError,
             EOFError,
             NotImplementedError,
@@ -121,25 +124,42 @@
             X = [X]  # type: ignore[assignment]
 
         # Run detector inference
         pred = []
         for x in X:
             # Prediction
             try:
-                pred.append(self._model.predict(x, **predict_kwargs))
+                current_pred = self._model.predict(x, **predict_kwargs)
+                pred.append(current_pred)
+                self._log_metrics(current_pred)
             except (ValueError, IndexError) as e:
                 raise InferenceError(
                     f"Invalid predict parameters for model {self._settings.name}: {e}"
                 ) from e
             # Save state if necessary
             if self._should_save_state:
                 self._save_state()
 
         return self._encode_response(self._postproc_pred(pred))
 
+    def _log_metrics(self, current_pred: dict) -> None:
+        if "data" not in current_pred:
+            return
+
+        data = current_pred["data"]
+        if "is_drift" in data:
+            # NOTE: is_drift may be an array larger than 1 (e.g. if drift is
+            # provided per input feature) or a single-value integer
+            is_drift = data["is_drift"]
+            if isinstance(is_drift, int):
+                is_drift = [is_drift]
+
+            for is_drift_instance in is_drift:
+                mlserver.log(seldon_model_drift=is_drift_instance)
+
     def _encode_response(self, y: dict) -> InferenceResponse:
         outputs = []
         for key in y["data"]:
             outputs.append(
                 NumpyCodec.encode_output(name=key, payload=np.array(y["data"][key]))
             )
```

### Comparing `mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/PKG-INFO` & `mlserver_alibi_detect-1.4.0.dev3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-detect
-Version: 1.4.0.dev2
+Version: 1.4.0.dev3
 Summary: Alibi-Detect runtime for MLServer
-Home-page: https://github.com/SeldonIO/MLServer.git
+License: Apache-2.0
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
-License: Apache 2.0
-Description: # Alibi-Detect runtime for MLServer
-        
-        This package provides a MLServer runtime compatible with
-        [alibi-detect](https://docs.seldon.io/projects/alibi-detect/en/latest/index.html)
-        models.
-        
-        ## Usage
-        
-        You can install the `mlserver-alibi-detect` runtime, alongside `mlserver`, as:
-        
-        ```bash
-        pip install mlserver mlserver-alibi-detect
-        ```
-        
-        For further information on how to use MLServer with Alibi-Detect, you can check
-        out this [worked out example](../../docs/examples/alibi-detect/README.md).
-        
-        ## Content Types
-        
-        If no [content type](../../docs/user-guide/content-type) is present on the
-        request or metadata, the Alibi-Detect runtime will try to decode the payload
-        as a [NumPy Array](../../docs/user-guide/content-type).
-        To avoid this, either send a different content type explicitly, or define the
-        correct one as part of your [model's
-        metadata](../../docs/reference/model-settings).
-        
-        ## Settings
-        
-        The Alibi Detect runtime exposes a couple setting flags which can be used to
-        customise how the runtime behaves.
-        These settings can be added under the `parameters.extra` section of your
-        `model-settings.json` file, e.g.
-        
-        ```{code-block} json
-        ---
-        emphasize-lines: 6-8
-        ---
-        {
-          "name": "drift-detector",
-          "implementation": "mlserver_alibi_detect.AlibiDetectRuntime",
-          "parameters": {
-            "uri": "./alibi-detect-artifact/",
-            "extra": {
-              "batch_size": 5
-            }
-          }
-        }
-        ```
-        
-        ### Reference
-        
-        You can find the full reference of the accepted extra settings for the Alibi
-        Detect runtime below:
-        
-        ```{eval-rst}
-        
-        .. autopydantic_settings:: mlserver_alibi_detect.runtime.AlibiDetectSettings
-        ```
-        
-Platform: UNKNOWN
+Requires-Python: >=3.8.1,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: alibi-detect[tensorflow]
+Requires-Dist: mlserver
 Description-Content-Type: text/markdown
+
+# Alibi-Detect runtime for MLServer
+
+This package provides a MLServer runtime compatible with
+[alibi-detect](https://docs.seldon.io/projects/alibi-detect/en/latest/index.html)
+models.
+
+## Usage
+
+You can install the `mlserver-alibi-detect` runtime, alongside `mlserver`, as:
+
+```bash
+pip install mlserver mlserver-alibi-detect
+```
+
+For further information on how to use MLServer with Alibi-Detect, you can check
+out this [worked out example](../../docs/examples/alibi-detect/README.md).
+
+## Content Types
+
+If no [content type](../../docs/user-guide/content-type) is present on the
+request or metadata, the Alibi-Detect runtime will try to decode the payload
+as a [NumPy Array](../../docs/user-guide/content-type).
+To avoid this, either send a different content type explicitly, or define the
+correct one as part of your [model's
+metadata](../../docs/reference/model-settings).
+
+## Settings
+
+The Alibi Detect runtime exposes a couple setting flags which can be used to
+customise how the runtime behaves.
+These settings can be added under the `parameters.extra` section of your
+`model-settings.json` file, e.g.
+
+```{code-block} json
+---
+emphasize-lines: 6-8
+---
+{
+  "name": "drift-detector",
+  "implementation": "mlserver_alibi_detect.AlibiDetectRuntime",
+  "parameters": {
+    "uri": "./alibi-detect-artifact/",
+    "extra": {
+      "batch_size": 5
+    }
+  }
+}
+```
+
+### Reference
+
+You can find the full reference of the accepted extra settings for the Alibi
+Detect runtime below:
+
+```{eval-rst}
+
+.. autopydantic_settings:: mlserver_alibi_detect.runtime.AlibiDetectSettings
+```
+
```

