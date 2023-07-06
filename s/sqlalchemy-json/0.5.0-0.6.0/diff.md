# Comparing `tmp/sqlalchemy-json-0.5.0.tar.gz` & `tmp/sqlalchemy-json-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-json-0.5.0.tar", last modified: Sun Mar 13 23:48:49 2022, max compression
+gzip compressed data, was "sqlalchemy-json-0.6.0.tar", last modified: Thu Jul  6 21:44:12 2023, max compression
```

## Comparing `sqlalchemy-json-0.5.0.tar` & `sqlalchemy-json-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2022-03-13 23:48:49.836149 sqlalchemy-json-0.5.0/
--rw-rw-r--   0 elmer     (1000) elmer     (1000)     7752 2022-03-13 23:48:49.836149 sqlalchemy-json-0.5.0/PKG-INFO
--rw-rw-r--   0 elmer     (1000) elmer     (1000)     5905 2022-03-13 23:44:08.000000 sqlalchemy-json-0.5.0/README.rst
--rw-r--r--   0 elmer     (1000) elmer     (1000)       61 2022-03-13 23:48:49.836149 sqlalchemy-json-0.5.0/setup.cfg
--rw-rw-r--   0 elmer     (1000) elmer     (1000)      996 2022-03-13 23:45:36.000000 sqlalchemy-json-0.5.0/setup.py
-drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2022-03-13 23:48:49.832149 sqlalchemy-json-0.5.0/sqlalchemy_json/
--rw-rw-r--   0 elmer     (1000) elmer     (1000)     1774 2022-03-13 22:58:56.000000 sqlalchemy-json-0.5.0/sqlalchemy_json/__init__.py
--rwxrwxr-x   0 elmer     (1000) elmer     (1000)     6267 2022-03-13 23:04:37.000000 sqlalchemy-json-0.5.0/sqlalchemy_json/track.py
-drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2022-03-13 23:48:49.836149 sqlalchemy-json-0.5.0/sqlalchemy_json.egg-info/
--rw-rw-r--   0 elmer     (1000) elmer     (1000)     7752 2022-03-13 23:48:49.000000 sqlalchemy-json-0.5.0/sqlalchemy_json.egg-info/PKG-INFO
--rw-rw-r--   0 elmer     (1000) elmer     (1000)      343 2022-03-13 23:48:49.000000 sqlalchemy-json-0.5.0/sqlalchemy_json.egg-info/SOURCES.txt
--rw-rw-r--   0 elmer     (1000) elmer     (1000)        1 2022-03-13 23:48:49.000000 sqlalchemy-json-0.5.0/sqlalchemy_json.egg-info/dependency_links.txt
--rw-rw-r--   0 elmer     (1000) elmer     (1000)        1 2015-08-11 09:41:31.000000 sqlalchemy-json-0.5.0/sqlalchemy_json.egg-info/not-zip-safe
--rw-rw-r--   0 elmer     (1000) elmer     (1000)       20 2022-03-13 23:48:49.000000 sqlalchemy-json-0.5.0/sqlalchemy_json.egg-info/requires.txt
--rw-rw-r--   0 elmer     (1000) elmer     (1000)       16 2022-03-13 23:48:49.000000 sqlalchemy-json-0.5.0/sqlalchemy_json.egg-info/top_level.txt
-drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2022-03-13 23:48:49.836149 sqlalchemy-json-0.5.0/test/
--rw-rw-r--   0 elmer     (1000) elmer     (1000)     3381 2022-03-13 23:07:20.000000 sqlalchemy-json-0.5.0/test/test_sqlalchemy_json.py
+drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2023-07-06 21:44:12.526032 sqlalchemy-json-0.6.0/
+-rw-r--r--   0 elmer     (1000) elmer     (1000)     1319 2014-04-13 12:34:35.000000 sqlalchemy-json-0.6.0/LICENSE
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)     6769 2023-07-06 21:44:12.526032 sqlalchemy-json-0.6.0/PKG-INFO
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)     6142 2023-07-06 21:43:16.000000 sqlalchemy-json-0.6.0/README.rst
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)       38 2023-07-06 21:44:12.526032 sqlalchemy-json-0.6.0/setup.cfg
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)     1011 2023-07-06 21:43:16.000000 sqlalchemy-json-0.6.0/setup.py
+drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2023-07-06 21:44:12.526032 sqlalchemy-json-0.6.0/sqlalchemy_json/
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)     1956 2023-07-06 21:43:16.000000 sqlalchemy-json-0.6.0/sqlalchemy_json/__init__.py
+-rwxrwxr-x   0 elmer     (1000) elmer     (1000)     6244 2023-01-15 22:00:23.000000 sqlalchemy-json-0.6.0/sqlalchemy_json/track.py
+drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2023-07-06 21:44:12.526032 sqlalchemy-json-0.6.0/sqlalchemy_json.egg-info/
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)     6769 2023-07-06 21:44:12.000000 sqlalchemy-json-0.6.0/sqlalchemy_json.egg-info/PKG-INFO
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)      341 2023-07-06 21:44:12.000000 sqlalchemy-json-0.6.0/sqlalchemy_json.egg-info/SOURCES.txt
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)        1 2023-07-06 21:44:12.000000 sqlalchemy-json-0.6.0/sqlalchemy_json.egg-info/dependency_links.txt
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)        1 2015-08-11 09:41:31.000000 sqlalchemy-json-0.6.0/sqlalchemy_json.egg-info/not-zip-safe
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)       16 2023-07-06 21:44:12.000000 sqlalchemy-json-0.6.0/sqlalchemy_json.egg-info/requires.txt
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)       16 2023-07-06 21:44:12.000000 sqlalchemy-json-0.6.0/sqlalchemy_json.egg-info/top_level.txt
+drwxrwxr-x   0 elmer     (1000) elmer     (1000)        0 2023-07-06 21:44:12.526032 sqlalchemy-json-0.6.0/test/
+-rw-rw-r--   0 elmer     (1000) elmer     (1000)     4320 2023-07-06 21:43:16.000000 sqlalchemy-json-0.6.0/test/test_sqlalchemy_json.py
```

### Comparing `sqlalchemy-json-0.5.0/README.rst` & `sqlalchemy-json-0.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -89,26 +89,33 @@
             return json.dumps(value)
 
         def process_result_value(self, value, dialect):
             return json.loads(value)
 
 
     postgres_jsonb_mutable = mutable_json_type(dbtype=JSONB)
-    string_backed_nested_mutable = mutable)json_type(dbtype=JsonString, nested=True)
+    string_backed_nested_mutable = mutable_json_type(dbtype=JsonString, nested=True)
 
 
 Dependencies
 ============
 
-* ``six`` to support both Python 2 and 3.
+* ``sqlalchemy``
 
 
 Changelog
 =========
 
+0.6.0
+-----
+
+* Fixes pickling support (https://github.com/edelooff/sqlalchemy-json/issues/36)
+* Drops python 2.x support (previously claimed, but already broken for some time)
+* Removes test runners for CPython 3.6 since Github actions support has been dropped
+
 0.5.0
 -----
 * Fixes a lingering Python 3 compatibility issue (``cmp`` parameter for ``TrackedList.sort``)
 * Adds pickling and unpickling support (https://github.com/edelooff/sqlalchemy-json/pull/28)
 * Adds tracking for dictionary in-place updates (https://github.com/edelooff/sqlalchemy-json/pull/33)
 
 0.4.0
```

### Comparing `sqlalchemy-json-0.5.0/setup.py` & `sqlalchemy-json-0.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
     here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(here, filename)) as fp:
         return fp.read()
 
 
 setup(
     name="sqlalchemy-json",
-    version="0.5.0",
+    version="0.6.0",
     author="Elmer de Looff",
     author_email="elmer.delooff@gmail.com",
     description="JSON type with nested change tracking for SQLAlchemy",
     long_description=contents("README.rst"),
+    long_description_content_type="text/x-rst",
     keywords="sqlalchemy json mutable",
     license="BSD",
     url="https://github.com/edelooff/sqlalchemy-json",
     packages=["sqlalchemy_json"],
-    install_requires=[
-        "six",
-        "sqlalchemy>=0.7"],
+    python_requires=">= 3.6",
+    install_requires=["sqlalchemy>=0.7"],
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
-        "Topic :: Database"])
+        "Topic :: Database",
+    ],
+)
```

### Comparing `sqlalchemy-json-0.5.0/sqlalchemy_json/__init__.py` & `sqlalchemy-json-0.6.0/sqlalchemy_json/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from sqlalchemy.ext.mutable import Mutable, MutableDict
 from sqlalchemy.types import JSON
 
 from .track import TrackedDict, TrackedList
 
 __all__ = "MutableJson", "NestedMutableJson", "mutable_json_type"
+__version__ = "0.6.0"
 
 
-class NestedMutableDict(TrackedDict, Mutable):
+class _PickleMixin:
+    def __getstate__(self):
+        d = self.__dict__.copy()
+        d.pop("_parents", None)
+        return d
+
+
+class NestedMutableDict(TrackedDict, Mutable, _PickleMixin):
     @classmethod
     def coerce(cls, key, value):
         if isinstance(value, cls):
             return value
         if isinstance(value, dict):
             return cls(value)
         return super(cls).coerce(key, value)
 
 
-class NestedMutableList(TrackedList, Mutable):
+class NestedMutableList(TrackedList, Mutable, _PickleMixin):
     @classmethod
     def coerce(cls, key, value):
         if isinstance(value, cls):
             return value
         if isinstance(value, list):
             return cls(value)
         return super(cls).coerce(key, value)
```

### Comparing `sqlalchemy-json-0.5.0/sqlalchemy_json/track.py` & `sqlalchemy-json-0.6.0/sqlalchemy_json/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 A function for automatic conversion of dicts and lists to their tracked
 counterparts is also included.
 """
 
 import logging
 from itertools import chain
 
-from six import iteritems
 from sqlalchemy.ext.mutable import Mutable
 
 
 logger = logging.getLogger(__name__)
 
 
 class TrackedObject(object):
@@ -83,15 +82,15 @@
     def convert_items(self, items):
         """Generator like `convert_iterable`, but for 2-tuple iterators."""
         return ((key, self.convert(value, self)) for key, value in items)
 
     def convert_mapping(self, mapping):
         """Convenience method to track either a dict or a 2-tuple iterator."""
         if isinstance(mapping, dict):
-            return self.convert_items(iteritems(mapping))
+            return self.convert_items(iter(mapping.items()))
         return self.convert_items(mapping)
 
     def _repr(self):
         """Simple object representation."""
         return "<%(namespace)s.%(type)s object at 0x%(address)0xd>" % {
             "namespace": __name__,
             "type": type(self).__name__,
```

### Comparing `sqlalchemy-json-0.5.0/test/test_sqlalchemy_json.py` & `sqlalchemy-json-0.6.0/test/test_sqlalchemy_json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import pickle
 import sys
 
 import pytest
 
 from sqlalchemy import (
     Column,
@@ -13,14 +14,15 @@
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
 from sqlalchemy_json import (
     MutableJson,
     NestedMutableDict,
     NestedMutableJson,
+    NestedMutableList,
 )
 
 SQLALCHEMY_DATABASE_URL = "sqlite://"
 Base = declarative_base()
 
 
 class Author(Base):
@@ -97,28 +99,54 @@
     article.references["github.com"]["zzzeek/sqlalchemy"].append(4)
     session.commit()
     assert article.references["github.com"]["edelooff/sqlalchemy-json"] == 5
     assert article.references["github.com"]["zzzeek/sqlalchemy"] == [1, 2, 3, 4]
 
 
 def test_nested_pickling():
-    one = NestedMutableDict({"numbers": [1, 2, 3, 4]})
-    two = NestedMutableDict({"numbers": [5, 6, 7]})
+    one = NestedMutableDict({"numbers": [1, 2, 3, {"4": 4}]})
+    two = NestedMutableList([5, 6, 7, {"numbers": [8, 9, 10]}])
+
+    # Force evaluation of _parents property
+    one._parents
+    two._parents
+
     one_reloaded = pickle.loads(pickle.dumps(one))
     two_reloaded = pickle.loads(pickle.dumps(two))
     assert one == one_reloaded
     assert two == two_reloaded
 
     one_reloaded["numbers"].append(5)
-    assert one_reloaded["numbers"] == [1, 2, 3, 4, 5]
-    assert one["numbers"] == [1, 2, 3, 4]
-
+    assert one_reloaded["numbers"] == [1, 2, 3, {"4": 4}, 5]
+    assert one["numbers"] == [1, 2, 3, {"4": 4}]
     assert one_reloaded["numbers"].parent is one_reloaded
-    assert two_reloaded["numbers"].parent is two_reloaded
-    assert one_reloaded is not two_reloaded
+    assert one_reloaded["numbers"][3].parent is one_reloaded["numbers"]
+
+    two_reloaded.append(11)
+    assert two_reloaded == [5, 6, 7, {"numbers": [8, 9, 10]}, 11]
+    assert two == [5, 6, 7, {"numbers": [8, 9, 10]}]
+    assert two_reloaded[3].parent is two_reloaded
+    assert two_reloaded[3]["numbers"].parent is two_reloaded[3]
+
+
+def test_deepcopy(session, article):
+    """Modifying a copy of a MutableJSON instance does not affect the source."""
+    new_repo = "someone/newrepo"
+    assert new_repo not in article.references["github.com"]
+
+    article_copy = Article(
+        author=article.author,
+        content=article.content,
+        references=copy.deepcopy(article.references),
+    )
+    article_copy.references["github.com"][new_repo] = 10
+    article_copy.references["modified"] = True
+
+    assert new_repo not in article.references["github.com"]
+    assert not session.dirty
 
 
 @pytest.mark.skipif(sys.version_info < (3, 9), reason="Python 3.9+ required")
 def test_dict_merging(session, article):
     article.references["github.com"] |= {"someone/somerepo": 10}
     session.commit()
     assert article.references == {
```

