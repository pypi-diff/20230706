# Comparing `tmp/powertools_oas_validator-0.5.5.tar.gz` & `tmp/powertools_oas_validator-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.5.5.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.5.6.tar", max compression
```

## Comparing `powertools_oas_validator-0.5.5.tar` & `powertools_oas_validator-0.5.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/LICENSE
--rw-r--r--   0        0        0     2375 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/README.md
--rw-r--r--   0        0        0       13 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      252 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0     1031 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     4861 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/services/error_handler.py
--rw-r--r--   0        0        0     3196 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     1884 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1805 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      975 2023-07-05 05:07:13.746699 powertools_oas_validator-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.5/setup.py
--rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 04:57:04.206518 powertools_oas_validator-0.5.6/LICENSE
+-rw-r--r--   0        0        0     2375 2023-07-06 04:57:04.206518 powertools_oas_validator-0.5.6/README.md
+-rw-r--r--   0        0        0       13 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1031 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     4933 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/services/error_handler.py
+-rw-r--r--   0        0        0     3196 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     1884 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1909 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      975 2023-07-06 04:57:04.210518 powertools_oas_validator-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.6/setup.py
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.6/PKG-INFO
```

### Comparing `powertools_oas_validator-0.5.5/LICENSE` & `powertools_oas_validator-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/README.md` & `powertools_oas_validator-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/overrides/validators.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/services/error_handler.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/services/error_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from aws_lambda_powertools.utilities.validation.exceptions import SchemaValidationError
 from openapi_core.templating.security.exceptions import SecurityNotFound
 from openapi_core.validation.request.exceptions import ParameterValidationError
 from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
 
 from powertools_oas_validator.exceptions import UnhandledValidationError
-from powertools_oas_validator.types import Request
+from powertools_oas_validator.types import ParamError, Request
 
 
 class ErrorHandler:
     @staticmethod
     def raise_schema_validation_error(
         ex: Exception,
         request: Request,
@@ -75,44 +75,46 @@
     def _handle_body_error(
         ex: InvalidSchemaValue, request: Request
     ) -> SchemaValidationError:
         violating_req_params = []
 
         for error in ex.schema_errors:
             err_msg = str(error.message)  # type: ignore
-            if "required" in err_msg or "one of" in err_msg:
-                violating_req_params.append(
-                    (
-                        ErrorHandler._get_violating_param(err_msg),
-                        error.message,  # type: ignore
-                    )
-                )
+
+            violating_param = ErrorHandler._get_violating_param(err_msg)
+            if "required" in err_msg:
+                param = violating_param
             else:
-                raise ValueError(
-                    (
-                        "Unmapped error type. Consider adding case for"
-                        + f"'{ex.message}'"  # type: ignore
+                kv_swap = {v: k for k, v in ex.value.items()}  # type: ignore
+                param = kv_swap[violating_param]
+
+            violating_req_params.append(
+                (
+                    ParamError(
+                        param=param,
+                        validation_message=err_msg,
+                        value=violating_param,
                     )
                 )
-
+            )
         try:
             name = ErrorHandler._get_name(
-                request, "requestBody", violating_req_params[0][0]
+                request, "requestBody", violating_req_params[0].param
             )
             path = ErrorHandler._get_path(name)
 
         except KeyError:
             name = ErrorHandler._get_name(request, "request_body", "")
             path = ErrorHandler._get_path("")
 
         validation_message = ""
 
         if violating_req_params:
             try:
-                validation_message = violating_req_params[0][1]
+                validation_message = violating_req_params[0].validation_message
             except KeyError:
                 ...
 
         return SchemaValidationError(
             message=None,
             validation_message=validation_message,
             name=name,
```

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.5/powertools_oas_validator/types.py` & `powertools_oas_validator-0.5.6/powertools_oas_validator/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,21 @@
     minor: int
     pico: int
 
     def __str__(self) -> str:
         return f"{self.major}.{self.minor}.{self.pico}"
 
 
+@dataclass
+class ParamError:
+    param: str = ""
+    validation_message: str = ""
+    value: str = ""
+
+
 class Request(CoreRequest):
     def __init__(
         self,
         host_url: str,
         path: str,
         full_url_pattern: str,
         method: str,
```

### Comparing `powertools_oas_validator-0.5.5/pyproject.toml` & `powertools_oas_validator-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.5.5"
+version = "0.5.6"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 homepage = "https://github.com/RasmusFangel/powertools-oas-validator"
 repository = "https://github.com/RasmusFangel/powertools-oas-validator"
```

### Comparing `powertools_oas_validator-0.5.5/setup.py` & `powertools_oas_validator-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.5.5',
+    'version': '0.5.6',
     'description': '',
     'long_description': '# powertools-oas-validator\n<br><a href="https://badge.fury.io/py/powertools-oas-validator"><img src="https://badge.fury.io/py/powertools-oas-validator.svg" alt="PyPI version"></a>  ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg) <img src="https://coveralls.io/repos/RasmusFangel/powertools-oas-validator/badge.svg?branch=main" alt="Coveralls"></a>\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Installation\nPoetry:\n`poetry add powertools-oas-validator`\n\nPip:\n`pip install powertools-oas-validator`\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have a nice validation message, in case you rely on piping it straight back to the client.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/RasmusFangel/powertools-oas-validator',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['powertools_oas_validator', 'powertools_oas_validator.overrides',
 'powertools_oas_validator.services'] package_data = \ {'': ['*']}
 install_requires = \ ['aws-lambda-powertools>=2.18.0,<3.0.0',
 'fastjsonschema>=2.17.1,<3.0.0', 'jmespath>=1.0.1,<2.0.0', 'openapi-
 core>=0.17.2,<0.18.0'] setup_kwargs = { 'name': 'powertools-oas-validator',
-'version': '0.5.5', 'description': '', 'long_description': '# powertools-oas-
+'version': '0.5.6', 'description': '', 'long_description': '# powertools-oas-
 validator\n
 [PyPI_version] ![CI](https://github.com/RasmusFangel/powertools-oas-validator/
 workflows/CI/badge.svg) [Coveralls]
 \n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/
 aws-powertools/powertools-lambda-python) is an awesome set of tools for
 supercharging your lambdas. Powertools supports validating incoming requests
 (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is
```

### Comparing `powertools_oas_validator-0.5.5/PKG-INFO` & `powertools_oas_validator-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.5.5
+Version: 0.5.6
 Summary: 
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powertools-oas-validator Version: 0.5.5 Summary:
+Metadata-Version: 2.1 Name: powertools-oas-validator Version: 0.5.6 Summary:
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator License:
 MIT Author: Rasmus Hansen Author-email: R.FangelHansen@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-lambda-powertools (>=2.18.0,<3.0.0) Requires-Dist:
 fastjsonschema (>=2.17.1,<3.0.0) Requires-Dist: jmespath (>=1.0.1,<2.0.0)
```

