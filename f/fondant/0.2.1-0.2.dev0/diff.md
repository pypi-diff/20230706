# Comparing `tmp/fondant-0.2.1.tar.gz` & `tmp/fondant-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondant-0.2.1.tar", max compression
+gzip compressed data, was "fondant-0.2.dev0.tar", max compression
```

## Comparing `fondant-0.2.1.tar` & `fondant-0.2.dev0.tar`

### file list

```diff
@@ -1,95 +1,18 @@
--rw-r--r--   0        0        0    11356 2023-07-05 09:48:05.287195 fondant-0.2.1/LICENSE
--rw-r--r--   0        0        0    18121 2023-07-05 09:48:05.287195 fondant-0.2.1/README.md
--rw-r--r--   0        0        0      130 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/__init__.py
--rw-r--r--   0        0        0    11364 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/cli.py
--rw-r--r--   0        0        0     6333 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/compiler.py
--rw-r--r--   0        0        0    13679 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/component.py
--rw-r--r--   0        0        0    11441 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/component_spec.py
--rw-r--r--   0        0        0      598 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/caption_images/Dockerfile
--rw-r--r--   0        0        0      295 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/caption_images/README.md
--rw-r--r--   0        0        0      519 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/caption_images/fondant_component.yaml
--rw-r--r--   0        0        0       63 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/caption_images/requirements.txt
--rw-r--r--   0        0        0     3097 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/caption_images/src/main.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/download_images/Dockerfile
--rw-r--r--   0        0        0      661 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/download_images/README.md
--rw-r--r--   0        0        0     1047 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/download_images/fondant_component.yaml
--rw-r--r--   0        0        0       73 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/download_images/requirements.txt
--rw-r--r--   0        0        0     4222 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/download_images/src/main.py
--rw-r--r--   0        0        0    10656 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/download_images/src/resizer.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/embedding_based_laion_retrieval/Dockerfile
--rw-r--r--   0        0        0      745 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/embedding_based_laion_retrieval/fondant_component.yaml
--rw-r--r--   0        0        0       15 2023-07-05 10:13:58.252161 fondant-0.2.1/fondant/components/embedding_based_laion_retrieval/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/embedding_based_laion_retrieval/src/__init__.py
--rw-r--r--   0        0        0     5853 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/embedding_based_laion_retrieval/src/clip_client.py
--rw-r--r--   0        0        0     2462 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/embedding_based_laion_retrieval/src/main.py
--rw-r--r--   0        0        0      570 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_comments/Dockerfile
--rw-r--r--   0        0        0      395 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_comments/fondant_component.yaml
--rw-r--r--   0        0        0       29 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_comments/requirements.txt
--rw-r--r--   0        0        0     1333 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_comments/src/main.py
--rw-r--r--   0        0        0     4179 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_comments/src/utils/text_extraction.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_image_resolution/Dockerfile
--rw-r--r--   0        0        0      420 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_image_resolution/fondant_component.yaml
--rw-r--r--   0        0        0       28 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_image_resolution/requirements.txt
--rw-r--r--   0        0        0     1355 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_image_resolution/src/main.py
--rw-r--r--   0        0        0      570 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_line_length/Dockerfile
--rw-r--r--   0        0        0      616 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/filter_line_length/fondant_component.yaml
--rw-r--r--   0        0        0       29 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_line_length/requirements.txt
--rw-r--r--   0        0        0     1409 2023-07-05 10:13:58.256161 fondant-0.2.1/fondant/components/filter_line_length/src/main.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_cropping/Dockerfile
--rw-r--r--   0        0        0     1182 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_cropping/README.md
--rw-r--r--   0        0        0      717 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_cropping/fondant_component.yaml
--rw-r--r--   0        0        0       42 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_cropping/requirements.txt
--rw-r--r--   0        0        0     2927 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_cropping/src/image_crop.py
--rw-r--r--   0        0        0     1897 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_cropping/src/main.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_embedding/Dockerfile
--rw-r--r--   0        0        0      500 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_embedding/fondant_component.yaml
--rw-r--r--   0        0        0       63 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_embedding/requirements.txt
--rw-r--r--   0        0        0     2972 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_embedding/src/main.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_resolution_extraction/Dockerfile
--rw-r--r--   0        0        0      364 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_resolution_extraction/fondant_component.yaml
--rw-r--r--   0        0        0       45 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_resolution_extraction/requirements.txt
--rw-r--r--   0        0        0     1343 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/image_resolution_extraction/src/main.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/load_from_hf_hub/Dockerfile
--rw-r--r--   0        0        0      845 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/load_from_hf_hub/fondant_component.yaml
--rw-r--r--   0        0        0       66 2023-07-05 10:13:58.260161 fondant-0.2.1/fondant/components/load_from_hf_hub/requirements.txt
--rw-r--r--   0        0        0     1919 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/load_from_hf_hub/src/main.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/Dockerfile
--rw-r--r--   0        0        0     1038 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/README.md
--rw-r--r--   0        0        0      352 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/fondant_component.yaml
--rw-r--r--   0        0        0       92 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/requirements.txt
--rw-r--r--   0        0        0    26294 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/src/gibberish_data/big.model
--rw-r--r--   0        0        0     1805 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/src/main.py
--rw-r--r--   0        0        0     1447 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/src/pii_detection.py
--rw-r--r--   0        0        0     5436 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/src/pii_redaction.py
--rw-r--r--   0        0        0      869 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/src/replacements.json
--rw-r--r--   0        0        0     9261 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/src/utils/emails_ip_addresses_detection.py
--rw-r--r--   0        0        0     5022 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/pii_redaction/src/utils/keys_detection.py
--rw-r--r--   0        0        0      569 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/prompt_based_laion_retrieval/Dockerfile
--rw-r--r--   0        0        0      518 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/prompt_based_laion_retrieval/README.md
--rw-r--r--   0        0        0      699 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/prompt_based_laion_retrieval/fondant_component.yaml
--rw-r--r--   0        0        0       15 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/prompt_based_laion_retrieval/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/prompt_based_laion_retrieval/src/__init__.py
--rw-r--r--   0        0        0     5860 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/prompt_based_laion_retrieval/src/clip_client.py
--rw-r--r--   0        0        0     2304 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/prompt_based_laion_retrieval/src/main.py
--rw-r--r--   0        0        0      598 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/segment_images/Dockerfile
--rw-r--r--   0        0        0      462 2023-07-05 10:13:58.268161 fondant-0.2.1/fondant/components/segment_images/fondant_component.yaml
--rw-r--r--   0        0        0       63 2023-07-05 10:13:58.264161 fondant-0.2.1/fondant/components/segment_images/requirements.txt
--rw-r--r--   0        0        0     3834 2023-07-05 10:13:58.268161 fondant-0.2.1/fondant/components/segment_images/src/main.py
--rw-r--r--   0        0        0     3681 2023-07-05 10:13:58.268161 fondant-0.2.1/fondant/components/segment_images/src/palette.py
--rw-r--r--   0        0        0      570 2023-07-05 10:13:58.268161 fondant-0.2.1/fondant/components/write_to_hf_hub/Dockerfile
--rw-r--r--   0        0        0      788 2023-07-05 10:13:58.268161 fondant-0.2.1/fondant/components/write_to_hf_hub/fondant_component.yaml
--rw-r--r--   0        0        0       83 2023-07-05 10:13:58.268161 fondant-0.2.1/fondant/components/write_to_hf_hub/requirements.txt
--rw-r--r--   0        0        0     3476 2023-07-05 10:13:58.268161 fondant-0.2.1/fondant/components/write_to_hf_hub/src/main.py
--rw-r--r--   0        0        0     6188 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/data_io.py
--rw-r--r--   0        0        0      733 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/exceptions.py
--rw-r--r--   0        0        0     1402 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/explorer.py
--rw-r--r--   0        0        0     2229 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/import_utils.py
--rw-r--r--   0        0        0    10147 2023-07-05 09:48:05.319195 fondant-0.2.1/fondant/manifest.py
--rw-r--r--   0        0        0    22148 2023-07-05 09:48:05.323195 fondant-0.2.1/fondant/pipeline.py
--rw-r--r--   0        0        0      467 2023-07-05 09:48:05.323195 fondant-0.2.1/fondant/runner.py
--rw-r--r--   0        0        0     4763 2023-07-05 09:48:05.323195 fondant-0.2.1/fondant/schema.py
--rw-r--r--   0        0        0     1215 2023-07-05 09:48:05.323195 fondant-0.2.1/fondant/schemas/common.json
--rw-r--r--   0        0        0     2050 2023-07-05 09:48:05.323195 fondant-0.2.1/fondant/schemas/component_spec.json
--rw-r--r--   0        0        0     1251 2023-07-05 09:48:05.323195 fondant-0.2.1/fondant/schemas/manifest.json
--rw-r--r--   0        0        0     3117 2023-07-05 10:13:47.792035 fondant-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    19686 1970-01-01 00:00:00.000000 fondant-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-14 09:12:43.912402 fondant-0.2.dev0/LICENSE
+-rw-r--r--   0        0        0     4290 2023-04-14 09:23:54.059098 fondant-0.2.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 09:12:43.929663 fondant-0.2.dev0/fondant/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-14 09:12:43.929762 fondant-0.2.dev0/fondant/components/__init__.py
+-rw-r--r--   0        0        0    17668 2023-04-14 09:15:10.579020 fondant-0.2.dev0/fondant/components/common.py
+-rw-r--r--   0        0        0     5456 2023-04-14 09:15:05.225089 fondant-0.2.dev0/fondant/components/hf_datasets_components.py
+-rw-r--r--   0        0        0     4697 2023-04-14 09:15:06.732962 fondant-0.2.dev0/fondant/components/pandas_components.py
+-rw-r--r--   0        0        0      342 2023-04-14 09:16:45.591739 fondant-0.2.dev0/fondant/exceptions.py
+-rw-r--r--   0        0        0     5287 2023-04-14 09:19:51.255014 fondant-0.2.dev0/fondant/gcp_storage.py
+-rw-r--r--   0        0        0     2241 2023-04-14 09:12:43.930278 fondant-0.2.dev0/fondant/import_utils.py
+-rw-r--r--   0        0        0      874 2023-04-14 09:12:43.930343 fondant-0.2.dev0/fondant/io.py
+-rw-r--r--   0        0        0      605 2023-04-14 09:12:43.930408 fondant-0.2.dev0/fondant/logger.py
+-rw-r--r--   0        0        0     6594 2023-04-14 09:21:24.391801 fondant-0.2.dev0/fondant/manifest.py
+-rw-r--r--   0        0        0     1444 2023-04-14 09:20:04.669266 fondant-0.2.dev0/fondant/pipeline_utils.py
+-rw-r--r--   0        0        0     1672 2023-04-14 09:12:43.930673 fondant-0.2.dev0/fondant/schemas/manifest.json
+-rw-r--r--   0        0        0     4361 2023-04-14 09:12:43.930743 fondant-0.2.dev0/fondant/storage_interface.py
+-rw-r--r--   0        0        0     2162 2023-04-14 09:26:06.225285 fondant-0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0     6225 1970-01-01 00:00:00.000000 fondant-0.2.dev0/PKG-INFO
```

### Comparing `fondant-0.2.1/LICENSE` & `fondant-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `fondant-0.2.1/fondant/import_utils.py` & `fondant-0.2.dev0/fondant/import_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,68 @@
-"""Import utils."""
-import importlib.metadata
-import importlib.util
+"""
+Import utils
+"""
 import logging
-import sys
+import importlib.util
+import importlib.metadata
 from pathlib import Path
+import sys
 
 logger = logging.getLogger(__name__)
 
 PANDAS_IMPORT_ERROR = """
-`{0}` requires the pandas library but it was not found in your environment. Please install fondant
+`{0}` requires the pandas library but it was not found in your environment. Please install express
  using the 'pandas' extra.
 """
 
 DATASETS_IMPORT_ERROR = """
 `{0}` requires the 🤗 Datasets library but it was not found in your environment.
-Please install fondant using the 'datasets' extra.
+Please install express using the 'datasets' extra.
 Note that if you have a local folder named `datasets` or a local python file named
- `datasets.py` in your current working directory, python may try to import this instead of the 🤗
+ `datasets.py` in your current working directory, python may try to import this instead of the 🤗 
  Datasets library. You should rename this folder or that python file if that's the case.
   Please note that you may need to restart your runtime after installation.
 """
 
 KFP_IMPORT_ERROR = """
 `{0}` requires the kubeflow pipelines (kfp) library but it was not found in your environment.
-Please install fondant using the 'pipelines' extra.
+Please install express using the 'pipelines' extra.
 """
 
 
 def is_package_available(package_name: str, import_error_msg: str) -> bool:
     """
     Function that checks if a given package is available
     Args:
         package_name (str): the name of the package
         import_error_msg (str): the error message to return if the package is not found
     Returns:
-        bool: check if package is available.
+        bool: check if package is available
     """
+
     package_available = importlib.util.find_spec(package_name) is not None
 
     try:
         package_version = importlib.metadata.version(package_name)
         logger.debug(f"Successfully imported {package_name} version {package_version}")
     except importlib.metadata.PackageNotFoundError:
         package_available = False
 
     if package_available:
         return package_available
-
-    raise ModuleNotFoundError(import_error_msg.format(Path(sys.argv[0]).stem))
+    else:
+        raise ModuleNotFoundError(import_error_msg.format(Path(sys.argv[0]).stem))
 
 
 def is_datasets_available():
-    """Check if 'datasets' is available."""
+    """Check if 'datasets' is available"""
     return is_package_available("datasets", DATASETS_IMPORT_ERROR)
 
 
 def is_pandas_available():
-    """Check if 'pandas' is available."""
+    """Check if 'pandas' is available"""
     return is_package_available("pandas", PANDAS_IMPORT_ERROR)
 
 
 def is_kfp_available():
-    """Check if 'pandas' is available."""
+    """Check if 'pandas' is available"""
     return is_package_available("kfp", KFP_IMPORT_ERROR)
```

### Comparing `fondant-0.2.1/fondant/schemas/common.json` & `fondant-0.2.dev0/fondant/schemas/manifest.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.13666666666666666%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-04/schema#'",*

 * * "'definitions'": "{'field': {'properties': {'type': {'enum': ['bool', 'int8', 'int16', 'int32', "*

 * *                  "'uint8', 'uint16', 'uint32', 'uint64', 'float16', 'float32', 'float64', "*

 * *                  "'decimal', 'time32', 'time64', 'timestamp', 'date32', 'date64', 'duration', "*

 * *                  "'utf8', 'binary', 'categorical', 'list', 'struct'], delete: ['$ref']}, delete: "*

 * *                  "['items']}, delete: ['additionalProperties']} […]*

```diff
@@ -1,27 +1,38 @@
 {
+    "$schema": "http://json-schema.org/draft-04/schema#",
     "definitions": {
         "field": {
-            "additionalProperties": false,
             "properties": {
-                "items": {
-                    "oneOf": [
-                        {
-                            "$ref": "#/definitions/field"
-                        },
-                        {
-                            "items": {
-                                "$ref": "#/definitions/field"
-                            },
-                            "type": "array"
-                        }
-                    ]
-                },
                 "type": {
-                    "$ref": "#/definitions/subset_data_type",
+                    "enum": [
+                        "bool",
+                        "int8",
+                        "int16",
+                        "int32",
+                        "uint8",
+                        "uint16",
+                        "uint32",
+                        "uint64",
+                        "float16",
+                        "float32",
+                        "float64",
+                        "decimal",
+                        "time32",
+                        "time64",
+                        "timestamp",
+                        "date32",
+                        "date64",
+                        "duration",
+                        "utf8",
+                        "binary",
+                        "categorical",
+                        "list",
+                        "struct"
+                    ],
                     "type": "string"
                 }
             },
             "required": [
                 "type"
             ],
             "type": "object"
@@ -29,38 +40,65 @@
         "fields": {
             "additionalProperties": {
                 "$ref": "#/definitions/field"
             },
             "minProperties": 1,
             "type": "object"
         },
-        "subset_data_type": {
-            "enum": [
-                "bool",
-                "int8",
-                "int16",
-                "int32",
-                "uint8",
-                "uint16",
-                "uint32",
-                "uint64",
-                "float16",
-                "float32",
-                "float64",
-                "decimal",
-                "time32",
-                "time64",
-                "timestamp",
-                "date32",
-                "date64",
-                "duration",
-                "utf8",
-                "string",
-                "binary",
-                "list",
-                "struct",
-                "array"
+        "subset": {
+            "properties": {
+                "fields": {
+                    "$ref": "#/definitions/fields"
+                },
+                "location": {
+                    "pattern": "/.*",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "location",
+                "fields"
             ],
-            "type": "string"
+            "type": "object"
+        },
+        "subsets": {
+            "additionalProperties": {
+                "$ref": "#/definitions/subset"
+            },
+            "type": "object"
+        }
+    },
+    "properties": {
+        "index": {
+            "properties": {
+                "location": {
+                    "type": "string"
+                }
+            },
+            "required": [
+                "location"
+            ],
+            "type": "object"
+        },
+        "metadata": {
+            "properties": {
+                "base_path": {
+                    "format": "uri",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "base_path"
+            ],
+            "type": "object"
+        },
+        "subsets": {
+            "$ref": "#/definitions/subsets"
         }
-    }
+    },
+    "required": [
+        "metadata",
+        "index",
+        "subsets"
+    ],
+    "type": "object"
 }
```

