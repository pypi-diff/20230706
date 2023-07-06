# Comparing `tmp/mlserver-huggingface-1.4.0.dev2.tar.gz` & `tmp/mlserver_huggingface-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-huggingface-1.4.0.dev2.tar", last modified: Thu May  4 09:30:40 2023, max compression
+gzip compressed data, was "mlserver_huggingface-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-huggingface-1.4.0.dev2.tar` & `mlserver_huggingface-1.4.0.dev3.tar`

### file list

```diff
@@ -1,30 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.794301 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/jsonlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/numpylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0     1706 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0       74 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/__init__.py
+-rw-r--r--   0        0        0      593 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/__init__.py
+-rw-r--r--   0        0        0     6684 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/base.py
+-rw-r--r--   0        0        0     1976 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/conversation.py
+-rw-r--r--   0        0        0     2464 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/image.py
+-rw-r--r--   0        0        0     1745 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/json.py
+-rw-r--r--   0        0        0     1938 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/jsonlist.py
+-rw-r--r--   0        0        0     2154 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/numpylist.py
+-rw-r--r--   0        0        0     1560 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/raw.py
+-rw-r--r--   0        0        0     5541 2023-07-05 11:14:00.408527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/utils.py
+-rw-r--r--   0        0        0     2538 2023-07-05 11:14:00.412527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/common.py
+-rw-r--r--   0        0        0     1291 2023-07-05 11:14:00.412527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/errors.py
+-rw-r--r--   0        0        0     9842 2023-07-05 11:14:00.412527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/metadata.py
+-rw-r--r--   0        0        0     2391 2023-07-05 11:14:00.412527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/runtime.py
+-rw-r--r--   0        0        0     5255 2023-07-05 11:14:00.412527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/settings.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:14:00.412527 mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/version.py
+-rw-r--r--   0        0        0      654 2023-07-05 11:14:00.412527 mlserver_huggingface-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 mlserver_huggingface-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-huggingface-1.4.0.dev2/LICENSE` & `mlserver_huggingface-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/PKG-INFO` & `mlserver_huggingface-1.4.0.dev3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-Metadata-Version: 2.1
-Name: mlserver-huggingface
-Version: 1.4.0.dev2
-Summary: HuggingFace runtime for MLServer
-Home-page: https://github.com/SeldonIO/MLServer.git
-Author: Seldon Technologies Ltd.
-Author-email: hello@seldon.io
-License: Apache 2.0
-Description: # HuggingFace runtime for MLServer
-        
-        This package provides a MLServer runtime compatible with HuggingFace Transformers.
-        
-        ## Usage
-        
-        You can install the runtime, alongside `mlserver`, as:
-        
-        ```bash
-        pip install mlserver mlserver-huggingface
-        ```
-        
-        For further information on how to use MLServer with HuggingFace, you can check
-        out this [worked out example](../../docs/examples/huggingface/README.md).
-        
-        ## Settings
-        
-        The HuggingFace runtime exposes a couple extra parameters which can be used to
-        customise how the runtime behaves.
-        These settings can be added under the `parameters.extra` section of your
-        `model-settings.json` file, e.g.
-        
-        ```{code-block} json
-        ---
-        emphasize-lines: 5-8
-        ---
-        {
-          "name": "qa",
-          "implementation": "mlserver_huggingface.HuggingFaceRuntime",
-          "parameters": {
-            "extra": {
-              "task": "question-answering",
-              "optimum_model": true
-            }
-          }
-        }
-        ```
-        
-        ````{note}
-        These settings can also be injected through environment variables prefixed with `MLSERVER_MODEL_HUGGINGFACE_`, e.g.
-        
-        ```bash
-        MLSERVER_MODEL_HUGGINGFACE_TASK="question-answering"
-        MLSERVER_MODEL_HUGGINGFACE_OPTIMUM_MODEL=true
-        ```
-        ````
-        
-        ### Reference
-        
-        You can find the full reference of the accepted extra settings for the
-        HuggingFace runtime below:
-        
-        ```{eval-rst}
-        
-        .. autopydantic_settings:: mlserver_huggingface.settings.HuggingFaceSettings
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# HuggingFace runtime for MLServer
+
+This package provides a MLServer runtime compatible with HuggingFace Transformers.
+
+## Usage
+
+You can install the runtime, alongside `mlserver`, as:
+
+```bash
+pip install mlserver mlserver-huggingface
+```
+
+For further information on how to use MLServer with HuggingFace, you can check
+out this [worked out example](../../docs/examples/huggingface/README.md).
+
+## Content Types
+
+The HuggingFace runtime will always decode the input request using its own
+built-in codec.
+Therefore, [content type annotations](../../docs/user-guide/content-type) at
+the request level will **be ignored**.
+Not that this **doesn't include [input-level content
+type](../../docs/user-guide/content-type#Codecs) annotations**, which will be
+respected as usual.
+
+## Settings
+
+The HuggingFace runtime exposes a couple extra parameters which can be used to
+customise how the runtime behaves.
+These settings can be added under the `parameters.extra` section of your
+`model-settings.json` file, e.g.
+
+```{code-block} json
+---
+emphasize-lines: 5-8
+---
+{
+  "name": "qa",
+  "implementation": "mlserver_huggingface.HuggingFaceRuntime",
+  "parameters": {
+    "extra": {
+      "task": "question-answering",
+      "optimum_model": true
+    }
+  }
+}
+```
+
+````{note}
+These settings can also be injected through environment variables prefixed with `MLSERVER_MODEL_HUGGINGFACE_`, e.g.
+
+```bash
+MLSERVER_MODEL_HUGGINGFACE_TASK="question-answering"
+MLSERVER_MODEL_HUGGINGFACE_OPTIMUM_MODEL=true
+```
+````
+
+### Reference
+
+You can find the full reference of the accepted extra settings for the
+HuggingFace runtime below:
+
+```{eval-rst}
+
+.. autopydantic_settings:: mlserver_huggingface.settings.HuggingFaceSettings
+```
```

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/__init__.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/base.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class MultiInputRequestCodec(RequestCodec):
     """
     Huggingface codecs is prefered, then mlserver's
     """
 
     DefaultCodec: Type["InputCodecTy"] = StringCodec
     InputCodecsWithPriority: List[Type[InputCodecTy]] = []
-    ContentType = StringCodec.ContentType
+    ContentType = ""
 
     @classmethod
     def _find_encode_codecs(
         cls, payload: Dict[str, Any]
     ) -> Dict[str, Union[Type["InputCodecTy"], "InputCodecTy", None]]:
         field_codec: Dict[str, Union[Type["InputCodecTy"], "InputCodecTy", None]] = {}
         for field, value in payload.items():
@@ -190,9 +190,9 @@
         PILImageCodec,
         HuggingfaceSingleJSONCodec,
         HuggingfaceListJSONCodec,
         HuggingfaceConversationCodec,
         NumpyListCodec,
         RawCodec,
     ]
-    ContentType = StringCodec.ContentType
+    ContentType = "hf"
     DefaultCodec = StringCodec
```

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/conversation.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/conversation.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/image.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/image.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/json.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/json.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/jsonlist.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/jsonlist.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/numpylist.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/numpylist.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/raw.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/raw.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/utils.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/codecs/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/common.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/common.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/errors.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/metadata.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/metadata.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/runtime.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/runtime.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import torch
 
 from mlserver.model import MLModel
 from mlserver.settings import ModelSettings
 from mlserver.logging import logger
 from mlserver.types import (
     InferenceRequest,
     InferenceResponse,
@@ -34,24 +35,39 @@
         # Now we load the cached model which should not block asyncio
         self._model = load_pipeline_from_settings(self.hf_settings, self.settings)
         self._merge_metadata()
         return True
 
     async def predict(self, payload: InferenceRequest) -> InferenceResponse:
         # TODO: convert and validate?
-        kwargs = self.decode_request(payload, default_codec=HuggingfaceRequestCodec)
+        kwargs = HuggingfaceRequestCodec.decode_request(payload)
         args = kwargs.pop("args", [])
 
         array_inputs = kwargs.pop("array_inputs", [])
         if array_inputs:
             args = [list(array_inputs)] + args
         prediction = self._model(*args, **kwargs)
 
         return self.encode_response(
             payload=prediction, default_codec=HuggingfaceRequestCodec
         )
 
+    async def unload(self) -> bool:
+        # TODO: Free up Tensorflow's GPU memory
+        is_torch = self._model.framework == "pt"
+        if not is_torch:
+            return True
+
+        uses_gpu = torch.cuda.is_available() and self._model.device != -1
+        if not uses_gpu:
+            # Nothing to free
+            return True
+
+        # Free up Torch's GPU memory
+        torch.cuda.empty_cache()
+        return True
+
     def _merge_metadata(self) -> None:
         meta = METADATA.get(self.hf_settings.task)
         if meta:
             self.inputs += meta.get("inputs", [])  # type: ignore
             self.outputs += meta.get("outputs", [])  # type: ignore
```

### Comparing `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/settings.py` & `mlserver_huggingface-1.4.0.dev3/mlserver_huggingface/settings.py`

 * *Files identical despite different names*

