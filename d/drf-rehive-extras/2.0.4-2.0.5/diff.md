# Comparing `tmp/drf-rehive-extras-2.0.4.tar.gz` & `tmp/drf-rehive-extras-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-2.0.4.tar", last modified: Fri Jun 30 12:07:13 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.0.5.tar", last modified: Thu Jul  6 15:38:40 2023, max compression
```

## Comparing `drf-rehive-extras-2.0.4.tar` & `drf-rehive-extras-2.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.4/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7035 2023-06-30 12:04:34.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6578 2023-06-30 12:05:21.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2685 2023-06-30 09:48:56.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-30 12:06:37.000000 drf-rehive-extras-2.0.4/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.5/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6491 2023-07-06 15:37:54.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2023-07-06 15:33:27.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6579 2023-07-06 15:32:54.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-06 15:33:03.000000 drf-rehive-extras-2.0.5/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-07-06 15:37:16.000000 drf-rehive-extras-2.0.5/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.5/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.5/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-07-06 15:38:40.000000 drf-rehive-extras-2.0.5/PKG-INFO
```

### Comparing `drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.0.5/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.4
+Version: 2.0.5
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.4.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.5.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-2.0.4/README.md` & `drf-rehive-extras-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.4/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.0.5/drf_rehive_extras/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from rest_framework.response import Response
 from rest_framework.settings import api_settings
+from rest_framework.mixins import (
+    CreateModelMixin as DRFCreateModelMixin,
+    ListModelMixin as DRFListModelMixin,
+    RetrieveModelMixin as DRFRetrieveModelMixin,
+    UpdateModelMixin as DRFUpdateModelMixin,
+    DestroyModelMixin as DRFDestroyModelMixin
+)
 from django_filters.rest_framework import DjangoFilterBackend
 
 from .pagination import PageNumberPagination, CursorPagination
 
 
 def add_resource_data(request, instance):
     """
@@ -32,15 +39,15 @@
         resource_id = getattr(instance, field)
     except AttributeError:
         return
     else:
         request._resource_id = str(resource_id)
 
 
-class CreateModelMixin:
+class CreateModelMixin(DRFCreateModelMixin):
     """
     Create a model instance.
     """
 
     def create(self, request, *args, **kwargs):
         """
         Handle object creation on the view.
@@ -63,33 +70,16 @@
 
         return Response(
             data={'status': 'success', 'data': data},
             status=self.get_response_status_code(),
             headers=headers
         )
 
-    def perform_create(self, serializer):
-        """
-        Perform creation using the serializer.
-        """
-
-        serializer.save()
-
-    def get_success_headers(self, data):
-        """
-        Get special headers for the success response on object creation.
-        """
 
-        try:
-            return {'Location': data[api_settings.URL_FIELD_NAME]}
-        except (TypeError, KeyError):
-            return {}
-
-
-class ListModelMixin:
+class ListModelMixin(DRFListModelMixin):
     """
     List a queryset.
     """
 
     filter_backends = (DjangoFilterBackend,)
     pagination_class = PageNumberPagination
 
@@ -142,15 +132,15 @@
 
         return Response(
             data={'status': 'success', 'data': serializer.data},
             status=self.get_response_status_code()
         )
 
 
-class RetrieveModelMixin:
+class RetrieveModelMixin(DRFRetrieveModelMixin):
     """
     Retrieve a model instance.
     """
 
     def retrieve(self, request, *args, **kwargs):
         """
         Handle object retrieval on the view.
@@ -167,15 +157,15 @@
 
         return Response(
             data={'status': 'success', 'data': serializer.data},
             status=self.get_response_status_code()
         )
 
 
-class UpdateModelMixin:
+class UpdateModelMixin(DRFUpdateModelMixin):
     """
     Update a model instance.
     """
 
     def update(self, request, *args, **kwargs):
         """
         Handle object update on the view.
@@ -202,31 +192,16 @@
         data = self.get_response_serializer(serializer.instance).data
 
         return Response(
             data={'status': 'success', 'data': data},
             status=self.get_response_status_code(),
         )
 
-    def perform_update(self, serializer):
-        """
-        Perform update using the serializer.
-        """
 
-        serializer.save()
-
-    def partial_update(self, request, *args, **kwargs):
-        """
-        Perform a partial update (PATCH).
-        """
-
-        kwargs['partial'] = True
-        return self.update(request, *args, **kwargs)
-
-
-class DestroyModelMixin:
+class DestroyModelMixin(DRFDestroyModelMixin):
     """
     Destroy a model instance.
     """
 
     def destroy(self, request, *args, **kwargs):
         """
         Handle object destruction on the view.
@@ -242,14 +217,7 @@
         serializer = self.get_serializer(instance, data=request.data)
         self.perform_destroy(serializer)
 
         return Response(
             data={'status': 'success'},
             status=self.get_response_status_code()
         )
-
-    def perform_destroy(self, serializer):
-        """
-        Perform destroy using the serializer.
-        """
-
-        serializer.destroy()
```

### Comparing `drf-rehive-extras-2.0.4/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.0.5/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.4/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.0.5/drf_rehive_extras/generics.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     #  - {"GET": ObjectSerializer}
     #  - {"GET": (RequestObjectSerializer, ResponseObjectSerializer,)}
     serializer_classes = {}
 
     # Modify the statuses used by the view based on the request method.
     # This attributes can take the following format:
     #  - `{"GET": status.HTTP_200_OK}`
-    response_status_codes ={}
+    response_status_codes = {}
 
     # The default statuses used by the view based on the request method.
     default_response_status_codes = {
         "GET": status.HTTP_200_OK,
         "POST": status.HTTP_201_CREATED,
         "PUT": status.HTTP_200_OK,
         "PATCH": status.HTTP_200_OK,
```

### Comparing `drf-rehive-extras-2.0.4/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.0.5/drf_rehive_extras/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from datetime import datetime
 from functools import reduce
 
 from django.utils.timezone import make_aware
-
 from django.utils.translation import gettext_lazy as _
 from rest_framework import serializers
 
 
 class MetadataField(serializers.JSONField):
     """
     JSON field for metadata serialization.
```

### Comparing `drf-rehive-extras-2.0.4/setup.py` & `drf-rehive-extras-2.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '2.0.4'
+VERSION = '2.0.5'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-2.0.4/LICENSE` & `drf-rehive-extras-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.4/PKG-INFO` & `drf-rehive-extras-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.4
+Version: 2.0.5
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.4.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.5.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

