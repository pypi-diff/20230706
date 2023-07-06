# Comparing `tmp/drf-serializer-prefetch-1.0.9.tar.gz` & `tmp/drf-serializer-prefetch-1.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-serializer-prefetch-1.0.9.tar", last modified: Thu Jun 22 20:25:03 2023, max compression
+gzip compressed data, was "drf-serializer-prefetch-1.1.0b0.tar", last modified: Thu Jul  6 13:17:34 2023, max compression
```

## Comparing `drf-serializer-prefetch-1.0.9.tar` & `drf-serializer-prefetch-1.1.0b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.977120 drf-serializer-prefetch-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-06-22 20:25:03.977120 drf-serializer-prefetch-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.973120 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.973120 drf-serializer-prefetch-1.0.9/serializer_prefetch/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/serializer_prefetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/serializer_prefetch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:25:03.977120 drf-serializer-prefetch-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.973120 drf-serializer-prefetch-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/test_serializers.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.251536 drf-serializer-prefetch-1.1.0b0/
+-rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.1.0b0/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)     9307 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     8990 2023-06-21 19:04:46.000000 drf-serializer-prefetch-1.1.0b0/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)     9307 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      465 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       40 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       26 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/top_level.txt
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/serializer_prefetch/
+-rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.1.0b0/serializer_prefetch/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    14025 2023-07-06 13:14:30.000000 drf-serializer-prefetch-1.1.0b0/serializer_prefetch/base.py
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-07-06 13:17:34.251536 drf-serializer-prefetch-1.1.0b0/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      680 2023-07-06 13:17:25.000000 drf-serializer-prefetch-1.1.0b0/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/tests/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-20 15:59:03.000000 drf-serializer-prefetch-1.1.0b0/tests/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      674 2023-07-06 13:14:30.000000 drf-serializer-prefetch-1.1.0b0/tests/models.py
+-rw-rw-r--   0 max       (1000) max       (1000)      708 2023-06-21 14:24:52.000000 drf-serializer-prefetch-1.1.0b0/tests/serializers.py
+-rw-rw-r--   0 max       (1000) max       (1000)      381 2023-06-20 18:58:38.000000 drf-serializer-prefetch-1.1.0b0/tests/settings.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4003 2023-07-06 13:14:30.000000 drf-serializer-prefetch-1.1.0b0/tests/test_conditions.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2404 2023-06-21 15:24:05.000000 drf-serializer-prefetch-1.1.0b0/tests/test_errors.py
+-rw-rw-r--   0 max       (1000) max       (1000)    25671 2023-07-06 13:14:35.000000 drf-serializer-prefetch-1.1.0b0/tests/test_serializers.py
```

### Comparing `drf-serializer-prefetch-1.0.9/LICENSE` & `drf-serializer-prefetch-1.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.9/PKG-INFO` & `drf-serializer-prefetch-1.1.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.9
+Version: 1.1.0b0
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drf-serializer-prefetch-1.0.9/README.md` & `drf-serializer-prefetch-1.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/PKG-INFO` & `drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.9
+Version: 1.1.0b0
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drf-serializer-prefetch-1.0.9/serializer_prefetch/base.py` & `drf-serializer-prefetch-1.1.0b0/serializer_prefetch/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextlib import suppress
 from collections.abc import Iterable
 
-from django.db.models import Model, QuerySet, prefetch_related_objects
+from django.db.models import Model, QuerySet, prefetch_related_objects, Prefetch
 from django.utils.translation import gettext as _
 from rest_framework.fields import empty
 from rest_framework import serializers
 from rest_framework.utils import model_meta
 
 
 class PrefetchingLogicMixin:
@@ -17,17 +17,21 @@
         if hasattr(serializer, "get_select_related"):
             return serializer.get_select_related()
 
         return getattr(serializer, "select_related", [])
 
     def get_prefetch_related_data(self, serializer):
         if hasattr(serializer, "get_prefetch_related"):
-            return serializer.get_prefetch_related()
+            return self._transform_iterable_to_prefetches(
+                serializer.get_prefetch_related()
+            )
 
-        return getattr(serializer, "prefetch_related", [])
+        return self._transform_iterable_to_prefetches(
+            getattr(serializer, "prefetch_related", [])
+        )
 
     def get_additional_serializers_data(self, serializer):
         if hasattr(serializer, "get_additional_serializers"):
             return serializer.get_additional_serializers()
 
         return getattr(serializer, "additional_serializers", [])
 
@@ -65,15 +69,20 @@
         """
         return super().to_representation(instance)
 
     def call_other_prefetching_methods(self):
         for method in self._other_prefetching_methods:
             method()
 
-    def get_prefetch(self, serializer, current_relation="", should_prefetch=False):
+    def get_prefetch(
+        self,
+        serializer: serializers.Serializer,
+        current_relation: Prefetch = None,
+        should_prefetch: bool = False,
+    ):
         if hasattr(serializer, "child"):
             serializer = serializer.child
 
         select_items, prefetch_items = self._get_custom_relations(
             serializer, current_relation
         )
         self._extend_relation_items(
@@ -92,15 +101,20 @@
             self._other_prefetching_methods.append(serializer.other_prefetching)
 
         if should_prefetch:
             return [], select_items + prefetch_items
 
         return select_items, prefetch_items
 
-    def _extend_relation_items(self, select_items, prefetch_items, return_values):
+    def _extend_relation_items(
+        self,
+        select_items: Iterable[str],
+        prefetch_items: Iterable[Prefetch],
+        return_values: Iterable[Iterable[Prefetch | str]],
+    ):
         return select_items.extend(return_values[0]), prefetch_items.extend(
             return_values[1]
         )
 
     def _get_custom_relations(self, serializer, current_relation):
         select_related_attr = self.get_select_related_data(serializer)
         prefetch_related_attr = self.get_prefetch_related_data(serializer)
@@ -116,16 +130,16 @@
     def _get_additional_serializers_relations(self, serializer, current_relation):
         additional_serializers = self.get_additional_serializers_data(serializer)
 
         select_items = []
         prefetch_items = []
 
         for additional_serializer_data in additional_serializers:
-            custom_current_relation = additional_serializer_data.get(
-                "relation_and_field", ""
+            custom_current_relation = self._transform_str_to_prefetch(
+                additional_serializer_data.get("relation_and_field", "")
             )
 
             if current_relation:
                 custom_current_relation = self._get_joined_prefetch(
                     current_relation, custom_current_relation
                 )
 
@@ -177,14 +191,17 @@
                 continue
 
             if relation.to_many:
                 future_should_prefetch = True
 
             append_to = prefetch_items if future_should_prefetch else select_items
 
+            if should_prefetch:
+                source = Prefetch(source)
+
             if current_relation:
                 source = self._get_joined_prefetch(current_relation, source)
 
             append_to.append(source)
 
             add_to_select, add_to_prefetch = self.get_prefetch(
                 field,
@@ -193,15 +210,15 @@
             )
 
             select_items.extend(add_to_select)
             prefetch_items.extend(add_to_prefetch)
 
         return select_items, prefetch_items
 
-    def _get_custom_related(self, related_attr, current_relation=""):
+    def _get_custom_related(self, related_attr, current_relation=None):
         if current_relation:
             computed_related = self._build_computed_related(
                 related_attr, current_relation
             )
         else:
             computed_related = related_attr
 
@@ -211,34 +228,69 @@
         with suppress(AttributeError):
             return serializer.Meta.model
 
         with suppress(AttributeError):
             return serializer.child.Meta.model
 
     @staticmethod
-    def _get_joined_prefetch(current_relation, item):
-        return "__".join([current_relation, item])
+    def _get_joined_prefetch(current_relation: Prefetch | str, item: Prefetch | str):
+        if isinstance(item, str):
+            return "__".join(
+                (
+                    current_relation
+                    if isinstance(current_relation, str)
+                    else current_relation.prefetch_through,
+                    item,
+                )
+            )
+
+        current_relation_through = (
+            current_relation
+            if isinstance(current_relation, str)
+            else current_relation.prefetch_through
+        )
+        current_relation_to = (
+            current_relation
+            if isinstance(current_relation, str)
+            else current_relation.prefetch_to
+        )
+
+        item.prefetch_through = "__".join(
+            [current_relation_through, item.prefetch_through]
+        )
+        item.prefetch_to = "__".join([current_relation_to, item.prefetch_to])
+
+        return item
 
     def _build_computed_related(self, related_attr, current_relation):
         return [
             self._get_joined_prefetch(current_relation, item) for item in related_attr
         ]
 
+    def _transform_str_to_prefetch(self, item):
+        if isinstance(item, str):
+            return Prefetch(item)
+
+        return item
+
+    def _transform_iterable_to_prefetches(self, iterable_items):
+        return [self._transform_str_to_prefetch(item) for item in iterable_items]
+
 
 class List(list):
-    _serializer_prefetch_done = False
+    _braindate_prefetch_done = False
 
 
 class PrefetchingListSerializer(PrefetchingLogicMixin, serializers.ListSerializer):
     def __init__(self, *args, auto_prefetch=True, **kwargs):
         self._auto_prefetch = auto_prefetch
         super().__init__(*args, **kwargs)
 
     def to_representation(self, instance, *args, **kwargs):
-        prefetch_done = getattr(instance, "_serializer_prefetch_done", False)
+        prefetch_done = getattr(instance, "_braindate_prefetch_done", False)
         if prefetch_done or self.parent is not None or not self._auto_prefetch:
             return super().to_representation(instance)
 
         child = self.child
         select_items, prefetch_items = self.get_prefetch(child)
 
         if isinstance(instance, QuerySet):
@@ -257,30 +309,30 @@
 
             for related_lookup in set(select_items + prefetch_items):
                 prefetch_related_objects(instance, related_lookup)
 
         if isinstance(instance, list):
             instance = List(instance)
 
-        instance._serializer_prefetch_done = True
+        instance._braindate_prefetch_done = True
 
         self.call_other_prefetching_methods()
 
         return self.call_to_representation(instance)
 
 
 class Dict(dict):
-    _serializer_prefetch_done = False
+    _braindate_prefetch_done = False
 
 
 class PrefetchingSerializerMixin(PrefetchingLogicMixin):
     default_list_serializer_class = PrefetchingListSerializer
 
     def to_representation(self, instance, *args, **kwargs):
-        prefetch_done = getattr(instance, "_serializer_prefetch_done", False)
+        prefetch_done = getattr(instance, "_braindate_prefetch_done", False)
         if (
             not prefetch_done
             and self._auto_prefetch
             and not self.parent
             and not getattr(instance, "_prefetched_objects_cache", None)
         ):
             select_items, prefetch_items = self.get_prefetch(self)
@@ -294,15 +346,15 @@
                             "Got an AttributeError. You might have forgotten to "
                             "add `many=True` on the serializer."
                         )
                     ) from exc
 
             if isinstance(instance, dict):
                 instance = Dict(instance)
-            instance._serializer_prefetch_done = True
+            instance._braindate_prefetch_done = True
 
             self.call_other_prefetching_methods()
 
             if isinstance(instance, Model):
                 return self.call_to_representation(instance)
 
         return super().to_representation(instance)
```

### Comparing `drf-serializer-prefetch-1.0.9/setup.py` & `drf-serializer-prefetch-1.1.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
-VERSION = "1.0.9"
+VERSION = "1.1.0b"
 DESCRIPTION = "An automatic prefetcher for django-rest-framework."
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 setup(
     name="drf-serializer-prefetch",
     version=VERSION,
```

### Comparing `drf-serializer-prefetch-1.0.9/tests/models.py` & `drf-serializer-prefetch-1.1.0b0/tests/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from django.db import models
 
 
+class Continent(models.Model):
+    label = models.CharField(max_length=50)
+
+
 class Country(models.Model):
     label = models.CharField(max_length=50)
+    continent = models.ForeignKey(Continent, on_delete=models.CASCADE, null=True)
 
 
 class Pizza(models.Model):
     label = models.CharField(max_length=50)
     provenance = models.ForeignKey(Country, on_delete=models.CASCADE)
```

### Comparing `drf-serializer-prefetch-1.0.9/tests/serializers.py` & `drf-serializer-prefetch-1.1.0b0/tests/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.9/tests/test_conditions.py` & `drf-serializer-prefetch-1.1.0b0/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.9/tests/test_errors.py` & `drf-serializer-prefetch-1.1.0b0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.9/tests/test_serializers.py` & `drf-serializer-prefetch-1.1.0b0/tests/test_serializers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+from django.db.models import Prefetch
 from django.test import TestCase
 
 from rest_framework import serializers
 
 from serializer_prefetch import PrefetchingSerializerMixin
 
-from tests.models import Pizza, Topping, Country
+from tests.models import Pizza, Topping, Country, Continent
 from tests.serializers import PizzaSerializer, ToppingSerializer, CountrySerializer
 
 
 class SerializersTestCase(TestCase):
     @classmethod
     def setUpTestData(cls) -> None:
-        cls.canada = Country.objects.create(label="Canada")
-        cls.usa = Country.objects.create(label="USA")
-        cls.china = Country.objects.create(label="China")
-        cls.argentina = Country.objects.create(label="Argentina")
+        cls.america = Continent.objects.create(label="America")
+        cls.asia = Continent.objects.create(label="Asia")
+
+        cls.canada = Country.objects.create(label="Canada", continent=cls.america)
+        cls.usa = Country.objects.create(label="USA", continent=cls.america)
+        cls.china = Country.objects.create(label="China", continent=cls.asia)
+        cls.argentina = Country.objects.create(label="Argentina", continent=cls.america)
 
         cls.hawaian_pizza = Pizza.objects.create(
             label="Hawaiian", provenance=cls.canada
         )
         cls.ham_topping = Topping.objects.create(
             pizza=cls.hawaian_pizza, label="Ham", origin=cls.china
         )
@@ -275,14 +279,147 @@
                     "label": "Pepperoni",
                     "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
                     "provenance": {"label": "USA"},
                 },
             ],
         )
 
+    def test_select_related_with_depth(self):
+        class CountrySerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            continent = serializers.SerializerMethodField()
+
+            def get_continent(self, obj):
+                return obj.continent.label
+
+            class Meta:
+                model = Country
+                fields = ("label", "continent")
+
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = CountrySerializer()
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+            provenance = CountrySerializer()
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings", "provenance")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(8):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {
+                            "label": "Ham",
+                            "origin": {"label": "China", "continent": "Asia"},
+                        },
+                        {
+                            "label": "Pineapple",
+                            "origin": {"label": "Argentina", "continent": "America"},
+                        },
+                    ],
+                    "provenance": {"label": "Canada", "continent": "America"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [
+                        {
+                            "label": "Pepperoni",
+                            "origin": {"label": "USA", "continent": "America"},
+                        }
+                    ],
+                    "provenance": {"label": "USA", "continent": "America"},
+                },
+            ],
+        )
+
+        class CountrySerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            select_related = ("continent",)
+
+            continent = serializers.SerializerMethodField()
+
+            def get_continent(self, obj):
+                return obj.continent.label
+
+            class Meta:
+                model = Country
+                fields = ("label", "continent")
+
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = CountrySerializer()
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+            provenance = CountrySerializer()
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings", "provenance")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(4):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {
+                            "label": "Ham",
+                            "origin": {"label": "China", "continent": "Asia"},
+                        },
+                        {
+                            "label": "Pineapple",
+                            "origin": {"label": "Argentina", "continent": "America"},
+                        },
+                    ],
+                    "provenance": {"label": "Canada", "continent": "America"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [
+                        {
+                            "label": "Pepperoni",
+                            "origin": {"label": "USA", "continent": "America"},
+                        }
+                    ],
+                    "provenance": {"label": "USA", "continent": "America"},
+                },
+            ],
+        )
+
     def test_get_additional_serializers_with_depth(self):
         class ToppingSerializer(
             PrefetchingSerializerMixin, serializers.ModelSerializer
         ):
             origin = CountrySerializer()
 
             class Meta:
@@ -531,7 +668,153 @@
                     "label": "Pepperoni",
                     "toppings": [
                         {"label": "Pepperoni", "origin": "USA"},
                     ],
                 },
             ],
         )
+
+    def test_allow_passing_prefetch_object(self):
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            american_toppings = serializers.SerializerMethodField()
+
+            def get_american_toppings(self, obj):
+                return [
+                    topping.label
+                    for topping in obj.toppings.filter(
+                        origin__continent__label="America"
+                    )
+                ]
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "american_toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "american_toppings": ["Pineapple"],
+                },
+                {
+                    "label": "Pepperoni",
+                    "american_toppings": ["Pepperoni"],
+                },
+            ],
+        )
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            prefetch_related = (
+                Prefetch(
+                    "toppings",
+                    queryset=Topping.objects.filter(origin__continent__label="America"),
+                    to_attr="american_toppings",
+                ),
+            )
+
+            american_toppings = serializers.SerializerMethodField()
+
+            def get_american_toppings(self, obj):
+                return [topping.label for topping in obj.american_toppings]
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "american_toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "american_toppings": ["Pineapple"],
+                },
+                {
+                    "label": "Pepperoni",
+                    "american_toppings": ["Pepperoni"],
+                },
+            ],
+        )
+
+    def test_allow_passing_prefetch_object_with_depth(self):
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = serializers.SerializerMethodField()
+
+            def get_origin(self, obj):
+                return obj.origin.label
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(5):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": "China"},
+                        {"label": "Pineapple", "origin": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": "USA"}],
+                },
+            ],
+        )
+
+        class ToppingSerializer(ToppingSerializer):
+            prefetch_related = (Prefetch("origin"),)
+
+        class PizzaSerializer(PizzaSerializer):
+            toppings = ToppingSerializer(many=True)
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": "China"},
+                        {"label": "Pineapple", "origin": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": "USA"}],
+                },
+            ],
+        )
```

