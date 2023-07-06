# Comparing `tmp/django-tree-0.5.1.tar.gz` & `tmp/django-tree-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tree-0.5.1.tar", last modified: Thu Jul  6 00:47:50 2023, max compression
+gzip compressed data, was "dist/django-tree-0.5.2.tar", last modified: Thu Jul  6 14:18:28 2023, max compression
```

## Comparing `django-tree-0.5.1.tar` & `django-tree-0.5.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9500 2023-07-06 00:47:09.000000 django-tree-0.5.1/README.rst
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/benchmark/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/benchmark/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.1/benchmark/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.1/benchmark/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/router.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.1/benchmark/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/utils.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.1/requirements.txt
--rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.1/setup.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/requires.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/top_level.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12446 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.1/django_tree.egg-info/not-zip-safe
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.1/MANIFEST.in
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tests/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tests/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/migrations/0003_test_migrations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.1/tests/migrations/0002_add_tmp_model.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2494 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tests/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      825 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.1/tests/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    45481 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tests/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12446 2023-07-06 00:47:50.000000 django-tree-0.5.1/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1565 2023-07-06 00:47:08.000000 django-tree-0.5.1/CHANGELOG.rst
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.1/LICENSE
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 00:47:50.000000 django-tree-0.5.1/setup.cfg
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tree/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tree/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/migrations/0002_remove_old_functions.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tree/migrations/__init__.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tree/sql/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9369 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/sql/postgresql.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/sql/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tree/sql/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/transforms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/query.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/signals.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.1/tree/forms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/apps.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/lookups.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/operations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/types.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 00:46:36.000000 django-tree-0.5.1/tree/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4689 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/fields.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9498 2023-07-06 13:11:50.000000 django-tree-0.5.2/README.rst
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/benchmark/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/benchmark/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.2/benchmark/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.2/benchmark/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/router.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.2/benchmark/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/utils.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.2/requirements.txt
+-rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.2/setup.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/requires.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/top_level.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.2/django_tree.egg-info/not-zip-safe
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.2/MANIFEST.in
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tests/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tests/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.2/tests/migrations/0003_test_migrations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.2/tests/migrations/0002_add_tmp_model.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2958 2023-07-06 10:40:54.000000 django-tree-0.5.2/tests/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tests/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      910 2023-07-06 10:40:54.000000 django-tree-0.5.2/tests/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.2/tests/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    48189 2023-07-06 14:12:28.000000 django-tree-0.5.2/tests/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tests/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:18:28.000000 django-tree-0.5.2/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1712 2023-07-06 14:16:01.000000 django-tree-0.5.2/CHANGELOG.rst
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.2/LICENSE
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 14:18:28.000000 django-tree-0.5.2/setup.cfg
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tree/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tree/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/migrations/0002_remove_old_functions.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tree/migrations/__init__.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tree/sql/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9343 2023-07-06 14:10:37.000000 django-tree-0.5.2/tree/sql/postgresql.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/sql/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tree/sql/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/transforms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/query.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/signals.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.2/tree/forms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/apps.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/lookups.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/operations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/types.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 14:16:02.000000 django-tree-0.5.2/tree/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4716 2023-07-06 10:40:54.000000 django-tree-0.5.2/tree/fields.py
```

### Comparing `django-tree-0.5.1/README.rst` & `django-tree-0.5.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     class YourModel(Model, TreeModelMixin):
         name = CharField(max_length=30)
         parent = ForeignKey('self', null=True, blank=True)
         path = PathField()
         public = BooleanField(default=False)
 
         class Meta:
-            ordering = ('path',)
+            ordering = ['path']
 
 Then you need to create the SQL trigger that will automatically update ``path``.
 To do that, create a migration with a dependency
 to the latest django-tree migration and add a ``CreateTreeTrigger`` operation:
 
 .. code:: python
 
@@ -147,15 +147,15 @@
         name = CharField(max_length=30)
         parent = ForeignKey('self', null=True, blank=True)
         position = IntegerField(default=1)
         path = PathField(order_by=['position', 'name'])
         public = BooleanField(default=False)
 
         class Meta:
-            ordering = ('path',)
+            ordering = ['path']
 
 And the corresponding migration:
 
 .. code:: python
 
     from django.db import models, migrations
     from tree.operations import CreateTreeTrigger
```

### Comparing `django-tree-0.5.1/benchmark/migrations/0001_initial.py` & `django-tree-0.5.2/benchmark/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/benchmark/models.py` & `django-tree-0.5.2/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/benchmark/base.py` & `django-tree-0.5.2/benchmark/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/benchmark/utils.py` & `django-tree-0.5.2/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/setup.py` & `django-tree-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/django_tree.egg-info/SOURCES.txt` & `django-tree-0.5.2/django_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/django_tree.egg-info/PKG-INFO` & `django-tree-0.5.2/django_tree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.1
+Version: 0.5.2
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
@@ -92,15 +92,15 @@
             class YourModel(Model, TreeModelMixin):
                 name = CharField(max_length=30)
                 parent = ForeignKey('self', null=True, blank=True)
                 path = PathField()
                 public = BooleanField(default=False)
         
                 class Meta:
-                    ordering = ('path',)
+                    ordering = ['path']
         
         Then you need to create the SQL trigger that will automatically update ``path``.
         To do that, create a migration with a dependency
         to the latest django-tree migration and add a ``CreateTreeTrigger`` operation:
         
         .. code:: python
         
@@ -155,15 +155,15 @@
                 name = CharField(max_length=30)
                 parent = ForeignKey('self', null=True, blank=True)
                 position = IntegerField(default=1)
                 path = PathField(order_by=['position', 'name'])
                 public = BooleanField(default=False)
         
                 class Meta:
-                    ordering = ('path',)
+                    ordering = ['path']
         
         And the corresponding migration:
         
         .. code:: python
         
             from django.db import models, migrations
             from tree.operations import CreateTreeTrigger
```

### Comparing `django-tree-0.5.1/tests/migrations/0003_test_migrations.py` & `django-tree-0.5.2/tests/migrations/0003_test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tests/migrations/0002_add_tmp_model.py` & `django-tree-0.5.2/tests/migrations/0002_add_tmp_model.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tests/migrations/0001_initial.py` & `django-tree-0.5.2/tests/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,23 +35,29 @@
             bases=(TreeModelMixin, models.Model),
         ),
         CreateTreeTrigger('tests.Place'),
         migrations.CreateModel(
             name='Person',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('century', models.SmallIntegerField(null=True, blank=True)),
                 ('first_name', models.CharField(blank=True, max_length=20)),
                 ('last_name', models.CharField(max_length=50)),
                 ('parent', models.ForeignKey('self', blank=True, null=True, on_delete=CASCADE)),
-                ('path', PathField(order_by=['last_name', 'first_name'], size=None)),
+                ('path', PathField(order_by=['century', 'last_name', 'first_name'])),
             ],
             options={
                 'ordering': ['path'],
                 'indexes': [
                     Index(Func(F('path'), 1, function='trim_array'), name='person_path_parent_index'),
-                    Index(F('path__len'), name='person_path_length_index')
+                    Index(F('path__len'), name='person_path_length_index'),
+                    Index(F('path__0_1'), name='person_path_slice_1_index'),
+                    Index(F('path__0_2'), name='person_path_slice_2_index'),
+                    Index(F('path__0_3'), name='person_path_slice_3_index'),
+                    Index(F('path__0_4'), name='person_path_slice_4_index'),
+                    Index(F('path__0_5'), name='person_path_slice_5_index'),
                 ],
             },
             bases=(TreeModelMixin, models.Model),
         ),
         CreateTreeTrigger('tests.Person'),
     ]
```

### Comparing `django-tree-0.5.1/tests/models.py` & `django-tree-0.5.2/tests/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.db.models import CharField, ForeignKey, CASCADE
+from django.db.models import CharField, ForeignKey, CASCADE, SmallIntegerField
 
 from tree.fields import PathField
 from tree.models import TreeModel
 
 
 class Place(TreeModel):
     name = CharField(max_length=50)
@@ -13,17 +13,18 @@
         ordering = ['path', 'name']
         indexes = [
             *PathField.get_indexes('place', 'path'),
         ]
 
 
 class Person(TreeModel):
+    century = SmallIntegerField(null=True, blank=True)
     first_name = CharField(max_length=20, blank=True)
     last_name = CharField(max_length=50)
     parent = ForeignKey('self', null=True, blank=True, on_delete=CASCADE)
-    path = PathField(order_by=['last_name', 'first_name'])
+    path = PathField(order_by=['century', 'last_name', 'first_name'])
 
     class Meta:
         ordering = ['path']
         indexes = [
             *PathField.get_indexes('person', 'path'),
         ]
```

### Comparing `django-tree-0.5.1/tests/base.py` & `django-tree-0.5.2/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1135,95 +1135,155 @@
             cursor.execute('SELECT %s;', [place1.path])
         place2 = self.create_place('place2', place1)
         with connection.cursor() as cursor:
             cursor.execute('SELECT %s;', [place2.path])
 
 
 class MultipleOrderByFieldsTest(TransactionTestCase):
+    maxDiff = None
+
     def setUp(self):
         self.correct_raw_persons_data = [
-            (path(-2), 'Leopold', 'Mozart'),
-            (path(-2, -1), 'Maria Anna', 'Mozart'),
-            (path(-2, 0), 'Wolfgang Amadeus', 'Mozart'),
-            (path(-1.75), '', 'Strauss'),
-            (path(-1.5), 'Johann (father)', 'Strauss'),
-            (path(-1.5, 0), 'Johann (son)', 'Strauss'),
-            (path(-1), 'Piotr Ilyich', 'Tchaikovski'),
-            (path(0), 'Antonio Lucio', 'Vivaldi'),
+            (path(-3), 18, 'Leopold', 'Mozart'),
+            (path(-3, -1), 18, 'Maria Anna', 'Mozart'),
+            (path(-3, 0), 18, 'Wolfgang Amadeus', 'Mozart'),
+            (path(-1), 18, 'Antonio Lucio', 'Vivaldi'),
+            (path(-0.75), 19, 'Johann (father)', 'Strauss'),
+            (path(-0.75, 0), 19, 'Johann (son)', 'Strauss'),
+            (path(-0.5), 19, 'Piotr Ilyich', 'Tchaikovski'),
+            (path(-0.25), 20, '', 'Strauss'),
+            (path(0), None, '', 'Anonymous'),
         ]
         self.correct_persons_data = [
-            (path(0), 'Leopold', 'Mozart'),
-            (path(0, 0), 'Maria Anna', 'Mozart'),
-            (path(0, 1), 'Wolfgang Amadeus', 'Mozart'),
-            (path(1), '', 'Strauss'),
-            (path(2), 'Johann (father)', 'Strauss'),
-            (path(2, 0), 'Johann (son)', 'Strauss'),
-            (path(3), 'Piotr Ilyich', 'Tchaikovski'),
-            (path(4), 'Antonio Lucio', 'Vivaldi'),
+            (path(0), 18, 'Leopold', 'Mozart'),
+            (path(0, 0), 18, 'Maria Anna', 'Mozart'),
+            (path(0, 1), 18, 'Wolfgang Amadeus', 'Mozart'),
+            (path(1), 18, 'Antonio Lucio', 'Vivaldi'),
+            (path(2), 19, 'Johann (father)', 'Strauss'),
+            (path(2, 0), 19, 'Johann (son)', 'Strauss'),
+            (path(3), 19, 'Piotr Ilyich', 'Tchaikovski'),
+            (path(4), 20, '', 'Strauss'),
+            (path(5), None, '', 'Anonymous'),
         ]
+        self.anonymous = Person.objects.create(
+            last_name='Anonymous',
+        )
         self.vivaldi = Person.objects.create(
-            first_name='Antonio Lucio', last_name='Vivaldi',
+            century=18, first_name='Antonio Lucio', last_name='Vivaldi',
         )
         self.wolfgang_mozart = Person.objects.create(
-            first_name='Wolfgang Amadeus', last_name='Mozart',
+            century=18, first_name='Wolfgang Amadeus', last_name='Mozart',
         )
         self.leopold_mozart = Person.objects.create(
-            first_name='Leopold', last_name='Mozart',
+            century=18, first_name='Leopold', last_name='Mozart',
         )
         self.wolfgang_mozart.parent = self.leopold_mozart
         self.wolfgang_mozart.save()
         self.maria_anna_mozart = Person.objects.create(
             parent=self.leopold_mozart,
-            first_name='Maria Anna', last_name='Mozart',
+            century=18, first_name='Maria Anna', last_name='Mozart',
         )
         self.tchaikovski = Person.objects.create(
-            first_name='Piotr Ilyich', last_name='Tchaikovski',
+            century=19, first_name='Piotr Ilyich', last_name='Tchaikovski',
         )
         self.strauss_father = Person.objects.create(
-            first_name='Johann (father)', last_name='Strauss',
+            century=19, first_name='Johann (father)', last_name='Strauss',
         )
         self.strauss_son = Person.objects.create(
             parent=self.strauss_father,
-            first_name='Johann (son)', last_name='Strauss',
+            century=19, first_name='Johann (son)', last_name='Strauss',
         )
         self.strauss = Person.objects.create(
-            last_name='Strauss',
+            century=20, last_name='Strauss',
         )
 
     def assertPersons(self, values, queryset=None, n_queries=1):
         with self.assertNumQueries(n_queries):
             if queryset is None:
                 queryset = Person.objects.all()
             persons = list(queryset)
             self.assertListEqual(
-                [(p.path.value, p.first_name, p.last_name) for p in persons],
+                [
+                    (p.path.value, p.century, p.first_name, p.last_name)
+                    for p in persons
+                ],
                 values,
             )
 
     def test_rebuild(self):
         self.assertPersons(self.correct_raw_persons_data)
         with Person.disabled_tree_trigger():
             for i, person in enumerate(
                 Person.objects.order_by('-last_name', '-first_name')
             ):
-                person.path = [i]
+                # We add 10 to make sure
+                # we do not clash with the existing paths.
+                person.path = [10 + i]
                 person.save()
         self.assertPersons([
-            (path(0), 'Antonio Lucio', 'Vivaldi'),
-            (path(1), 'Piotr Ilyich', 'Tchaikovski'),
-            (path(2), 'Johann (son)', 'Strauss'),
-            (path(3), 'Johann (father)', 'Strauss'),
-            (path(4), '', 'Strauss'),
-            (path(5), 'Wolfgang Amadeus', 'Mozart'),
-            (path(6), 'Maria Anna', 'Mozart'),
-            (path(7), 'Leopold', 'Mozart'),
+            (path(10), 18, 'Antonio Lucio', 'Vivaldi'),
+            (path(11), 19, 'Piotr Ilyich', 'Tchaikovski'),
+            (path(12), 19, 'Johann (son)', 'Strauss'),
+            (path(13), 19, 'Johann (father)', 'Strauss'),
+            (path(14), 20, '', 'Strauss'),
+            (path(15), 18, 'Wolfgang Amadeus', 'Mozart'),
+            (path(16), 18, 'Maria Anna', 'Mozart'),
+            (path(17), 18, 'Leopold', 'Mozart'),
+            (path(18), None, '', 'Anonymous'),
         ])
         Person.rebuild_paths()
         self.assertPersons(self.correct_persons_data)
 
+    def test_clash_on_insert(self):
+        """
+        Checks that instances with exactly the same `order_by` values
+        are assigned different paths on insertion, sorted by primary key.
+        """
+        vivaldi2 = Person.objects.create(
+            century=18, first_name='Antonio Lucio', last_name='Vivaldi',
+        )
+        self.assertGreater(vivaldi2.pk, self.vivaldi.pk)
+        self.assertGreater(vivaldi2.path, self.vivaldi.path)
+        self.assertPersons([
+            (path(-1), 18, 'Antonio Lucio', 'Vivaldi'),
+            (path(-0.875), 18, 'Antonio Lucio', 'Vivaldi'),
+        ], queryset=Person.objects.filter(last_name='Vivaldi'))
+        Person.rebuild_paths()
+        self.assertPersons([
+            (path(1), 18, 'Antonio Lucio', 'Vivaldi'),
+            (path(2), 18, 'Antonio Lucio', 'Vivaldi'),
+        ], queryset=Person.objects.filter(last_name='Vivaldi'))
+
+    def test_clash_on_update(self):
+        """
+        Checks that instances with exactly the same `order_by` values
+        are assigned different paths on update, sorted by primary key.
+        """
+        vivaldi2 = Person.objects.create(
+            century=18, first_name='Some', last_name='Guy',
+        )
+        self.assertGreater(vivaldi2.pk, self.vivaldi.pk)
+        self.assertLess(vivaldi2.path, self.vivaldi.path)
+        self.assertPersons([
+            (path(-4), 18, 'Some', 'Guy'),
+            (path(-1), 18, 'Antonio Lucio', 'Vivaldi'),
+        ], queryset=Person.objects.filter(last_name__in=['Vivaldi', 'Guy']))
+        vivaldi2.first_name = 'Antonio Lucio'
+        vivaldi2.last_name = 'Vivaldi'
+        vivaldi2.save()
+        self.assertPersons([
+            (path(-1), 18, 'Antonio Lucio', 'Vivaldi'),
+            (path(-0.875), 18, 'Antonio Lucio', 'Vivaldi'),
+        ], queryset=Person.objects.filter(last_name='Vivaldi'))
+        Person.rebuild_paths()
+        self.assertPersons([
+            (path(1), 18, 'Antonio Lucio', 'Vivaldi'),
+            (path(2), 18, 'Antonio Lucio', 'Vivaldi'),
+        ], queryset=Person.objects.filter(last_name='Vivaldi'))
+
 
 class QuerySetTest(CommonTest):
     def test_get_descendants(self):
         self.create_all_test_places()
 
         places = Place.objects.filter(name__in=('Normandie', 'Österreich'))
         self.assertPlaces([
```

### Comparing `django-tree-0.5.1/PKG-INFO` & `django-tree-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.1
+Version: 0.5.2
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
@@ -92,15 +92,15 @@
             class YourModel(Model, TreeModelMixin):
                 name = CharField(max_length=30)
                 parent = ForeignKey('self', null=True, blank=True)
                 path = PathField()
                 public = BooleanField(default=False)
         
                 class Meta:
-                    ordering = ('path',)
+                    ordering = ['path']
         
         Then you need to create the SQL trigger that will automatically update ``path``.
         To do that, create a migration with a dependency
         to the latest django-tree migration and add a ``CreateTreeTrigger`` operation:
         
         .. code:: python
         
@@ -155,15 +155,15 @@
                 name = CharField(max_length=30)
                 parent = ForeignKey('self', null=True, blank=True)
                 position = IntegerField(default=1)
                 path = PathField(order_by=['position', 'name'])
                 public = BooleanField(default=False)
         
                 class Meta:
-                    ordering = ('path',)
+                    ordering = ['path']
         
         And the corresponding migration:
         
         .. code:: python
         
             from django.db import models, migrations
             from tree.operations import CreateTreeTrigger
```

### Comparing `django-tree-0.5.1/CHANGELOG.rst` & `django-tree-0.5.2/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.5.2 (2023-07-06)
+==================
+
+Fixes a source of path clashes when the objects have exactly the same values
+for all ``order_by`` columns.
+
 0.5.1 (2023-07-06)
 ==================
 
 Big rewrite using arrays of decimals instead of strings to represent the path.
 
 Performance
 -----------
```

### Comparing `django-tree-0.5.1/LICENSE` & `django-tree-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/migrations/0002_remove_old_functions.py` & `django-tree-0.5.2/tree/migrations/0002_remove_old_functions.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/sql/postgresql.py` & `django-tree-0.5.2/tree/sql/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,28 @@
     meta = model._meta
     pk = meta.pk
     path_field = meta.get_field(path_field_lookup)
     parent_field = path_field.parent_field
     order_by = path_field.order_by
     if not (pk.attname in order_by or pk.name in order_by
             or 'pk' in order_by):
-        order_by += ('pk',)
+        order_by = [*order_by, 'pk']
 
     # TODO: Handle related lookups in `order_by`.
     where_columns = []
     sql_order_by = []
     sql_reversed_order_by = []
     for field_name in order_by:
         descending = field_name[0] == '-'
         if descending:
             field_name = field_name[1:]
         field = (meta.pk if field_name == 'pk'
                  else meta.get_field(field_name))
         quoted_field_name = quote_ident(field.attname)
-        if field_name != 'pk':
-            where_columns.append(quoted_field_name)
+        where_columns.append(quoted_field_name)
         sql_order_by.append(
             f'{quoted_field_name} {"DESC" if descending else "ASC"}'
         )
         sql_reversed_order_by.append(
             f'{quoted_field_name} {"ASC" if descending else "DESC"}'
         )
```

### Comparing `django-tree-0.5.1/tree/sql/base.py` & `django-tree-0.5.2/tree/sql/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/query.py` & `django-tree-0.5.2/tree/query.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/signals.py` & `django-tree-0.5.2/tree/signals.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/apps.py` & `django-tree-0.5.2/tree/apps.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/models.py` & `django-tree-0.5.2/tree/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/lookups.py` & `django-tree-0.5.2/tree/lookups.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/operations.py` & `django-tree-0.5.2/tree/operations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/types.py` & `django-tree-0.5.2/tree/types.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.1/tree/fields.py` & `django-tree-0.5.2/tree/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     def deconstruct(self):
         name, path, args, kwargs = super(PathField, self).deconstruct()
         del kwargs['base_field']
         if not kwargs['editable']:
             del kwargs['editable']
         del kwargs['default']
         del kwargs['null']
+        del kwargs['size']
         if self.order_by != []:
             kwargs['order_by'] = self.order_by
         if self.parent_field_name != 'parent':
             kwargs['parent_field_name'] = self.parent_field_name
         return name, path, args, kwargs
 
     def from_db_value(self, value, expression, connection):
```

