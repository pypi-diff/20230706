# Comparing `tmp/lollipop-1.1.7.tar.gz` & `tmp/lollipop-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lollipop-1.1.7.tar", last modified: Thu Apr 12 22:32:59 2018, max compression
+gzip compressed data, was "lollipop-1.1.8.tar", last modified: Thu Jul  6 02:34:48 2023, max compression
```

## Comparing `lollipop-1.1.7.tar` & `lollipop-1.1.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mkulkin    (501) staff       (20)        0 2018-04-12 22:32:59.000000 lollipop-1.1.7/
-drwxr-xr-x   0 mkulkin    (501) staff       (20)        0 2018-04-12 22:32:59.000000 lollipop-1.1.7/lollipop/
--rw-r--r--   0 mkulkin    (501) staff       (20)      833 2017-06-26 17:19:57.000000 lollipop-1.1.7/lollipop/compat.py
--rw-r--r--   0 mkulkin    (501) staff       (20)     4312 2016-08-26 21:45:15.000000 lollipop-1.1.7/lollipop/ordereddict.py
--rw-r--r--   0 mkulkin    (501) staff       (20)    12008 2017-06-26 17:19:57.000000 lollipop-1.1.7/lollipop/validators.py
--rw-r--r--   0 mkulkin    (501) staff       (20)       50 2018-04-12 22:29:48.000000 lollipop-1.1.7/lollipop/__init__.py
--rw-r--r--   0 mkulkin    (501) staff       (20)    62840 2018-04-12 22:28:52.000000 lollipop-1.1.7/lollipop/types.py
--rw-r--r--   0 mkulkin    (501) staff       (20)     1946 2016-09-26 20:10:42.000000 lollipop-1.1.7/lollipop/type_registry.py
--rw-r--r--   0 mkulkin    (501) staff       (20)     4725 2017-09-25 19:30:29.000000 lollipop-1.1.7/lollipop/utils.py
--rw-r--r--   0 mkulkin    (501) staff       (20)     5749 2017-02-07 09:12:15.000000 lollipop-1.1.7/lollipop/errors.py
--rw-r--r--   0 mkulkin    (501) staff       (20)     5582 2018-04-12 22:32:59.000000 lollipop-1.1.7/PKG-INFO
--rw-r--r--   0 mkulkin    (501) staff       (20)     1079 2016-07-19 18:11:31.000000 lollipop-1.1.7/LICENSE
-drwxr-xr-x   0 mkulkin    (501) staff       (20)        0 2018-04-12 22:32:59.000000 lollipop-1.1.7/tests/
--rw-r--r--   0 mkulkin    (501) staff       (20)     9941 2017-09-25 19:30:29.000000 lollipop-1.1.7/tests/test_utils.py
--rw-r--r--   0 mkulkin    (501) staff       (20)     6937 2016-07-28 20:01:31.000000 lollipop-1.1.7/tests/test_errors.py
--rw-r--r--   0 mkulkin    (501) staff       (20)     1403 2016-09-26 20:10:42.000000 lollipop-1.1.7/tests/test_type_registry.py
--rw-r--r--   0 mkulkin    (501) staff       (20)    15361 2017-06-26 17:19:57.000000 lollipop-1.1.7/tests/test_validators.py
--rw-r--r--   0 mkulkin    (501) staff       (20)   108126 2018-04-12 22:28:52.000000 lollipop-1.1.7/tests/test_types.py
--rw-r--r--   0 mkulkin    (501) staff       (20)      214 2016-07-28 18:32:14.000000 lollipop-1.1.7/MANIFEST.in
-drwxr-xr-x   0 mkulkin    (501) staff       (20)        0 2018-04-12 22:32:59.000000 lollipop-1.1.7/docs/
--rw-r--r--   0 mkulkin    (501) staff       (20)      344 2017-02-02 19:34:14.000000 lollipop-1.1.7/docs/install.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)      558 2016-08-21 06:34:28.000000 lollipop-1.1.7/docs/index.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)     1746 2017-06-26 17:19:57.000000 lollipop-1.1.7/docs/custom_types.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)      441 2016-09-26 20:10:42.000000 lollipop-1.1.7/docs/api_reference.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)       28 2016-07-27 17:46:46.000000 lollipop-1.1.7/docs/requirements.txt
--rw-r--r--   0 mkulkin    (501) staff       (20)     7614 2016-07-28 20:01:31.000000 lollipop-1.1.7/docs/Makefile
--rw-r--r--   0 mkulkin    (501) staff       (20)     1915 2016-08-21 06:34:28.000000 lollipop-1.1.7/docs/why.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)    10133 2017-06-26 17:28:14.000000 lollipop-1.1.7/docs/conf.py
--rw-r--r--   0 mkulkin    (501) staff       (20)      243 2016-09-26 20:10:42.000000 lollipop-1.1.7/docs/kudos.rst
-drwxr-xr-x   0 mkulkin    (501) staff       (20)        0 2018-04-12 22:32:59.000000 lollipop-1.1.7/docs/_static/
--rw-r--r--   0 mkulkin    (501) staff       (20)       46 2016-08-12 01:32:21.000000 lollipop-1.1.7/docs/_static/custom.css
--rw-r--r--   0 mkulkin    (501) staff       (20)    20856 2016-08-12 01:32:21.000000 lollipop-1.1.7/docs/_static/lollipop.png
--rw-r--r--   0 mkulkin    (501) staff       (20)     5591 2016-09-26 20:10:42.000000 lollipop-1.1.7/docs/quickstart.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)       48 2016-08-21 06:34:28.000000 lollipop-1.1.7/docs/license.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)    11234 2016-09-26 20:10:42.000000 lollipop-1.1.7/docs/objects.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)       46 2016-08-12 01:42:27.000000 lollipop-1.1.7/docs/changelog.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)     3196 2016-08-21 06:34:28.000000 lollipop-1.1.7/docs/validation.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)     1942 2016-08-21 06:34:28.000000 lollipop-1.1.7/docs/modifiers.rst
-drwxr-xr-x   0 mkulkin    (501) staff       (20)        0 2018-04-12 22:32:59.000000 lollipop-1.1.7/lollipop.egg-info/
--rw-r--r--   0 mkulkin    (501) staff       (20)     5582 2018-04-12 22:32:58.000000 lollipop-1.1.7/lollipop.egg-info/PKG-INFO
--rw-r--r--   0 mkulkin    (501) staff       (20)        1 2016-07-28 20:02:35.000000 lollipop-1.1.7/lollipop.egg-info/not-zip-safe
--rw-r--r--   0 mkulkin    (501) staff       (20)      820 2018-04-12 22:32:59.000000 lollipop-1.1.7/lollipop.egg-info/SOURCES.txt
--rw-r--r--   0 mkulkin    (501) staff       (20)        9 2018-04-12 22:32:58.000000 lollipop-1.1.7/lollipop.egg-info/top_level.txt
--rw-r--r--   0 mkulkin    (501) staff       (20)        1 2018-04-12 22:32:58.000000 lollipop-1.1.7/lollipop.egg-info/dependency_links.txt
--rw-r--r--   0 mkulkin    (501) staff       (20)     1483 2018-01-25 19:42:09.000000 lollipop-1.1.7/setup.py
--rw-r--r--   0 mkulkin    (501) staff       (20)      100 2018-04-12 22:32:59.000000 lollipop-1.1.7/setup.cfg
--rw-r--r--   0 mkulkin    (501) staff       (20)     3551 2017-02-02 19:33:34.000000 lollipop-1.1.7/README.rst
--rw-r--r--   0 mkulkin    (501) staff       (20)     3839 2018-04-12 22:31:57.000000 lollipop-1.1.7/CHANGELOG.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-06 02:34:48.923911 lollipop-1.1.8/
+-rw-r--r--   0 max        (501) staff       (20)     4086 2023-07-06 02:27:43.000000 lollipop-1.1.8/CHANGELOG.rst
+-rw-r--r--   0 max        (501) staff       (20)     1079 2023-04-18 02:45:20.000000 lollipop-1.1.8/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)      214 2023-04-18 02:45:20.000000 lollipop-1.1.8/MANIFEST.in
+-rw-r--r--   0 max        (501) staff       (20)     4541 2023-07-06 02:34:48.923986 lollipop-1.1.8/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     3551 2023-04-18 02:45:20.000000 lollipop-1.1.8/README.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-06 02:34:48.921172 lollipop-1.1.8/docs/
+-rw-r--r--   0 max        (501) staff       (20)     7614 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/Makefile
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-06 02:34:48.921422 lollipop-1.1.8/docs/_static/
+-rw-r--r--   0 max        (501) staff       (20)       46 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/_static/custom.css
+-rw-r--r--   0 max        (501) staff       (20)    20856 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/_static/lollipop.png
+-rw-r--r--   0 max        (501) staff       (20)      441 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/api_reference.rst
+-rw-r--r--   0 max        (501) staff       (20)       46 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/changelog.rst
+-rw-r--r--   0 max        (501) staff       (20)    10133 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/conf.py
+-rw-r--r--   0 max        (501) staff       (20)     1746 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/custom_types.rst
+-rw-r--r--   0 max        (501) staff       (20)      558 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/index.rst
+-rw-r--r--   0 max        (501) staff       (20)      344 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/install.rst
+-rw-r--r--   0 max        (501) staff       (20)      243 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/kudos.rst
+-rw-r--r--   0 max        (501) staff       (20)       48 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/license.rst
+-rw-r--r--   0 max        (501) staff       (20)     1942 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/modifiers.rst
+-rw-r--r--   0 max        (501) staff       (20)    11234 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/objects.rst
+-rw-r--r--   0 max        (501) staff       (20)     5591 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/quickstart.rst
+-rw-r--r--   0 max        (501) staff       (20)       28 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)     3196 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/validation.rst
+-rw-r--r--   0 max        (501) staff       (20)     1915 2023-04-18 02:45:20.000000 lollipop-1.1.8/docs/why.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-06 02:34:48.922475 lollipop-1.1.8/lollipop/
+-rw-r--r--   0 max        (501) staff       (20)       50 2023-07-06 02:28:01.000000 lollipop-1.1.8/lollipop/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)      949 2023-04-18 02:46:25.000000 lollipop-1.1.8/lollipop/compat.py
+-rw-r--r--   0 max        (501) staff       (20)     5749 2023-04-18 02:45:20.000000 lollipop-1.1.8/lollipop/errors.py
+-rw-r--r--   0 max        (501) staff       (20)     4312 2023-04-18 02:45:20.000000 lollipop-1.1.8/lollipop/ordereddict.py
+-rw-r--r--   0 max        (501) staff       (20)     1946 2023-04-18 02:45:20.000000 lollipop-1.1.8/lollipop/type_registry.py
+-rw-r--r--   0 max        (501) staff       (20)    63049 2023-07-06 02:25:47.000000 lollipop-1.1.8/lollipop/types.py
+-rw-r--r--   0 max        (501) staff       (20)     4891 2023-04-18 02:47:39.000000 lollipop-1.1.8/lollipop/utils.py
+-rw-r--r--   0 max        (501) staff       (20)    12008 2023-04-18 02:45:20.000000 lollipop-1.1.8/lollipop/validators.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-06 02:34:48.923116 lollipop-1.1.8/lollipop.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     4541 2023-07-06 02:34:48.000000 lollipop-1.1.8/lollipop.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      820 2023-07-06 02:34:48.000000 lollipop-1.1.8/lollipop.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-07-06 02:34:48.000000 lollipop-1.1.8/lollipop.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-07-06 02:31:37.000000 lollipop-1.1.8/lollipop.egg-info/not-zip-safe
+-rw-r--r--   0 max        (501) staff       (20)        9 2023-07-06 02:34:48.000000 lollipop-1.1.8/lollipop.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)       79 2023-07-06 02:34:48.924182 lollipop-1.1.8/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)     1483 2023-04-18 02:45:20.000000 lollipop-1.1.8/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-06 02:34:48.923787 lollipop-1.1.8/tests/
+-rw-r--r--   0 max        (501) staff       (20)     6937 2023-04-18 02:45:20.000000 lollipop-1.1.8/tests/test_errors.py
+-rw-r--r--   0 max        (501) staff       (20)     1403 2023-04-18 02:45:20.000000 lollipop-1.1.8/tests/test_type_registry.py
+-rw-r--r--   0 max        (501) staff       (20)   109088 2023-07-06 02:25:47.000000 lollipop-1.1.8/tests/test_types.py
+-rw-r--r--   0 max        (501) staff       (20)    10416 2023-04-18 02:47:39.000000 lollipop-1.1.8/tests/test_utils.py
+-rw-r--r--   0 max        (501) staff       (20)    15361 2023-04-18 02:45:20.000000 lollipop-1.1.8/tests/test_validators.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lollipop-1.1.7/lollipop/compat.py` & `lollipop-1.1.8/lollipop/compat.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,10 +22,16 @@
 
 if PY26:
     from .ordereddict import OrderedDict
     from UserDict import DictMixin
 else:
     from collections import OrderedDict
     try:
-        from collections import MutableMapping as DictMixin
+        from collections import (
+            MutableMapping as DictMixin,
+            Mapping,
+            Sequence)
     except ImportError:
-        from collections.abc import MutableMapping as DictMixin
+        from collections.abc import (
+            MutableMapping as DictMixin,
+            Mapping,
+            Sequence)
```

### Comparing `lollipop-1.1.7/lollipop/ordereddict.py` & `lollipop-1.1.8/lollipop/ordereddict.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/lollipop/validators.py` & `lollipop-1.1.8/lollipop/validators.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/lollipop/types.py` & `lollipop-1.1.8/lollipop/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,25 +170,27 @@
                 * data - actual value
     """
     num_type = float
     default_error_messages = {
         'invalid': 'Value should be number',
     }
 
+    _invalid_types = string_types + (bool,)
+
     def _normalize(self, value):
         try:
             return self.num_type(value)
         except (TypeError, ValueError):
             self._fail('invalid', data=value)
 
     def load(self, data, *args, **kwargs):
         if data is MISSING or data is None:
             self._fail('required')
 
-        if isinstance(data, string_types):
+        if isinstance(data, self._invalid_types):
             self._fail('invalid')
 
         return super(Number, self).load(self._normalize(data), *args, **kwargs)
 
     def dump(self, value, *args, **kwargs):
         if value is MISSING or value is None:
             self._fail('required')
@@ -802,43 +804,45 @@
             'foo': 'hello', 'bar': 123,
         })
 
     :param dict value_types: A single :class:`Type` for all dict values or mapping
         of allowed keys to :class:`Type` instances (defaults to :class:`Any`)
     :param Type key_type: Type for dictionary keys (defaults to :class:`Any`).
         Can be used to either transform or validate dictionary keys.
+    :param bool ordered: Preserve items order of a dictionary.
     :param kwargs: Same keyword arguments as for :class:`Type`.
 
     Error message keys:
         * invalid - invalid value type. Interpolation data:
                 * data - actual value
     """
 
     default_error_messages = {
         'invalid': 'Value should be dict',
     }
 
-    def __init__(self, value_types=None, key_type=None, **kwargs):
+    def __init__(self, value_types=None, key_type=None, ordered=False, **kwargs):
         super(Dict, self).__init__(**kwargs)
         if value_types is None:
             value_types = DictWithDefault(default=Any())
         elif isinstance(value_types, Type):
             value_types = DictWithDefault(default=value_types)
         self.value_types = value_types
         self.key_type = key_type or Any()
+        self.ordered = ordered
 
     def load(self, data, *args, **kwargs):
         if data is MISSING or data is None:
             self._fail('required')
 
         if not is_mapping(data):
             self._fail('invalid', data=data)
 
         errors_builder = ValidationErrorBuilder()
-        result = {}
+        result = OrderedDict() if self.ordered else {}
         for k, v in iteritems(data):
             try:
                 k = self.key_type.load(k, *args, **kwargs)
             except ValidationError as ve:
                 errors_builder.add_error(k, ve.messages)
 
             if k is MISSING:
@@ -874,15 +878,15 @@
         if value is MISSING or value is None:
             self._fail('required')
 
         if not is_mapping(value):
             self._fail('invalid', data=value)
 
         errors_builder = ValidationErrorBuilder()
-        result = {}
+        result = OrderedDict() if self.ordered else {}
         for k, v in iteritems(value):
             value_type = self.value_types.get(k)
             if value_type is None:
                 continue
 
             try:
                 k = self.key_type.dump(k, *args, **kwargs)
@@ -1283,18 +1287,18 @@
         not be specified.
     :param fields: List of name-to-value tuples or mapping of object field names to
         :class:`Type`, :class:`Field` objects or constant values.
     :param callable contructor: Deserialized value constructor. Constructor
         should take all fields values as keyword arguments.
     :param Field default_field_type: Default field type to use for fields defined
         by their type.
-    :param (bool, :class:`Type` or :class:`Field`) allow_extra_fields: If False,
-        it will raise :exc:`~lollipop.errors.ValidationError` for all extra dict
-        keys during deserialization. If True, will ignore all extra fields.
-        If Type or Field, extra fields will be loaded and validated with given
+    :param allow_extra_fields: If False, it will raise
+        :exc:`~lollipop.errors.ValidationError` for all extra dict keys during
+        deserialization. If True, will ignore all extra fields. If :class:`Type` or
+        :class:`Field`, extra fields will be loaded and validated with given
         type/field and stored in load result.
     :param only: Field name or list of field names to include in this object
         from it's base classes. All other base classes' fields won't be used.
         Does not affect own fields.
     :param exclude: Field name or list of field names to exclude from this
         object from base classes. All other base classes' fields will be included.
         Does not affect own fields.
```

### Comparing `lollipop-1.1.7/lollipop/type_registry.py` & `lollipop-1.1.8/lollipop/type_registry.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/lollipop/utils.py` & `lollipop-1.1.8/lollipop/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import inspect
 import re
-from lollipop.compat import DictMixin, iterkeys
-import collections
+from lollipop.compat import DictMixin, Sequence, Mapping, iterkeys, PY2
 
 
 def identity(value):
     """Function that returns its argument."""
     return value
 
 def constant(value):
@@ -13,19 +12,29 @@
     def func(*args, **kwargs):
         return value
     return func
 
 
 def is_sequence(value):
     """Returns True if value supports list interface; False - otherwise"""
-    return isinstance(value, collections.Sequence)
+    return isinstance(value, Sequence)
 
 def is_mapping(value):
     """Returns True if value supports dict interface; False - otherwise"""
-    return isinstance(value, collections.Mapping)
+    return isinstance(value, Mapping)
+
+def get_arg_count(func):
+    """Calculates a number of arguments based on a signature."""
+
+    if PY2:
+        return len(inspect.getargspec(func).args)
+
+    spec = inspect.getfullargspec(func)
+
+    return len(spec.args) + len(spec.kwonlyargs)
 
 
 # Backward compatibility
 is_list = is_sequence
 is_dict = is_mapping
 
 
@@ -33,21 +42,21 @@
     """
     Check if given function has no more arguments than given. If so, wrap it
     into another function that takes extra argument and drops it.
     Used to support user providing callback functions that are not context aware.
     """
     try:
         if inspect.ismethod(func):
-            arg_count = len(inspect.getargspec(func).args) - 1
+            arg_count = get_arg_count(func) - 1
         elif inspect.isfunction(func):
-            arg_count = len(inspect.getargspec(func).args)
+            arg_count = get_arg_count(func)
         elif inspect.isclass(func):
-            arg_count = len(inspect.getargspec(func.__init__).args) - 1
+            arg_count = get_arg_count(func.__init__) - 1
         else:
-            arg_count = len(inspect.getargspec(func.__call__).args) - 1
+            arg_count = get_arg_count(func.__call__) - 1
     except TypeError:
         arg_count = numargs
 
     if arg_count <= numargs:
         def normalized(*args):
             return func(*args[:-1])
```

### Comparing `lollipop-1.1.7/lollipop/errors.py` & `lollipop-1.1.8/lollipop/errors.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/PKG-INFO` & `lollipop-1.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: lollipop
-Version: 1.1.7
+Version: 1.1.8
 Summary: Data serialization and validation library
 Home-page: https://github.com/maximkulkin/lollipop
 Author: Maxim Kulkin
 Author-email: maxim.kulkin@gmail.com
 License: MIT
-Description: ********
-        lollipop
-        ********
-        
-        .. image:: https://img.shields.io/pypi/l/lollipop.svg
-            :target: https://github.com/maximkulkin/lollipop/blob/master/LICENSE
-            :alt: License: MIT
-        
-        .. image:: https://img.shields.io/travis/maximkulkin/lollipop.svg
-            :target: https://travis-ci.org/maximkulkin/lollipop
-            :alt: Build Status
-        
-        .. image:: https://readthedocs.org/projects/lollipop/badge/?version=latest
-            :target: http://lollipop.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/pypi/v/lollipop.svg
-            :target: https://pypi.python.org/pypi/lollipop
-            :alt: PyPI
-        
-        Data serialization and validation library
-        
-        Features
-        ========
-        * flexible schema definition API with powerful type combinators
-        * data validation
-        * serialization/deserialization
-        * in-place deserialization
-        
-        Example
-        =======
-        .. code-block:: python
-        
-            from lollipop.types import Object, String, Date
-            from lollipop.validators import Length
-            from collections import namedtuple
-            from datetime import date
-        
-            Person = namedtuple('Person', ['name'])
-            Book = namedtuple('Book', ['title', 'publish_date', 'author'])
-        
-            PersonType = Object({
-                'name': String(validate=Length(min=1)),
-            }, constructor=Person)
-        
-            BookType = Object({
-                'title': String(),
-                'publish_date': Date(),
-                'author': PersonType,
-            }, constructor=Book)
-        
-            harryPotter1 = Book(
-                title='Harry Potter and the Philosopher\'s Stone',
-                publish_date=date(1997, 6, 26),
-                author=Person(name='J. K. Rowling')
-            )
-        
-            # Dumping
-            BookType.dump(harryPotter1)
-            # => {'title': 'Harry Potter and the Philosopher\'s Stone',
-            #     'publish_date': '1997-06-26',
-            #     'author': {'name': 'J. K. Rowling'}}
-        
-            # Loading
-            BookType.load({'title': 'Harry Potter and the Philosopher\'s Stone',
-                           'publish_date': '1997-06-26',
-                           'author': {'name': 'J. K. Rowling'}})
-            # => Book(title='Harry Potter and the Philosopher\'s Stone',
-            #         publish_date=date(1997, 06, 26),
-            #         author=User(name='J. K. Rowling'))
-        
-            # Partial inplace loading
-            BookType.load_into(harryPotter1, {'publish_date': '1997-06-27'})
-            # => Book(title='Harry Potter and the Philosopher\'s Stone',
-            #         publish_date=date(1997, 06, 27),
-            #         author=User(name='J. K. Rowling'))
-        
-            # Loading list of objects
-            List(BookType).load([
-                {'title': 'Harry Potter and the Philosopher\'s Stone',
-                 'publish_date': '1997-06-26',
-                 'author': {'name': 'J. K. Rowling'}},
-                {'title': 'Harry Potter and the Chamber of Secrets',
-                 'publish_date': '1998-07-02',
-                 'author': {'name': 'J. K. Rowling'}},
-            ])
-            # => [Book(...), Book(...)]
-        
-            # Validation
-            BookType.validate({
-                'title': 'Harry Potter and the Philosopher\'s Stone',
-                'author': {'name': ''},
-            })
-            # => {'author': {'name': 'Length should be at least 1'},
-            #     'publish_date': 'Value is required'}
-        
-        
-        Installation
-        ============
-        
-        ::
-        
-            $ pip install lollipop
-        
-        
-        Documentation
-        =============
-        
-        Documentation is available at http://lollipop.readthedocs.io/ .
-        
-        
-        Requirements
-        ============
-        
-        - Python >= 2.6 or <= 3.6
-        
-        
-        Project Links
-        =============
-        
-        - Documentation: http://lollipop.readthedocs.io/
-        - PyPI: https://pypi.python.org/pypi/lollipop
-        - Issues: https://github.com/maximkulkin/lollipop/issues
-        
-        
-        License
-        =======
-        
-        MIT licensed. See the bundled `LICENSE <https://github.com/maximkulkin/lollipop/blob/master/LICENSE>`_ file for more details.
-        
 Keywords: serialization,rest,json,api,marshal,marshalling,deserialization,validation,schema,marshmallow
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+
+********
+lollipop
+********
+
+.. image:: https://img.shields.io/pypi/l/lollipop.svg
+    :target: https://github.com/maximkulkin/lollipop/blob/master/LICENSE
+    :alt: License: MIT
+
+.. image:: https://img.shields.io/travis/maximkulkin/lollipop.svg
+    :target: https://travis-ci.org/maximkulkin/lollipop
+    :alt: Build Status
+
+.. image:: https://readthedocs.org/projects/lollipop/badge/?version=latest
+    :target: http://lollipop.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/lollipop.svg
+    :target: https://pypi.python.org/pypi/lollipop
+    :alt: PyPI
+
+Data serialization and validation library
+
+Features
+========
+* flexible schema definition API with powerful type combinators
+* data validation
+* serialization/deserialization
+* in-place deserialization
+
+Example
+=======
+.. code-block:: python
+
+    from lollipop.types import Object, String, Date
+    from lollipop.validators import Length
+    from collections import namedtuple
+    from datetime import date
+
+    Person = namedtuple('Person', ['name'])
+    Book = namedtuple('Book', ['title', 'publish_date', 'author'])
+
+    PersonType = Object({
+        'name': String(validate=Length(min=1)),
+    }, constructor=Person)
+
+    BookType = Object({
+        'title': String(),
+        'publish_date': Date(),
+        'author': PersonType,
+    }, constructor=Book)
+
+    harryPotter1 = Book(
+        title='Harry Potter and the Philosopher\'s Stone',
+        publish_date=date(1997, 6, 26),
+        author=Person(name='J. K. Rowling')
+    )
+
+    # Dumping
+    BookType.dump(harryPotter1)
+    # => {'title': 'Harry Potter and the Philosopher\'s Stone',
+    #     'publish_date': '1997-06-26',
+    #     'author': {'name': 'J. K. Rowling'}}
+
+    # Loading
+    BookType.load({'title': 'Harry Potter and the Philosopher\'s Stone',
+                   'publish_date': '1997-06-26',
+                   'author': {'name': 'J. K. Rowling'}})
+    # => Book(title='Harry Potter and the Philosopher\'s Stone',
+    #         publish_date=date(1997, 06, 26),
+    #         author=User(name='J. K. Rowling'))
+
+    # Partial inplace loading
+    BookType.load_into(harryPotter1, {'publish_date': '1997-06-27'})
+    # => Book(title='Harry Potter and the Philosopher\'s Stone',
+    #         publish_date=date(1997, 06, 27),
+    #         author=User(name='J. K. Rowling'))
+
+    # Loading list of objects
+    List(BookType).load([
+        {'title': 'Harry Potter and the Philosopher\'s Stone',
+         'publish_date': '1997-06-26',
+         'author': {'name': 'J. K. Rowling'}},
+        {'title': 'Harry Potter and the Chamber of Secrets',
+         'publish_date': '1998-07-02',
+         'author': {'name': 'J. K. Rowling'}},
+    ])
+    # => [Book(...), Book(...)]
+
+    # Validation
+    BookType.validate({
+        'title': 'Harry Potter and the Philosopher\'s Stone',
+        'author': {'name': ''},
+    })
+    # => {'author': {'name': 'Length should be at least 1'},
+    #     'publish_date': 'Value is required'}
+
+
+Installation
+============
+
+::
+
+    $ pip install lollipop
+
+
+Documentation
+=============
+
+Documentation is available at http://lollipop.readthedocs.io/ .
+
+
+Requirements
+============
+
+- Python >= 2.6 or <= 3.6
+
+
+Project Links
+=============
+
+- Documentation: http://lollipop.readthedocs.io/
+- PyPI: https://pypi.python.org/pypi/lollipop
+- Issues: https://github.com/maximkulkin/lollipop/issues
+
+
+License
+=======
+
+MIT licensed. See the bundled `LICENSE <https://github.com/maximkulkin/lollipop/blob/master/LICENSE>`_ file for more details.
```

### Comparing `lollipop-1.1.7/LICENSE` & `lollipop-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/tests/test_utils.py` & `lollipop-1.1.8/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from lollipop.compat import iterkeys, itervalues, iteritems
 from lollipop.utils import call_with_context, to_camel_case, to_snake_case, \
     constant, identity, OpenStruct, DictWithDefault
 import pytest
 
 
 class ObjMethodDummy:
@@ -24,14 +25,27 @@
 
 class ObjClassDummy:
     def __init__(self, a, b, c):
         self.args = (a, b, c)
 
 
 class TestCallWithContext:
+    @pytest.mark.skipif(sys.version_info < (3, 8), reason='Requires python 3.8+')
+    def test_calls_complex_signature(self):
+        class NonLocal:
+            args = None
+
+        def func(a, b, /, c, *d, e=1, f=2, **g):
+            NonLocal.args = a, b, c, d, e, f, g
+            return 42
+
+        context = object()
+        assert call_with_context(func, context, 1, 'foo', True) == 42
+        assert NonLocal.args == (1, 'foo', True, (context,), 1, 2, {})
+
     def test_calls_function_with_given_arguments(self):
         class NonLocal:
             args = None
 
         def func(a, b, c):
             NonLocal.args = (a, b, c)
             return 42
```

### Comparing `lollipop-1.1.7/tests/test_errors.py` & `lollipop-1.1.8/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/tests/test_type_registry.py` & `lollipop-1.1.8/tests/test_type_registry.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/tests/test_validators.py` & `lollipop-1.1.8/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/tests/test_types.py` & `lollipop-1.1.8/tests/test_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,19 +215,29 @@
         assert Number().load(1.23) == 1.23
 
     def test_loading_numeric_as_string(self):
         with pytest.raises(ValidationError) as exc_info:
             Number().load("123")
         assert exc_info.value.messages == Number.default_error_messages['invalid']
 
-    def test_loading_non_numeric_value_raises_ValidationError(self):
+    def test_loading_string_value_raises_ValidationError(self):
         with pytest.raises(ValidationError) as exc_info:
             Number().load("abc")
         assert exc_info.value.messages == Number.default_error_messages['invalid']
 
+    def test_loading_boolean_value_raises_ValidationError(self):
+        with pytest.raises(ValidationError) as exc_info:
+            Number().load(False)
+        assert exc_info.value.messages == Number.default_error_messages['invalid']
+
+    def test_loading_object_value_raises_ValidationError(self):
+        with pytest.raises(ValidationError) as exc_info:
+            Number().load(object())
+        assert exc_info.value.messages == Number.default_error_messages['invalid']
+
     def test_dumping_float_value(self):
         assert Number().dump(1.23) == 1.23
 
     def test_dumping_non_numeric_value_raises_ValidationError(self):
         with pytest.raises(ValidationError) as exc_info:
             Number().dump("abc")
         assert exc_info.value.messages == Number.default_error_messages['invalid']
@@ -781,14 +791,20 @@
 
     def test_loading_passes_context_to_inner_type_load(self):
         inner_type = SpyType()
         context = object()
         Dict(inner_type).load({'foo': 123}, context)
         assert inner_type.load_context == context
 
+    def test_loading_preserves_ordering_when_requested(self):
+        value = OrderedDict([(456, 'bar'), (123, 'foo'), ((789), ('baz'))])
+        assert Dict(Any(), key_type=Integer(), ordered=True).load(
+            value
+        ) == value
+
     def test_dumping_dict_with_custom_key_type(self):
         assert Dict(Any(), key_type=Transform(Integer(), post_dump=str))\
             .dump({123: 'foo', 456: 'bar'}) == {'123': 'foo', '456': 'bar'}
 
     def test_dumping_accepts_any_key_if_key_type_is_not_specified(self):
         assert Dict(Any())\
             .dump({'123': 'foo', 456: 'bar'}) == {'123': 'foo', 456: 'bar'}
@@ -874,14 +890,20 @@
 
     def test_dumping_passes_context_to_inner_type_dump(self):
         inner_type = SpyType()
         context = object()
         Dict(inner_type).dump({'foo': 123}, context)
         assert inner_type.dump_context == context
 
+    def test_dumping_preserves_ordering_when_requested(self):
+        value = OrderedDict([(456, 'bar'), (123, 'foo'), ((789), ('baz'))])
+        assert Dict(Any(), key_type=Integer(), ordered=True).dump(
+            value,
+        ) == value
+
 
 class TestOneOf:
     def test_loading_values_of_one_of_listed_types(self):
         one_of = OneOf([Integer(), String()])
         assert one_of.load('foo') == 'foo'
         assert one_of.load(123) == 123
```

### Comparing `lollipop-1.1.7/docs/index.rst` & `lollipop-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/custom_types.rst` & `lollipop-1.1.8/docs/custom_types.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/Makefile` & `lollipop-1.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/why.rst` & `lollipop-1.1.8/docs/why.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/conf.py` & `lollipop-1.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/_static/lollipop.png` & `lollipop-1.1.8/docs/_static/lollipop.png`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/quickstart.rst` & `lollipop-1.1.8/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/objects.rst` & `lollipop-1.1.8/docs/objects.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/validation.rst` & `lollipop-1.1.8/docs/validation.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/docs/modifiers.rst` & `lollipop-1.1.8/docs/modifiers.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/lollipop.egg-info/PKG-INFO` & `lollipop-1.1.8/lollipop.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: lollipop
-Version: 1.1.7
+Version: 1.1.8
 Summary: Data serialization and validation library
 Home-page: https://github.com/maximkulkin/lollipop
 Author: Maxim Kulkin
 Author-email: maxim.kulkin@gmail.com
 License: MIT
-Description: ********
-        lollipop
-        ********
-        
-        .. image:: https://img.shields.io/pypi/l/lollipop.svg
-            :target: https://github.com/maximkulkin/lollipop/blob/master/LICENSE
-            :alt: License: MIT
-        
-        .. image:: https://img.shields.io/travis/maximkulkin/lollipop.svg
-            :target: https://travis-ci.org/maximkulkin/lollipop
-            :alt: Build Status
-        
-        .. image:: https://readthedocs.org/projects/lollipop/badge/?version=latest
-            :target: http://lollipop.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/pypi/v/lollipop.svg
-            :target: https://pypi.python.org/pypi/lollipop
-            :alt: PyPI
-        
-        Data serialization and validation library
-        
-        Features
-        ========
-        * flexible schema definition API with powerful type combinators
-        * data validation
-        * serialization/deserialization
-        * in-place deserialization
-        
-        Example
-        =======
-        .. code-block:: python
-        
-            from lollipop.types import Object, String, Date
-            from lollipop.validators import Length
-            from collections import namedtuple
-            from datetime import date
-        
-            Person = namedtuple('Person', ['name'])
-            Book = namedtuple('Book', ['title', 'publish_date', 'author'])
-        
-            PersonType = Object({
-                'name': String(validate=Length(min=1)),
-            }, constructor=Person)
-        
-            BookType = Object({
-                'title': String(),
-                'publish_date': Date(),
-                'author': PersonType,
-            }, constructor=Book)
-        
-            harryPotter1 = Book(
-                title='Harry Potter and the Philosopher\'s Stone',
-                publish_date=date(1997, 6, 26),
-                author=Person(name='J. K. Rowling')
-            )
-        
-            # Dumping
-            BookType.dump(harryPotter1)
-            # => {'title': 'Harry Potter and the Philosopher\'s Stone',
-            #     'publish_date': '1997-06-26',
-            #     'author': {'name': 'J. K. Rowling'}}
-        
-            # Loading
-            BookType.load({'title': 'Harry Potter and the Philosopher\'s Stone',
-                           'publish_date': '1997-06-26',
-                           'author': {'name': 'J. K. Rowling'}})
-            # => Book(title='Harry Potter and the Philosopher\'s Stone',
-            #         publish_date=date(1997, 06, 26),
-            #         author=User(name='J. K. Rowling'))
-        
-            # Partial inplace loading
-            BookType.load_into(harryPotter1, {'publish_date': '1997-06-27'})
-            # => Book(title='Harry Potter and the Philosopher\'s Stone',
-            #         publish_date=date(1997, 06, 27),
-            #         author=User(name='J. K. Rowling'))
-        
-            # Loading list of objects
-            List(BookType).load([
-                {'title': 'Harry Potter and the Philosopher\'s Stone',
-                 'publish_date': '1997-06-26',
-                 'author': {'name': 'J. K. Rowling'}},
-                {'title': 'Harry Potter and the Chamber of Secrets',
-                 'publish_date': '1998-07-02',
-                 'author': {'name': 'J. K. Rowling'}},
-            ])
-            # => [Book(...), Book(...)]
-        
-            # Validation
-            BookType.validate({
-                'title': 'Harry Potter and the Philosopher\'s Stone',
-                'author': {'name': ''},
-            })
-            # => {'author': {'name': 'Length should be at least 1'},
-            #     'publish_date': 'Value is required'}
-        
-        
-        Installation
-        ============
-        
-        ::
-        
-            $ pip install lollipop
-        
-        
-        Documentation
-        =============
-        
-        Documentation is available at http://lollipop.readthedocs.io/ .
-        
-        
-        Requirements
-        ============
-        
-        - Python >= 2.6 or <= 3.6
-        
-        
-        Project Links
-        =============
-        
-        - Documentation: http://lollipop.readthedocs.io/
-        - PyPI: https://pypi.python.org/pypi/lollipop
-        - Issues: https://github.com/maximkulkin/lollipop/issues
-        
-        
-        License
-        =======
-        
-        MIT licensed. See the bundled `LICENSE <https://github.com/maximkulkin/lollipop/blob/master/LICENSE>`_ file for more details.
-        
 Keywords: serialization,rest,json,api,marshal,marshalling,deserialization,validation,schema,marshmallow
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+
+********
+lollipop
+********
+
+.. image:: https://img.shields.io/pypi/l/lollipop.svg
+    :target: https://github.com/maximkulkin/lollipop/blob/master/LICENSE
+    :alt: License: MIT
+
+.. image:: https://img.shields.io/travis/maximkulkin/lollipop.svg
+    :target: https://travis-ci.org/maximkulkin/lollipop
+    :alt: Build Status
+
+.. image:: https://readthedocs.org/projects/lollipop/badge/?version=latest
+    :target: http://lollipop.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/lollipop.svg
+    :target: https://pypi.python.org/pypi/lollipop
+    :alt: PyPI
+
+Data serialization and validation library
+
+Features
+========
+* flexible schema definition API with powerful type combinators
+* data validation
+* serialization/deserialization
+* in-place deserialization
+
+Example
+=======
+.. code-block:: python
+
+    from lollipop.types import Object, String, Date
+    from lollipop.validators import Length
+    from collections import namedtuple
+    from datetime import date
+
+    Person = namedtuple('Person', ['name'])
+    Book = namedtuple('Book', ['title', 'publish_date', 'author'])
+
+    PersonType = Object({
+        'name': String(validate=Length(min=1)),
+    }, constructor=Person)
+
+    BookType = Object({
+        'title': String(),
+        'publish_date': Date(),
+        'author': PersonType,
+    }, constructor=Book)
+
+    harryPotter1 = Book(
+        title='Harry Potter and the Philosopher\'s Stone',
+        publish_date=date(1997, 6, 26),
+        author=Person(name='J. K. Rowling')
+    )
+
+    # Dumping
+    BookType.dump(harryPotter1)
+    # => {'title': 'Harry Potter and the Philosopher\'s Stone',
+    #     'publish_date': '1997-06-26',
+    #     'author': {'name': 'J. K. Rowling'}}
+
+    # Loading
+    BookType.load({'title': 'Harry Potter and the Philosopher\'s Stone',
+                   'publish_date': '1997-06-26',
+                   'author': {'name': 'J. K. Rowling'}})
+    # => Book(title='Harry Potter and the Philosopher\'s Stone',
+    #         publish_date=date(1997, 06, 26),
+    #         author=User(name='J. K. Rowling'))
+
+    # Partial inplace loading
+    BookType.load_into(harryPotter1, {'publish_date': '1997-06-27'})
+    # => Book(title='Harry Potter and the Philosopher\'s Stone',
+    #         publish_date=date(1997, 06, 27),
+    #         author=User(name='J. K. Rowling'))
+
+    # Loading list of objects
+    List(BookType).load([
+        {'title': 'Harry Potter and the Philosopher\'s Stone',
+         'publish_date': '1997-06-26',
+         'author': {'name': 'J. K. Rowling'}},
+        {'title': 'Harry Potter and the Chamber of Secrets',
+         'publish_date': '1998-07-02',
+         'author': {'name': 'J. K. Rowling'}},
+    ])
+    # => [Book(...), Book(...)]
+
+    # Validation
+    BookType.validate({
+        'title': 'Harry Potter and the Philosopher\'s Stone',
+        'author': {'name': ''},
+    })
+    # => {'author': {'name': 'Length should be at least 1'},
+    #     'publish_date': 'Value is required'}
+
+
+Installation
+============
+
+::
+
+    $ pip install lollipop
+
+
+Documentation
+=============
+
+Documentation is available at http://lollipop.readthedocs.io/ .
+
+
+Requirements
+============
+
+- Python >= 2.6 or <= 3.6
+
+
+Project Links
+=============
+
+- Documentation: http://lollipop.readthedocs.io/
+- PyPI: https://pypi.python.org/pypi/lollipop
+- Issues: https://github.com/maximkulkin/lollipop/issues
+
+
+License
+=======
+
+MIT licensed. See the bundled `LICENSE <https://github.com/maximkulkin/lollipop/blob/master/LICENSE>`_ file for more details.
```

### Comparing `lollipop-1.1.7/lollipop.egg-info/SOURCES.txt` & `lollipop-1.1.8/lollipop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/setup.py` & `lollipop-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/README.rst` & `lollipop-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `lollipop-1.1.7/CHANGELOG.rst` & `lollipop-1.1.8/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 ---------
 
+1.1.8 (2023-07-05)
+++++++++++++++++++
+Support "ordered" for the Dict type
+Support PEP3102 and PEP570
+Use correct import paths for Mapping and Sequence
+Fix Number not reporting error for booleans
+Fix Object.allow_extra_fields documentation markup
+
 1.1.7 (2018-04-12)
 ++++++++++++++++++
 
 * Fix Dict missing keys validation on load which resulted in multiple errors
 * Fix missing Modifier export
 
 1.1.6 (2018-01-25)
```

