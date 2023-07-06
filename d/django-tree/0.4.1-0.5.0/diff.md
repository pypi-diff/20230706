# Comparing `tmp/django-tree-0.4.1.tar.gz` & `tmp/django-tree-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tree-0.4.1.tar", last modified: Sun Jun 27 19:41:25 2021, max compression
+gzip compressed data, was "dist/django-tree-0.5.0.tar", last modified: Thu Jul  6 00:43:19 2023, max compression
```

## Comparing `django-tree-0.4.1.tar` & `django-tree-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     8885 2018-03-23 16:18:47.000000 django-tree-0.4.1/README.rst
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/benchmark/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/benchmark/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3208 2018-03-23 15:51:15.000000 django-tree-0.4.1/benchmark/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.4.1/benchmark/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1557 2018-03-23 22:12:31.000000 django-tree-0.4.1/benchmark/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.4.1/benchmark/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.4.1/benchmark/router.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    27850 2018-03-23 22:41:30.000000 django-tree-0.4.1/benchmark/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.4.1/benchmark/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.4.1/benchmark/utils.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2021-06-27 19:39:46.000000 django-tree-0.4.1/requirements.txt
--rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1117 2018-02-09 14:18:58.000000 django-tree-0.4.1/setup.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/django_tree.egg-info/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      954 2021-06-27 19:41:25.000000 django-tree-0.4.1/django_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2021-06-27 19:41:25.000000 django-tree-0.4.1/django_tree.egg-info/requires.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2021-06-27 19:41:25.000000 django-tree-0.4.1/django_tree.egg-info/top_level.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    11493 2021-06-27 19:41:25.000000 django-tree-0.4.1/django_tree.egg-info/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.4.1/django_tree.egg-info/not-zip-safe
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2021-06-27 19:41:25.000000 django-tree-0.4.1/django_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.4.1/MANIFEST.in
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/tests/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/tests/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      709 2018-03-23 15:51:15.000000 django-tree-0.4.1/tests/migrations/0003_test_migrations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.4.1/tests/migrations/0002_add_tmp_model.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      913 2018-03-23 15:51:15.000000 django-tree-0.4.1/tests/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.4.1/tests/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      427 2018-03-23 21:24:39.000000 django-tree-0.4.1/tests/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.4.1/tests/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    36214 2018-03-24 04:27:49.000000 django-tree-0.4.1/tests/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.4.1/tests/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    11493 2021-06-27 19:41:25.000000 django-tree-0.4.1/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.4.1/CHANGELOG.rst
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.4.1/LICENSE
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2021-06-27 19:41:25.000000 django-tree-0.4.1/setup.cfg
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/tree/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/tree/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      178 2018-02-09 14:18:58.000000 django-tree-0.4.1/tree/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.4.1/tree/migrations/__init__.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2021-06-27 19:41:25.000000 django-tree-0.4.1/tree/sql/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    14028 2018-03-24 04:18:59.000000 django-tree-0.4.1/tree/sql/postgresql.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      441 2018-03-23 15:51:15.000000 django-tree-0.4.1/tree/sql/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.4.1/tree/sql/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      623 2018-03-23 15:51:15.000000 django-tree-0.4.1/tree/transforms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1456 2018-03-23 22:32:26.000000 django-tree-0.4.1/tree/query.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.4.1/tree/forms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      485 2018-03-23 15:51:15.000000 django-tree-0.4.1/tree/apps.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4911 2018-03-23 21:58:13.000000 django-tree-0.4.1/tree/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1453 2018-03-23 15:51:15.000000 django-tree-0.4.1/tree/lookups.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5563 2018-03-23 15:51:15.000000 django-tree-0.4.1/tree/operations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6951 2021-06-27 18:12:58.000000 django-tree-0.4.1/tree/types.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2021-06-27 19:40:31.000000 django-tree-0.4.1/tree/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4292 2021-06-27 18:19:40.000000 django-tree-0.4.1/tree/fields.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9393 2023-07-06 00:41:03.000000 django-tree-0.5.0/README.rst
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/benchmark/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/benchmark/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.0/benchmark/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.0/benchmark/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/router.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.0/benchmark/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/utils.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.0/requirements.txt
+-rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1117 2018-02-09 14:18:58.000000 django-tree-0.5.0/setup.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/requires.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/top_level.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12113 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.0/django_tree.egg-info/not-zip-safe
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.0/MANIFEST.in
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tests/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tests/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/migrations/0003_test_migrations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.0/tests/migrations/0002_add_tmp_model.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2494 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tests/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      825 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.0/tests/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    45481 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tests/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12113 2023-07-06 00:43:19.000000 django-tree-0.5.0/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1565 2023-07-06 00:41:33.000000 django-tree-0.5.0/CHANGELOG.rst
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.0/LICENSE
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 00:43:19.000000 django-tree-0.5.0/setup.cfg
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tree/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tree/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/migrations/0002_remove_old_functions.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tree/migrations/__init__.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tree/sql/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9369 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/sql/postgresql.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/sql/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tree/sql/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/transforms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/query.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/signals.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.0/tree/forms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/apps.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/lookups.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/operations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/types.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-05 21:45:26.000000 django-tree-0.5.0/tree/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4689 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/fields.py
```

### Comparing `django-tree-0.4.1/README.rst` & `django-tree-0.5.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 .. image:: http://img.shields.io/travis/BertrandBordage/django-tree/master.svg?style=flat-square
    :target: https://travis-ci.org/BertrandBordage/django-tree
 
 .. image:: http://img.shields.io/coveralls/BertrandBordage/django-tree/master.svg?style=flat-square
    :target: https://coveralls.io/r/BertrandBordage/django-tree?branch=master
 
-**In alpha, it can’t be used yet in production.**
+**In beta, it can’t be used yet in production.**
 
 This tool works in a very similar way to **django-mptt**
 and **django-treebeard**, however it’s so different in conception
 that it was better and faster to start from scratch
 than to rewrite the existing solutions.
 
 Compared to these solutions, django-tree aims to have these advantages
@@ -33,14 +33,28 @@
 - faster for all operations
 
 However, there is nothing groundbreaking here: this is only the result of
 a proper use of the latest Django improvements, combined with a good knowledge
 of SQL.
 
 
+Benchmark
+---------
+
+`The detailed benchmark <benchmark/results/results.rst>`_ gives a good idea
+on how well django-tree performs compared to other Django solutions.
+All that while being simpler to use, more robust and fully generalized to raw SQL, bulk etc.
+
+A few noteworthy extracts of the benchmark (less is better):
+
+.. image:: benchmark/results/postgresql_-_Create_all_objects.svg
+.. image:: benchmark/results/postgresql_-_Rebuild_paths.svg
+.. image:: benchmark/results/postgresql_-_Create_[root].svg
+
+
 Installation
 ------------
 
 Django-tree requires Django 1.8, 1.11 or 2.0 and Python 2 or 3.
 For the moment, django-tree is only for PostgreSQL.
 It will be adapted in the future for other databases.
```

### Comparing `django-tree-0.4.1/benchmark/migrations/0001_initial.py` & `django-tree-0.5.0/benchmark/migrations/0001_initial.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.db import migrations
 from django.db.models import (
     AutoField, CharField, ForeignKey, PositiveIntegerField, Manager, CASCADE,
+    Index, Func, F,
 )
 from mptt.fields import TreeForeignKey
 from tree.fields import PathField
 from tree.operations import CreateTreeTrigger
 
 from ..models import get_random_name
 
@@ -34,16 +35,27 @@
 
         migrations.CreateModel(
             name='TreePlace',
             fields=[
                 ('id', AutoField(verbose_name='ID', serialize=False, auto_created=True, primary_key=True)),
                 ('name', CharField(max_length=50, unique=True, default=get_random_name)),
                 ('parent', ForeignKey('self', blank=True, null=True, on_delete=CASCADE)),
-                ('path', PathField(order_by=('name',), db_index=True)),
+                ('path', PathField(order_by=['name'], db_index=True)),
             ],
+            options={
+                'indexes': [
+                    Index(Func(F('path'), 1, function='trim_array'), name='treeplace_path_parent_index'),
+                    Index(F('path__level'), name='treeplace_path_level_index'),
+                    Index(F('path__0_1'), name='treeplace_path_slice_1_index'),
+                    Index(F('path__0_2'), name='treeplace_path_slice_2_index'),
+                    Index(F('path__0_3'), name='treeplace_path_slice_3_index'),
+                    Index(F('path__0_4'), name='treeplace_path_slice_4_index'),
+                    Index(F('path__0_5'), name='treeplace_path_slice_5_index'),
+                ],
+            },
         ),
         CreateTreeTrigger('TreePlace'),
 
         migrations.CreateModel(
             name='TreebeardALPlace',
             fields=[
                 ('id', AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
```

### Comparing `django-tree-0.4.1/benchmark/models.py` & `django-tree-0.5.0/benchmark/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,20 @@
         order_insertion_by = ('name',)
 
 
 class TreePlace(TreeModel):
     name = CharField(max_length=50, unique=True, default=get_random_name)
     parent = ForeignKey('self', null=True, blank=True, related_name='children',
                         on_delete=CASCADE)
-    path = PathField(order_by=('name',), db_index=True)
+    path = PathField(order_by=['name'], db_index=True)
+
+    class Meta:
+        indexes = [
+            *PathField.get_indexes('treeplace', 'path'),
+        ]
 
 
 class TreebeardALPlace(AL_Node):
     name = CharField(max_length=50, unique=True, default=get_random_name)
     parent = ForeignKey('self', null=True, blank=True, related_name='children',
                         on_delete=CASCADE)
     node_order_by = ('name',)
```

### Comparing `django-tree-0.4.1/benchmark/base.py` & `django-tree-0.5.0/benchmark/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import print_function
 from collections import Iterable
 import os
 from time import time
+from typing import Type, List, Optional
 
 from django.db import connections, router, transaction
-from django.db.models import Max, F
+from django.db.models import Max, F, Model
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FuncFormatter
 import pandas as pd
 from tqdm import tqdm
 
 from .models import (
     TreePlace, MPTTPlace, TreebeardMPPlace, TreebeardNSPlace, TreebeardALPlace,
@@ -39,15 +40,23 @@
     ticks_formatters = {
         DISK_USAGE: BYTES_FORMATTER,
         READ_LATENCY: SECONDS_FORMATTER,
         WRITE_LATENCY: SECONDS_FORMATTER,
     }
     results_path = 'benchmark/results/'
 
-    def __init__(self):
+    def __init__(
+        self,
+        run_django_tree_only: bool = False,
+        db_optimization_interval: int = 100,
+        selected_tests: Optional[List[str]] = None,
+    ):
+        self.run_django_tree_only = run_django_tree_only
+        self.db_optimization_interval = db_optimization_interval
+        self.selected_tests = selected_tests
         self.data = []
         self.router = router.routers[0]
 
         self.rows_count = 0
         n = 1
         for i in self.siblings_per_level:
             n *= i
@@ -114,30 +123,36 @@
         def inner(test_class):
             for model in models:
                 cls.tests[(name, model, y_label)] = test_class
             return test_class
 
         return inner
 
+    def skip_test(self, test_name: str) -> bool:
+        return self.selected_tests and test_name not in self.selected_tests
+
     def run_tests(self, tested_model, count):
         connection = connections[self.current_db_alias]
         for (test_name, model, y_label), test_class in self.tests.items():
-            if model is not tested_model:
+            if model is not tested_model or self.skip_test(test_name):
                 continue
             benchmark_test = test_class(self, model)
-            with transaction.atomic(using=self.current_db_alias):
-                try:
-                    benchmark_test.setup()
-                except SkipTest:
-                    value = elapsed_time = None
+            try:
+                benchmark_test.setup()
+            except SkipTest:
+                value = elapsed_time = None
+            else:
+                start = time()
+                if benchmark_test.rollback:
+                    with transaction.atomic(using=self.current_db_alias):
+                        value = benchmark_test.run()
+                        connection.needs_rollback = True
                 else:
-                    start = time()
                     value = benchmark_test.run()
-                    elapsed_time = time() - start
-                connection.needs_rollback = True
+                elapsed_time = time() - start
             if value is None:
                 value = elapsed_time
             self.add_data(model, test_name, count, value, y_label=y_label)
 
     def plot(self, df, database_name, test_name, y_label):
         means = df.rolling(max(df.index.max() // 20, 1)).mean()
         ax = means.plot(
@@ -160,22 +175,34 @@
         filename = ('%s - %s.svg' % (database_name,
                                      test_name)).replace(' ', '_')
         plt.savefig(
             os.path.join(self.results_path, filename),
             bbox_extra_artists=(legend,), bbox_inches='tight',
         )
 
+    def force_update_db_stats_and_indexes(self, model: Type[Model]):
+        with connections[self.current_db_alias].cursor() as cursor:
+            # This makes sure the table statistics are
+            # up to date and the disk usage is optimised.
+            cursor.execute(
+                'VACUUM FULL ANALYZE "%s";' % model._meta.db_table)
+            # This makes sure the indexes are up to date.
+            cursor.execute(
+                'REINDEX TABLE "%s";' % model._meta.db_table)
+
     def run(self):
         self.create_databases()
 
         for db_alias in connections:
             self.current_db_alias = db_alias
             connection = connections[db_alias]
 
             for model in sorted(self.models, key=lambda m: m.__name__):
+                if self.run_django_tree_only and model is not TreePlace:
+                    continue
                 print('-' * 50)
                 print('%s on %s' % (self.models[model], connection.vendor))
                 it = self.populate_database(model)
                 progress = tqdm(it, total=self.rows_count)
                 elapsed_time = 0.0
                 while True:
                     try:
@@ -183,29 +210,29 @@
                         count = next(it)
                         elapsed_time = time() - start
                     except StopIteration:
                         break
                     progress.update(count - progress.n)
                     self.add_data(model, 'Create all objects', count,
                                   elapsed_time, y_label=WRITE_LATENCY)
-                    with connection.cursor() as cursor:
-                        # This makes sure the table statistics are
-                        # up to date and the disk usage is optimised.
-                        cursor.execute(
-                            'VACUUM ANALYZE "%s";' % model._meta.db_table)
-                        # This makes sure the indexes are up to date.
-                        cursor.execute(
-                            'REINDEX TABLE "%s";' % model._meta.db_table)
+                    if count % self.db_optimization_interval == 0:
+                        self.force_update_db_stats_and_indexes(model)
                     self.run_tests(model, count)
                 # We delete the objects to avoid impacting
                 # the following tests and to clear some disk space.
                 model.objects.all().delete()
 
-        df = pd.DataFrame(self.data)
-        df.to_csv(os.path.join(self.results_path, 'data.csv'), index=False)
+        csv_path = os.path.join(self.results_path, 'data.csv')
+        if self.run_django_tree_only:
+            df = pd.read_csv(csv_path)
+            df = df[df['Implementation'] != self.models[TreePlace]]
+            df = df.append(pd.DataFrame(self.data))
+        else:
+            df = pd.DataFrame(self.data)
+        df.to_csv(csv_path, index=False)
 
         stats_df = df.set_index(['Database', 'Test name', 'Count'])
         stats_df.sort_index(inplace=True)
         group_by = stats_df.groupby(level=[0, 1, 2])
         min_values_series = group_by.min()['Value']
         max_values_series = group_by.max()['Value']
         stats_df['Value'] = ((stats_df['Value'] - min_values_series)
@@ -216,40 +243,48 @@
                              .apply(lambda f: '%.1f / 20' % f))
         stats_df.to_html(os.path.join(self.results_path, 'stats.html'),
                          header=False)
 
         df.set_index('Count', inplace=True)
         for database_name in df['Database'].unique():
             for test_name in df['Test name'].unique():
+                if self.skip_test(test_name):
+                    continue
                 sub_df = df[(df['Database'] == database_name)
                             & (df['Test name'] == test_name)]
                 y_labels = sub_df['Y label'].unique()
                 assert len(y_labels) == 1
                 sub_df = sub_df.pivot(columns='Implementation', values='Value')
                 self.plot(sub_df, database_name, test_name, y_labels[0])
 
 
 class BenchmarkTest:
+    rollback: bool = False
+
     def __init__(self, benchmark, model):
         self.benchmark = benchmark
         self.model = model
 
     def setup(self):
         pass
 
     def run(self):
         raise NotImplementedError
 
 
+class BenchmarkWriteTest(BenchmarkTest):
+    rollback = True
+
+
 @Benchmark.register_test('Table disk usage (including indexes)',
                          y_label=DISK_USAGE)
 class TestDiskUsage(BenchmarkTest):
     def run(self):
         with connections[self.benchmark.current_db_alias].cursor() as cursor:
-            cursor.execute("SELECT pg_relation_size('%s');"
+            cursor.execute("SELECT pg_total_relation_size('%s');"
                            % self.model._meta.db_table)
             return cursor.fetchone()[0]
 
 
 class GetRootMixin:
     def setup(self):
         qs = self.model._default_manager.all()
@@ -270,15 +305,15 @@
             if isinstance(descendants, list):
                 descendants = [d.pk for d in descendants]
             qs = qs.exclude(pk__in=descendants)
 
         if self.model is MPTTPlace:
             qs = qs.filter(level=1)
         elif self.model is TreePlace:
-            qs = qs.filter(path__level=2)
+            qs = qs.filter(path__len=2)
         elif self.model is TreebeardALPlace:
             qs = qs.filter(parent__isnull=False, parent__parent__isnull=True)
         else:
             qs = qs.filter(depth=2)
         try:
             self.branch = qs[qs.count() // 2]
         except IndexError:
@@ -692,213 +727,257 @@
 
 #
 # Rebuild
 #
 
 
 @Benchmark.register_test('Rebuild paths', MPTTPlace, y_label=WRITE_LATENCY)
-class TestRebuildPaths(BenchmarkTest):
+class TestRebuildPaths(BenchmarkWriteTest):
     def run(self):
         self.model._default_manager.rebuild()
 
 
 @Benchmark.register_test('Rebuild paths', TreePlace, y_label=WRITE_LATENCY)
-class TestRebuildPaths(BenchmarkTest):
+class TestRebuildPaths(BenchmarkWriteTest):
     def run(self):
         self.model.rebuild_paths()
 
 
 @Benchmark.register_test('Rebuild paths', (TreebeardALPlace, TreebeardNSPlace),
                          y_label=WRITE_LATENCY)
-class TestRebuildPaths(BenchmarkTest):
+class TestRebuildPaths(BenchmarkWriteTest):
     def setup(self):
         raise SkipTest
 
 
 @Benchmark.register_test('Rebuild paths', TreebeardMPPlace,
                          y_label=WRITE_LATENCY)
-class TestRebuildPaths(BenchmarkTest):
+class TestRebuildPaths(BenchmarkWriteTest):
     def run(self):
         self.model.fix_tree()
 
 
 #
 # Create
 #
 
 
 @Benchmark.register_test(
     'Create [root]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestCreateRoot(BenchmarkTest):
+class TestCreateRoot(BenchmarkWriteTest):
     def run(self):
         self.model.objects.create()
 
 
 @Benchmark.register_test(
     'Create [root]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestCreateRoot(BenchmarkTest):
+class TestCreateRoot(BenchmarkWriteTest):
     def run(self):
         self.model.add_root()
 
 
 @Benchmark.register_test(
     'Create [branch]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestCreateBranch(GetRootMixin, BenchmarkTest):
+class TestCreateBranch(GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.model.objects.create(parent=self.root)
 
 
 @Benchmark.register_test(
     'Create [branch]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestCreateBranch(GetRootMixin, BenchmarkTest):
+class TestCreateBranch(GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.root.add_child()
 
 
 @Benchmark.register_test(
     'Create [leaf]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestCreateLeaf(GetLeafMixin, BenchmarkTest):
+class TestCreateLeaf(GetLeafMixin, BenchmarkWriteTest):
     def run(self):
         self.model.objects.create(parent=self.leaf)
 
 
 @Benchmark.register_test(
     'Create [leaf]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestCreateLeaf(GetLeafMixin, BenchmarkTest):
+class TestCreateLeaf(GetLeafMixin, BenchmarkWriteTest):
     def run(self):
         self.leaf.add_child()
 
 
 #
+# Save without any change
+#
+
+
+@Benchmark.register_test('Save without change [root]', y_label=WRITE_LATENCY)
+class TestSaveRootWithoutChange(GetRootMixin, BenchmarkWriteTest):
+    def run(self):
+        self.root.save()
+
+
+@Benchmark.register_test('Save without change [branch]', y_label=WRITE_LATENCY)
+class TestSaveBranchWithoutChange(GetBranchMixin, BenchmarkWriteTest):
+    def run(self):
+        self.branch.save()
+
+
+@Benchmark.register_test('Save without change [leaf]', y_label=WRITE_LATENCY)
+class TestSaveLeafWithoutChange(GetLeafMixin, BenchmarkWriteTest):
+    def run(self):
+        self.leaf.save()
+
+
+#
 # Move
 #
 
 
+@Benchmark.register_test('Move [same root path]', y_label=WRITE_LATENCY)
+class TestMoveSameRootPath(GetRootMixin, BenchmarkWriteTest):
+    def run(self):
+        self.root.name += ' 2'
+        self.root.save()
+
+
+@Benchmark.register_test('Move [same branch path]', y_label=WRITE_LATENCY)
+class TestMoveSameBranchPath(GetBranchMixin, BenchmarkWriteTest):
+    def run(self):
+        self.branch.name += ' 2'
+        self.branch.save()
+
+
+@Benchmark.register_test('Move [same leaf path]', y_label=WRITE_LATENCY)
+class TestMoveSameLeafPath(GetLeafMixin, BenchmarkWriteTest):
+    def run(self):
+        self.leaf.name += ' 2'
+        self.leaf.save()
+
+
 @Benchmark.register_test(
     'Move [root to branch]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestMoveRootToBranch(GetBranchMixin, GetRootMixin, BenchmarkTest):
+class TestMoveRootToBranch(GetBranchMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.root.parent = self.branch
         self.root.save()
 
 
 @Benchmark.register_test(
     'Move [root to branch]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestMoveRootToBranch(GetBranchMixin, GetRootMixin, BenchmarkTest):
+class TestMoveRootToBranch(GetBranchMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.root.move(self.branch, pos='sorted-child')
 
 
 @Benchmark.register_test(
     'Move [root to leaf]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestMoveRootToLeaf(GetLeafMixin, GetRootMixin, BenchmarkTest):
+class TestMoveRootToLeaf(GetLeafMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.root.parent = self.leaf
         self.root.save()
 
 
 @Benchmark.register_test(
     'Move [root to leaf]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestMoveRootToLeaf(GetLeafMixin, GetRootMixin, BenchmarkTest):
+class TestMoveRootToLeaf(GetLeafMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.root.move(self.leaf, pos='sorted-child')
 
 
 @Benchmark.register_test(
     'Move [branch to root]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestMoveBranchToRoot(GetBranchMixin, BenchmarkTest):
+class TestMoveBranchToRoot(GetBranchMixin, BenchmarkWriteTest):
     def run(self):
         self.branch.parent = None
         self.branch.save()
 
 
 @Benchmark.register_test(
     'Move [branch to root]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestMoveBranchToRoot(GetBranchMixin, GetRootMixin, BenchmarkTest):
+class TestMoveBranchToRoot(GetBranchMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.branch.move(self.root, pos='sorted-sibling')
 
 
 @Benchmark.register_test(
     'Move [branch to leaf]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestMoveBranchToLeaf(GetLeafMixin, GetBranchMixin, BenchmarkTest):
+class TestMoveBranchToLeaf(GetLeafMixin, GetBranchMixin, BenchmarkWriteTest):
     def run(self):
         self.branch.parent = self.leaf
         self.branch.save()
 
 
 @Benchmark.register_test(
     'Move [branch to leaf]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestMoveBranchToLeaf(GetLeafMixin, GetBranchMixin, BenchmarkTest):
+class TestMoveBranchToLeaf(GetLeafMixin, GetBranchMixin, BenchmarkWriteTest):
     def run(self):
         self.branch.move(self.leaf, pos='sorted-child')
 
 
 @Benchmark.register_test(
     'Move [leaf to root]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestMoveLeafToRoot(GetLeafMixin, BenchmarkTest):
+class TestMoveLeafToRoot(GetLeafMixin, BenchmarkWriteTest):
     def run(self):
         self.leaf.parent = None
         self.leaf.save()
 
 
 @Benchmark.register_test(
     'Move [leaf to root]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestMoveLeafToRoot(GetLeafMixin, GetRootMixin, BenchmarkTest):
+class TestMoveLeafToRoot(GetLeafMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.leaf.move(self.root, pos='sorted-sibling')
 
 
 @Benchmark.register_test(
     'Move [leaf to branch]',
     (MPTTPlace, TreePlace, TreebeardALPlace), y_label=WRITE_LATENCY)
-class TestMoveLeafToBranch(GetLeafMixin, GetRootMixin, BenchmarkTest):
+class TestMoveLeafToBranch(GetLeafMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.leaf.parent = self.root
         self.leaf.save()
 
 
 @Benchmark.register_test(
     'Move [leaf to branch]',
     (TreebeardMPPlace, TreebeardNSPlace), y_label=WRITE_LATENCY)
-class TestMoveLeafToBranch(GetLeafMixin, GetRootMixin, BenchmarkTest):
+class TestMoveLeafToBranch(GetLeafMixin, GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.leaf.move(self.root, pos='sorted-child')
 
 
 #
 # Delete
 #
 
 
 @Benchmark.register_test('Delete [root]', y_label=WRITE_LATENCY)
-class TestDeleteRoot(GetRootMixin, BenchmarkTest):
+class TestDeleteRoot(GetRootMixin, BenchmarkWriteTest):
     def run(self):
         self.root.delete()
 
 
 @Benchmark.register_test('Delete [branch]', y_label=WRITE_LATENCY)
-class TestDeleteBranch(GetBranchMixin, BenchmarkTest):
+class TestDeleteBranch(GetBranchMixin, BenchmarkWriteTest):
     def run(self):
         self.branch.delete()
 
 
 @Benchmark.register_test('Delete [leaf]', y_label=WRITE_LATENCY)
-class TestDeleteLeaf(GetLeafMixin, BenchmarkTest):
+class TestDeleteLeaf(GetLeafMixin, BenchmarkWriteTest):
     def run(self):
         self.leaf.delete()
```

### Comparing `django-tree-0.4.1/benchmark/utils.py` & `django-tree-0.5.0/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.4.1/setup.py` & `django-tree-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.4.1/django_tree.egg-info/SOURCES.txt` & `django-tree-0.5.0/django_tree.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 tree/apps.py
 tree/fields.py
 tree/forms.py
 tree/lookups.py
 tree/models.py
 tree/operations.py
 tree/query.py
+tree/signals.py
 tree/transforms.py
 tree/types.py
 tree/migrations/0001_initial.py
+tree/migrations/0002_remove_old_functions.py
 tree/migrations/__init__.py
 tree/sql/__init__.py
 tree/sql/base.py
 tree/sql/postgresql.py
```

### Comparing `django-tree-0.4.1/django_tree.egg-info/PKG-INFO` & `django-tree-0.5.0/django_tree.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.4.1
+Version: 0.5.0
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
@@ -16,15 +16,15 @@
         
         .. image:: http://img.shields.io/travis/BertrandBordage/django-tree/master.svg?style=flat-square
            :target: https://travis-ci.org/BertrandBordage/django-tree
         
         .. image:: http://img.shields.io/coveralls/BertrandBordage/django-tree/master.svg?style=flat-square
            :target: https://coveralls.io/r/BertrandBordage/django-tree?branch=master
         
-        **In alpha, it can’t be used yet in production.**
+        **In beta, it can’t be used yet in production.**
         
         This tool works in a very similar way to **django-mptt**
         and **django-treebeard**, however it’s so different in conception
         that it was better and faster to start from scratch
         than to rewrite the existing solutions.
         
         Compared to these solutions, django-tree aims to have these advantages
@@ -41,14 +41,28 @@
         - faster for all operations
         
         However, there is nothing groundbreaking here: this is only the result of
         a proper use of the latest Django improvements, combined with a good knowledge
         of SQL.
         
         
+        Benchmark
+        ---------
+        
+        `The detailed benchmark <benchmark/results/results.rst>`_ gives a good idea
+        on how well django-tree performs compared to other Django solutions.
+        All that while being simpler to use, more robust and fully generalized to raw SQL, bulk etc.
+        
+        A few noteworthy extracts of the benchmark (less is better):
+        
+        .. image:: benchmark/results/postgresql_-_Create_all_objects.svg
+        .. image:: benchmark/results/postgresql_-_Rebuild_paths.svg
+        .. image:: benchmark/results/postgresql_-_Create_[root].svg
+        
+        
         Installation
         ------------
         
         Django-tree requires Django 1.8, 1.11 or 2.0 and Python 2 or 3.
         For the moment, django-tree is only for PostgreSQL.
         It will be adapted in the future for other databases.
```

### Comparing `django-tree-0.4.1/tests/migrations/0002_add_tmp_model.py` & `django-tree-0.5.0/tests/migrations/0002_add_tmp_model.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.4.1/PKG-INFO` & `django-tree-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.4.1
+Version: 0.5.0
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
@@ -16,15 +16,15 @@
         
         .. image:: http://img.shields.io/travis/BertrandBordage/django-tree/master.svg?style=flat-square
            :target: https://travis-ci.org/BertrandBordage/django-tree
         
         .. image:: http://img.shields.io/coveralls/BertrandBordage/django-tree/master.svg?style=flat-square
            :target: https://coveralls.io/r/BertrandBordage/django-tree?branch=master
         
-        **In alpha, it can’t be used yet in production.**
+        **In beta, it can’t be used yet in production.**
         
         This tool works in a very similar way to **django-mptt**
         and **django-treebeard**, however it’s so different in conception
         that it was better and faster to start from scratch
         than to rewrite the existing solutions.
         
         Compared to these solutions, django-tree aims to have these advantages
@@ -41,14 +41,28 @@
         - faster for all operations
         
         However, there is nothing groundbreaking here: this is only the result of
         a proper use of the latest Django improvements, combined with a good knowledge
         of SQL.
         
         
+        Benchmark
+        ---------
+        
+        `The detailed benchmark <benchmark/results/results.rst>`_ gives a good idea
+        on how well django-tree performs compared to other Django solutions.
+        All that while being simpler to use, more robust and fully generalized to raw SQL, bulk etc.
+        
+        A few noteworthy extracts of the benchmark (less is better):
+        
+        .. image:: benchmark/results/postgresql_-_Create_all_objects.svg
+        .. image:: benchmark/results/postgresql_-_Rebuild_paths.svg
+        .. image:: benchmark/results/postgresql_-_Create_[root].svg
+        
+        
         Installation
         ------------
         
         Django-tree requires Django 1.8, 1.11 or 2.0 and Python 2 or 3.
         For the moment, django-tree is only for PostgreSQL.
         It will be adapted in the future for other databases.
```

### Comparing `django-tree-0.4.1/LICENSE` & `django-tree-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tree-0.4.1/tree/query.py` & `django-tree-0.5.0/tree/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import operator
+from functools import reduce
+
 from django.core.exceptions import FieldDoesNotExist
-from django.db.models import QuerySet
+from django.db.models import QuerySet, Q
 from django.db.models.manager import Manager
 
 from .fields import PathField
 
 
 def _get_path_fields(model, name=None):
     if name is None:
@@ -21,26 +24,32 @@
     if n == 1:
         return path_fields[0]
     raise ValueError(
         'You need to specify which `PathField` to use for this query '
         'among these values: %s' % [f.name for f in path_fields])
 
 
+# TODO: Implement a faster `QuerySet.delete` and add it to the benchmark.
 class TreeQuerySetMixin:
     def _get_path_field_name(self, name):
         return _get_path_field(self.model, name).name
 
     def get_descendants(self, include_self=False, path_field=None):
         name = self._get_path_field_name(path_field)
-        # TODO: Avoids doing an extra query.
-        pattern = r'^(%s)' % '|'.join([
-            p.value for p in self.values_list(name, flat=True)])
+        # TODO: Avoid doing an extra query.
+        ancestor_paths = list(self.values_list(name, flat=True))
+        queryset = self.model.objects.all()
         if not include_self:
-            pattern += r'.'
-        return self.model.objects.filter(**{name + '__regex': pattern})
+            queryset = queryset.exclude(**{name + '__in': ancestor_paths})
+        return queryset.filter(
+            reduce(operator.or_, [
+                Q(**{name + '__descendant_of': ancestor_path})
+                for ancestor_path in ancestor_paths
+            ])
+        )
 
 
 class TreeQuerySet(TreeQuerySetMixin, QuerySet):
     pass
 
 
 class TreeManager(Manager.from_queryset(TreeQuerySet)):
```

### Comparing `django-tree-0.4.1/tree/models.py` & `django-tree-0.5.0/tree/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from contextlib import contextmanager
+from typing import Optional
 
 from django.db import DEFAULT_DB_ALIAS, transaction
 from django.db.models import Model
 
 from .query import _get_path_fields, _get_path_field, TreeManager
 
 
 class TreeModelMixin:
     @classmethod
-    def _get_path_fields(cls, name):
+    def _get_path_fields(cls, name: Optional[str] = None):
         return _get_path_fields(cls, name)
 
     @classmethod
     def _get_path_field(cls, name):
         return _get_path_field(cls, name)
 
     def _get_path_value(self, path_field):
```

### Comparing `django-tree-0.4.1/tree/lookups.py` & `django-tree-0.5.0/tree/lookups.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,40 +3,44 @@
 
 class AncestorOf(Lookup):
     lookup_name = 'ancestor_of'
 
     def as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
-        return "%s LIKE %s || '%%%%'" % (rhs, lhs), rhs_params + lhs_params
+        return (
+            '%s = (%s)[:array_length(%s, 1)]' % (lhs, rhs, lhs),
+            lhs_params + rhs_params + lhs_params,
+        )
 
 
 class SiblingOf(Lookup):
     lookup_name = 'sibling_of'
 
     def as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
-        level_size = self.lhs.output_field.level_size
-        return "%s LIKE left(%s, %s) || '%s'" % (
-            lhs, rhs, -level_size, '_' * level_size,
-        ), lhs_params + rhs_params
+        return (
+            'trim_array(%s, 1) = trim_array(%s, 1)' % (lhs, rhs),
+            lhs_params + rhs_params,
+        )
 
 
 class ChildOf(Lookup):
     lookup_name = 'child_of'
 
     def as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
-        return "%s LIKE %s || '%s'" % (
-            lhs, rhs, '_' * self.lhs.output_field.level_size,
-        ), lhs_params + rhs_params
+        return 'trim_array(%s, 1) = %s' % (lhs, rhs), lhs_params + rhs_params
 
 
 class DescendantOf(Lookup):
     lookup_name = 'descendant_of'
 
     def as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
-        return "%s LIKE %s || '%%%%'" % (lhs, rhs), lhs_params + rhs_params
+        return (
+            '(%s)[:array_length(%s, 1)] = %s' % (lhs, rhs, rhs),
+            lhs_params + rhs_params + rhs_params,
+        )
```

### Comparing `django-tree-0.4.1/tree/types.py` & `django-tree-0.5.0/tree/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from django.db.models import QuerySet
 
-from .sql.base import to_alphanum, from_alphanum
 
-
-class Path(object):
+class Path:
     def __init__(self, field, value):
         self.field = field
-        self.level_size = self.field.level_size
         self.attname = getattr(self.field, 'attname', None)
         self.field_bound = self.attname is not None
         self.qs = (self.field.model._default_manager.all()
                    if self.field_bound else QuerySet())
         self.value = value
 
     def __repr__(self):
@@ -67,50 +64,62 @@
             return True
         if isinstance(other, Path):
             other = other.value
         if not other:
             return False
         return self.value >= other
 
+    def __iter__(self):
+        return iter(self.value)
+
     def get_children(self):
         if not self.value:
             return self.qs.none()
-        return self.qs.filter(**{self.attname + '__child_of': self.value})
+        return self.qs.filter(**{
+            f'{self.attname}__child_of': self.value,
+        })
 
     def get_ancestors(self, include_self=False):
         if not self.value or (self.is_root() and not include_self):
             return self.qs.none()
-        paths = [self.value[:i+self.level_size]
-                 for i in range(0, len(self.value), self.level_size)]
+        path = self.value
         if not include_self:
-            paths.pop()
-        return self.qs.filter(**{self.attname + '__in': paths})
+            path = path[:-1]
+        # Using the lookup `ancestor_of` here is slower,
+        # so we explicitly specify the ancestors’ paths.
+        return self.qs.filter(**{self.attname + '__in': [
+            path[:i] for i in range(1, len(path) + 1)
+        ]})
 
     def get_descendants(self, include_self=False):
         if not self.value:
             return self.qs.none()
-        qs = self.qs.filter(**{self.attname + '__descendant_of': self.value})
+        # Using the lookup `descendant_of` here is slower,
+        # so we explicitly specify the path slicing comparison.
+        qs = self.qs.filter(**{
+            f'{self.attname}__0_{len(self.value)}': self.value,
+        })
         if include_self:
             return qs
-        return qs.exclude(**{self.attname: self.value})
+        return qs.filter(**{f'{self.attname}__level__gt': len(self.value)})
 
     def get_siblings(self, include_self=False, queryset=None):
         if not self.value:
             return self.qs.none()
 
         qs = self.qs if queryset is None else queryset
-        qs = qs.filter(**{self.attname + '__sibling_of': self.value})
+        qs = qs.filter(**{
+            self.attname + '__sibling_of': self.value,
+        })
         if include_self:
             return qs
         return qs.exclude(**{self.attname: self.value})
 
     def get_prev_siblings(self, include_self=False, queryset=None):
-        if not self.value or (
-                not include_self and (self.value[-self.level_size:]
-                                      == self.field.first_sibling_value)):
+        if not self.value:
             return self.qs.none()
         siblings = self.get_siblings(include_self=include_self,
                                      queryset=queryset)
         lookup = '__lte' if include_self else '__lt'
         return (siblings.filter(**{self.attname + lookup: self.value})
                 .order_by('-' + self.attname))
 
@@ -122,86 +131,72 @@
         lookup = '__gte' if include_self else '__gt'
         return (siblings.filter(**{self.attname + lookup: self.value})
                 .order_by(self.attname))
 
     def get_prev_sibling(self, queryset=None):
         if not self.value:
             return
-        current_label = self.value[-self.level_size:]
-        if current_label == self.field.first_sibling_value:
-            return
 
-        if queryset is not None:
-            return self.get_prev_siblings(queryset=queryset).first()
-
-        # TODO: Handle the case where the trigger is not in place.
-
-        prev_label = self.value[:-self.level_size] + to_alphanum(
-            from_alphanum(current_label) - 1, self.level_size)
-        return self.qs.get(**{self.attname: prev_label})
+        return self.get_prev_siblings(queryset=queryset).first()
 
     def get_next_sibling(self, queryset=None):
         if not self.value:
             return None
 
-        if queryset is not None:
-            return self.get_next_siblings(queryset=queryset).first()
-
-        # TODO: Handle the case where the trigger is not in place.
-
-        next_label = self.value[:-self.level_size] + to_alphanum(
-            from_alphanum(self.value[-self.level_size:]) + 1, self.level_size)
-        return self.qs.filter(**{self.attname: next_label}).first()
+        return self.get_next_siblings(queryset=queryset).first()
 
     def get_level(self):
         if self.value:
-            return len(self.value) // self.level_size
+            return len(self.value)
 
     def is_root(self):
         if self.value:
-            return len(self.value) == self.level_size
+            return len(self.value) == 1
 
     def is_leaf(self):
         if self.value:
             return not self.get_children().exists()
 
     def is_ancestor_of(self, other, include_self=False):
         if not self.value:
             return False
         if isinstance(other, Path):
             other = other.value
         if not other:
             return False
-        if not isinstance(other, str):
-            raise TypeError('`other` must be a `Path` instance or a string.')
+        if not isinstance(other, list):
+            raise TypeError(
+                '`other` must be a `Path` instance or a list of decimals.'
+            )
         if not include_self and self.value == other:
             return False
-        return other.startswith(self.value)
+        return other[:len(self.value)] == self.value
 
     def is_descendant_of(self, other, include_self=False):
         if not self.value:
             return False
         if isinstance(other, Path):
             other = other.value
         if not other:
             return False
-        if not isinstance(other, str):
-            raise TypeError('`other` must be a `Path` instance or a string.')
+        if not isinstance(other, list):
+            raise TypeError(
+                '`other` must be a `Path` instance or a list of decimals.'
+            )
         if not include_self and self.value == other:
             return False
-        return self.value.startswith(other)
+        return self.value[:len(other)] == other
 
 
 # Tells psycopg2 how to prepare a Path object for the database,
 # in case it doesn't go through the ORM.
 try:
     import psycopg2
 except ImportError:
     pass
 else:
-    from psycopg2.extensions import register_adapter, AsIs, QuotedString
+    from psycopg2.extensions import register_adapter, adapt
 
     def adapt_path(path):
-        v = path.value
-        return AsIs(v) if v is None else QuotedString(v)
+        return adapt(path.value)
 
     register_adapter(Path, adapt_path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-tree-0.4.1/tree/fields.py` & `django-tree-0.5.0/tree/fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,89 @@
 from contextlib import contextmanager
 
+from django.contrib.postgres.fields import ArrayField
 from django.core.exceptions import ImproperlyConfigured
 from django.db import DEFAULT_DB_ALIAS, connections, transaction
-from django.db.models import TextField
+from django.db.models import DecimalField, Index, Func, F
 from django.utils.translation import ugettext_lazy as _
 
 from .sql import postgresql
-from .sql.base import DEFAULT_MAX_SIBLINGS, ALPHANUM_LEN, PAD_CHAR
 from .types import Path
 
 
 # TODO: Handle ManyToManyField('self') instead of ForeignKey('self').
 # TODO: Add queryset methods like `get_descendants` in a mixin.
-# TODO: Implement an alternative using regex for other db backends.
+# TODO: Implement an alternative for other db backends.
 
 
-class PathField(TextField):
+class PathField(ArrayField):
     description = _('Tree path')
 
-    def __init__(self, *args, **kwargs):
-        kwargs.setdefault('editable', False)
-        self.original_default = kwargs.get('default')
-        kwargs['default'] = lambda: Path(self, self.original_default)
-        for kwarg in ('null', 'unique'):
+    @classmethod
+    def get_indexes(
+        cls,
+        table_name: str,
+        path_field_name: str,
+        max_indexed_level: int = 5,
+    ):
+        return [
+            Index(
+                Func(F(path_field_name), 1, function='trim_array'),
+                name=f'{table_name}_{path_field_name}_parent_index',
+            ),
+            Index(
+                F(f'{path_field_name}__level'),
+                name=f'{table_name}_{path_field_name}_level_index',
+            ),
+            *[
+                Index(
+                    F(f'{path_field_name}__0_{level}'),
+                    name=f'{table_name}_{path_field_name}_slice_{level}_index',
+                )
+                for level in range(1, max_indexed_level + 1)
+            ]
+        ]
+
+    def __init__(self, *args, parent_field_name: str = 'parent', **kwargs):
+        for kwarg in ('base_field', 'default', 'null', 'unique'):
             if kwarg in kwargs:
                 raise ImproperlyConfigured('Cannot set `PathField.%s`.'
                                            % kwarg)
-        kwargs['null'] = True
 
-        self.order_by = tuple(kwargs.pop('order_by', ()))
+        kwargs['base_field'] = DecimalField(max_digits=20, decimal_places=10)
+        kwargs['default'] = lambda: Path(self, None)
+        kwargs.setdefault('editable', False)
+        kwargs['null'] = True
 
-        max_siblings = kwargs.pop('max_siblings', DEFAULT_MAX_SIBLINGS)
-        if not (isinstance(max_siblings, int) and max_siblings > 0):
-            raise ImproperlyConfigured(
-                '`max_siblings` must be a positive integer, not %s.'
-                % repr(max_siblings))
-        self.max_siblings = max_siblings
-        i = self.max_siblings
-        n = 0
-        while i > 1.0:
-            i /= ALPHANUM_LEN
-            n += 1
-        self.level_size = n
-        self.first_sibling_value = PAD_CHAR * self.level_size
+        self.order_by = list(kwargs.pop('order_by', []))
+        self.parent_field_name = parent_field_name
 
         super(PathField, self).__init__(*args, **kwargs)
 
+    @property
+    def parent_field(self):
+        return self.model._meta.get_field(self.parent_field_name)
+
     def contribute_to_class(self, cls, name, *args, **kwargs):
         if name in self.order_by:
             raise ImproperlyConfigured(
                 '`PathField.order_by` cannot reference itself.' % name)
         super(PathField, self).contribute_to_class(cls, name, *args, **kwargs)
 
     def deconstruct(self):
         name, path, args, kwargs = super(PathField, self).deconstruct()
+        del kwargs['base_field']
         if not kwargs['editable']:
             del kwargs['editable']
         del kwargs['default']
         del kwargs['null']
-        if self.original_default is not None:
-            kwargs['default'] = self.original_default
-        if self.max_siblings != DEFAULT_MAX_SIBLINGS:
-            kwargs['max_siblings'] = self.max_siblings
-        if self.order_by != ():
+        if self.order_by != []:
             kwargs['order_by'] = self.order_by
+        if self.parent_field_name != 'parent':
+            kwargs['parent_field_name'] = self.parent_field_name
         return name, path, args, kwargs
 
     def from_db_value(self, value, expression, connection):
         if isinstance(value, Path):
             return value
         return Path(self, value)
 
@@ -79,16 +95,17 @@
     def get_prep_value(self, value):
         if isinstance(value, Path):
             return value.value
         return value
 
     # TODO: Move this method to a queryset.
     def get_roots(self):
-        return self.model._default_manager.filter(
-            **{self.attname + '__level': 1})
+        return self.model._default_manager.filter(**{
+            f'{self.attname}__level': 1,
+        })
 
     def _check_database_backend(self, db_alias):
         if connections[db_alias].vendor != 'postgresql':
             raise NotImplementedError(
                 'django-tree is only for PostgreSQL for now.')
 
     def rebuild(self, db_alias=DEFAULT_DB_ALIAS):
```

