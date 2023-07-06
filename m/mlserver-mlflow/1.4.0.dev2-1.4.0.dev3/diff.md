# Comparing `tmp/mlserver-mlflow-1.4.0.dev2.tar.gz` & `tmp/mlserver_mlflow-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-mlflow-1.4.0.dev2.tar", last modified: Thu May  4 09:30:52 2023, max compression
+gzip compressed data, was "mlserver_mlflow-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-mlflow-1.4.0.dev2.tar` & `mlserver_mlflow-1.4.0.dev3.tar`

### file list

```diff
@@ -1,18 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0      843 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0      119 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/__init__.py
+-rw-r--r--   0        0        0     2115 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/codecs.py
+-rw-r--r--   0        0        0     2526 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/metadata.py
+-rw-r--r--   0        0        0     7217 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/runtime.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/version.py
+-rw-r--r--   0        0        0      605 2023-07-05 11:14:00.549366 mlserver_mlflow-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 mlserver_mlflow-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-mlflow-1.4.0.dev2/LICENSE` & `mlserver_mlflow-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.4.0.dev2/PKG-INFO` & `mlserver_mlflow-1.4.0.dev3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,27 @@
-Metadata-Version: 2.1
-Name: mlserver-mlflow
-Version: 1.4.0.dev2
-Summary: MLflow runtime for MLServer
-Home-page: https://github.com/SeldonIO/MLServer.git
-Author: Seldon Technologies Ltd.
-Author-email: hello@seldon.io
-License: Apache 2.0
-Description: # MLflow runtime for MLServer
-        
-        This package provides a MLServer runtime compatible with [MLflow
-        models](https://www.mlflow.org/docs/latest/models.html).
-        
-        ## Usage
-        
-        You can install the runtime, alongside `mlserver`, as:
-        
-        ```bash
-        pip install mlserver mlserver-mlflow
-        ```
-        
-        ## Content Types
-        
-        The MLflow inference runtime introduces a new `dict` content type, which
-        decodes an incoming V2 request as a [dictionary of
-        tensors](https://www.mlflow.org/docs/latest/models.html#deploy-mlflow-models).
-        This is useful for certain MLflow-serialised models, which will expect that the
-        model inputs are serialised in this format.
-        
-        ```{note}
-        The `dict` content type can be _stacked_ with other content types, like
-        [`np`](../../docs/user-guide/content-type).
-        This allows the user to use a different set of content types to decode each of
-        the dict entries.
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# MLflow runtime for MLServer
+
+This package provides a MLServer runtime compatible with [MLflow
+models](https://www.mlflow.org/docs/latest/models.html).
+
+## Usage
+
+You can install the runtime, alongside `mlserver`, as:
+
+```bash
+pip install mlserver mlserver-mlflow
+```
+
+## Content Types
+
+The MLflow inference runtime introduces a new `dict` content type, which
+decodes an incoming V2 request as a [dictionary of
+tensors](https://www.mlflow.org/docs/latest/models.html#deploy-mlflow-models).
+This is useful for certain MLflow-serialised models, which will expect that the
+model inputs are serialised in this format.
+
+```{note}
+The `dict` content type can be _stacked_ with other content types, like
+[`np`](../../docs/user-guide/content-type).
+This allows the user to use a different set of content types to decode each of
+the dict entries.
+```
```

### Comparing `mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/codecs.py` & `mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/codecs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import Optional, Dict
 
-from mlserver.types import InferenceRequest, InferenceResponse
+from mlserver.types import InferenceRequest, InferenceResponse, Parameters
 from mlserver.codecs import (
     NumpyCodec,
     RequestCodec,
     register_request_codec,
     get_decoded_or_raw,
 )
 from mlserver.codecs.lists import is_list_of
@@ -42,15 +42,18 @@
     ) -> InferenceResponse:
         outputs = [
             NumpyCodec.encode_output(name, value, **kwargs)
             for name, value in payload.items()
         ]
 
         return InferenceResponse(
-            model_name=model_name, model_version=model_version, outputs=outputs
+            model_name=model_name,
+            model_version=model_version,
+            outputs=outputs,
+            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_response(cls, response: InferenceResponse) -> TensorDict:
         return {
             response_output.name: NumpyCodec.decode_output(response_output)
             for response_output in response.outputs
@@ -59,15 +62,17 @@
     @classmethod
     def encode_request(cls, payload: TensorDict, **kwargs) -> InferenceRequest:
         inputs = [
             NumpyCodec.encode_input(name, value, **kwargs)
             for name, value in payload.items()
         ]
 
-        return InferenceRequest(inputs=inputs)
+        return InferenceRequest(
+            inputs=inputs, parameters=Parameters(content_type=cls.ContentType)
+        )
 
     @classmethod
     def decode_request(cls, request: InferenceRequest) -> TensorDict:
         return {
             request_input.name: get_decoded_or_raw(request_input)
             for request_input in request.inputs
         }
```

### Comparing `mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/metadata.py` & `mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/metadata.py`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/runtime.py` & `mlserver_mlflow-1.4.0.dev3/mlserver_mlflow/runtime.py`

 * *Files identical despite different names*

