# Comparing `tmp/yao-0.0.6.tar.gz` & `tmp/yao-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.0.6.tar", last modified: Thu Jun  1 10:16:59 2023, max compression
+gzip compressed data, was "yao-0.0.7.tar", last modified: Thu Jul  6 03:02:51 2023, max compression
```

## Comparing `yao-0.0.6.tar` & `yao-0.0.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.137529 yao-0.0.6/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-06-01 10:16:59.137302 yao-0.0.6/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-06-01 10:16:59.137581 yao-0.0.6/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)      971 2023-06-01 10:15:55.000000 yao-0.0.6/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.130591 yao-0.0.6/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    19302 2023-05-06 07:07:58.000000 yao-0.0.6/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-05-04 09:42:20.000000 yao-0.0.6/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 09:42:20.000000 yao-0.0.6/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.132001 yao-0.0.6/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.132771 yao-0.0.6/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.133430 yao-0.0.6/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.134027 yao-0.0.6/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.135046 yao-0.0.6/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)      992 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.135661 yao-0.0.6/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      665 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.136350 yao-0.0.6/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.137031 yao-0.0.6/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-06-01 10:08:02.000000 yao-0.0.6/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-05-04 09:42:20.000000 yao-0.0.6/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-05-04 09:42:20.000000 yao-0.0.6/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    12834 2023-06-01 10:08:43.000000 yao-0.0.6/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     2062 2023-05-12 09:17:23.000000 yao-0.0.6/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-06-01 10:16:59.131371 yao-0.0.6/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      166 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-06-01 10:16:59.000000 yao-0.0.6/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.457090 yao-0.0.7/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-07-06 03:02:51.456892 yao-0.0.7/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2023-07-06 03:02:51.457139 yao-0.0.7/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)      971 2023-07-06 03:00:38.000000 yao-0.0.7/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.451218 yao-0.0.7/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    19955 2023-07-01 08:54:38.000000 yao-0.0.7/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-05-04 09:42:20.000000 yao-0.0.7/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 09:42:20.000000 yao-0.0.7/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.452328 yao-0.0.7/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.452991 yao-0.0.7/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.453717 yao-0.0.7/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.454324 yao-0.0.7/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.454853 yao-0.0.7/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)      992 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.455371 yao-0.0.7/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      665 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.456045 yao-0.0.7/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.456659 yao-0.0.7/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-07-06 02:56:41.000000 yao-0.0.7/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-05-04 09:42:20.000000 yao-0.0.7/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-05-04 09:42:20.000000 yao-0.0.7/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    12903 2023-06-28 03:18:34.000000 yao-0.0.7/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2062 2023-05-12 09:17:23.000000 yao-0.0.7/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:02:51.451945 yao-0.0.7/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-07-06 03:02:51.000000 yao-0.0.7/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-07-06 03:02:51.000000 yao-0.0.7/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2023-07-06 03:02:51.000000 yao-0.0.7/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      166 2023-07-06 03:02:51.000000 yao-0.0.7/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2023-07-06 03:02:51.000000 yao-0.0.7/yao.egg-info/top_level.txt
```

### Comparing `yao-0.0.6/setup.py` & `yao-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.0.6",
+    version="0.0.7",
     description="Dev",
-    python_requires=">=3.9",
+    python_requires=">=3.6",
     author="Lsshu",
     author_email="admin@lsshu.cn",
     url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv3",
     classifiers=[
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 3 - Alpha",
     ],
     install_requires=[
         "fastapi[all]",
         "python-jose[cryptography]",
         "passlib[bcrypt]",
```

### Comparing `yao-0.0.6/yao/crud.py` & `yao-0.0.7/yao/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         if bool(where) and (type(where) == tuple or type(where) == list):
             if len(where) == 2:
                 """('content', '西')"""
                 _query = _query.filter(getattr(model_class, where[0]) == where[1])
             elif len(where) == 3:
                 if where[1] == "==" or where[1] == "=" or where[1] == "eq":
                     """('content', '==', '西')"""
-                    _query = _query.filter(getattr(model_class, where[0]) == where[2])
+                    _query = _query.filter(getattr(model_class, where[0]) == (where[2] if where[2] != "_#None" else None))
                 elif where[1] == "!=" or where[1] == "<>" or where[1] == "><" or where[1] == "neq" or where[1] == "ne":
                     """('content', '!=', '西')"""
                     _query = _query.filter(getattr(model_class, where[0]) != where[2])
                 elif where[1] == ">" or where[1] == "gt":
                     """('content', '>', '西')"""
                     _query = _query.filter(getattr(model_class, where[0]) > where[2])
                 elif where[1] == ">=" or where[1] == "ge":
@@ -138,15 +138,15 @@
                                     fil in where[2]]
                         _query = _query.filter(or_(*_filters))
                 elif where[1] in ["between"] and type(where[2]) in [list, tuple] and len(where[2]) == 2:
                     _query = _query.filter(getattr(getattr(model_class, where[0]), where[1])(where[2][0], where[2][1]))
                 elif where[1] in ["datebetween"] and type(where[2]) in [list, tuple] and len(where[2]) == 2:
                     _query = _query.filter(getattr(getattr(model_class, where[0]), 'between')(where[2][0], where[2][1]))
                 elif where[1] in ["datetimebetween"] and type(where[2]) in [list, tuple] and len(where[2]) == 2:
-                    _query = _query.filter(getattr(getattr(model_class, where[0]), 'between')("%s 00:00:00" % where[2][0], "%s 23:59:59" % where[2][1]))
+                    _query = _query.filter(getattr(getattr(model_class, where[0]), 'between')("%s" % where[2][0], "%s 23:59:59" % where[2][1]))
                 elif where[1] in ["in"] and type(where[2]) in [list, tuple]:
                     _query = _query.filter(getattr(getattr(model_class, where[0]), "in_")(where[2]))
                 elif where[1] in ["is"]:
                     _query = _query.filter(getattr(getattr(model_class, where[0]), "is_")(where[2]))
                 elif where[1] in ["notin"] and type(where[2]) in [list, tuple]:
                     _query = _query.filter(getattr(getattr(model_class, where[0]), "notin_")(where[2]))
                 else:
@@ -311,26 +311,27 @@
         self.__init_params(**kwargs)
         self._query_order()
         response = self.query.first()
         close and session.close()
         return response
 
     def update(self, session, where=None, item: BaseModel = None, data: dict = None, commit: bool = True, refresh: bool = True, close: bool = False, exclude_unset=True,
-               event: bool = False, **kwargs):
+               event: bool = False, synchronize_session="evaluate", **kwargs):
         """
         更新数据
         :param session:
         :param where:
         :param item:
         :param data:
         :param commit:
         :param refresh:
         :param close:
         :param exclude_unset:
         :param event:
+        :param synchronize_session:
         :param kwargs:
         :return:
         """
         if event:
             obj_item = self.first(session=session, where=where, **kwargs)
             # relationships
             if bool(self.relationships):
@@ -356,15 +357,15 @@
                         setattr(obj_item, relation, _relation)
                     elif not bool(getattr(item, relation)) and relation in item.dict(exclude_unset=exclude_unset):
                         [getattr(obj_item, relation).remove(rela) for rela in list(getattr(obj_item, relation))]  # 出错
                     hasattr(item, relation) and delattr(item, relation)
             # relationships
             self.__init_query(session=session)
             self.__init_params(where=where, **kwargs)
-            self.query.update(item.dict(exclude_unset=exclude_unset))
+            self.query.update(item.dict(exclude_unset=exclude_unset), synchronize_session=synchronize_session)
             commit and session.commit()
             close and session.close()
 
     def store(self, session, item: BaseModel = None, data: dict = None, commit: bool = True, refresh: bool = True, close: bool = False, **kwargs):
         """
         创建模型数据
         :param session:
@@ -390,14 +391,30 @@
         db_item = self.model_class(**item.dict(exclude_unset=True))
         session.add(db_item)
         commit and session.commit()
         refresh and session.refresh(db_item)
         close and session.close()
         return db_item
 
+    def many_store(self, session, items: List[BaseModel], commit: bool = True, close: bool = False, **kwargs):
+        """
+        批量创建模型数据
+        :param session:
+        :param items:
+        :param commit:
+        :param close:
+        :param kwargs:
+        :return:
+        """
+        db_items = [self.model_class(**item.dict(exclude_unset=True)) for item in items]
+        session.add_all(db_items)
+        commit and session.commit()
+        close and session.close()
+        return db_items
+
     def delete(self, session, commit: bool = True, close: bool = False, event: bool = False, **kwargs):
         """
         删除多模型数据
         :param session:
         :param commit:
         :param close:
         :param event:
```

### Comparing `yao-0.0.6/yao/db.py` & `yao-0.0.7/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/depends.py` & `yao-0.0.7/yao/depends.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/annex/main.py` & `yao-0.0.7/yao/function/annex/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/annex/schema.py` & `yao-0.0.7/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/appointment/crud.py` & `yao-0.0.7/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/appointment/main.py` & `yao-0.0.7/yao/function/appointment/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/appointment/schema.py` & `yao-0.0.7/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/company/main.py` & `yao-0.0.7/yao/function/company/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/company/schema.py` & `yao-0.0.7/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/department/main.py` & `yao-0.0.7/yao/function/department/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/department/schema.py` & `yao-0.0.7/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/log/main.py` & `yao-0.0.7/yao/function/log/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/log/schema.py` & `yao-0.0.7/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/main.py` & `yao-0.0.7/yao/function/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/model.py` & `yao-0.0.7/yao/function/model.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/permission/main.py` & `yao-0.0.7/yao/function/permission/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/permission/schema.py` & `yao-0.0.7/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/user/crud.py` & `yao-0.0.7/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/user/main.py` & `yao-0.0.7/yao/function/user/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/function/user/schema.py` & `yao-0.0.7/yao/function/user/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/helpers.py` & `yao-0.0.7/yao/helpers.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao/method.py` & `yao-0.0.7/yao/method.py`

 * *Files 6% similar despite different names*

```diff
@@ -342,15 +342,24 @@
 
 def get_attr(object, name: str, default=None):
     """
     获取对象属性 多层 以.分割
     """
     _name = name.split('.')
     for name in _name:
-        object = getattr(object, name, default)
+        if type(object) is dict:
+            object = object.get(name, default)
+        else:
+            object = getattr(object, name, default)
+    if object is None:
+        object = ""
+    if object is True:
+        object = 1
+    if object is False:
+        object = 0
     return object
 
 
 def export_file(sheet_name: str, export_name: str, col_items: dict, db_list: list):
     """
     导出文件
     """
@@ -359,18 +368,15 @@
     ws = wb.active
     ws.title = sheet_name
     ws.append([datum for datum in col_items.values()])
     # [ws.append([str(get_attr(db_obj, key, "")) for key in col_items]) for db_obj in db_list]
     for db_obj in db_list:
         _list = []
         for key in col_items:
-            if type(db_obj) is dict:
-                _list.append(db_obj.get(key, ""))
-            else:
-                _list.append(get_attr(db_obj, key, ""))
+            _list.append(get_attr(db_obj, key, ""))
         ws.append(_list)
 
     if not os.path.exists(os.path.dirname(export_name)):
         os.makedirs(os.path.dirname(export_name))
     return wb.save(export_name)
 
 
@@ -378,22 +384,21 @@
     """
     导出文件
     """
     from openpyxl import Workbook
     wb = Workbook()
     for key, sheet in enumerate(sheet_data):
         ws = wb.create_sheet(sheet.get("sheet_name"), key)
-        ws.append([datum for datum in sheet.get("col_items", {}).values()])
+        header_label = sheet.get("col_items", {})
+        if sheet.get("is_label", True):
+            ws.append([datum for datum in header_label.values()])
         for db_obj in sheet.get("db_list", []):
             _list = []
-            for key in sheet.get("col_items", {}):
-                if type(db_obj) is dict:
-                    _list.append(db_obj.get(key, ""))
-                else:
-                    _list.append(get_attr(db_obj, key, ""))
+            for key in header_label.keys():
+                _list.append(get_attr(db_obj, key, ""))
             ws.append(_list)
 
         if not os.path.exists(os.path.dirname(export_name)):
             os.makedirs(os.path.dirname(export_name))
     return wb.save(export_name)
```

### Comparing `yao-0.0.6/yao/schema.py` & `yao-0.0.7/yao/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.6/yao.egg-info/SOURCES.txt` & `yao-0.0.7/yao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

