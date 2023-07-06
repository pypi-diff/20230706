# Comparing `tmp/caep-0.1.9.tar.gz` & `tmp/caep-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caep-0.1.9.tar", last modified: Thu Jun  8 06:03:50 2023, max compression
+gzip compressed data, was "caep-1.0.0b1.tar", last modified: Thu Jul  6 09:51:29 2023, max compression
```

## Comparing `caep-0.1.9.tar` & `caep-1.0.0b1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.9/LICENSE
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-06-08 06:03:50.793479 caep-0.1.9/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.9/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/caep/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.9/caep/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8348 2023-06-08 06:03:48.000000 caep-0.1.9/caep/config.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.9/caep/example.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1875 2023-06-08 06:03:48.000000 caep-0.1.9/caep/helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2023-01-02 09:23:36.000000 caep-0.1.9/caep/py.typed
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.9/caep/schema.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.9/caep/xdg.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/caep.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      357 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.9/caep.egg-info/zip-safe
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-06-08 06:03:50.793479 caep-0.1.9/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      994 2023-06-08 06:03:48.000000 caep-0.1.9/setup.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/tests/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.9/tests/test_config.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2217 2023-06-08 06:03:48.000000 caep-0.1.9/tests/test_helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    10271 2023-04-21 06:55:27.000000 caep-0.1.9/tests/test_schema.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-07-06 09:51:29.825722 caep-1.0.0b1/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-1.0.0b1/LICENSE
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9650 2023-07-06 09:51:29.825722 caep-1.0.0b1/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9179 2023-07-06 09:51:26.000000 caep-1.0.0b1/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-07-06 09:51:29.825722 caep-1.0.0b1/caep/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-1.0.0b1/caep/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8348 2023-06-08 06:03:48.000000 caep-1.0.0b1/caep/config.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-1.0.0b1/caep/example.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1875 2023-06-08 06:03:48.000000 caep-1.0.0b1/caep/helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2023-01-02 09:23:36.000000 caep-1.0.0b1/caep/py.typed
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    12002 2023-07-06 09:51:26.000000 caep-1.0.0b1/caep/schema.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-1.0.0b1/caep/xdg.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-07-06 09:51:29.825722 caep-1.0.0b1/caep.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9650 2023-07-06 09:51:29.000000 caep-1.0.0b1/caep.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      357 2023-07-06 09:51:29.000000 caep-1.0.0b1/caep.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-07-06 09:51:29.000000 caep-1.0.0b1/caep.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       28 2023-07-06 09:51:29.000000 caep-1.0.0b1/caep.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-07-06 09:51:29.000000 caep-1.0.0b1/caep.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-1.0.0b1/caep.egg-info/zip-safe
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-07-06 09:51:29.825722 caep-1.0.0b1/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1079 2023-07-06 09:51:26.000000 caep-1.0.0b1/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-07-06 09:51:29.825722 caep-1.0.0b1/tests/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-1.0.0b1/tests/test_config.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2239 2023-07-06 09:51:26.000000 caep-1.0.0b1/tests/test_helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    10271 2023-07-06 09:46:04.000000 caep-1.0.0b1/tests/test_schema.py
```

### Comparing `caep-0.1.9/LICENSE` & `caep-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `caep-0.1.9/PKG-INFO` & `caep-1.0.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.9
+Version: 1.0.0b1
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # CAEP
 
 Configuration library that supports loading configuration from ini, environment variables
 and arguments into a [pydantic](https://docs.pydantic.dev/) schema.
 
@@ -268,15 +269,15 @@
 
 ```python
 class ExampleConfig(BaseModel):
     username: Optional[str] = Field(description="Username")
     password: Optional[str] = Field(description="Password")
     parent_id: Optional[str] = Field(description="Parent ID")
 
-    @root_validator
+    @root_validator(skip_on_failure=True)
     def check_arguments(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """If one argument is set, they should all be set"""
 
         raise_if_some_and_not_all(
             values, ["username", "password", "parent_id"]
         )
```

### Comparing `caep-0.1.9/README.md` & `caep-1.0.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
 ```python
 class ExampleConfig(BaseModel):
     username: Optional[str] = Field(description="Username")
     password: Optional[str] = Field(description="Password")
     parent_id: Optional[str] = Field(description="Parent ID")
 
-    @root_validator
+    @root_validator(skip_on_failure=True)
     def check_arguments(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """If one argument is set, they should all be set"""
 
         raise_if_some_and_not_all(
             values, ["username", "password", "parent_id"]
         )
```

### Comparing `caep-0.1.9/caep/config.py` & `caep-1.0.0b1/caep/config.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.9/caep/example.py` & `caep-1.0.0b1/caep/example.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.9/caep/helpers.py` & `caep-1.0.0b1/caep/helpers.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.9/caep/schema.py` & `caep-1.0.0b1/caep/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 
 import argparse
 import re
 import sys
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, cast
 
+import pydantic
 from pydantic import BaseModel, ValidationError
 
 import caep
 
+PYDANTIC_MAJOR_VERSION = pydantic.__version__.split(".")[0]
+
 DEFAULT_SPLIT = ","
 
 DEFAULT_KV_SPLIT = ":"
 
 # Map of pydantic schema types to python types
 TYPE_MAPPING: Dict[str, type] = {
     "string": str,
@@ -81,15 +84,14 @@
 
     if value is None or not value.strip():
         d = {}
 
     else:
         # Split on specified field, unless they are escaped
         for items in escape_split(value, dict_info.split):
-
             try:
                 # Split key val on first occurence of specified split value
                 key, val = escape_split(items, dict_info.kv_split, maxsplit=2)
             except ValueError:
                 raise FieldError(f"Unable to split {items} by `{dict_info.kv_split}`")
 
             d[key.strip()] = dict_info.dict_type(val.strip())
@@ -138,15 +140,14 @@
                                        and ArrayInfo (type + split) as value
         dicts: dict[str, ArrayInfo] -  Dictionary with field name as key
                                        and DictInfo (type + split/kv_split) as value
     """
     args_with_list_split = {}
 
     for field, value in vars(args).items():
-
         if field in arrays:
             value = split_list(value, arrays[field], field)
 
         elif field in dicts:
             value = split_dict(value, dicts[field], field)
 
         args_with_list_split[field] = value
@@ -226,14 +227,34 @@
     # Loop over all pydantic schema fields
     for field, schema in fields.items():
         # for lists, dicts and sets we will use the default (str), but
         # for other types we will raise an error if field_type is not specified
         field_type: type = str
         default = schema.get("default")
 
+        # In pydantic 2.0+ some fields are represented with anyOf, like this:
+        #
+        # "path": {
+        #     "anyOf": [
+        #         {
+        #             "format": "path",
+        #             "type": "string"
+        #         },
+        #         {
+        #             "type": "null"
+        #         }
+        #     ],
+        #     "description": "Path",
+        #     "title": "Path"
+        #
+
+        for types in schema.get("anyOf", []):
+            if types.get("type") != "null":
+                schema.update(**types)
+
         if "type" not in schema:
             raise FieldError(
                 "No type specified, recursive models are not supported: "
                 f"{field}: {schema}"
             )
 
         if schema["type"] == "array":
@@ -266,15 +287,14 @@
                 dict_type=dict_type,
                 split=schema.get("split", DEFAULT_SPLIT),
                 kv_split=schema.get("kv_split", DEFAULT_KV_SPLIT),
                 min_size=schema.get("min_size", 0),
             )
 
         else:
-
             if schema["type"] not in TYPE_MAPPING:
                 raise FieldError(
                     f"Unsupported pydantic type for field {field}: {schema}"
                 )
 
             field_type = TYPE_MAPPING[schema["type"]]
 
@@ -314,15 +334,14 @@
     section_name: Optional[str] = None,
     alias: bool = False,
     opts: Optional[List[str]] = None,
     raise_on_validation_error: bool = False,
     exit_on_validation_error: bool = True,
     epilog: Optional[str] = None,
 ) -> BaseModelType:
-
     """
 
     Load ceap config as derived from pydantic model
 
     Arguments:
 
         model: BaseModelType            - Pydantic Model
@@ -338,15 +357,21 @@
         epilog: str                     - Add epilog text to --help output
 
     Returns parsed model
 
     """
 
     # Get all pydantic fields
-    fields = model.schema(alias).get("properties")
+    # In pydantix 1.x we use the `schema()` method, but this is replaced with
+    # `model_json_schema` in pydantic 2.x.
+
+    if PYDANTIC_MAJOR_VERSION == "2":
+        fields = model.model_json_schema(alias).get("properties")  # type: ignore
+    else:
+        fields = model.schema(alias).get("properties")
 
     if not fields:
         raise SchemaError(f"Unable to get properties from schema {model}")
 
     # Build argument parser based on pydantic fields
     parser, arrays, dicts = build_parser(fields, description, epilog)
 
@@ -355,15 +380,15 @@
             parser, config_id, config_file_name, section_name, opts=opts
         ),
         arrays=arrays,
         dicts=dicts,
     )
 
     try:
-        return model(**args)
+        return cast(BaseModelType, model(**args))  # type: ignore
     except ValidationError as e:
         if raise_on_validation_error:
             raise
         else:
             # ValidationError(model='Arguments',
             #                  errors=[{'loc': ('str_arg',),
             #                          'msg': 'none is not an allowed value',
```

### Comparing `caep-0.1.9/caep/xdg.py` & `caep-1.0.0b1/caep/xdg.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.9/caep.egg-info/PKG-INFO` & `caep-1.0.0b1/caep.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.9
+Version: 1.0.0b1
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # CAEP
 
 Configuration library that supports loading configuration from ini, environment variables
 and arguments into a [pydantic](https://docs.pydantic.dev/) schema.
 
@@ -268,15 +269,15 @@
 
 ```python
 class ExampleConfig(BaseModel):
     username: Optional[str] = Field(description="Username")
     password: Optional[str] = Field(description="Password")
     parent_id: Optional[str] = Field(description="Parent ID")
 
-    @root_validator
+    @root_validator(skip_on_failure=True)
     def check_arguments(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """If one argument is set, they should all be set"""
 
         raise_if_some_and_not_all(
             values, ["username", "password", "parent_id"]
         )
```

### Comparing `caep-0.1.9/setup.py` & `caep-1.0.0b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,35 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "rb") as f:
     long_description = f.read().decode("utf-8")
 
 setup(
     name="caep",
-    version="0.1.9",
+    version="1.0.0b1",
     author="mnemonic AS",
     zip_safe=True,
     author_email="opensource@mnemonic.no",
     description="Config Argument Env Parser (CAEP)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="ISC",
     keywords="mnemonic",
     packages=["caep"],
     url="https://github.com/mnemonic-no/caep",
     python_requires=">=3.6, <4",
     package_data={"caep": ["py.typed"]},
     install_requires=[
-        "pydantic>=1.8.0,<2.0.0",
+        "pydantic",
     ],
+    extras_require={
+        "dev": [
+            "mypy",
+            "pytest",
+        ]
+    },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Topic :: Utilities",
         "License :: OSI Approved :: ISC License (ISCL)",
     ],
 )
```

### Comparing `caep-0.1.9/tests/test_config.py` & `caep-1.0.0b1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.9/tests/test_helpers.py` & `caep-1.0.0b1/tests/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class ExampleConfig(BaseModel):
     username: Optional[str] = Field(description="Username")
     password: Optional[str] = Field(description="Password")
     parent_id: Optional[str] = Field(description="Parent ID")
 
-    @root_validator
+    @root_validator(skip_on_failure=True)
     def check_arguments(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """If one argument is set, they should all be set"""
 
         caep.raise_if_some_and_not_all(values, ["username", "password", "parent_id"])
 
         return values
```

### Comparing `caep-0.1.9/tests/test_schema.py` & `caep-1.0.0b1/tests/test_schema.py`

 * *Files identical despite different names*

