# Comparing `tmp/powertools_oas_validator-0.5.7.tar.gz` & `tmp/powertools_oas_validator-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.5.7.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.5.8.tar", max compression
```

## Comparing `powertools_oas_validator-0.5.7.tar` & `powertools_oas_validator-0.5.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-07-06 05:03:57.604734 powertools_oas_validator-0.5.7/LICENSE
--rw-r--r--   0        0        0     2714 2023-07-06 05:03:57.604734 powertools_oas_validator-0.5.7/README.md
--rw-r--r--   0        0        0       13 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      252 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0     1031 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     4933 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/services/error_handler.py
--rw-r--r--   0        0        0     3196 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     1884 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1909 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      975 2023-07-06 05:03:57.608734 powertools_oas_validator-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.7/setup.py
--rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/LICENSE
+-rw-r--r--   0        0        0     2666 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/README.md
+-rw-r--r--   0        0        0       13 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1031 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     4933 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/error_handler.py
+-rw-r--r--   0        0        0     3196 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     1884 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1909 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      975 2023-07-06 05:10:35.157031 powertools_oas_validator-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.8/setup.py
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.8/PKG-INFO
```

### Comparing `powertools_oas_validator-0.5.7/LICENSE` & `powertools_oas_validator-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/README.md` & `powertools_oas_validator-0.5.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,12 +57,12 @@
 )
 ```
 
 ## Know Issues
 While all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`
 (same as the Powertools validator would), with as much of the optional attributes as possible.
 
-In summary, it is possible that not all `SchemaValidationErrors`'s will have a nice validation message, in case you rely on piping it straight back to the client.
+In summary, it is possible that not all `SchemaValidationErrors`'s will have the correct name and path attributes.
 
 
 ## Contributions
 Please make a pull request and I will review it ASAP.
```

#### html2text {}

```diff
@@ -25,10 +25,10 @@
 SchemaValidationError SchemaValidatonError( name="test-path.test-
 endpoint.requestBody[param_1]", path=["test-path", "test-endpoint",
 "requestBody", "param_1"], validation_message="'not an integer' is not of type
 'integer'" ) ``` ## Know Issues While all validation errors are caught, there
 is only limited information about the various errors. The decorator will try
 its best to throw a `SchemaValidatonError` (same as the Powertools validator
 would), with as much of the optional attributes as possible. In summary, it is
-possible that not all `SchemaValidationErrors`'s will have a nice validation
-message, in case you rely on piping it straight back to the client. ##
-Contributions Please make a pull request and I will review it ASAP.
+possible that not all `SchemaValidationErrors`'s will have the correct name and
+path attributes. ## Contributions Please make a pull request and I will review
+it ASAP.
```

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/overrides/validators.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/services/error_handler.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/services/error_handler.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/powertools_oas_validator/types.py` & `powertools_oas_validator-0.5.8/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.7/pyproject.toml` & `powertools_oas_validator-0.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.5.7"
+version = "0.5.8"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 homepage = "https://github.com/RasmusFangel/powertools-oas-validator"
 repository = "https://github.com/RasmusFangel/powertools-oas-validator"
```

### Comparing `powertools_oas_validator-0.5.7/setup.py` & `powertools_oas_validator-0.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.5.7',
+    'version': '0.5.8',
     'description': '',
-    'long_description': '# powertools-oas-validator\n<br><a href="https://badge.fury.io/py/powertools-oas-validator"><img src="https://badge.fury.io/py/powertools-oas-validator.svg" alt="PyPI version"></a>  ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg) <img src="https://coveralls.io/repos/RasmusFangel/powertools-oas-validator/badge.svg?branch=main" alt="Coveralls"></a>\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Installation\nPoetry:\n`poetry add powertools-oas-validator`\n\nPip:\n`pip install powertools-oas-validator`\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\nExample of a `SchemaValidatonError`:\n```python\nfrom aws_lambda_powertools.utilities.validation import SchemaValidationError\n\nSchemaValidatonError(\n  name="test-path.test-endpoint.requestBody[param_1]",\n  path=["test-path", "test-endpoint", "requestBody", "param_1"],\n  validation_message="\'not an integer\' is not of type \'integer\'"\n)\n```\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have a nice validation message, in case you rely on piping it straight back to the client.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
+    'long_description': '# powertools-oas-validator\n<br><a href="https://badge.fury.io/py/powertools-oas-validator"><img src="https://badge.fury.io/py/powertools-oas-validator.svg" alt="PyPI version"></a>  ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg) <img src="https://coveralls.io/repos/RasmusFangel/powertools-oas-validator/badge.svg?branch=main" alt="Coveralls"></a>\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Installation\nPoetry:\n`poetry add powertools-oas-validator`\n\nPip:\n`pip install powertools-oas-validator`\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\nExample of a `SchemaValidatonError`:\n```python\nfrom aws_lambda_powertools.utilities.validation import SchemaValidationError\n\nSchemaValidatonError(\n  name="test-path.test-endpoint.requestBody[param_1]",\n  path=["test-path", "test-endpoint", "requestBody", "param_1"],\n  validation_message="\'not an integer\' is not of type \'integer\'"\n)\n```\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have the correct name and path attributes.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/RasmusFangel/powertools-oas-validator',
     'packages': packages,
     'package_data': package_data,
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
-'version': '0.5.7', 'description': '', 'long_description': '# powertools-oas-
+'version': '0.5.8', 'description': '', 'long_description': '# powertools-oas-
 validator\n
 [PyPI_version] ![CI](https://github.com/RasmusFangel/powertools-oas-validator/
 workflows/CI/badge.svg) [Coveralls]
 \n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/
 aws-powertools/powertools-lambda-python) is an awesome set of tools for
 supercharging your lambdas. Powertools supports validating incoming requests
 (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is
@@ -35,15 +35,14 @@
 endpoint.requestBody[param_1]",\n path=["test-path", "test-endpoint",
 "requestBody", "param_1"],\n validation_message="\'not an integer\' is not of
 type \'integer\'"\n)\n```\n\n## Know Issues\nWhile all validation errors are
 caught, there is only limited information about the various errors. The
 decorator will try its best to throw a `SchemaValidatonError`\n(same as the
 Powertools validator would), with as much of the optional attributes as
 possible.\n\nIn summary, it is possible that not all
-`SchemaValidationErrors`\'s will have a nice validation message, in case you
-rely on piping it straight back to the client.\n\n\n## Contributions\nPlease
-make a pull request and I will review it ASAP.\n', 'author': 'Rasmus Hansen',
-'author_email': 'R.FangelHansen@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/RasmusFangel/powertools-
-oas-validator', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.10,<4.0', } setup
-(**setup_kwargs)
+`SchemaValidationErrors`\'s will have the correct name and path
+attributes.\n\n\n## Contributions\nPlease make a pull request and I will review
+it ASAP.\n', 'author': 'Rasmus Hansen', 'author_email':
+'R.FangelHansen@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
+'url': 'https://github.com/RasmusFangel/powertools-oas-validator', 'packages':
+packages, 'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `powertools_oas_validator-0.5.7/PKG-INFO` & `powertools_oas_validator-0.5.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.5.7
+Version: 0.5.8
 Summary: 
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -78,13 +78,13 @@
 )
 ```
 
 ## Know Issues
 While all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`
 (same as the Powertools validator would), with as much of the optional attributes as possible.
 
-In summary, it is possible that not all `SchemaValidationErrors`'s will have a nice validation message, in case you rely on piping it straight back to the client.
+In summary, it is possible that not all `SchemaValidationErrors`'s will have the correct name and path attributes.
 
 
 ## Contributions
 Please make a pull request and I will review it ASAP.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powertools-oas-validator Version: 0.5.7 Summary:
+Metadata-Version: 2.1 Name: powertools-oas-validator Version: 0.5.8 Summary:
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator License:
 MIT Author: Rasmus Hansen Author-email: R.FangelHansen@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-lambda-powertools (>=2.18.0,<3.0.0) Requires-Dist:
 fastjsonschema (>=2.17.1,<3.0.0) Requires-Dist: jmespath (>=1.0.1,<2.0.0)
@@ -36,10 +36,10 @@
 SchemaValidationError SchemaValidatonError( name="test-path.test-
 endpoint.requestBody[param_1]", path=["test-path", "test-endpoint",
 "requestBody", "param_1"], validation_message="'not an integer' is not of type
 'integer'" ) ``` ## Know Issues While all validation errors are caught, there
 is only limited information about the various errors. The decorator will try
 its best to throw a `SchemaValidatonError` (same as the Powertools validator
 would), with as much of the optional attributes as possible. In summary, it is
-possible that not all `SchemaValidationErrors`'s will have a nice validation
-message, in case you rely on piping it straight back to the client. ##
-Contributions Please make a pull request and I will review it ASAP.
+possible that not all `SchemaValidationErrors`'s will have the correct name and
+path attributes. ## Contributions Please make a pull request and I will review
+it ASAP.
```

