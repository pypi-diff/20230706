# Comparing `tmp/form_tools-0.1.2.tar.gz` & `tmp/form_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "form_tools-0.1.2.tar", max compression
+gzip compressed data, was "form_tools-0.1.3.tar", max compression
```

## Comparing `form_tools-0.1.2.tar` & `form_tools-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1090 2023-02-28 13:48:47.012024 form_tools-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     4999 2023-02-28 13:48:47.012024 form_tools-0.1.2/README.md
--rw-r--r--   0        0        0      110 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/__init__.py
--rw-r--r--   0        0        0     7244 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/command_line.py
--rw-r--r--   0        0        0       50 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_meta/__init__.py
--rw-r--r--   0        0        0    11382 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_meta/bounding_box.py
--rw-r--r--   0        0        0        0 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_meta/extractors/__init__.py
--rw-r--r--   0        0        0    15728 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_meta/extractors/pdf_form_extractor.py
--rw-r--r--   0        0        0     3001 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_meta/form_field.py
--rw-r--r--   0        0        0    12249 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_meta/form_meta.py
--rw-r--r--   0        0        0       54 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/__init__.py
--rw-r--r--   0        0        0     4736 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/bounding_box_operator.py
--rw-r--r--   0        0        0    27260 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/form_operator.py
--rw-r--r--   0        0        0    17563 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/form_page_operator.py
--rw-r--r--   0        0        0     1330 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/ocr_engines/base.py
--rw-r--r--   0        0        0     4298 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/ocr_engines/tesseract.py
--rw-r--r--   0        0        0     5051 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/operator_configs.py
--rw-r--r--   0        0        0     1298 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/form_operators/preprocessors.py
--rw-r--r--   0        0        0        0 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/utils/__init__.py
--rw-r--r--   0        0        0       33 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/utils/constants.py
--rw-r--r--   0        0        0     2008 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/utils/converters.py
--rw-r--r--   0        0        0    11489 2023-02-28 13:48:47.016024 form_tools-0.1.2/form_tools/utils/image_reader.py
--rw-r--r--   0        0        0      989 2023-02-28 13:48:47.016024 form_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5947 1970-01-01 00:00:00.000000 form_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-07-06 12:56:22.095092 form_tools-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     4999 2023-07-06 12:56:22.095092 form_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      110 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/__init__.py
+-rw-r--r--   0        0        0     7244 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/command_line.py
+-rw-r--r--   0        0        0       50 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_meta/__init__.py
+-rw-r--r--   0        0        0    11382 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_meta/bounding_box.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_meta/extractors/__init__.py
+-rw-r--r--   0        0        0    15728 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_meta/extractors/pdf_form_extractor.py
+-rw-r--r--   0        0        0     3001 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_meta/form_field.py
+-rw-r--r--   0        0        0    12249 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_meta/form_meta.py
+-rw-r--r--   0        0        0       54 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/__init__.py
+-rw-r--r--   0        0        0     4736 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/bounding_box_operator.py
+-rw-r--r--   0        0        0    27260 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/form_operator.py
+-rw-r--r--   0        0        0    17563 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/form_page_operator.py
+-rw-r--r--   0        0        0     1330 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/ocr_engines/base.py
+-rw-r--r--   0        0        0     4298 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/ocr_engines/tesseract.py
+-rw-r--r--   0        0        0     5051 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/operator_configs.py
+-rw-r--r--   0        0        0     1298 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/form_operators/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/utils/__init__.py
+-rw-r--r--   0        0        0       33 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/utils/constants.py
+-rw-r--r--   0        0        0     2008 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/utils/converters.py
+-rw-r--r--   0        0        0    11523 2023-07-06 12:56:22.095092 form_tools-0.1.3/form_tools/utils/image_reader.py
+-rw-r--r--   0        0        0     1030 2023-07-06 12:56:22.095092 form_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5947 1970-01-01 00:00:00.000000 form_tools-0.1.3/PKG-INFO
```

### Comparing `form_tools-0.1.2/LICENSE.md` & `form_tools-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/README.md` & `form_tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/command_line.py` & `form_tools-0.1.3/form_tools/command_line.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_meta/bounding_box.py` & `form_tools-0.1.3/form_tools/form_meta/bounding_box.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_meta/extractors/pdf_form_extractor.py` & `form_tools-0.1.3/form_tools/form_meta/extractors/pdf_form_extractor.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_meta/form_field.py` & `form_tools-0.1.3/form_tools/form_meta/form_field.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_meta/form_meta.py` & `form_tools-0.1.3/form_tools/form_meta/form_meta.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_operators/bounding_box_operator.py` & `form_tools-0.1.3/form_tools/form_operators/bounding_box_operator.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_operators/form_operator.py` & `form_tools-0.1.3/form_tools/form_operators/form_operator.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_operators/form_page_operator.py` & `form_tools-0.1.3/form_tools/form_operators/form_page_operator.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_operators/ocr_engines/base.py` & `form_tools-0.1.3/form_tools/form_operators/ocr_engines/base.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_operators/ocr_engines/tesseract.py` & `form_tools-0.1.3/form_tools/form_operators/ocr_engines/tesseract.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_operators/operator_configs.py` & `form_tools-0.1.3/form_tools/form_operators/operator_configs.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/form_operators/preprocessors.py` & `form_tools-0.1.3/form_tools/form_operators/preprocessors.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/utils/converters.py` & `form_tools-0.1.3/form_tools/utils/converters.py`

 * *Files identical despite different names*

### Comparing `form_tools-0.1.2/form_tools/utils/image_reader.py` & `form_tools-0.1.3/form_tools/utils/image_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,16 @@
             valid_suffix = (
                 valid_suffix if isinstance(valid_suffix, list) else [valid_suffix]
             )
 
             img_fps = [fp for fp in img_fps if Path(fp).suffix in valid_suffix]
 
         imgs_and_mp = [
-            ImageReader._read_image_file(fp, **reader_kwargs) for fp in img_fps
+            ImageReader._read_image_file(fp, **reader_kwargs)
+            for fp in sorted(img_fps, reverse=True)
         ]
 
         imgs = [imgs for _, imgs in imgs_and_mp]
 
         imgs_flattened = [img for imgs_list in imgs for img in imgs_list]
 
         if len(imgs_flattened) == 1:
```

### Comparing `form_tools-0.1.2/pyproject.toml` & `form_tools-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "form-tools"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["gwionap <gwion.aprhobat@justice.gov.uk>"]
 readme = "README.md"
 packages = [{include = "form_tools"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
@@ -25,19 +25,20 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 moto = "^4.1.3"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.20.0"
 scikit-image = "^0.19.3"
 mdx-include = "^1.4.2"
-mkdocs-material = "^8.5.6"
-mkdocstrings = "^0.19.0"
-mkdocstrings-python = "^0.7.1"
+mkdocs-material = ">=8.5.6"
+mkdocstrings = ">=0.19.0"
+mkdocstrings-python = ">=0.7.1"
 mypy = "^0.991"
 ipykernel = "^6.21.1"
+mkdocs-tech-docs-template = "^0.0.25"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 form-tools = "form_tools.command_line:Main"
```

### Comparing `form_tools-0.1.2/PKG-INFO` & `form_tools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: form-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: gwionap
 Author-email: gwion.aprhobat@justice.gov.uk
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

