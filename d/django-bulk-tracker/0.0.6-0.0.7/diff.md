# Comparing `tmp/django-bulk-tracker-0.0.6.tar.gz` & `tmp/django-bulk-tracker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bulk-tracker-0.0.6.tar", last modified: Sun May 28 12:32:30 2023, max compression
+gzip compressed data, was "django-bulk-tracker-0.0.7.tar", last modified: Thu Jul  6 16:33:01 2023, max compression
```

## Comparing `django-bulk-tracker-0.0.6.tar` & `django-bulk-tracker-0.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.561239 django-bulk-tracker-0.0.6/bulk_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/helper_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/bulk_tracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 12:32:30.000000 django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:30.565239 django-bulk-tracker-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/test_create_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/test_delete_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-28 12:32:13.000000 django-bulk-tracker-0.0.6/tests/test_update_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/bulk_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/helper_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/bulk_tracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 16:33:01.000000 django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.733406 django-bulk-tracker-0.0.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:33:01.737406 django-bulk-tracker-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/test_create_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/test_delete_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-06 16:32:46.000000 django-bulk-tracker-0.0.7/tests/test_update_signal.py
```

### Comparing `django-bulk-tracker-0.0.6/PKG-INFO` & `django-bulk-tracker-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-tracker
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Django app that allows you to have more control over bulk operations.
 Home-page: https://github.com/hassaanalansary/django-bulk-tracker
 Author: Hassaan Alansary
 Author-email: hassaanalansary@yahoo.com
 License: Mozilla Public License 2.0
 Keywords: django,django-bulk-tracker,bulk-update,bulk-create,signals,django-signals
 Classifier: Environment :: Web Environment
```

### Comparing `django-bulk-tracker-0.0.6/README.md` & `django-bulk-tracker-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/bulk_tracker/helper_objects.py` & `django-bulk-tracker-0.0.7/bulk_tracker/helper_objects.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/bulk_tracker/managers.py` & `django-bulk-tracker-0.0.7/bulk_tracker/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,17 @@
         return result
 
     def create(self, *, tracking_info_: TrackingInfo | None = None, **kwargs):
         """
         Create a new object with the given kwargs, saving it to the database
         and returning the created object.
         """
+
+        # NOTE: send_post_create_signal is called after 'create' gets executed, where model.save is called
         obj = super().create(**kwargs)
-        send_post_create_signal([obj], model=self.model, tracking_info_=tracking_info_)
         return obj
 
     # This function is just copied from django core, with minor modification to accept TrackingInfo
     def bulk_update(
         self, objs, fields, batch_size=None, *args, tracking_info_: TrackingInfo | None = None, **kwargs
     ) -> None:
         """
```

### Comparing `django-bulk-tracker-0.0.6/bulk_tracker/models.py` & `django-bulk-tracker-0.0.7/bulk_tracker/models.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/bulk_tracker/signals.py` & `django-bulk-tracker-0.0.7/bulk_tracker/signals.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/PKG-INFO` & `django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-tracker
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Django app that allows you to have more control over bulk operations.
 Home-page: https://github.com/hassaanalansary/django-bulk-tracker
 Author: Hassaan Alansary
 Author-email: hassaanalansary@yahoo.com
 License: Mozilla Public License 2.0
 Keywords: django,django-bulk-tracker,bulk-update,bulk-create,signals,django-signals
 Classifier: Environment :: Web Environment
```

### Comparing `django-bulk-tracker-0.0.6/django_bulk_tracker.egg-info/SOURCES.txt` & `django-bulk-tracker-0.0.7/django_bulk_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/docs/Makefile` & `django-bulk-tracker-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/docs/make.bat` & `django-bulk-tracker-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/docs/source/conf.py` & `django-bulk-tracker-0.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/docs/source/index.rst` & `django-bulk-tracker-0.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/docs/source/installation.rst` & `django-bulk-tracker-0.0.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/docs/source/usage.rst` & `django-bulk-tracker-0.0.7/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/setup.cfg` & `django-bulk-tracker-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-bulk-tracker-0.0.6/tests/test_create_signal.py` & `django-bulk-tracker-0.0.7/tests/test_delete_signal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,84 @@
 from __future__ import annotations
 
+from datetime import datetime
+
 from django.test import TestCase
 
 from bulk_tracker.helper_objects import ModifiedObject, TrackingInfo
-from bulk_tracker.signals import post_create_signal
+from bulk_tracker.signals import post_delete_signal
 from tests.models import Author, Post
 
 
-class TestCreateSignal(TestCase):
+class TestDeleteSignal(TestCase):
     @classmethod
     def setUpTestData(cls):
         cls.author_john = Author.objects.create(first_name="John", last_name="Doe")
 
-    def test_model_create_should_emit_post_create_signal(self):
+    def test_model_delete_should_emit_post_delete_signal(self):
         # Arrange
         signal_called_with = {}
 
-        def post_create_receiver(
+        def post_delete_receiver(
             sender,
             objects: list[ModifiedObject[Post]],
             tracking_info_: TrackingInfo | None = None,
             **kwargs,
         ):
             signal_called_with["objects"] = objects
             signal_called_with["tracking_info_"] = tracking_info_
 
-        post_create_signal.connect(post_create_receiver, sender=Post)
+        post_delete_signal.connect(post_delete_receiver, sender=Post)
+        post = Post.objects.create(title="Sound of Winter", publish_date="1998-03-08", author=self.author_john)
 
         # Act
-        Post.objects.create(title="Sound of Winter", publish_date="1998-03-08", author=self.author_john)
-
+        post.delete()
         # Assert
         self.assertTrue(signal_called_with != {})
         self.assertEqual(1, len(signal_called_with["objects"]))
         self.assertEqual(None, signal_called_with["tracking_info_"])
 
         modified_objects: list[ModifiedObject[Post]] = signal_called_with["objects"]
         self.assertEqual("Sound of Winter", modified_objects[0].instance.title)
         self.assertEqual("1998-03-08", modified_objects[0].instance.publish_date)
         self.assertEqual(self.author_john, modified_objects[0].instance.author)
         self.assertEqual({}, modified_objects[0].changed_values)
 
-    def test_bulk_create_should_emit_post_create_signal(self):
+    def test_query_delete_should_emit_post_delete_signal(self):
         # Arrange
         signal_called_with = {}
 
-        def post_create_receiver(
+        def post_delete_receiver(
             sender,
             objects: list[ModifiedObject[Post]],
             tracking_info_: TrackingInfo | None = None,
             **kwargs,
         ):
             signal_called_with["objects"] = objects
             signal_called_with["tracking_info_"] = tracking_info_
 
-        post_create_signal.connect(post_create_receiver, sender=Post)
+        post_delete_signal.connect(post_delete_receiver, sender=Post)
         posts = [
             Post(title="Sound of Winter", publish_date="1998-01-08", author=self.author_john),
             Post(title="Sound of Summer", publish_date="1998-06-08", author=self.author_john),
         ]
+        Post.objects.bulk_create(posts)
 
         # Act
-        Post.objects.bulk_create(posts)
+        Post.objects.all().order_by("publish_date").delete()
 
         # Assert
         self.assertTrue(signal_called_with != {})
         self.assertEqual(2, len(signal_called_with["objects"]))
         self.assertEqual(None, signal_called_with["tracking_info_"])
 
         modified_objects: list[ModifiedObject[Post]] = signal_called_with["objects"]
 
         self.assertEqual("Sound of Winter", modified_objects[0].instance.title)
-        self.assertEqual("1998-01-08", modified_objects[0].instance.publish_date)
+        self.assertEqual(datetime.strptime("1998-01-08", "%Y-%m-%d").date(), modified_objects[0].instance.publish_date)
         self.assertEqual(self.author_john, modified_objects[0].instance.author)
         self.assertEqual({}, modified_objects[0].changed_values)
 
         self.assertEqual("Sound of Summer", modified_objects[1].instance.title)
-        self.assertEqual("1998-06-08", modified_objects[1].instance.publish_date)
+        self.assertEqual(datetime.strptime("1998-06-08", "%Y-%m-%d").date(), modified_objects[1].instance.publish_date)
         self.assertEqual(self.author_john, modified_objects[1].instance.author)
         self.assertEqual({}, modified_objects[1].changed_values)
-
-    def test_model_save_should_emit_post_create_signal(self):
-        # Arrange
-        signal_called_with = {}
-
-        def post_create_receiver(
-            sender,
-            objects: list[ModifiedObject[Post]],
-            tracking_info_: TrackingInfo | None = None,
-            **kwargs,
-        ):
-            signal_called_with["objects"] = objects
-            signal_called_with["tracking_info_"] = tracking_info_
-
-        post_create_signal.connect(post_create_receiver, sender=Post)
-
-        # Act
-        Post(title="Sound of Winter", publish_date="1998-01-08", author=self.author_john).save()
-
-        # Assert
-        self.assertTrue(signal_called_with != {})
-        self.assertEqual(1, len(signal_called_with["objects"]))
-        self.assertEqual(None, signal_called_with["tracking_info_"])
-
-        modified_objects: list[ModifiedObject[Post]] = signal_called_with["objects"]
-
-        self.assertEqual("Sound of Winter", modified_objects[0].instance.title)
-        self.assertEqual("1998-01-08", modified_objects[0].instance.publish_date)
-        self.assertEqual(self.author_john, modified_objects[0].instance.author)
-        self.assertEqual({}, modified_objects[0].changed_values)
```

### Comparing `django-bulk-tracker-0.0.6/tests/test_update_signal.py` & `django-bulk-tracker-0.0.7/tests/test_update_signal.py`

 * *Files identical despite different names*

