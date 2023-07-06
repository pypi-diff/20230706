# Comparing `tmp/django-tree-0.5.4.tar.gz` & `tmp/django-tree-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tree-0.5.4.tar", last modified: Thu Jul  6 14:53:09 2023, max compression
+gzip compressed data, was "dist/django-tree-0.5.5.tar", last modified: Thu Jul  6 18:43:02 2023, max compression
```

## Comparing `django-tree-0.5.4.tar` & `django-tree-0.5.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9498 2023-07-06 13:11:50.000000 django-tree-0.5.4/README.rst
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/benchmark/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/benchmark/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.4/benchmark/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.4/benchmark/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.4/benchmark/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.4/benchmark/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.4/benchmark/router.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.4/benchmark/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.4/benchmark/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.4/benchmark/utils.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.4/requirements.txt
--rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.4/setup.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/django_tree.egg-info/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 14:53:08.000000 django-tree-0.5.4/django_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 14:53:08.000000 django-tree-0.5.4/django_tree.egg-info/requires.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 14:53:08.000000 django-tree-0.5.4/django_tree.egg-info/top_level.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:53:08.000000 django-tree-0.5.4/django_tree.egg-info/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.4/django_tree.egg-info/not-zip-safe
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 14:53:08.000000 django-tree-0.5.4/django_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.4/MANIFEST.in
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/tests/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/tests/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.4/tests/migrations/0003_test_migrations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.4/tests/migrations/0002_add_tmp_model.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2958 2023-07-06 10:40:54.000000 django-tree-0.5.4/tests/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.4/tests/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      910 2023-07-06 10:40:54.000000 django-tree-0.5.4/tests/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.4/tests/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    48189 2023-07-06 14:12:28.000000 django-tree-0.5.4/tests/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.4/tests/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:53:09.000000 django-tree-0.5.4/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1896 2023-07-06 14:52:54.000000 django-tree-0.5.4/CHANGELOG.rst
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.4/LICENSE
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 14:53:09.000000 django-tree-0.5.4/setup.cfg
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/tree/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/tree/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/migrations/0002_remove_old_functions.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.4/tree/migrations/__init__.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:53:09.000000 django-tree-0.5.4/tree/sql/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9408 2023-07-06 14:52:11.000000 django-tree-0.5.4/tree/sql/postgresql.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/sql/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.4/tree/sql/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/transforms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/query.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/signals.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.4/tree/forms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/apps.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/lookups.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/operations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.4/tree/types.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 14:52:54.000000 django-tree-0.5.4/tree/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4716 2023-07-06 10:40:54.000000 django-tree-0.5.4/tree/fields.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9498 2023-07-06 13:11:50.000000 django-tree-0.5.5/README.rst
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/benchmark/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/benchmark/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3945 2023-07-06 18:27:12.000000 django-tree-0.5.5/benchmark/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.5/benchmark/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/router.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.5/benchmark/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/utils.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.5/requirements.txt
+-rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.5/setup.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/django_tree.egg-info/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/requires.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/top_level.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.5/django_tree.egg-info/not-zip-safe
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.5/MANIFEST.in
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tests/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tests/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.5/tests/migrations/0003_test_migrations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.5/tests/migrations/0002_add_tmp_model.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3010 2023-07-06 18:27:12.000000 django-tree-0.5.5/tests/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tests/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      910 2023-07-06 10:40:54.000000 django-tree-0.5.5/tests/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.5/tests/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    48189 2023-07-06 14:12:28.000000 django-tree-0.5.5/tests/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tests/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 18:43:02.000000 django-tree-0.5.5/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1985 2023-07-06 18:42:44.000000 django-tree-0.5.5/CHANGELOG.rst
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.5/LICENSE
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 18:43:02.000000 django-tree-0.5.5/setup.cfg
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tree/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tree/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/migrations/0002_remove_old_functions.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tree/migrations/__init__.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tree/sql/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9408 2023-07-06 14:52:11.000000 django-tree-0.5.5/tree/sql/postgresql.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/sql/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tree/sql/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/transforms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/query.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/signals.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.5/tree/forms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/apps.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1815 2023-07-06 18:25:02.000000 django-tree-0.5.5/tree/lookups.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/operations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/types.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 18:42:44.000000 django-tree-0.5.5/tree/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4966 2023-07-06 18:27:12.000000 django-tree-0.5.5/tree/fields.py
```

### Comparing `django-tree-0.5.4/README.rst` & `django-tree-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/benchmark/migrations/0001_initial.py` & `django-tree-0.5.5/benchmark/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.db import migrations
 from django.db.models import (
     AutoField, CharField, ForeignKey, PositiveIntegerField, Manager, CASCADE,
-    Index, Func, F,
+    Index, F,
 )
+from django.db.models.expressions import RawSQL
 from mptt.fields import TreeForeignKey
 from tree.fields import PathField
 from tree.operations import CreateTreeTrigger
 
 from ..models import get_random_name
 
 
@@ -39,15 +40,15 @@
                 ('id', AutoField(verbose_name='ID', serialize=False, auto_created=True, primary_key=True)),
                 ('name', CharField(max_length=50, unique=True, default=get_random_name)),
                 ('parent', ForeignKey('self', blank=True, null=True, on_delete=CASCADE)),
                 ('path', PathField(order_by=['name'], db_index=True)),
             ],
             options={
                 'indexes': [
-                    Index(Func(F('path'), 1, function='trim_array'), name='treeplace_path_parent_index'),
+                    Index(RawSQL('path[:array_length(path, 1) - 1]', ()), name='treeplace_path_parent_index'),
                     Index(F('path__level'), name='treeplace_path_level_index'),
                     Index(F('path__0_1'), name='treeplace_path_slice_1_index'),
                     Index(F('path__0_2'), name='treeplace_path_slice_2_index'),
                     Index(F('path__0_3'), name='treeplace_path_slice_3_index'),
                     Index(F('path__0_4'), name='treeplace_path_slice_4_index'),
                     Index(F('path__0_5'), name='treeplace_path_slice_5_index'),
                 ],
```

### Comparing `django-tree-0.5.4/benchmark/models.py` & `django-tree-0.5.5/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/benchmark/base.py` & `django-tree-0.5.5/benchmark/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/benchmark/utils.py` & `django-tree-0.5.5/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/setup.py` & `django-tree-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/django_tree.egg-info/SOURCES.txt` & `django-tree-0.5.5/django_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/django_tree.egg-info/PKG-INFO` & `django-tree-0.5.5/django_tree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.4
+Version: 0.5.5
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
```

### Comparing `django-tree-0.5.4/tests/migrations/0003_test_migrations.py` & `django-tree-0.5.5/tests/migrations/0003_test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tests/migrations/0002_add_tmp_model.py` & `django-tree-0.5.5/tests/migrations/0002_add_tmp_model.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tests/migrations/0001_initial.py` & `django-tree-0.5.5/tests/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.db import models, migrations
-from django.db.models import CASCADE, Index, Func, F
+from django.db.models import CASCADE, Index, F
+from django.db.models.expressions import RawSQL
 
 from tree.fields import PathField
 from tree.models import TreeModelMixin
 from tree.operations import CreateTreeTrigger
 
 
 class Migration(migrations.Migration):
@@ -19,15 +20,15 @@
                 ('name', models.CharField(max_length=50)),
                 ('parent', models.ForeignKey('self', blank=True, null=True, on_delete=CASCADE)),
                 ('path', PathField(order_by=['name'])),
             ],
             options={
                 'ordering': ['path', 'name'],
                 'indexes': [
-                    Index(Func(F('path'), 1, function='trim_array'), name='place_path_parent_index'),
+                    Index(RawSQL('path[:array_length(path, 1) - 1]', ()), name='place_path_parent_index'),
                     Index(F('path__level'), name='place_path_level_index'),
                     Index(F('path__0_1'), name='place_path_slice_1_index'),
                     Index(F('path__0_2'), name='place_path_slice_2_index'),
                     Index(F('path__0_3'), name='place_path_slice_3_index'),
                     Index(F('path__0_4'), name='place_path_slice_4_index'),
                     Index(F('path__0_5'), name='place_path_slice_5_index'),
                 ],
@@ -44,15 +45,15 @@
                 ('last_name', models.CharField(max_length=50)),
                 ('parent', models.ForeignKey('self', blank=True, null=True, on_delete=CASCADE)),
                 ('path', PathField(order_by=['century', 'last_name', 'first_name'])),
             ],
             options={
                 'ordering': ['path'],
                 'indexes': [
-                    Index(Func(F('path'), 1, function='trim_array'), name='person_path_parent_index'),
+                    Index(RawSQL('path[:array_length(path, 1) - 1]', ()), name='person_path_parent_index'),
                     Index(F('path__len'), name='person_path_length_index'),
                     Index(F('path__0_1'), name='person_path_slice_1_index'),
                     Index(F('path__0_2'), name='person_path_slice_2_index'),
                     Index(F('path__0_3'), name='person_path_slice_3_index'),
                     Index(F('path__0_4'), name='person_path_slice_4_index'),
                     Index(F('path__0_5'), name='person_path_slice_5_index'),
                 ],
```

### Comparing `django-tree-0.5.4/tests/models.py` & `django-tree-0.5.5/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tests/base.py` & `django-tree-0.5.5/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/PKG-INFO` & `django-tree-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.4
+Version: 0.5.5
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
```

### Comparing `django-tree-0.5.4/CHANGELOG.rst` & `django-tree-0.5.5/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.5.5 (2023-07-06)
+==================
+
+Fixes another PostgreSQL 12 compatibility issue.
+
 0.5.4 (2023-07-06)
 ==================
 
 Fixes an SQL syntax error.
 
 0.5.3 (2023-07-06)
 ==================
```

### Comparing `django-tree-0.5.4/LICENSE` & `django-tree-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/migrations/0002_remove_old_functions.py` & `django-tree-0.5.5/tree/migrations/0002_remove_old_functions.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/sql/postgresql.py` & `django-tree-0.5.5/tree/sql/postgresql.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/sql/base.py` & `django-tree-0.5.5/tree/sql/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/query.py` & `django-tree-0.5.5/tree/query.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/signals.py` & `django-tree-0.5.5/tree/signals.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/apps.py` & `django-tree-0.5.5/tree/apps.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/models.py` & `django-tree-0.5.5/tree/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/lookups.py` & `django-tree-0.5.5/tree/lookups.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,35 @@
 
 class SiblingOf(Lookup):
     lookup_name = 'sibling_of'
 
     def as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
+        # TODO: Simplify using `trim_array` once support for PostgreSQL < 14
+        #       is dropped.
         return (
-            'trim_array(%s, 1) = trim_array(%s, 1)' % (lhs, rhs),
-            lhs_params + rhs_params,
+            '(%s)[:array_length(%s, 1) - 1] = (%s)[:array_length(%s, 1) - 1]'
+            % (lhs, lhs, rhs, rhs),
+            lhs_params + lhs_params + rhs_params + rhs_params,
         )
 
 
 class ChildOf(Lookup):
     lookup_name = 'child_of'
 
     def as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
-        return 'trim_array(%s, 1) = %s' % (lhs, rhs), lhs_params + rhs_params
+        # TODO: Simplify using `trim_array` once support for PostgreSQL < 14
+        #       is dropped.
+        return (
+            '(%s)[:array_length(%s, 1) - 1] = %s' % (lhs, lhs, rhs),
+            lhs_params + lhs_params + rhs_params
+        )
 
 
 class DescendantOf(Lookup):
     lookup_name = 'descendant_of'
 
     def as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
```

### Comparing `django-tree-0.5.4/tree/operations.py` & `django-tree-0.5.5/tree/operations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/types.py` & `django-tree-0.5.5/tree/types.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.4/tree/fields.py` & `django-tree-0.5.5/tree/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from contextlib import contextmanager
 
 from django.contrib.postgres.fields import ArrayField
 from django.core.exceptions import ImproperlyConfigured
 from django.db import DEFAULT_DB_ALIAS, connections, transaction
 from django.db.models import DecimalField, Index, Func, F
+from django.db.models.expressions import RawSQL
 from django.utils.translation import ugettext_lazy as _
 
 from .sql import postgresql
 from .types import Path
 
 
 # TODO: Handle ManyToManyField('self') instead of ForeignKey('self').
@@ -23,15 +24,20 @@
         cls,
         table_name: str,
         path_field_name: str,
         max_indexed_level: int = 5,
     ):
         return [
             Index(
-                Func(F(path_field_name), 1, function='trim_array'),
+                # TODO: Simplify using `trim_array`
+                #       once support for PostgreSQL < 14 is dropped.
+                RawSQL(
+                    f'{path_field_name}[:array_length({path_field_name}, 1) - 1]',
+                    ()
+                ),
                 name=f'{table_name}_{path_field_name}_parent_index',
             ),
             Index(
                 F(f'{path_field_name}__level'),
                 name=f'{table_name}_{path_field_name}_level_index',
             ),
             *[
```

