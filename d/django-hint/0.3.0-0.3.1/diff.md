# Comparing `tmp/django_hint-0.3.0.tar.gz` & `tmp/django_hint-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hint-0.3.0.tar", last modified: Wed Jun 28 20:11:43 2023, max compression
+gzip compressed data, was "django_hint-0.3.1.tar", last modified: Thu Jul  6 20:32:28 2023, max compression
```

## Comparing `django_hint-0.3.0.tar` & `django_hint-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ramtin     (501) admin       (80)        0 2023-06-28 20:11:43.672194 django_hint-0.3.0/
--rw-r--r--   0 ramtin     (501) admin       (80)     1073 2023-06-28 16:12:43.000000 django_hint-0.3.0/LICENSE
--rw-r--r--   0 ramtin     (501) admin       (80)     3895 2023-06-28 20:11:43.672089 django_hint-0.3.0/PKG-INFO
--rw-r--r--   0 ramtin     (501) admin       (80)     3490 2023-06-28 20:08:31.000000 django_hint-0.3.0/README.md
-drwxr-xr-x   0 ramtin     (501) admin       (80)        0 2023-06-28 20:11:43.671468 django_hint-0.3.0/django_hint/
--rw-r--r--   0 ramtin     (501) admin       (80)      575 2023-06-28 16:12:43.000000 django_hint-0.3.0/django_hint/__init__.py
--rw-r--r--   0 ramtin     (501) admin       (80)     9229 2023-06-28 20:07:55.000000 django_hint-0.3.0/django_hint/typehint.py
-drwxr-xr-x   0 ramtin     (501) admin       (80)        0 2023-06-28 20:11:43.671945 django_hint-0.3.0/django_hint.egg-info/
--rw-r--r--   0 ramtin     (501) admin       (80)     3895 2023-06-28 20:11:43.000000 django_hint-0.3.0/django_hint.egg-info/PKG-INFO
--rw-r--r--   0 ramtin     (501) admin       (80)      214 2023-06-28 20:11:43.000000 django_hint-0.3.0/django_hint.egg-info/SOURCES.txt
--rw-r--r--   0 ramtin     (501) admin       (80)        1 2023-06-28 20:11:43.000000 django_hint-0.3.0/django_hint.egg-info/dependency_links.txt
--rw-r--r--   0 ramtin     (501) admin       (80)       12 2023-06-28 20:11:43.000000 django_hint-0.3.0/django_hint.egg-info/top_level.txt
--rw-r--r--   0 ramtin     (501) admin       (80)       38 2023-06-28 20:11:43.672225 django_hint-0.3.0/setup.cfg
--rw-r--r--   0 ramtin     (501) admin       (80)      615 2023-06-28 20:08:12.000000 django_hint-0.3.0/setup.py
+drwxr-xr-x   0 ramtin     (501) admin       (80)        0 2023-07-06 20:32:28.529854 django_hint-0.3.1/
+-rw-r--r--   0 ramtin     (501) admin       (80)     1073 2023-06-28 16:12:43.000000 django_hint-0.3.1/LICENSE
+-rw-r--r--   0 ramtin     (501) admin       (80)     3895 2023-07-06 20:32:28.529682 django_hint-0.3.1/PKG-INFO
+-rw-r--r--   0 ramtin     (501) admin       (80)     3490 2023-06-28 20:16:57.000000 django_hint-0.3.1/README.md
+drwxr-xr-x   0 ramtin     (501) admin       (80)        0 2023-07-06 20:32:28.527784 django_hint-0.3.1/django_hint/
+-rw-r--r--   0 ramtin     (501) admin       (80)      594 2023-07-06 20:31:54.000000 django_hint-0.3.1/django_hint/__init__.py
+-rw-r--r--   0 ramtin     (501) admin       (80)     9229 2023-07-06 20:26:10.000000 django_hint-0.3.1/django_hint/typehint.py
+drwxr-xr-x   0 ramtin     (501) admin       (80)        0 2023-07-06 20:32:28.529344 django_hint-0.3.1/django_hint.egg-info/
+-rw-r--r--   0 ramtin     (501) admin       (80)     3895 2023-07-06 20:32:28.000000 django_hint-0.3.1/django_hint.egg-info/PKG-INFO
+-rw-r--r--   0 ramtin     (501) admin       (80)      214 2023-07-06 20:32:28.000000 django_hint-0.3.1/django_hint.egg-info/SOURCES.txt
+-rw-r--r--   0 ramtin     (501) admin       (80)        1 2023-07-06 20:32:28.000000 django_hint-0.3.1/django_hint.egg-info/dependency_links.txt
+-rw-r--r--   0 ramtin     (501) admin       (80)       12 2023-07-06 20:32:28.000000 django_hint-0.3.1/django_hint.egg-info/top_level.txt
+-rw-r--r--   0 ramtin     (501) admin       (80)       38 2023-07-06 20:32:28.529934 django_hint-0.3.1/setup.cfg
+-rw-r--r--   0 ramtin     (501) admin       (80)      615 2023-07-06 20:31:54.000000 django_hint-0.3.1/setup.py
```

### Comparing `django_hint-0.3.0/LICENSE` & `django_hint-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hint-0.3.0/PKG-INFO` & `django_hint-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hint
-Version: 0.3.0
+Version: 0.3.1
 Summary: Type hinting package for django
 Home-page: https://github.com/Vieolo/django-hint
 Author: Vieolo OÜ
 Author-email: info@vieolo.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django_hint-0.3.0/README.md` & `django_hint-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_hint-0.3.0/django_hint/__init__.py` & `django_hint-0.3.1/django_hint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .typehint import QueryType, RequestType, DRFTokenRequestType, StandardModelType, List, Optional, Union, Deque, Dict, DefaultDict, FrozenSet, ChainMap, Counter, Set
 from .typehint import Generic, Callable, Tuple, TypeVar, Type, ClassVar
 __all__ = [
     "QueryType",
     "RequestType",
     "DRFTokenRequestType",
+    "QueryFilter",
     "StandardModelType",
     "List",
     "Optional",
     "Union",
     "Dict",
     "DefaultDict",
     "Set",
```

### Comparing `django_hint-0.3.0/django_hint/typehint.py` & `django_hint-0.3.1/django_hint/typehint.py`

 * *Files identical despite different names*

### Comparing `django_hint-0.3.0/django_hint.egg-info/PKG-INFO` & `django_hint-0.3.1/django_hint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hint
-Version: 0.3.0
+Version: 0.3.1
 Summary: Type hinting package for django
 Home-page: https://github.com/Vieolo/django-hint
 Author: Vieolo OÜ
 Author-email: info@vieolo.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django_hint-0.3.0/setup.py` & `django_hint-0.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django_hint",
-    version="0.3.0",
+    version="0.3.1",
     author="Vieolo OÜ",
     author_email="info@vieolo.com",
     description="Type hinting package for django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Vieolo/django-hint",
     packages=setuptools.find_packages(),
```

