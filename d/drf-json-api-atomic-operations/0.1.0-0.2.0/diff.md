# Comparing `tmp/drf-json-api-atomic-operations-0.1.0.tar.gz` & `tmp/drf-json-api-atomic-operations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-json-api-atomic-operations-0.1.0.tar", last modified: Tue Jul  4 14:19:24 2023, max compression
+gzip compressed data, was "drf-json-api-atomic-operations-0.2.0.tar", last modified: Thu Jul  6 07:21:43 2023, max compression
```

## Comparing `drf-json-api-atomic-operations-0.1.0.tar` & `drf-json-api-atomic-operations-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:19:24.106743 drf-json-api-atomic-operations-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-04 14:19:24.106743 drf-json-api-atomic-operations-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:19:24.106743 drf-json-api-atomic-operations-0.1.0/atomic_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/atomic_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/atomic_operations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/atomic_operations/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/atomic_operations/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/atomic_operations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:19:24.106743 drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-04 14:19:24.000000 drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-04 14:19:24.000000 drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:19:24.000000 drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:19:24.000000 drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 14:19:24.000000 drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 14:19:24.000000 drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-04 14:19:24.110743 drf-json-api-atomic-operations-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:19:24.106743 drf-json-api-atomic-operations-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-07-04 14:19:18.000000 drf-json-api-atomic-operations-0.1.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.583011 drf-json-api-atomic-operations-0.2.0/atomic_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/tests/test_views.py
```

### Comparing `drf-json-api-atomic-operations-0.1.0/LICENSE` & `drf-json-api-atomic-operations-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.1.0/atomic_operations/renderers.py` & `drf-json-api-atomic-operations-0.2.0/atomic_operations/renderers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 """
 import json
 from typing import List, OrderedDict
 
 from rest_framework_json_api.renderers import JSONRenderer
 from rest_framework_json_api.utils import get_resource_type_from_serializer
 
+from atomic_operations.consts import (
+    ATOMIC_CONTENT_TYPE,
+    ATOMIC_MEDIA_TYPE,
+    ATOMIC_RESULTS,
+)
+
 
 class AtomicResultRenderer(JSONRenderer):
     """
     The `JSONRenderer` exposes a number of methods that you may override if you need highly
     custom rendering control.
 
     Render a JSON response per the JSON:API spec:
@@ -29,16 +35,16 @@
                 "title": "JSON API paints my bikeshed!"
               }
             }
           }]
         }
     """
 
-    media_type = 'application/vnd.api+json;ext="https://jsonapi.org/ext/atomic'
-    format = 'vnd.api+json;ext="https://jsonapi.org/ext/atomic'
+    media_type = ATOMIC_CONTENT_TYPE
+    format = ATOMIC_MEDIA_TYPE
 
     def check_error(self, operation_result_data, accepted_media_type, renderer_context):
         # primitive check if any operation has errors while parsing
         status = operation_result_data.get("status")
         try:
             status = int(status)
             if status >= 400 and status <= 600:
@@ -61,10 +67,10 @@
                 operation_result_data.serializer)
             rendered_primary_data = super().render(
                 operation_result_data, accepted_media_type, renderer_context)
             atomic_results.append(rendered_primary_data.decode("UTF-8"))
 
         atomic_results_str = f"[{','.join(atomic_results)}]"
 
-        rendered_content = '{"atomic:results":' + atomic_results_str + '}'
+        rendered_content = '{"' + ATOMIC_RESULTS + '":' + atomic_results_str + '}'
 
         return rendered_content.encode()
```

### Comparing `drf-json-api-atomic-operations-0.1.0/atomic_operations/views.py` & `drf-json-api-atomic-operations-0.2.0/atomic_operations/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
 from django.db.transaction import atomic
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
+from atomic_operations.consts import ATOMIC_OPERATIONS
 from atomic_operations.exceptions import UnprocessableEntity
 from atomic_operations.parsers import AtomicOperationParser
 from atomic_operations.renderers import AtomicResultRenderer
 
 
 class AtomicOperationView(APIView):
     """View which handles JSON:API Atomic Operations extension https://jsonapi.org/ext/atomic/"""
@@ -61,15 +62,15 @@
                 })
             except ObjectDoesNotExist:
                 raise UnprocessableEntity([
                     {
                         "id": "object-does-not-exist",
                         "detail": f'Object with id `{kwargs["data"]["id"]}` received for operation with index `{idx}` does not exist',
                         "source": {
-                            "pointer": f"/atomic:operations/{idx}/data/id"
+                            "pointer": f"/{ATOMIC_OPERATIONS}/{idx}/data/id"
                         },
                         "status": "422"
                     }
                 ]
                 )
 
         return serializer_class(*args, **kwargs)
@@ -78,14 +79,15 @@
         """
         Extra context provided to the serializer class.
         """
         return {
             'request': self.request,
             'format': self.format_kwarg,
             'view': self
+
         }
 
     def post(self, request, *args, **kwargs):
         return self.perform_operations(request.data)
 
     def perform_operations(self, parsed_operations: List[Dict]):
         response_data: List[Dict] = []
@@ -93,19 +95,24 @@
             for idx, operation in enumerate(parsed_operations):
                 op_code = next(iter(operation))
                 obj = operation[op_code]
                 # TODO: collect operations of same op_code and resource type to support bulk_create | bulk_update | filter(id__in=[1,2,3]).delete()
                 serializer = self.get_serializer(
                     idx=idx,
                     data=obj,
-                    operation_code=op_code,
-                    resource_type=obj["type"]
+                    operation_code="update" if op_code == "update-relationship" else op_code,
+                    resource_type=obj["type"],
+                    partial=True if "update" in op_code else False
                 )
-                if op_code in ["add", "update"]:
+                if op_code in ["add", "update", "update-relationship"]:
                     serializer.is_valid(raise_exception=True)
                     serializer.save()
+                    # FIXME: check if it is just a relationship update
+                    if op_code == "update-relationship":
+                        # relation update. No response data
+                        continue
                     response_data.append(serializer.data)
                 else:
                     # remove
                     serializer.instance.delete()
 
         return Response(response_data, status=status.HTTP_200_OK if response_data else status.HTTP_204_NO_CONTENT)
```

### Comparing `drf-json-api-atomic-operations-0.1.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt` & `drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 atomic_operations/__init__.py
+atomic_operations/consts.py
 atomic_operations/exceptions.py
 atomic_operations/parsers.py
 atomic_operations/renderers.py
 atomic_operations/views.py
 drf_json_api_atomic_operations.egg-info/PKG-INFO
 drf_json_api_atomic_operations.egg-info/SOURCES.txt
 drf_json_api_atomic_operations.egg-info/dependency_links.txt
```

### Comparing `drf-json-api-atomic-operations-0.1.0/setup.cfg` & `drf-json-api-atomic-operations-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.1.0/setup.py` & `drf-json-api-atomic-operations-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.1.0/tests/test_parsers.py` & `drf-json-api-atomic-operations-0.2.0/tests/test_parsers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,75 @@
 import json
 from io import BytesIO
 
 from django.test import RequestFactory, TestCase
-from rest_framework.exceptions import ParseError
 
+from atomic_operations.consts import ATOMIC_OPERATIONS
+from atomic_operations.exceptions import JsonApiParseError
 from atomic_operations.parsers import AtomicOperationParser
 from tests.views import ConcretAtomicOperationView
 
 
 class TestAtomicOperationParser(TestCase):
 
     def setUp(self):
         self.factory = RequestFactory()
         self.parser = AtomicOperationParser()
         self.parser_context = {"request": self.factory.post(
             "/"), "kwargs": {}, "view": ConcretAtomicOperationView()}
+        self.maxDiff = None
 
     def test_parse(self):
         data = {
-            "atomic:operations": [
+            ATOMIC_OPERATIONS: [
                 {
                     "op": "add",
-                    "href": "/blogPosts",
                     "data": {
                         "type": "articles",
                         "attributes": {
                             "title": "JSON API paints my bikeshed!"
                         }
                     }
                 }, {
                     "op": "update",
-                    "href": "/blogPosts",
                     "data": {
                         "id": "1",
                         "type": "articles",
                         "attributes": {
                             "title": "JSON API paints my bikeshed!"
                         }
                     }
                 }, {
                     "op": "remove",
                     "ref": {
                         "id": "1",
                         "type": "articles",
                     }
+                }, {
+                    "op": "update",
+                    "ref": {
+                        "type": "articles",
+                        "id": "13",
+                        "relationship": "author"
+                    },
+                    "data": {
+                        "type": "people",
+                        "id": "9"
+                    }
+                }, {
+                    "op": "update",
+                    "ref": {
+                        "type": "articles",
+                        "id": "13",
+                        "relationship": "tags"
+                    },
+                    "data": [
+                        {"type": "tags", "id": "2"},
+                        {"type": "tags", "id": "3"}
+                    ]
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
 
         result = self.parser.parse(stream, parser_context=self.parser_context)
 
@@ -66,33 +88,43 @@
                 }
             },
             {
                 "remove": {
                     "id": "1",
                     "type": "articles",
                 }
+            }, {
+                "update-relationship": {
+                    "id": "13",
+                    "type": "articles",
+                    "author": {"type": "people", "id": "9"}
+                }
+            }, {
+                "update-relationship": {
+                    "id": "13",
+                    "type": "articles",
+                    "tags": [{'type': 'tags', 'id': '2'}, {'type': 'tags', 'id': '3'}]
+                }
             }
         ]
         self.assertEqual(expected_result, result)
 
     def test_unsupported_operation_code(self):
         data = {
-            "atomic:operations": [
+            ATOMIC_OPERATIONS: [
                 {
                     "op": "add",
-                    "href": "/blogPosts",
                     "data": {
                         "type": "articles",
                         "attributes": {
                             "title": "JSON API paints my bikeshed!"
                         }
                     }
                 }, {
                     "op": "unknown",
-                    "href": "/blogPosts",
                     "data": {
                         "id": "1",
                         "type": "articles",
                         "attributes": {
                             "title": "JSON API paints my bikeshed!"
                         }
                     }
@@ -103,37 +135,35 @@
                         "type": "articles",
                     }
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
-            "Unknown operation `unknown` received for operation with index 1",
+            JsonApiParseError,
+            "Unknown operation `unknown` received",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
     def test_missing_operation_code(self):
         data = {
-            "atomic:operations": [
+            ATOMIC_OPERATIONS: [
                 {
                     "op": "add",
-                    "href": "/blogPosts",
                     "data": {
                         "type": "articles",
                         "attributes": {
                             "title": "JSON API paints my bikeshed!"
                         }
                     }
                 }, {
-                    "href": "/blogPosts",
                     "data": {
                         "id": "1",
                         "type": "articles",
                         "attributes": {
                             "title": "JSON API paints my bikeshed!"
                         }
                     }
@@ -144,124 +174,121 @@
                         "type": "articles",
                     }
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
-            "Received operation with index 1 does not provide an operation code",
+            JsonApiParseError,
+            "Received operation does not provide an operation code",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
-    def test_missing_ref_href_on_remove(self):
+    def test_missing_ref_on_remove(self):
         data = {
-            "atomic:operations": [
+            ATOMIC_OPERATIONS: [
                 {
                     "op": "remove",
 
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
-            "either ref or href must be part of the remove operation with index 0",
+            JsonApiParseError,
+            "`ref` must be part of remove operation",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
-    def test_using_ref_href_together_on_remove(self):
+    def test_using_href(self):
         data = {
-            "atomic:operations": [
+            ATOMIC_OPERATIONS: [
                 {
                     "op": "remove",
                     "href": "/somearticle",
-                    "ref": {
-                        "id": "1",
-                        "type": "articles",
-                    }
+
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
-            "using ref and href together on operation with index 0 is not allowed",
+            JsonApiParseError,
+            "Received operation using `href` to refencing objects which is not implemented by this api. Use `ref` instead.",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
     def test_primary_data_without_id(self):
         data = {
-            "atomic:operations": [
-                {
-                    "op": "remove",
-                    "ref": {
-                        "type": "articles",
-                    }
-                }
+            ATOMIC_OPERATIONS: [
+               {
+                   "op": "remove",
+                   "ref": {
+                       "type": "articles",
+                   }
+               }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
-            "The resource identifier object with index 0 must contain an `id` member",
+            JsonApiParseError,
+            "The resource identifier object must contain an `id` member",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
         data = {
-            "atomic:operations": [
+            ATOMIC_OPERATIONS: [
                 {
                     "op": "update",
                     "ref": {
                         "type": "articles",
                     }
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
-            "The resource identifier object with index 0 must contain an `id` member",
+            JsonApiParseError,
+            "The resource identifier object must contain an `id` member",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
     def test_primary_data(self):
         data = {
-            "atomic:operations": [
+            ATOMIC_OPERATIONS: [
                 {
                     "op": "update",
                     "id": "1",
                     "data": []
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
-            "Received data of operation with index 0 is not a valid JSON:API Operation Object",
+            JsonApiParseError,
+            "primary data object musst be present",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
@@ -279,41 +306,41 @@
                         }
                     }
                 }
             ]
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
+            JsonApiParseError,
             "Received document does not contain operations objects",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
         data = []
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
+            JsonApiParseError,
             "Received document does not contain operations objects",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
         data = {
-            "atomic:operations": {}
+            ATOMIC_OPERATIONS: {}
         }
         stream = BytesIO(json.dumps(data).encode("utf-8"))
         self.assertRaisesRegex(
-            ParseError,
+            JsonApiParseError,
             "Received operation objects is not a valid JSON:API atomic operation request",
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
```

