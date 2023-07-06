# Comparing `tmp/django-tree-0.5.0.tar.gz` & `tmp/django-tree-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tree-0.5.0.tar", last modified: Thu Jul  6 00:43:19 2023, max compression
+gzip compressed data, was "dist/django-tree-0.5.1.tar", last modified: Thu Jul  6 00:47:50 2023, max compression
```

## Comparing `django-tree-0.5.0.tar` & `django-tree-0.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9393 2023-07-06 00:41:03.000000 django-tree-0.5.0/README.rst
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/benchmark/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/benchmark/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.0/benchmark/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.0/benchmark/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/router.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.0/benchmark/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.0/benchmark/utils.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.0/requirements.txt
--rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1117 2018-02-09 14:18:58.000000 django-tree-0.5.0/setup.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/requires.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/top_level.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12113 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.0/django_tree.egg-info/not-zip-safe
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 00:43:19.000000 django-tree-0.5.0/django_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.0/MANIFEST.in
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tests/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tests/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/migrations/0003_test_migrations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.0/tests/migrations/0002_add_tmp_model.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2494 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tests/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      825 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.0/tests/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    45481 2023-07-06 00:41:03.000000 django-tree-0.5.0/tests/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tests/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12113 2023-07-06 00:43:19.000000 django-tree-0.5.0/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1565 2023-07-06 00:41:33.000000 django-tree-0.5.0/CHANGELOG.rst
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.0/LICENSE
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 00:43:19.000000 django-tree-0.5.0/setup.cfg
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tree/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tree/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/migrations/0002_remove_old_functions.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tree/migrations/__init__.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:43:19.000000 django-tree-0.5.0/tree/sql/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9369 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/sql/postgresql.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/sql/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.0/tree/sql/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/transforms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/query.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/signals.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.0/tree/forms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/apps.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/lookups.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/operations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/types.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-05 21:45:26.000000 django-tree-0.5.0/tree/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4689 2023-07-06 00:41:03.000000 django-tree-0.5.0/tree/fields.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9500 2023-07-06 00:47:09.000000 django-tree-0.5.1/README.rst
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/benchmark/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/benchmark/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3898 2023-07-06 00:41:03.000000 django-tree-0.5.1/benchmark/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.1/benchmark/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/router.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.1/benchmark/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.1/benchmark/utils.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.1/requirements.txt
+-rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.1/setup.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/requires.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/top_level.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12446 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.1/django_tree.egg-info/not-zip-safe
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 00:47:50.000000 django-tree-0.5.1/django_tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.1/MANIFEST.in
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tests/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tests/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/migrations/0003_test_migrations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.1/tests/migrations/0002_add_tmp_model.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2494 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tests/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      825 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.1/tests/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    45481 2023-07-06 00:41:03.000000 django-tree-0.5.1/tests/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tests/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12446 2023-07-06 00:47:50.000000 django-tree-0.5.1/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1565 2023-07-06 00:47:08.000000 django-tree-0.5.1/CHANGELOG.rst
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.1/LICENSE
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 00:47:50.000000 django-tree-0.5.1/setup.cfg
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tree/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tree/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/migrations/0002_remove_old_functions.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tree/migrations/__init__.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 00:47:50.000000 django-tree-0.5.1/tree/sql/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9369 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/sql/postgresql.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/sql/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.1/tree/sql/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/transforms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/query.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/signals.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.1/tree/forms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/apps.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1464 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/lookups.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/operations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/types.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 00:46:36.000000 django-tree-0.5.1/tree/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4689 2023-07-06 00:41:03.000000 django-tree-0.5.1/tree/fields.py
```

### Comparing `django-tree-0.5.0/README.rst` & `django-tree-0.5.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Django-tree
 ===========
 
+⚠ Open to financing MySQL & SQLite compatibility ⚠
+--------------------------------------------------
+
 Fast and easy tree structures.
 
 .. image:: http://img.shields.io/pypi/v/django-tree.svg?style=flat-square
    :target: https://pypi.python.org/pypi/django-tree
 
 .. image:: http://img.shields.io/travis/BertrandBordage/django-tree/master.svg?style=flat-square
    :target: https://travis-ci.org/BertrandBordage/django-tree
```

### Comparing `django-tree-0.5.0/benchmark/migrations/0001_initial.py` & `django-tree-0.5.1/benchmark/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/benchmark/models.py` & `django-tree-0.5.1/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/benchmark/base.py` & `django-tree-0.5.1/benchmark/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/benchmark/utils.py` & `django-tree-0.5.1/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/django_tree.egg-info/SOURCES.txt` & `django-tree-0.5.1/django_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/django_tree.egg-info/PKG-INFO` & `django-tree-0.5.1/django_tree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
         
+        ⚠ Open to financing MySQL & SQLite compatibility ⚠
+        --------------------------------------------------
+        
         Fast and easy tree structures.
         
         .. image:: http://img.shields.io/pypi/v/django-tree.svg?style=flat-square
            :target: https://pypi.python.org/pypi/django-tree
         
         .. image:: http://img.shields.io/travis/BertrandBordage/django-tree/master.svg?style=flat-square
            :target: https://travis-ci.org/BertrandBordage/django-tree
@@ -266,10 +269,14 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `django-tree-0.5.0/tests/migrations/0003_test_migrations.py` & `django-tree-0.5.1/tests/migrations/0003_test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tests/migrations/0002_add_tmp_model.py` & `django-tree-0.5.1/tests/migrations/0002_add_tmp_model.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tests/migrations/0001_initial.py` & `django-tree-0.5.1/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tests/models.py` & `django-tree-0.5.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tests/base.py` & `django-tree-0.5.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/PKG-INFO` & `django-tree-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
         
+        ⚠ Open to financing MySQL & SQLite compatibility ⚠
+        --------------------------------------------------
+        
         Fast and easy tree structures.
         
         .. image:: http://img.shields.io/pypi/v/django-tree.svg?style=flat-square
            :target: https://pypi.python.org/pypi/django-tree
         
         .. image:: http://img.shields.io/travis/BertrandBordage/django-tree/master.svg?style=flat-square
            :target: https://travis-ci.org/BertrandBordage/django-tree
@@ -266,10 +269,14 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `django-tree-0.5.0/CHANGELOG.rst` & `django-tree-0.5.1/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-0.5.0 (2023-07-06)
+0.5.1 (2023-07-06)
 ==================
 
 Big rewrite using arrays of decimals instead of strings to represent the path.
 
 Performance
 -----------
```

### Comparing `django-tree-0.5.0/LICENSE` & `django-tree-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/migrations/0002_remove_old_functions.py` & `django-tree-0.5.1/tree/migrations/0002_remove_old_functions.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/sql/postgresql.py` & `django-tree-0.5.1/tree/sql/postgresql.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/sql/base.py` & `django-tree-0.5.1/tree/sql/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/query.py` & `django-tree-0.5.1/tree/query.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/signals.py` & `django-tree-0.5.1/tree/signals.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/apps.py` & `django-tree-0.5.1/tree/apps.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/models.py` & `django-tree-0.5.1/tree/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/lookups.py` & `django-tree-0.5.1/tree/lookups.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/operations.py` & `django-tree-0.5.1/tree/operations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/types.py` & `django-tree-0.5.1/tree/types.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.0/tree/fields.py` & `django-tree-0.5.1/tree/fields.py`

 * *Files identical despite different names*

