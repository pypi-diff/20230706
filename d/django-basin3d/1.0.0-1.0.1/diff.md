# Comparing `tmp/django-basin3d-1.0.0.tar.gz` & `tmp/django-basin3d-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-basin3d-1.0.0.tar", last modified: Fri Jun 23 13:27:33 2023, max compression
+gzip compressed data, was "django-basin3d-1.0.1.tar", last modified: Thu Jul  6 15:27:51 2023, max compression
```

## Comparing `django-basin3d-1.0.0.tar` & `django-basin3d-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:33.162228 django-basin3d-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-06-23 13:27:33.162228 django-basin3d-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:33.162228 django-basin3d-1.0.0/django_basin3d/
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:33.162228 django-basin3d-1.0.0/django_basin3d/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:33.162228 django-basin3d-1.0.0/django_basin3d/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/synthesis/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/synthesis/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:33.162228 django-basin3d-1.0.0/django_basin3d/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/templatetags/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/django_basin3d/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:27:33.162228 django-basin3d-1.0.0/django_basin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-06-23 13:27:33.000000 django-basin3d-1.0.0/django_basin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-23 13:27:33.000000 django-basin3d-1.0.0/django_basin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:27:33.000000 django-basin3d-1.0.0/django_basin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 13:27:33.000000 django-basin3d-1.0.0/django_basin3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 13:27:33.000000 django-basin3d-1.0.0/django_basin3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/doecode.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-23 13:27:19.000000 django-basin3d-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:27:33.166228 django-basin3d-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.031828 django-basin3d-1.0.1/django_basin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/synthesis/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/synthesis/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/templatetags/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/django_basin3d/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/django_basin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 15:27:51.000000 django-basin3d-1.0.1/django_basin3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/doecode.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-06 15:27:37.000000 django-basin3d-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 15:27:51.035828 django-basin3d-1.0.1/setup.cfg
```

### Comparing `django-basin3d-1.0.0/LICENSE` & `django-basin3d-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/PKG-INFO` & `django-basin3d-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.0
+Version: 1.0.1
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
@@ -64,14 +64,17 @@
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
+[![Python package](https://github.com/BASIN-3D/django-basin3d/actions/workflows/main.yml/badge.svg)](https://github.com/BASIN-3D/django-basin3d/actions/workflows/main.yml) 
+[![Pypi](https://img.shields.io/pypi/v/django-basin3d)](https://pypi.org/project/django-basin3d/)
+
 # django-basin3d
 Django web framework for Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets
 
 ## Using django-basin3d
 Knowledge of Django is required to use django-basin3d.
 
 See [Django documentation](https://docs.djangoproject.com/) for details on creating a Django app.
```

### Comparing `django-basin3d-1.0.0/README.md` & `django-basin3d-1.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![Python package](https://github.com/BASIN-3D/django-basin3d/actions/workflows/main.yml/badge.svg)](https://github.com/BASIN-3D/django-basin3d/actions/workflows/main.yml) 
+[![Pypi](https://img.shields.io/pypi/v/django-basin3d)](https://pypi.org/project/django-basin3d/)
+
 # django-basin3d
 Django web framework for Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets
 
 ## Using django-basin3d
 Knowledge of Django is required to use django-basin3d.
 
 See [Django documentation](https://docs.djangoproject.com/) for details on creating a Django app.
```

### Comparing `django-basin3d-1.0.0/django_basin3d/__init__.py` & `django-basin3d-1.0.1/django_basin3d/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/admin.py` & `django-basin3d-1.0.1/django_basin3d/admin.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/catalog.py` & `django-basin3d-1.0.1/django_basin3d/catalog.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/migrations/0001_initial.py` & `django-basin3d-1.0.1/django_basin3d/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/models.py` & `django-basin3d-1.0.1/django_basin3d/models.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/serializers.py` & `django-basin3d-1.0.1/django_basin3d/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/settings.py` & `django-basin3d-1.0.1/django_basin3d/settings.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/synthesis/__init__.py` & `django-basin3d-1.0.1/django_basin3d/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/synthesis/serializers.py` & `django-basin3d-1.0.1/django_basin3d/synthesis/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/synthesis/viewsets.py` & `django-basin3d-1.0.1/django_basin3d/synthesis/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/urls.py` & `django-basin3d-1.0.1/django_basin3d/urls.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/views.py` & `django-basin3d-1.0.1/django_basin3d/views.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d/viewsets.py` & `django-basin3d-1.0.1/django_basin3d/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/django_basin3d.egg-info/PKG-INFO` & `django-basin3d-1.0.1/django_basin3d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.0
+Version: 1.0.1
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
@@ -64,14 +64,17 @@
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
+[![Python package](https://github.com/BASIN-3D/django-basin3d/actions/workflows/main.yml/badge.svg)](https://github.com/BASIN-3D/django-basin3d/actions/workflows/main.yml) 
+[![Pypi](https://img.shields.io/pypi/v/django-basin3d)](https://pypi.org/project/django-basin3d/)
+
 # django-basin3d
 Django web framework for Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets
 
 ## Using django-basin3d
 Knowledge of Django is required to use django-basin3d.
 
 See [Django documentation](https://docs.djangoproject.com/) for details on creating a Django app.
```

### Comparing `django-basin3d-1.0.0/django_basin3d.egg-info/SOURCES.txt` & `django-basin3d-1.0.1/django_basin3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/doecode.yml` & `django-basin3d-1.0.1/doecode.yml`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.0/pyproject.toml` & `django-basin3d-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Topic :: Scientific/Engineering :: Hydrology"
 ]
 description = "BASIN-3D Django Web Framework"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = '>=3.8,<3.11'
 dependencies = [
-    'basin3d==0.4.0',
+    'basin3d==0.4.1',
     'django>=4.0',
     'djangorestframework',
     'django-filter',
     'markdown',
     'pygments'
 ]
```

