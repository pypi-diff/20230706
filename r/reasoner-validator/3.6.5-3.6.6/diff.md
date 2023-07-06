# Comparing `tmp/reasoner_validator-3.6.5.tar.gz` & `tmp/reasoner_validator-3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.6.5.tar", max compression
+gzip compressed data, was "reasoner_validator-3.6.6.tar", max compression
```

## Comparing `reasoner_validator-3.6.5.tar` & `reasoner_validator-3.6.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/LICENSE
--rw-r--r--   0        0        0    12620 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/README.md
--rw-r--r--   0        0        0      131 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/conf.py
--rw-r--r--   0        0        0    19640 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-04 00:47:05.182017 reasoner_validator-3.6.5/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    35958 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2092 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/pyproject.toml
--rw-r--r--   0        0        0    38413 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    63014 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39199 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    28625 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4592 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    10750 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14019 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    10707 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      410 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:47:05.186017 reasoner_validator-3.6.5/tests/conftest.py
--rw-r--r--   0        0        0   114356 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62106 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    38591 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_response_validator.py
--rw-r--r--   0        0        0     5528 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_semver.py
--rw-r--r--   0        0        0     1913 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26525 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_validate.py
--rw-r--r--   0        0        0    20333 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-04 00:47:05.190017 reasoner_validator-3.6.5/tests/test_workflows.py
--rw-r--r--   0        0        0    14658 1970-01-01 00:00:00.000000 reasoner_validator-3.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/LICENSE
+-rw-r--r--   0        0        0    12620 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/README.md
+-rw-r--r--   0        0        0      131 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/conf.py
+-rw-r--r--   0        0        0    19640 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    35958 2023-07-06 07:30:20.170284 reasoner_validator-3.6.6/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2094 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/pyproject.toml
+-rw-r--r--   0        0        0    38154 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    63014 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39199 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    28625 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    11484 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14019 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    11621 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      709 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 07:30:20.174285 reasoner_validator-3.6.6/tests/conftest.py
+-rw-r--r--   0        0        0   114459 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62106 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    38058 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_response_validator.py
+-rw-r--r--   0        0        0     5997 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_semver.py
+-rw-r--r--   0        0        0     2209 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26558 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_validate.py
+-rw-r--r--   0        0        0    20333 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-06 07:30:20.178285 reasoner_validator-3.6.6/tests/test_workflows.py
+-rw-r--r--   0        0        0    14660 1970-01-01 00:00:00.000000 reasoner_validator-3.6.6/PKG-INFO
```

### Comparing `reasoner_validator-3.6.5/LICENSE` & `reasoner_validator-3.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/README.md` & `reasoner_validator-3.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
 ### API
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
-  "trapi_version": "1.4.0",
+  "trapi_version": "1.4.1",
   "biolink_version": "3.5.0",
   "sources": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
@@ -180,15 +180,15 @@
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
-  "trapi_version": "1.4.0",
+  "trapi_version": "1.4.1",
   "biolink_version": "3.5.0",
   "response": {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
@@ -223,15 +223,15 @@
 }
 ```
 
 one should typically get a response body something like the following JSON validation result back:
 
 ```json
 {
-  "trapi_version": "1.4.0",
+  "trapi_version": "1.4.1",
   "biolink_version": "3.2.1",
   "messages": {
     # some categories of messages may be absent, hence, empty dictionaries
     "critical": {},
     "errors": {
       "error.knowledge_graph.node.category.missing": {
           # this message template does not have any additional parameters
```

### Comparing `reasoner_validator-3.6.5/docs/Makefile` & `reasoner_validator-3.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/docs/conf.py` & `reasoner_validator-3.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/docs/index.rst` & `reasoner_validator-3.6.6/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 }
             }
         ]
     }
 
     }
     validator = TRAPIResponseValidator(
-        trapi_version="1.4.0",
+        trapi_version="1.4.1",
 
         # If omit or set the Biolink Model version parameter to None,
         # then the current Biolink Model Toolkit default release applies
         biolink_version="3.5.0",
 
         # 'sources' are set to trigger checking of expected edge knowledge source provenance
         sources={
@@ -249,15 +249,15 @@
         # If the TRAPI version is omitted or set to None, then the 'latest' TRAPI version is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'schema_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the following trapi_version parameter is given, then it overrides the TRAPI Response 'schema_version';
         # Otherwise, the TRAPI Response 'schema_version' (not 'latest') becomes the default validation version.
 
-        trapi_version="1.4.0",
+        trapi_version="1.4.1",
 
         # If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'biolink_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the 'biolink_version' given here is assumed, which overrides the TRAPI Response stated 'biolink_version';
         # Otherwise, the TRAPI Response stated 'biolink_version' (not BMT) becomes the default validation version.
@@ -304,15 +304,15 @@
 --------------
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data as input to the **/validate** endpoint:
 
 .. code-block:: json
 
     {
-        "schema_version": "1.4.0",
+        "schema_version": "1.4.1",
         "biolink_version": "3.5.0",
         "message": {
             "query_graph": {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {"categories": ["biolink:Drug"]}
                 },
@@ -368,15 +368,15 @@
     }
 
 then, one should typically get a response body like the following JSON validation result back:
 
 .. code-block:: json
 
     {
-      "trapi_version": "1.4.0",
+      "trapi_version": "1.4.1",
       "biolink_version": "3.4.3",
       "messages": {
         "critical": {},
         "errors": {
           "error.knowledge_graph.node.category.missing": {
             "MONDO:0005148": [
               {
```

### Comparing `reasoner_validator-3.6.5/docs/make.bat` & `reasoner_validator-3.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/docs/validation_codes_dictionary.md` & `reasoner_validator-3.6.6/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/pyproject.toml` & `reasoner_validator-3.6.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.6.5"
+version = "3.6.6"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -41,15 +41,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bmt = "^1.1.0"
 jsonschema = "^4.17.0"
 PyYAML = "^6.0"
 requests = "^2.28.1"
-pydantic = "^1.8.0"
+pydantic = "^1.10.11"
 urllib3 = "^1.26.15"
 numpydoc = {version = "^1.5.0", optional = true}
 sphinx = {version = "^5.3.0", optional = true}
 myst-parser = {version = "^0.18.1", optional = true}
 fastapi = {version = "^0.68", optional = true}
 uvicorn = {version = "^0.15", optional = true}
 pytest-cov = {version = "^4.0.0", optional = true}
```

### Comparing `reasoner_validator-3.6.5/reasoner_validator/__init__.py` & `reasoner_validator-3.6.6/reasoner_validator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,26 @@
     BiolinkValidator,
     get_biolink_model_toolkit,
     TRAPIGraphType
 )
 
 # Maximum number of data points to scrutinize
 # in various parts TRAPI Query Response.Message
-from reasoner_validator.trapi import check_trapi_validity, TRAPISchemaValidator
+from reasoner_validator.trapi import (
+    TRAPI_1_3_0_SEMVER,
+    TRAPI_1_4_0_SEMVER,
+    TRAPI_1_4_1_SEMVER,
+    TRAPI_1_4_0_BETA3_SEMVER,
+    TRAPI_1_4_0_BETA4_SEMVER,
+    LATEST_TRAPI_MAJOR_RELEASE_SEMVER,
+    LATEST_TRAPI_RELEASE_SEMVER,
+    LATEST_TRAPI_RELEASE,
+    check_trapi_validity,
+    TRAPISchemaValidator
+)
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
 from reasoner_validator.versioning import SemVer, SemVerError
 from reasoner_validator.sri.util import get_aliases
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -27,20 +38,14 @@
 
 
 class TRAPIResponseValidator(ValidationReporter):
     """
     TRAPI Validator is an overall wrapper class for validating
     conformance of TRAPI Responses to TRAPI and the Biolink Model.
     """
-
-    TRAPI_1_3_0 = SemVer.from_string("1.3.0")
-    TRAPI_1_4_0 = SemVer.from_string("1.4.0")
-    TRAPI_1_4_0_BETA3 = SemVer.from_string("1.4.0-beta3")
-    TRAPI_1_4_0_BETA4 = SemVer.from_string("1.4.0-beta4")
-
     def __init__(
             self,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
             sources: Optional[Dict] = None,
             strict_validation: bool = False,
             suppress_empty_data_warnings: bool = False
@@ -63,44 +68,56 @@
             self,
             prefix="Validate TRAPI Response",
             trapi_version=trapi_version,
             biolink_version=biolink_version,
             sources=sources,
             strict_validation=strict_validation
         )
-        self.suppress_empty_data_warnings = suppress_empty_data_warnings
+        self._is_trapi_1_4: Optional[bool] = None
+        self.suppress_empty_data_warnings: bool = suppress_empty_data_warnings
+
+    def is_trapi_1_4(self) -> bool:
+        assert self.trapi_version
+        try:  # try block ... Sanity check: in case the trapi_version is somehow invalid?
+            target_major_version: SemVer = SemVer.from_string(self.trapi_version, core_fields=['major', 'minor'])
+            self._is_trapi_1_4 = target_major_version >= LATEST_TRAPI_MAJOR_RELEASE_SEMVER
+        except SemVerError as sve:
+            logger.error(f"Current TRAPI release '{self.trapi_version}' seems invalid: {str(sve)}. Reset to latest?")
+            self.trapi_version = LATEST_TRAPI_RELEASE
+            self._is_trapi_1_4 = True
+        return self._is_trapi_1_4
 
     def sanitize_trapi_response(self, response: Dict) -> Dict:
         """
         Some component TRAPI Responses cannot be validated further due to missing tags and None values.
         This method is a temporary workaround to sanitize the query for additional validation.
 
         :param response: Dict full TRAPI Response JSON object
         :return: Dict, response with discretionary removal of content which
                        triggers (temporarily) unwarranted TRAPI validation failures
         """
         # Temporary workaround for "1.4.0-beta4" schema bugs
         current_version: SemVer = SemVer.from_string(self.trapi_version)
         # the message is not empty
         if 'knowledge_graph' in response['message'] and response['message']['knowledge_graph'] is not None and \
-                self.TRAPI_1_4_0_BETA4 >= current_version != self.TRAPI_1_3_0:
+                TRAPI_1_4_0_BETA4_SEMVER >= current_version != TRAPI_1_3_0_SEMVER:
             for key, edge in response['message']['knowledge_graph']['edges'].items():
                 edge_id = f"{str(edge['subject'])}--{str(edge['predicate'])}->{str(str(edge['object']))}"
                 if 'sources' not in edge or not edge['sources']:
                     self.report("error.knowledge_graph.edge.sources.missing", identifier=edge_id)
                     continue
                 for source in edge['sources']:
                     if 'source_record_urls' not in source or source['source_record_urls'] is None:
                         source['source_record_urls'] = list()
                     if 'upstream_resource_ids' not in source or source['upstream_resource_ids'] is None:
                         source['upstream_resource_ids'] = list()
 
         # 'auxiliary_graphs' (introduced the TRAPI 1.4.0-beta3 pre-releases,
-        # full updated in the full 1.4.0 release) ought to be nullable
-        if self.TRAPI_1_4_0_BETA4 >= current_version >= self.TRAPI_1_4_0_BETA3 and \
+        # full fixed in the 1.4.1 release) ought to be nullable.
+        if TRAPI_1_4_0_SEMVER >= current_version >= TRAPI_1_4_0_BETA3_SEMVER and \
                 ('auxiliary_graphs' not in response['message'] or response['message']['auxiliary_graphs'] is None):
             response['message']['auxiliary_graphs'] = dict()
 
         if 'workflow' in response and response['workflow']:
             # a 'workflow' is a list of steps, which are JSON object specifications
             workflow_steps: List[Dict] = response['workflow']
             for step in workflow_steps:
@@ -375,23 +392,14 @@
         """
 
         #     :param output_element: test target, as edge 'subject' or 'object'
         #     :type output_element: str
         #     :param output_node_binding: node 'a' or 'b' of the ('one hop') QGraph test query
         #     :type output_node_binding: str
 
-        trapi_1_4_0: bool
-        try:  # try block ... Sanity check: in case the trapi_version is somehow invalid?
-            target_version: SemVer = SemVer.from_string(self.trapi_version)
-            trapi_1_4_0 = target_version >= SemVer.from_string("1.4.0")
-        except SemVerError as sve:
-            logger.error(f"has_valid_results() 'self.trapi_version' seems invalid: {str(sve)}. Reset to latest?")
-            self.trapi_version = "1.4.0"
-            trapi_1_4_0 = True
-
         # The Message.Results key should not be missing?
         if 'results' not in message:
             if not self.suppress_empty_data_warnings:
                 self.report(code="error.trapi.response.results.missing")
         else:
             results = message['results']
 
@@ -419,15 +427,15 @@
                         trapi_version=self.trapi_version
                     )
                     if trapi_validator.has_messages():
                         # Record the error messages associated with the Result set then... don't continue
                         self.merge(trapi_validator)
 
                     # Maybe some additional TRAPI-release specific non-schematic validation here?
-                    if trapi_1_4_0:
+                    if self.is_trapi_1_4():
                         # TODO: implement me!
                         pass
                     else:
                         pass
 
                     # TODO: here, we could try to compare the Results against the contents of the KnowledgeGraph,
                     #       with respect to node input values from the QueryGraph, but this is tricky to do solely
@@ -529,24 +537,14 @@
         :param subject_id: str, subject node (CURIE) identifier
         :param object_id:  str, subject node (CURIE) identifier
         :param edge_id:  str, subject node (CURIE) identifier
         :param results: List of (TRAPI-version specific) Result objects
         :param trapi_version: str, target TRAPI version of the Response being validated
         :return: bool, True if case S-P-O edge was found in the results
         """
-        trapi_1_4_0: bool
-        try:
-            # try block ... Sanity check: in case the trapi_version is somehow invalid?
-            # ignore any prerelease/build qualifiers
-            target_version: SemVer = SemVer.from_string(trapi_version, ext_fields=[])
-            trapi_1_4_0 = target_version >= SemVer.from_string("1.4.0")
-        except SemVerError as sve:
-            logger.warning(f"case_result_found() 'trapi_version' seems invalid: {str(sve)}. Default to latest?")
-            trapi_1_4_0 = True
-
         result_found: bool = False
         result: Dict
 
         for result in results:
 
             # Node binding validation still currently same for recent TRAPI versions
             node_bindings: Dict = result["node_bindings"]
@@ -559,15 +557,15 @@
                         if subject_id == details["id"]:
                             subject_id_found = True
                         if object_id == details["id"]:
                             object_id_found = True
 
             # However, TRAPI 1.4.0 Message 'Results' 'edge_bindings' are reported differently
             #          from 1.3.0, rather, embedded in 'Analysis' objects (and 'Auxiliary Graphs')
-            if trapi_1_4_0:
+            if self.is_trapi_1_4():
                 #
                 #     "auxiliary_graphs": {
                 #         "a0": {
                 #             "edges": [
                 #                 "e02",
                 #                 "e12"
                 #             ]
```

### Comparing `reasoner_validator-3.6.5/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.6.6/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/reasoner_validator/codes.yaml` & `reasoner_validator-3.6.6/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/reasoner_validator/report.py` & `reasoner_validator-3.6.6/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/reasoner_validator/sri/util.py` & `reasoner_validator-3.6.6/reasoner_validator/sri/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,25 @@
                             #
                             # Decided that it was a bad idea to remove
                             # the original identifier from the aliases...
                             # aliases.remove(identifier)
                             #
                             # print(dumps(aliases, indent=2))
                         else:
-                            logging.warning(f"get_aliases(): missing the 'equivalent identifiers' for the '{identifier}' clique?")
+                            logging.warning(
+                                f"get_aliases(): missing the 'equivalent identifiers' for the '{identifier}' clique?"
+                            )
                     else:
-                        logging.warning(f"get_aliases(): missing the preferred 'id' for the '{identifier}' clique?")
+                        logging.warning(
+                            f"get_aliases(): missing the preferred 'id' for the '{identifier}' clique?"
+                        )
                 else:
-                    logging.warning(f"get_aliases(): '{identifier}' is a singleton in its clique thus has no aliases...")
+                    logging.warning(
+                        f"get_aliases(): '{identifier}' is a singleton in its clique thus has no aliases..."
+                    )
 
     if not aliases:
         # Logging various errors but always
         # return the identifier as its own alias
         aliases = [identifier]
 
     return aliases
```

### Comparing `reasoner_validator-3.6.5/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.6.6/reasoner_validator/trapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,35 @@
     GIT_ORG,
     GIT_REPO
 )
 
 import logging
 logger = logging.getLogger(__name__)
 
+TRAPI_1_3_0_SEMVER = SemVer.from_string("v1.3.0")
+TRAPI_1_3_0: str = str(TRAPI_1_3_0_SEMVER)
+
+TRAPI_1_4_0_SEMVER = SemVer.from_string("v1.4.0")
+TRAPI_1_4_0: str = str(TRAPI_1_4_0_SEMVER)
+# patch version to fix 'auxiliary_graphs' model in 1.4.0
+TRAPI_1_4_1_SEMVER = SemVer.from_string("v1.4.1")
+TRAPI_1_4_1: str = str(TRAPI_1_4_1_SEMVER)
+
+TRAPI_1_4_0_BETA_SEMVER = SemVer.from_string("v1.4.0-beta")
+TRAPI_1_4_0_BETA = str(TRAPI_1_4_0_BETA_SEMVER)
+
+TRAPI_1_4_0_BETA2_SEMVER = SemVer.from_string("v1.4.0-beta2")
+TRAPI_1_4_0_BETA3_SEMVER = SemVer.from_string("v1.4.0-beta3")
+TRAPI_1_4_0_BETA4_SEMVER = SemVer.from_string("v1.4.0-beta4")
+
+LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_4_1_SEMVER
+LATEST_TRAPI_RELEASE: str = str(LATEST_TRAPI_RELEASE_SEMVER)
+
+LATEST_TRAPI_MAJOR_RELEASE_SEMVER: SemVer = SemVer.from_string("v1.4", core_fields=['major', 'minor'])
+LATEST_TRAPI_MAJOR_RELEASE: str = str(LATEST_TRAPI_MAJOR_RELEASE_SEMVER)
 
 # For testing, set TRAPI API query POST timeouts to 10 minutes == 600 seconds
 DEFAULT_TRAPI_POST_TIMEOUT = 600.0
 
 
 class TRAPIAccessError(RuntimeError):
     pass
@@ -145,42 +166,36 @@
             key: schema.pop(key)
             for key in list(schema.keys())
         },
         {"type": "null"},
     ]
 
 
-TRAPI_1_4_0_BETA = SemVer.from_string("1.4.0-beta")
-TRAPI_1_4_0_BETA3 = SemVer.from_string("1.4.0-beta3")
-TRAPI_1_4_0_BETA4 = SemVer.from_string("1.4.0-beta4")
-TRAPI_1_4_0 = SemVer.from_string("1.4.0")
-
-
 def map_semver(version: str):
     mapped_semver: Optional[SemVer]
     try:
         mapped_semver = SemVer.from_string(version)
     except SemVerError as sve:
         # if we cannot map the version, then it may simply
         # be a non-versioned branch of the schemata
         logger.error(str(sve))
         mapped_semver = None
     return mapped_semver
 
 
 def patch_schema(tag: str, schema: Dict, version: str):
     # temporary patch for small TRAPI schema bugs
-    # TODO: fix TRAPI schemata to eliminate these
     mapped_semver: Optional[SemVer] = map_semver(version)
     if (
             mapped_semver and
-            (TRAPI_1_4_0 >= mapped_semver >= TRAPI_1_4_0_BETA3)
+            (TRAPI_1_4_0_SEMVER >= mapped_semver >= TRAPI_1_4_0_BETA3_SEMVER)
     ):
         if tag == "auxiliary_graphs" and "oneOf" in schema:
-            # TODO: very short term workaround for problematics 'auxiliary_graphs' value schema
+            # TODO: very short term workaround for problematic
+            #       TRAPI 1.4.0 'auxiliary_graphs' value schema
             schema["type"] = "object"
             value_types: List[str] = schema.pop("oneOf")
             schema["additionalProperties"] = value_types[0]
 
 
 def openapi_to_jsonschema(schema, version: str) -> None:
     """
@@ -191,15 +206,15 @@
     """
     mapped_semver: Optional[SemVer] = map_semver(version)
 
     # we'll only tweak mapped schemata and
     # such releases that are prior to TRAPI 1.4.0-beta
     if (
             mapped_semver and
-            not (TRAPI_1_4_0_BETA4 >= mapped_semver >= TRAPI_1_4_0_BETA)
+            not (TRAPI_1_4_0_BETA4_SEMVER >= mapped_semver >= TRAPI_1_4_0_BETA_SEMVER)
     ) and "allOf" in schema:
         # September 1, 2022 hacky patch to rewrite 'allOf'
         # tagged schemata, in TRAPI 1.3.0 or earlier, to 'oneOf'
         schema["oneOf"] = schema.pop("allOf")
 
     if schema.get("type", None) == "object":
         for tag, prop in schema.get("properties", dict()).items():
```

### Comparing `reasoner_validator-3.6.5/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.6.6/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/reasoner_validator/validation_codes.py` & `reasoner_validator-3.6.6/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/reasoner_validator/versioning.py` & `reasoner_validator-3.6.6/reasoner_validator/versioning.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utilities."""
-import re
 from typing import NamedTuple, Optional, List
+from sys import stderr
 from os import environ
-from re import sub
+from re import sub, compile
 import requests
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
 
 
@@ -23,15 +23,15 @@
 branch_data = response.json()
 branches = [
     branch["name"] for branch in branch_data
 ]
 
 # This is modified version of a standard SemVer regex which
 # takes into account the possibility of capturing a non-numeric prefix
-semver_pattern = re.compile(
+semver_pattern = compile(
     r"^(?P<prefix>[a-zA-Z]*)(?P<major>0|[1-9]\d*)(\.(?P<minor>0|[1-9]\d*)(\.(?P<patch>0|[1-9]\d*))?)?" +
     r"(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][\da-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][\da-zA-Z-]*))*))?"
     r"(?:\+(?P<buildmetadata>[\da-zA-Z-]+(?:\.[\da-zA-Z-]+)*))?$"
 )
 
 
 class SemVerError(Exception):
@@ -69,16 +69,20 @@
                               the SemVer string value, e.g. a Git Release 'v' character (i.e. v1.2.3); Default: False.
         :param core_fields: List[str], list of names of core SemVer field to explicitly set (may NOT be empty?)
                                        (default: ['major', 'minor', 'patch']).
         :param ext_fields: List[str], list of names of extended SemVer fields to explicitly set (maybe empty?)
                                       (default: ['prerelease', 'buildmetadata']).
         :return:
         """
+        # sanity check on required and allowed parameters
         assert string
+        # print(core_fields, file=stderr)
         assert len(core_fields) > 0 and all([field in ['major', 'minor', 'patch'] for field in core_fields])
+        assert len(core_fields) >= 1 and 'major' in core_fields
+        assert len(core_fields) >= 2 and 'major' in core_fields and 'minor' in core_fields
         assert all([field in ['prerelease', 'buildmetadata'] for field in ext_fields])
 
         # If the string is a file path, generically detected using the .yaml file extension,
         # then assume that the file path string encodes the SemVer string, as a part of the
         # root file name just before the .yaml file extension, e.g. my_schema_3.2.1-beta5.yaml
         if string.endswith(".yaml"):
             root_path: str = string.replace(".yaml", "")
@@ -90,22 +94,36 @@
 
         if match is None:
             raise SemVerError(f"'{string}' is not a valid release version")
 
         captured = match.groupdict()
         missing_fields_errmsg = f"SemVer '{string}' is missing expected fields: {', '.join(core_fields)}"
 
-        if not all([group in captured for group in core_fields]):
-            raise SemVerUnderspecified(missing_fields_errmsg)
-
+        observed_prefix = captured["prefix"] if not ignore_prefix else ""
+        core_field_values: List[int] = list()
+        for field in ['major', 'minor', 'patch']:
+            if field in core_fields:
+                if field in captured and captured[field] is not None:
+                    core_field_values.append(int(captured[field]))
+                else:
+                    raise SemVerUnderspecified(missing_fields_errmsg)
+            else:
+                core_field_values.append(0)
+
+        ext_field_values: List[Optional[str]] = list()
+        for field in ['prerelease', 'buildmetadata']:
+            if field in ext_fields and field in captured:
+                ext_field_values.append(captured[field])
+            else:
+                ext_field_values.append(None)
         try:
             return cls(
-                captured["prefix"] if not ignore_prefix else "",
-                *[int(captured[group]) for group in core_fields],
-                *[captured[group] for group in ext_fields],
+                observed_prefix,
+                *core_field_values,
+                *ext_field_values
             )
         except TypeError:
             raise SemVerUnderspecified(missing_fields_errmsg)
 
     def __str__(self):
         """Generate string."""
         value = f"{self.prefix}{self.major}"
@@ -179,30 +197,32 @@
     # Clearcut cases of 'major' release ordering
     if obj.major > other.major:
         return True
     elif obj.major < other.major:
         return False
 
     # obj.major == other.major
-    # Check 'minor' level
+
+    # Now check 'minor' level
     elif obj.minor > other.minor:
         return True
     elif obj.minor < other.minor:
         return False
 
     # obj.minor == other.minor
-    # Check 'patch' level
+
+    # Now check 'patch' level
     elif obj.patch > other.patch:
         return True
     elif obj.patch < other.patch:
         return False
 
     # obj.patch == other.patch
 
-    # Check 'prerelease' tagging
+    # Now check 'prerelease' tagging
     elif obj.prerelease and not other.prerelease:
         return False
     elif not obj.prerelease:
         return True
 
     # or compare two non-empty prerelease spec strings
     elif obj.prerelease >= other.prerelease:
@@ -236,28 +256,30 @@
 
 SemVer.__ge__ = _semver_ge_
 
 _latest = dict()
 
 
 # Provide an accessor function for retrieving the latest version in string format
-def get_latest_version(release_tag: str) -> Optional[str]:
+def get_latest_version(release_tag: Optional[str]) -> Optional[str]:
     """
     Return the latest TRAPI version corresponding to the release tag given.
     Note that if the release tag looks like a YAML file, then it is assumed
     to be a direct schema specification. If a Git branch name in the schema
     repository, the branch name is also passed on.
 
     :param release_tag: (possibly partial) SemVer string, Git branch name,
                         or YAML schema file name identifying a release.
     :return: 'best' latest release of SemVer specification or the YAML file directly returned.
     """
     global _latest
 
-    if release_tag.lower().endswith(".yaml"):
+    if not release_tag:
+        return None
+    elif release_tag.lower().endswith(".yaml"):
         return release_tag
     elif release_tag in branches:
         # cases in which a branch name is
         # given instead of a release number
         return release_tag
     else:
         # strip any prefix from the release tag to ensure that
```

### Comparing `reasoner_validator-3.6.5/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.6.6/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pprint import PrettyPrinter
 import logging
 import pytest
 from bmt import Toolkit
 from linkml_runtime.linkml_model import SlotDefinition
 
 from reasoner_validator import TRAPISchemaValidator
+from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_0_BETA
 from reasoner_validator.biolink import (
     TRAPIGraphType,
     BiolinkValidator,
     get_biolink_model_toolkit,
     check_biolink_model_compliance_of_input_edge,
     check_biolink_model_compliance_of_query_graph,
     check_biolink_model_compliance_of_knowledge_graph
@@ -987,15 +988,15 @@
             "error.knowledge_graph.edge.attribute.empty"
         ),
     ]
 )
 def test_pre_trapi_1_4_0_validate_missing_or_empty_attributes(query: Tuple):
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
-        trapi_version="1.3.0",
+        trapi_version=TRAPI_1_3_0,
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
         sources=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
@@ -1130,15 +1131,15 @@
         )
     ]
 )
 def test_pre_1_4_0_validate_provenance(query: Tuple):
     """TRAPI pre-1.4.0 releases recorded provenance in attributes. This unit test checks for this"""
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
-        trapi_version="1.3.0",
+        trapi_version=TRAPI_1_3_0,
         biolink_version=LATEST_BIOLINK_MODEL_VERSION,
         sources=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
@@ -1311,15 +1312,15 @@
     # TODO: to review: which of the validation tests that may be overridden by earlier TRAPI validation
     # Sanity check: does TRAPI validation catch this first?
     trapi_validator = TRAPISchemaValidator(trapi_version=trapi_version)
     # Wrap Qualifiers inside a small mock QEdge
     mock_edge: Dict = deepcopy(query[0])
     mock_edge["subject"] = "mock_subject"
 
-    if trapi_validator.minimum_required_trapi_version("1.4.0-beta"):
+    if trapi_validator.minimum_required_trapi_version(TRAPI_1_4_0_BETA):
         # not testing Edge semantics here but rather, the qualifiers,
         # but from 1.4.0-beta(2) onwards, we also need
         # a non-null predicate and the new 'sources' field here!
         mock_edge["predicate"] = "biolink:related_to"
         mock_edge["sources"] = [
             {
                 "resource_id": "infores:molepro",
@@ -1652,20 +1653,20 @@
 }
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (  # Query 0 - 'qualifier_type_id' value not a Biolink CURIE - seen as 'unknown' in TRAPI < 1.4.0-beta
-            "1.3.0",
+            TRAPI_1_3_0,
             QC_QS_NOT_A_CURIE,
             "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
         (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
-            "1.4.0-beta",
+            TRAPI_1_4_0_BETA,
             QC_QS_NOT_A_CURIE,
             "critical.trapi.validation"
         )
     ]
 )
 def test_validate_biolink_curie_in_qualifier_constraints(query: Tuple[str, Dict, str]):
     qualifier_validator(
@@ -1817,20 +1818,20 @@
 }
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (  # Query 0 - 'qualifier_type_id' value not a Biolink CURIE - seen as 'unknown' in TRAPI < 1.4.0-beta
-                "1.3.0",
+                TRAPI_1_3_0,
                 Q_NOT_A_CURIE,
                 "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
         (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
-                "1.4.0-beta",
+                TRAPI_1_4_0_BETA,
                 Q_NOT_A_CURIE,
                 "critical.trapi.validation"
         )
     ]
 )
 def test_validate_biolink_curie_in_qualifiers(query: Tuple[str, Dict, str]):
     qualifier_validator(
@@ -2840,26 +2841,26 @@
 
 
 def test_pre_trapi_1_4_0_validate_attributes():
     # message edges must have at least some 'provenance' attributes
     edge_without_attributes = deepcopy(MESSAGE_EDGE_WITHOUT_ATTRIBUTES)
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
         graph=edge_without_attributes,
-        trapi_version="1.3.0",
+        trapi_version=TRAPI_1_3_0,
         biolink_version=LATEST_BIOLINK_MODEL_VERSION
     )
     check_messages(validator, "error.knowledge_graph.edge.attribute.missing")
 
 
 def test_suppress_biolink_validation_pre_trapi_1_4_0_validate_attributes():
     # message edges must have at least some 'provenance' attributes
     edge_without_attributes = deepcopy(MESSAGE_EDGE_WITHOUT_ATTRIBUTES)
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
         graph=edge_without_attributes,
-        trapi_version="1.3.0",
+        trapi_version=TRAPI_1_3_0,
         biolink_version=SUPPRESS_BIOLINK_MODEL_VALIDATION
     )
     check_messages(validator, "")
 
 
 SAMPLE_RETRIEVAL_SOURCE = {
     # required, infores CURIE to an Information Resource
```

### Comparing `reasoner_validator-3.6.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.6.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/tests/test_response_validator.py` & `reasoner_validator-3.6.6/tests/test_response_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 from json import dump
 
 from copy import deepcopy
 
 import pytest
 
 from reasoner_validator import TRAPIResponseValidator
+from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_1
 
 from tests import PATCHED_140_SCHEMA_FILEPATH
 from tests.test_validation_report import check_messages
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
-PRE_TRAPI_1_4_0 = "1.3.0"
-TRAPI_1_4_0 = "1.4.0"
-
 _TEST_QG_1 = {
     "nodes": {
         "type-2 diabetes": {"ids": ["MONDO:0005148"]},
         "drug": {
             "categories": ["biolink:Drug"]
         }
     },
@@ -228,15 +226,15 @@
 
 _TEST_KG_4 = {
     'nodes': _TEST_NODES_1,
     'edges': _TEST_EDGES_4
 }
 
 # From Implementation Guidlines circa June 2023
-_TEST_TRAPI_1_4_0_FULL_SAMPLE = {
+_TEST_TRAPI_1_4_1_FULL_SAMPLE = {
     "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
             "edges": {
@@ -246,18 +244,25 @@
         },
         "knowledge_graph": {
             "nodes": {
                 "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
                 "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
             },
             "edges": {
-                "df87ff82": {"subject": "ncats.drug:9100L32L2N", "predicate": "biolink:treats",
-                             "object": "MONDO:0005148", "sources": [
-                        {"resource_id": "infores:molepro",
-                         "resource_role": "primary_knowledge_source"}]}
+                "df87ff82": {
+                    "subject": "ncats.drug:9100L32L2N",
+                    "predicate": "biolink:treats",
+                    "object": "MONDO:0005148",
+                    "sources": [
+                        {
+                            "resource_id": "infores:molepro",
+                            "resource_role": "primary_knowledge_source"
+                        }
+                    ]
+                }
             }
         },
         "auxiliary_graphs": {
             "a0": {
                 "edges": [
                     "e02",
                     "e12"
@@ -289,16 +294,16 @@
                     }
                 ]
             }
         ]
     }
 }
 
-_TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH = deepcopy(_TEST_TRAPI_1_4_0_FULL_SAMPLE)
-_TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH["message"].pop("auxiliary_graphs")
+_TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH = deepcopy(_TEST_TRAPI_1_4_1_FULL_SAMPLE)
+_TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH["message"].pop("auxiliary_graphs")
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (   # Query 0 - No 'workflow' key in TRAPI Response
             {
@@ -464,44 +469,44 @@
     [
         (   # Query 0 - Completely empty Response.Message
             {
                 "message": {
 
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned an empty Message Query Graph!"
             "error.trapi.response.message.empty"
         ),
         (   # Query 1 - Response.Message also devoid of content, missing QGraph trapped first....
             {
                 "message": {
                     "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Query Graph!"
             "error.trapi.response.query_graph.missing"
         ),
         (   # Query 2 - Response.Message also devoid of content, null QGraph trapped first....
             {
                 "message": {
                     "query_graph": None,
                     "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned a null or empty Message Query Graph!"
             "error.trapi.response.query_graph.empty"
         ),
         (
@@ -510,15 +515,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     # "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Knowledge Graph component?"
             "error.trapi.response.knowledge_graph.missing"
         ),
         (
@@ -527,15 +532,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: WARNING - Response returned an empty Message Knowledge Graph?"
             "warning.trapi.response.knowledge_graph.empty"
         ),
         (
@@ -544,15 +549,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     # "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - TRAPI Message is missing its Results component!"
             "error.trapi.response.results.missing"
         ),
         (
@@ -561,15 +566,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: WARNING -Response returned empty Message.results?"
             "warning.trapi.response.results.empty"
         ),
         (
@@ -578,15 +583,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": {"invalid results"}
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - the 'Response.Message.Results' field
             # is not TRAPI schema validated since it has the wrong format!"
             "critical.trapi.validation"
         ),
@@ -596,15 +601,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": []
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned empty Message.results?"
             "warning.trapi.response.results.empty"
         ),
         (
@@ -612,45 +617,45 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 10 - Full Message, with strict validation - still passes
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             ""
         ),
         (
             # Query 11 - Full Message, with strict validation and non-null sources that match
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
@@ -661,15 +666,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "primary"
             },
             True,
@@ -680,15 +685,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             {
                 "ara_source": "infores:aragorn",
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
@@ -699,15 +704,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             {
                 "ara_source": "infores:molepro",
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
             },
             True,
@@ -718,15 +723,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "aggregator"
             },
             True,
@@ -738,15 +743,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_2,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "aggregator"
             },
             True,
@@ -758,15 +763,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_4,
                     "results": _TEST_RESULTS_1
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             {
                 "ara_source": None,
                 "kp_source": "infores:molepro",
                 "kp_source_type": "aggregator"
             },
             True,
@@ -781,30 +786,30 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_2,
                     "knowledge_graph": _TEST_KG_3,
                     "results": _TEST_RESULTS_2
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             "error.knowledge_graph.node.categories.not_concrete"
         ),
         (
             # Query 19 - Full Message, WITH strict validation - abstract predicate?
             {
                 "message": {
                     "query_graph": _TEST_QG_2,
                     "knowledge_graph": _TEST_KG_3,
                     "results": _TEST_RESULTS_2
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             "error.query_graph.edge.predicate.abstract"
         ),
         (
             # Query 20 - Valid full Message, under strict validation.
@@ -813,15 +818,15 @@
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": "workflows-not-an-array"
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             # "Validate TRAPI Response: ERROR - TRAPI schena error: the 'workflow' field must be an array"
             "critical.trapi.validation"
         ),
         (
@@ -832,15 +837,15 @@
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": ["not-a-valid-workflow-spec"]
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             # Validate TRAPI Response: ERROR - TRAPI schema error: the 'workflow' field must be an array of
             # a 'workflow' JSON objects, with contents as defined by the workflow schema.
             "critical.trapi.validation"
         ),
@@ -853,15 +858,15 @@
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": _TEST_RESULTS_1
                 },
                 "workflow": [{"id": "annotate"}]
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             ""   # this simple workflow spec should pass?
         ),
         (
             # Query 23 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
@@ -895,15 +900,15 @@
                       "id": "score"
                     },
                     {
                       "id": "complete_results"
                     }
                 ]
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             # "Validate TRAPI Response: ERROR - TRAPI schema validation error: the 'workflow'
             # field entry overlay_compute_ngd is missing a required parameter 'qnodes_keys'
             "critical.trapi.validation"
         ),
@@ -939,15 +944,15 @@
                       "id": "score"
                     },
                     {
                       "id": "complete_results"
                     }
                 ]
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             ""   # this simple workflow spec should pass?
         ),
         (
             # Query 25 - Valid full Message, under strict validation. Message is valid,
@@ -963,24 +968,24 @@
                     {
                         "id": "lookup",
                         "runner_parameters": None,
                         "parameters": None
                     }
                 ]
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             True,
             ""   # this filtered workflow spec should pass
         ),
         (   # Query 26 - We throw a full TRAPI JSON example here (taken directly from the
             #            TRAPI implementation guidelines...) just for fun and profit
-            _TEST_TRAPI_1_4_0_FULL_SAMPLE,
-            TRAPI_1_4_0,
+            _TEST_TRAPI_1_4_1_FULL_SAMPLE,
+            TRAPI_1_4_1,
             None,
             None,
             True,
             ""   # this filtered workflow spec should pass
         )
     ]
 )
@@ -1000,42 +1005,42 @@
     [
         (   # Query 0 - Completely empty Response.Message
             {
                 "message": {
 
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (   # Query 1 - Response.Message also devoid of content, missing QGraph trapped first....
             {
                 "message": {
                     "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (   # Query 2 - Response.Message also devoid of content, null QGraph trapped first....
             {
                 "message": {
                     "query_graph": None,
                     "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 3 - Partly empty Response.Message with a modest but
@@ -1043,15 +1048,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     # "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 4 - Partly empty Response.Message with a modest
@@ -1059,15 +1064,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": None,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 5 - Partly empty Response.Message with a modest but workable
@@ -1075,15 +1080,15 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     # "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 6 - Partly empty Response.Message with a modest but workable query and
@@ -1091,57 +1096,57 @@
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
                     "results": None
                 }
             },
-            PRE_TRAPI_1_4_0,  # trapi_version
+            TRAPI_1_3_0,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 7 - Full fake sample Response from TRAPI 1.4.0 implementation guidelines
-            _TEST_TRAPI_1_4_0_FULL_SAMPLE,
+            _TEST_TRAPI_1_4_1_FULL_SAMPLE,
             # 25 June 2023 1.4.0 trapi_version with
             # defective auxiliary_graphs schema model
             # now temporarily patched?
-            TRAPI_1_4_0,
+            TRAPI_1_4_1,
             None,
             None,
             False,
             ""  # would be a "critical.trapi.validation" if the schema was unpatched
         ),
         (
             # Query 8 - Full fake sample Response from TRAPI 1.4.0 implementation guidelines
-            _TEST_TRAPI_1_4_0_FULL_SAMPLE,
+            _TEST_TRAPI_1_4_1_FULL_SAMPLE,
             # patched 1.4.0 test schema - fixed critical
             # TRAPI schema parsing error with auxiliary_graphs
             PATCHED_140_SCHEMA_FILEPATH,
             None,
             None,
             False,
             ""
         ),
         (
             # Query 9 - Sample Response from TRAPI 1.4.0 implementation guidelines without auxiliary_graph
-            _TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
+            _TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
             # 25 June 2023 1.4.0 trapi_version with
             # defective auxiliary_graphs schema model
-            TRAPI_1_4_0,
+            TRAPI_1_4_1,
             None,
             None,
             False,
             ""  # nullable: true allows this outcome
         ),
         (
             # Query 10 - Sample Response from TRAPI 1.4.0 implementation guidelines without auxiliary_graph
-            _TEST_TRAPI_1_4_0_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
+            _TEST_TRAPI_1_4_1_FULL_SAMPLE_WITHOUT_AUX_GRAPH,
             # patched 1.4.0 test schema - fixed critical
             # TRAPI schema parsing error with auxiliary_graphs
             PATCHED_140_SCHEMA_FILEPATH,
             None,
             None,
             False,
             ""  # should still work if nullable: true
```

### Comparing `reasoner_validator-3.6.5/tests/test_semver.py` & `reasoner_validator-3.6.6/tests/test_semver.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 
 def test_underspecified_string():
     # test underspecified semver
     with pytest.raises(SemVerUnderspecified):
         assert str(SemVer.from_string("1.2"))
 
 
+def test_fewer_core_fields():
+    # test underspecified semver
+    assert SemVer.from_string("1.2", core_fields=["major", "minor"])
+
+
 def test_string_with_prefix():
     # test semver with (ignorable Pypi-style release) semver
     assert str(SemVer.from_string("v1.2.4", ignore_prefix=True)) == "1.2.4"
     assert str(SemVer.from_string("v1.2.4", ignore_prefix=False)) == "v1.2.4"
 
 
 zero_zero_one = SemVer.from_string("0.0.1")
@@ -47,16 +52,19 @@
 one_one_one_r_b = SemVer.from_string("1.1.1-R2+build456")
 one_three_zero = SemVer.from_string("1.3.0")
 one_three_zero_beta = SemVer.from_string("1.3.0-beta")
 one_four_zero = SemVer.from_string("1.4.0")
 one_four_one = SemVer.from_string("1.4.1")
 one_four_zero_beta = SemVer.from_string("1.4.0-beta")
 
+one_three_only = SemVer.from_string("1.3", core_fields=['major', 'minor'])
+one_four_only = SemVer.from_string("1.4", core_fields=['major', 'minor'])
+
 # special pruned
-one_four_one_beta_pruned = SemVer.from_string("1.4.1-beta", core_fields=['major', 'minor'], ext_fields=[])
+one_four_one_beta_pruned = SemVer.from_string("1.4.1-beta", ext_fields=[])
 
 one_four_zero_beta_one = SemVer.from_string("1.4.0-beta1")
 one_four_zero_beta_four = SemVer.from_string("1.4.0-beta4")
 
 
 def test_semver_greater_or_equal_to():
     # Major release diff
@@ -82,15 +90,18 @@
     assert not one_one_zero_r_b >= one_one_one_r_b
     assert one_one_one_r_b >= one_one_zero_r
     assert not one_one_zero_r >= one_one_one_r_b
     assert one_one_one_r_b >= one_one_zero
     assert not one_one_zero >= one_one_one_r_b
 
     # pruned SemVer comparisons
-    assert one_four_zero >= one_four_one_beta_pruned
+    assert one_four_one >= one_four_one_beta_pruned
+    assert one_four_one_beta_pruned >= one_four_zero
+    assert one_four_zero >= one_four_only
+    assert one_four_zero >= one_three_only
 
     # ... real world comparisons
     assert one_three_zero >= one_three_zero_beta
     assert one_three_zero >= one_three_zero
     assert not one_three_zero_beta >= one_three_zero
     assert one_four_zero >= one_four_zero_beta
     assert not one_four_zero_beta >= one_four_zero
@@ -118,15 +129,16 @@
 
     # Prerelease release diff
     assert not one_four_zero == one_four_zero_beta_one
     assert not one_four_zero_beta_one == one_four_zero
     assert not one_four_zero_beta_one == one_four_zero_beta_four
 
     # pruned SemVer comparisons
-    assert one_four_zero == one_four_one_beta_pruned
+    assert one_four_one == one_four_one_beta_pruned
+    assert one_four_zero == one_four_only
 
 
 def test_semver_not_equal_to():
     assert not one_four_zero != one_four_zero
     assert not one_four_zero_beta_one != one_four_zero_beta_one
 
     # Major release diff
@@ -140,15 +152,16 @@
 
     # Prerelease release diff
     assert one_four_zero != one_four_zero_beta_one
     assert one_four_zero_beta_one != one_four_zero
     assert one_four_zero_beta_one != one_four_zero_beta_four
 
     # pruned SemVer comparisons
-    assert not one_four_zero != one_four_one_beta_pruned
+    assert one_four_zero != one_four_one_beta_pruned
+    assert one_four_zero != one_three_only
 
 
 sample_schema_version = SemVer.from_string(PATCHED_SCHEMA_VERSION)
 sample_schema_file_semver = SemVer.from_string(PATCHED_140_SCHEMA_FILEPATH)
 
 
 def test_schema_file_versioning():
```

### Comparing `reasoner_validator-3.6.5/tests/test_trapi_versioning.py` & `reasoner_validator-3.6.6/tests/test_trapi_versioning.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 """Test TRAPI version handling."""
-from typing import Dict
+from typing import Dict, Optional
 
 import pytest
 
 from reasoner_validator.versioning import get_latest_version
-from reasoner_validator.trapi import load_schema, TRAPIAccessError
-from tests import PATCHED_140_SCHEMA_FILEPATH, LATEST_TRAPI_VERSION
+from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, load_schema, TRAPIAccessError
+from tests import PATCHED_140_SCHEMA_FILEPATH
+
+
+def test_release_tag_is_none():
+    trapi_version:  Optional[str] = get_latest_version(release_tag=None)
+    assert trapi_version is None
+
+
+def test_release_tag_is_empty_string():
+    trapi_version:  Optional[str] = get_latest_version(release_tag="")
+    assert trapi_version is None
 
 
 def test_semver_spec_trapi_version():
     trapi_version: str = get_latest_version(release_tag="1")
-    assert trapi_version == LATEST_TRAPI_VERSION
+    assert trapi_version == LATEST_TRAPI_RELEASE
 
 
 def test_unknown_semver_spec_trapi_version():
     trapi_version: str = get_latest_version(release_tag="2")
     assert trapi_version is None
 
 
 def test_semver_spec_trapi_version_with_prefix():
-    trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_VERSION)
-    assert trapi_version == LATEST_TRAPI_VERSION
+    trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_RELEASE)
+    assert trapi_version == LATEST_TRAPI_RELEASE
 
 
 def test_semver_spec_trapi_version_without_prefix():
-    trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_VERSION[1:])
-    assert trapi_version == LATEST_TRAPI_VERSION
+    trapi_version: str = get_latest_version(release_tag=LATEST_TRAPI_RELEASE[1:])
+    assert trapi_version == LATEST_TRAPI_RELEASE
 
 
 def test_schema_spec_trapi_version():
     trapi_version = get_latest_version(release_tag=PATCHED_140_SCHEMA_FILEPATH)
     assert trapi_version is not None
     assert trapi_version.endswith(".yaml")
```

### Comparing `reasoner_validator-3.6.5/tests/test_validate.py` & `reasoner_validator-3.6.6/tests/test_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 
 import pytest
 
 from jsonschema.exceptions import ValidationError
 
 from reasoner_validator.trapi import TRAPISchemaValidator, openapi_to_jsonschema, load_schema
 
-from tests import LATEST_TEST_VERSIONS
-
-PRE_1_4_0_TEST_VERSIONS = "1.2", "1.2.0", "1.3", "1.3.0"
-ALL_TEST_VERSIONS = PRE_1_4_0_TEST_VERSIONS + LATEST_TEST_VERSIONS
+from tests import LATEST_TEST_RELEASES, PRE_1_4_0_TEST_VERSIONS, ALL_TEST_VERSIONS
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (  # query 0
             {
@@ -49,95 +46,98 @@
                 'allOf':
                     [{'$ref': '#/components/schemas/CURIE'}],
                 'description': 'something',
                 'nullable': True
             },
             # this version keeps the 'allOf' but
             # buries it further downwards... Do we care?
-            LATEST_TEST_VERSIONS[2]
+            LATEST_TEST_RELEASES[2]
         ),
         (  # query 4
             {
                 'oneOf':
                     [{'$ref': '#/components/schemas/CURIE'}],
                 'description': 'something',
                 'nullable': True
             },
-            LATEST_TEST_VERSIONS[2]
+            LATEST_TEST_RELEASES[2]
         ),
         (  # query 5
             {
                 'description': 'something',
                 'nullable': True,
                 '$ref': '#/components/schemas/CURIE'
             },
-            LATEST_TEST_VERSIONS[2]
+            LATEST_TEST_RELEASES[2]
         )
     ]
 )
 def test_openapi_to_jsonschema(query: Tuple[Dict, str]):
     print(f"\nEntering openapi_to_jsonschema(schema: {str(query)})", file=stderr)
     openapi_to_jsonschema(schema=query[0], version=query[1])
     assert "oneOf" in query[0]  # the 'oneOf' creeps in one way or another
     print(f"\nExiting openapi_to_jsonschema(schema: {str(query)})", file=stderr)
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_load_schema(trapi_version):
+def test_load_schema(trapi_version: str):
     """Test load_schema(trapi_version)."""
     schema = load_schema(trapi_version)
     assert schema, f"TRAPI Schema for release '{trapi_version}' is not available?"
 
 
 def test_load_master_schema():
     """Test load_schema('master')."""
     schema = load_schema("master")
     assert schema, "TRAPI Schema for ('master') branch is not available?"
 
 
-@pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_query_and_version_completion(trapi_version):
+@pytest.mark.parametrize(
+    "trapi_version",
+    ALL_TEST_VERSIONS
+)
+def test_query_and_version_completion(trapi_version: str):
     """Test TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     validator.validate({
         "message": {},
     }, "Query")
     with pytest.raises(ValidationError):
         validator.validate({
             "foo": {},
             "bar": {},
         }, "Query")
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_edgebinding(trapi_version):
+def test_edgebinding(trapi_version: str):
     """Test TRAPIValidator(trapi_version=query).validate_EdgeBinding()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     validator.validate({
         "id": "hello",
     }, "EdgeBinding")
     with pytest.raises(ValidationError):
         validator.validate({
             "foo": {},
         }, "EdgeBinding")
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_nullable(trapi_version):
+def test_nullable(trapi_version: str):
     """Test nullable categories property."""
     qnode = {
         "categories": None
     }
     TRAPISchemaValidator(trapi_version=trapi_version).validate(qnode, "QNode")
     # I cannot really trigger anything using 'with pytest.raises(ValidationError)'
     # since QNode has 'additionalProperties: true' but no 'required:' properties
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_nullable_message_properties(trapi_version):
+def test_nullable_message_properties(trapi_version: str):
     """Test nullable message properties."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     message = {
         "knowledge_graph": None,
         "query_graph": None,
         "results": None,
     }
@@ -145,15 +145,15 @@
     with pytest.raises(ValidationError):
         validator.validate({
             "foo": {},  # additionalProperties: false and 'foo' is not a documented property...
         }, "Message")
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_nullable_query_level_properties(trapi_version):
+def test_nullable_query_level_properties(trapi_version: str):
     """Test nullable TRAPI Query level properties."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     trapi_query = {
         "message": {
             "knowledge_graph": None,
             "query_graph": None,
             "results": None,
@@ -190,15 +190,15 @@
             ]
         }
     }
 ]
 
 
 @pytest.mark.parametrize("trapi_version", PRE_1_4_0_TEST_VERSIONS)
-def test_query_trapi_pre_1_4_0_workflow_properties(trapi_version):
+def test_query_trapi_pre_1_4_0_workflow_properties(trapi_version: str):
     """Test flawed TRAPI Query workflow properties with pre-TRAPI 1.4.0."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     query = deepcopy(SAMPLE_QUERY)
     query["workflow"] = SAMPLE_WORKFLOW_1_0_0
     validator.validate(query, "Query")
     with pytest.raises(ValidationError):
         faulty_query_wf = deepcopy(query)
@@ -240,16 +240,16 @@
                 "allowlist": ["infores:aragorn"]
             }
         }
     }
 ]
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_query_latest_trapi_workflow_properties(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_query_latest_trapi_workflow_properties(trapi_version: str):
     """Test flawed TRAPI Query workflow properties."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     query = deepcopy(SAMPLE_QUERY)
     query["workflow"] = SAMPLE_WORKFLOW_1_3_4
     validator.validate(query, "Query")
     with pytest.raises(ValidationError):
         faulty_query_wf = deepcopy(query)
@@ -283,15 +283,15 @@
                 }
             }
         ]
         validator.validate(faulty_query_wf, "Query")
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_nullable_async_query_level_properties(trapi_version):
+def test_nullable_async_query_level_properties(trapi_version: str):
     """Test nullable TRAPI Query level properties."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     async_trapi_query = {
         "callback": "http://mykp.ncats.io/callback",
         "message": {
             "knowledge_graph": None,
             "query_graph": None,
@@ -304,15 +304,15 @@
     with pytest.raises(ValidationError):
         validator.validate({
             "foo": {},  # missing required: callback, message
         }, "AsyncQuery")
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_nullable_response_properties(trapi_version):
+def test_nullable_response_properties(trapi_version: str):
     """Test nullable TRAPI Query level properties."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     async_trapi_query = {
         "message": {
             "knowledge_graph": None,
             "query_graph": None,
             "results": None,
@@ -323,15 +323,15 @@
     with pytest.raises(ValidationError):
         validator.validate({
             "foo": {},  # missing required: message
         }, "Response")
 
 
 @pytest.mark.parametrize("trapi_version", PRE_1_4_0_TEST_VERSIONS)
-def test__trapi_pre_1_4_0_message_results_component_validation(trapi_version):
+def test_trapi_pre_1_4_0_message_results_component_validation(trapi_version: str):
     """Test Message.Results component in TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     sample_message_result = {
         "edge_bindings": {
             "ab": [
                 {
                     "attributes": None,
@@ -363,16 +363,16 @@
         validator.validate({
             # missing required: node_bindings, edge_bindings
             "foo": {},
             "bar": {},
         }, "Result")
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_latest_trapi_message_results_component_validation(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_message_results_component_validation(trapi_version: str):
     """Test Message.Results component in TRAPIValidator(trapi_version=query).validate()."""
     #     Result:
     #       type: object
     #       description: >-
     #         A Result object specifies the nodes and edges in the knowledge graph
     #         that satisfy the structure or conditions of a user-submitted query
     #         graph. It must contain a NodeBindings object (list of query graph node
@@ -509,15 +509,15 @@
             # missing required: node_bindings, edge_bindings
             "foo": {},
             "bar": {},
         }, "Result")
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_message_node_binding_component_validation(trapi_version):
+def test_message_node_binding_component_validation(trapi_version: str):
     """Test NodeBinding component in TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     sample_node_binding = {
         "id": "SGD:S000000065",
         # 'qnode_id' is not formally specified in spec, but it is an
         # example of an additionalProperties: true permitted field
         "qnode_id": "SGD:S000000065",
@@ -530,15 +530,15 @@
             # missing required: id
             "foo": {},
             "bar": {},
         }, "NodeBinding")
 
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_message_attribute_component_validation(trapi_version):
+def test_message_attribute_component_validation(trapi_version: str):
     """Test Attribute component in TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     sample_attribute = {
         "attribute_type_id": "some_attribute",
         "value": "value",
         "value_type_id": None
     }
@@ -554,15 +554,15 @@
             # these two attributes don't have 'nullable: true' so they should have values
             "attribute_type_id": None,
             "value": None
         }, "Attribute")
 
 
 @pytest.mark.parametrize("trapi_version", PRE_1_4_0_TEST_VERSIONS)
-def test_pre_1_4_0_trapi_message_edge_component_validation(trapi_version):
+def test_pre_1_4_0_trapi_message_edge_component_validation(trapi_version: str):
     """Test 'good' Message.KnowledgeGraph.Edge component in
        TRAPIValidator(trapi_version="PRE_1_4_0_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     sample_edge = {
         "subject": "aSubject",
         "predicate": None,  # the predicate could be missing in pre-1.4.0 schemata
         "object": "anObject"
@@ -599,64 +599,64 @@
     "object": "UniProtKB:P00738",   # subject must be a CURIE
     "sources": [  # an array of RetrievalSource
         SAMPLE_RETRIEVAL_SOURCE
     ]
 }
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_latest_trapi_good_message_edge_component_validation(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_good_message_edge_component_validation(trapi_version: str):
     """Test 'good' Message.KnowledgeGraph.Edge component in
        TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     validator.validate(SAMPLE_LATEST_TEST_EDGE, "Edge")
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_latest_trapi_missing_key_message_edge_component_validation(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_missing_key_message_edge_component_validation(trapi_version: str):
     """Test Message.KnowledgeGraph.Edge components missing their required keys
        in TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
         validator.validate({
             # missing required 'subject', 'predicate', 'object' and 'sources'
             "foo": {},
             "bar": {},
         }, "Edge")
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_latest_trapi_null_message_edge_component_validation(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_null_message_edge_component_validation(trapi_version: str):
     """Test Message.KnowledgeGraph.Edge components having null values in
        TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
         null_subject: Dict[str, Optional] = SAMPLE_LATEST_TEST_EDGE.copy()
         null_subject["subject"] = None
         validator.validate(null_subject, "Edge")
     with pytest.raises(ValidationError):
         null_predicate: Dict[str, Optional] = SAMPLE_LATEST_TEST_EDGE.copy()
         null_predicate["predicate"] = None
         validator.validate(null_predicate, "Edge")
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_latest_trapi_flawed_message_edge_component_validation(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_flawed_message_edge_component_validation(trapi_version: str):
     """Test invalid Message.KnowledgeGraph.Edge.predicate in
        TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
         faulty_predicate = SAMPLE_LATEST_TEST_EDGE.copy()
         # predicate is not a Biolink predicate term CURIE
         faulty_predicate["predicate"] = "not-a-biolink-predicate-CURIE"
         validator.validate(faulty_predicate, "Edge")
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_latest_trapi_more_flawed_message_edge_sources_component_validation(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_more_flawed_message_edge_sources_component_validation(trapi_version: str):
     """Test various invalid Message.KnowledgeGraph.Edge.sources values in
        TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
         faulty_sources = SAMPLE_LATEST_TEST_EDGE.copy()
         # 'sources' is not an array (of RetrievalSource objects)
         faulty_sources["sources"] = "not-an-array"
@@ -674,16 +674,16 @@
     with pytest.raises(ValidationError):
         faulty_sources = SAMPLE_LATEST_TEST_EDGE.copy()
         # items in the 'sources' array must be RetrievalSource objects
         faulty_sources["sources"] = [{"not-an-RetrievalSource-key": "something"}]
         validator.validate(faulty_sources, "Edge")
 
 
-@pytest.mark.parametrize("trapi_version", LATEST_TEST_VERSIONS)
-def test_latest_trapi_more_flawed_message_edge_sources_component_validation(trapi_version):
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_more_flawed_message_edge_sources_component_validation(trapi_version: str):
     """Test various invalid Message.KnowledgeGraph.Edge.sources values in
        TRAPIValidator(trapi_version="LATEST_TEST_VERSIONS").validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     with pytest.raises(ValidationError):
         faulty_rs = SAMPLE_RETRIEVAL_SOURCE.copy()
         # items in the 'sources' array must be
         # RetrievalSource objects with a 'resource' key
```

### Comparing `reasoner_validator-3.6.5/tests/test_validation_report.py` & `reasoner_validator-3.6.6/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.5/tests/test_workflows.py` & `reasoner_validator-3.6.6/tests/test_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 from typing import Dict
 from itertools import product
 from json import dumps
 
 from reasoner_validator.trapi import TRAPISchemaValidator
 
-from tests import LATEST_TEST_VERSIONS
+from tests import LATEST_TEST_RELEASES
 
 SAMPLE_QUERY_1 = {
     "message": {
         "knowledge_graph": None,
         "query_graph": None,
         "results": None,
     },
@@ -62,15 +62,15 @@
         },
         {
             "id": "lookup"
         }
     ]
 }
 
-QUERY_VERSION = [qv for qv in product(LATEST_TEST_VERSIONS, (SAMPLE_QUERY_1, SAMPLE_QUERY_2))]
+QUERY_VERSION = [qv for qv in product(LATEST_TEST_RELEASES, (SAMPLE_QUERY_1, SAMPLE_QUERY_2))]
 
 
 @pytest.mark.parametrize("trapi_version,query", QUERY_VERSION)
 def test_query_latest_trapi_workflow_properties(trapi_version: str, query: Dict):
     """Test flawed TRAPI Query workflow properties."""
 
     print(f"\nTRAPI release: '{trapi_version}'")
```

### Comparing `reasoner_validator-3.6.5/PKG-INFO` & `reasoner_validator-3.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.6.5
+Version: 3.6.6
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -23,15 +23,15 @@
 Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bmt (>=1.1.0,<2.0.0)
 Requires-Dist: fastapi (>=0.68,<0.69) ; extra == "web"
 Requires-Dist: jsonschema (>=4.17.0,<5.0.0)
 Requires-Dist: myst-parser (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
-Requires-Dist: pydantic (>=1.8.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0) ; extra == "dev"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "dev"
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.2.1,<2.0.0) ; extra == "docs"
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Requires-Dist: uvicorn (>=0.15,<0.16) ; extra == "web"
@@ -181,15 +181,15 @@
 
 ### API
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 ```json
 {
-  "trapi_version": "1.4.0",
+  "trapi_version": "1.4.1",
   "biolink_version": "3.5.0",
   "sources": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
@@ -223,15 +223,15 @@
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
-  "trapi_version": "1.4.0",
+  "trapi_version": "1.4.1",
   "biolink_version": "3.5.0",
   "response": {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
@@ -266,15 +266,15 @@
 }
 ```
 
 one should typically get a response body something like the following JSON validation result back:
 
 ```json
 {
-  "trapi_version": "1.4.0",
+  "trapi_version": "1.4.1",
   "biolink_version": "3.2.1",
   "messages": {
     # some categories of messages may be absent, hence, empty dictionaries
     "critical": {},
     "errors": {
       "error.knowledge_graph.node.category.missing": {
           # this message template does not have any additional parameters
```

