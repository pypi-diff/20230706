# Comparing `tmp/django-tree-0.5.2.tar.gz` & `tmp/django-tree-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tree-0.5.2.tar", last modified: Thu Jul  6 14:18:28 2023, max compression
+gzip compressed data, was "dist/django-tree-0.5.3.tar", last modified: Thu Jul  6 14:47:30 2023, max compression
```

## Comparing `django-tree-0.5.2.tar` & `django-tree-0.5.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9498 2023-07-06 13:11:50.000000 django-tree-0.5.2/README.rst
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/benchmark/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/benchmark/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.2/benchmark/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.2/benchmark/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/router.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.2/benchmark/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.2/benchmark/utils.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.2/requirements.txt
--rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.2/setup.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/requires.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/top_level.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.2/django_tree.egg-info/not-zip-safe
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 14:18:28.000000 django-tree-0.5.2/django_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.2/MANIFEST.in
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tests/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tests/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.2/tests/migrations/0003_test_migrations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.2/tests/migrations/0002_add_tmp_model.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2958 2023-07-06 10:40:54.000000 django-tree-0.5.2/tests/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tests/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      910 2023-07-06 10:40:54.000000 django-tree-0.5.2/tests/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.2/tests/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    48189 2023-07-06 14:12:28.000000 django-tree-0.5.2/tests/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tests/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:18:28.000000 django-tree-0.5.2/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1712 2023-07-06 14:16:01.000000 django-tree-0.5.2/CHANGELOG.rst
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.2/LICENSE
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 14:18:28.000000 django-tree-0.5.2/setup.cfg
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tree/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tree/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/migrations/0002_remove_old_functions.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tree/migrations/__init__.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:18:28.000000 django-tree-0.5.2/tree/sql/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9343 2023-07-06 14:10:37.000000 django-tree-0.5.2/tree/sql/postgresql.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/sql/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.2/tree/sql/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/transforms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/query.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/signals.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.2/tree/forms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/apps.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/lookups.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/operations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.2/tree/types.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 14:16:02.000000 django-tree-0.5.2/tree/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4716 2023-07-06 10:40:54.000000 django-tree-0.5.2/tree/fields.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9498 2023-07-06 13:11:50.000000 django-tree-0.5.3/README.rst
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/benchmark/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/benchmark/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.3/benchmark/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.3/benchmark/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.3/benchmark/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.3/benchmark/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.3/benchmark/router.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.3/benchmark/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.3/benchmark/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.3/benchmark/utils.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.3/requirements.txt
+-rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.3/setup.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/django_tree.egg-info/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 14:47:30.000000 django-tree-0.5.3/django_tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 14:47:30.000000 django-tree-0.5.3/django_tree.egg-info/requires.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 14:47:30.000000 django-tree-0.5.3/django_tree.egg-info/top_level.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:47:30.000000 django-tree-0.5.3/django_tree.egg-info/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.3/django_tree.egg-info/not-zip-safe
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 14:47:30.000000 django-tree-0.5.3/django_tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.3/MANIFEST.in
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/tests/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/tests/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.3/tests/migrations/0003_test_migrations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.3/tests/migrations/0002_add_tmp_model.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2958 2023-07-06 10:40:54.000000 django-tree-0.5.3/tests/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.3/tests/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      910 2023-07-06 10:40:54.000000 django-tree-0.5.3/tests/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.3/tests/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    48189 2023-07-06 14:12:28.000000 django-tree-0.5.3/tests/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.3/tests/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 14:47:30.000000 django-tree-0.5.3/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1829 2023-07-06 14:47:13.000000 django-tree-0.5.3/CHANGELOG.rst
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.3/LICENSE
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 14:47:30.000000 django-tree-0.5.3/setup.cfg
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/tree/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/tree/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/migrations/0002_remove_old_functions.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.3/tree/migrations/__init__.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 14:47:30.000000 django-tree-0.5.3/tree/sql/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9354 2023-07-06 14:45:35.000000 django-tree-0.5.3/tree/sql/postgresql.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/sql/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.3/tree/sql/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/transforms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/query.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/signals.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.3/tree/forms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/apps.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/lookups.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/operations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.3/tree/types.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 14:46:42.000000 django-tree-0.5.3/tree/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4716 2023-07-06 10:40:54.000000 django-tree-0.5.3/tree/fields.py
```

### Comparing `django-tree-0.5.2/README.rst` & `django-tree-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/benchmark/migrations/0001_initial.py` & `django-tree-0.5.3/benchmark/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/benchmark/models.py` & `django-tree-0.5.3/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/benchmark/base.py` & `django-tree-0.5.3/benchmark/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/benchmark/utils.py` & `django-tree-0.5.3/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/setup.py` & `django-tree-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/django_tree.egg-info/SOURCES.txt` & `django-tree-0.5.3/django_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/django_tree.egg-info/PKG-INFO` & `django-tree-0.5.3/django_tree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.2
+Version: 0.5.3
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
```

### Comparing `django-tree-0.5.2/tests/migrations/0003_test_migrations.py` & `django-tree-0.5.3/tests/migrations/0003_test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tests/migrations/0002_add_tmp_model.py` & `django-tree-0.5.3/tests/migrations/0002_add_tmp_model.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tests/migrations/0001_initial.py` & `django-tree-0.5.3/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tests/models.py` & `django-tree-0.5.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tests/base.py` & `django-tree-0.5.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/PKG-INFO` & `django-tree-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.2
+Version: 0.5.3
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
```

### Comparing `django-tree-0.5.2/CHANGELOG.rst` & `django-tree-0.5.3/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.5.3 (2023-07-06)
+==================
+
+Fixes a PostgreSQL implicit type casting that was not done in PostgreSQL 12.
+
 0.5.2 (2023-07-06)
 ==================
 
 Fixes a source of path clashes when the objects have exactly the same values
 for all ``order_by`` columns.
 
 0.5.1 (2023-07-06)
```

### Comparing `django-tree-0.5.2/LICENSE` & `django-tree-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/migrations/0002_remove_old_functions.py` & `django-tree-0.5.3/tree/migrations/0002_remove_old_functions.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/sql/postgresql.py` & `django-tree-0.5.3/tree/sql/postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 SELECT {parent}, NULL::decimal[]
                 FROM {table}
                 WHERE {parent} IS NULL
                 LIMIT 1
             ) UNION ALL (
                 SELECT
                     t2.{pk},
-                    t1.path || row_number() OVER (
+                    t1.path || row_number()::decimal[] OVER (
                         PARTITION BY t1.pk ORDER BY {sql_t2_order_by}
                     ) - 1
                 FROM generate_paths AS t1
                 INNER JOIN {table} AS t2 ON (
                     t2.{parent} = t1.pk
                     OR (t1.pk IS NULL AND t2.{parent} IS NULL))
             )
```

### Comparing `django-tree-0.5.2/tree/sql/base.py` & `django-tree-0.5.3/tree/sql/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/query.py` & `django-tree-0.5.3/tree/query.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/signals.py` & `django-tree-0.5.3/tree/signals.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/apps.py` & `django-tree-0.5.3/tree/apps.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/models.py` & `django-tree-0.5.3/tree/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/lookups.py` & `django-tree-0.5.3/tree/lookups.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/operations.py` & `django-tree-0.5.3/tree/operations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/types.py` & `django-tree-0.5.3/tree/types.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.2/tree/fields.py` & `django-tree-0.5.3/tree/fields.py`

 * *Files identical despite different names*

