# Comparing `tmp/packg-0.2.16.tar.gz` & `tmp/packg-0.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.16.tar", last modified: Thu Jun 29 13:21:09 2023, max compression
+gzip compressed data, was "packg-0.2.18.tar", last modified: Thu Jul  6 08:49:20 2023, max compression
```

## Comparing `packg-0.2.16.tar` & `packg-0.2.18.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.899574 packg-0.2.16/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.16/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-06-29 13:21:09.899574 packg-0.2.16/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-06-29 13:20:48.000000 packg-0.2.16/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2317 2023-06-21 09:57:15.000000 packg-0.2.16/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       87 2023-06-29 13:20:48.000000 packg-0.2.16/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-29 13:21:09.903574 packg-0.2.16/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.803572 packg-0.2.16/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.855573 packg-0.2.16/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      130 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7270 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.895574 packg-0.2.16/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      525 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/compressed.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3779 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4735 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4317 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2678 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/paths.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5458 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/strings.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.879574 packg-0.2.16/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      678 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       87 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.16/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.366962 packg-0.2.18/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.18/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-06 08:49:20.366962 packg-0.2.18/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-06 08:46:49.000000 packg-0.2.18/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.18/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-06 08:46:49.000000 packg-0.2.18/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-06 08:49:20.366962 packg-0.2.18/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.242959 packg-0.2.18/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.302960 packg-0.2.18/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7270 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.362961 packg-0.2.18/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      592 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/compressed.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/gitmatcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3779 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5493 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/paths.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/strings.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.322960 packg-0.2.18/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      733 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.18/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.16/LICENSE` & `packg-0.2.18/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/PKG-INFO` & `packg-0.2.18/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.16
+Version: 0.2.18
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.16 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.18 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.16/README.md` & `packg-0.2.18/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/pyproject.toml` & `packg-0.2.18/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 jobs = 1
 
 [tool.pylint.messages_control]
 
 enable = "all"
 
 disable = [
-    'suppressed-message', 'locally-disabled', 'line-too-long', 'missing-module-docstring',
+    'suppressed-message', 'locally-disabled', 'file-ignored',
+    'line-too-long', 'missing-module-docstring',
     'missing-class-docstring', 'missing-function-docstring', 'fixme',
     'f-string-without-interpolation', 'invalid-name',
     'logging-fstring-interpolation', 'consider-iterating-dictionary',
     'use-implicit-booleaness-not-comparison',
     'attribute-defined-outside-init', 'consider-using-with', 'global-statement',
     'import-outside-toplevel', 'super-init-not-called', 'broad-exception-caught',
     'disallowed-name', 'redefined-outer-name', ]
```

### Comparing `packg-0.2.16/src/packg/caching.py` & `packg-0.2.18/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg/constclass.py` & `packg-0.2.18/src/packg/constclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 
 class InstanceToClassDelegator(ABCMeta):
     """Metaclass to delegate instance methods to class methods, e.g.:
     __str__(MyClass) will call MyClass._class_str()."""
 
     def __str__(cls):
-        return cls._class_str()
+        return cls._class_str()  # noqa  # pylint: disable=no-value-for-parameter
 
     def __repr__(cls):
-        return cls._class_repr()
+        return cls._class_repr()  # noqa  # pylint: disable=no-value-for-parameter
 
     def __iter__(cls):
-        return cls._class_iter()
+        return cls._class_iter()  # noqa  # pylint: disable=no-value-for-parameter
 
     def __len__(cls):
-        return cls._class_len()
+        return cls._class_len()  # noqa  # pylint: disable=no-value-for-parameter
 
     def __instancecheck__(cls, instance):
-        return cls._class_instancecheck()
+        return cls._class_instancecheck()  # noqa  # pylint: disable=no-value-for-parameter
 
     @abstractmethod
     def _class_str(cls):
         pass
 
     @abstractmethod
     def _class_repr(cls):
```

### Comparing `packg-0.2.16/src/packg/import_from_source.py` & `packg-0.2.18/src/packg/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg/iotools/__init__.py` & `packg-0.2.18/src/packg/iotools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from .misc import set_working_directory
 from .jsonext import (
     load_json, loads_json, load_jsonl, loads_jsonl,
     dump_json, dumps_json, dump_jsonl, dumps_jsonl ,
     load_json_xz, dump_json_xz)
 
 from .yamlext import load_yaml, loads_yaml, dump_yaml, dumps_yaml
+from .gitmatcher import make_git_pathspec
 
 __all__ = [
     "set_working_directory",
     "load_json", "loads_json", "load_jsonl", "loads_jsonl",
     "dump_json", "dumps_json", "dump_jsonl", "dumps_jsonl",
     "load_json_xz", "dump_json_xz",
     "load_yaml", "loads_yaml", "dump_yaml", "dumps_yaml",
+    "make_git_pathspec",
 ]
```

### Comparing `packg-0.2.16/src/packg/iotools/jsonext.py` & `packg-0.2.18/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.18/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg/iotools/misc.py` & `packg-0.2.18/src/packg/iotools/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg/iotools/yamlext.py` & `packg-0.2.18/src/packg/iotools/yamlext.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """
 Wrapper functions for YAML I/O.
 """
+import os
 import sys
 from collections import abc
 from pathlib import Path
 from typing import Any
 
 import yaml
+from typedparser.objects import is_any_mapping, is_any_iterable
 
 from packg.iotools.misc import read_text_from_file_or_io
-from typedparser.objects import is_any_mapping, is_any_iterable
 from packg.typext import PathOrIO, PathTypeCls
 
 
 def load_yaml(file_or_io: PathOrIO) -> Any:
     yaml_str = read_text_from_file_or_io(file_or_io)
     return loads_yaml(yaml_str)
 
 
 def loads_yaml(yaml_str: str) -> Any:
     return yaml.load(yaml_str, Loader=yaml.SafeLoader)
 
 
 def dump_yaml(obj: Any, file_or_io: PathOrIO, standard_format: bool = True,
-              check_roundtrip: bool = True, **kwargs) -> None:
+              check_roundtrip: bool = True, create_parent=False, **kwargs) -> None:
     """
     convert python object to yaml string and write to file. see dumps_yaml for details.
     """
     s = dumps_yaml(obj, standard_format=standard_format, check_roundtrip=check_roundtrip, **kwargs)
     if isinstance(file_or_io, PathTypeCls):
+        if create_parent:
+            os.makedirs(Path(file_or_io).parent, exist_ok=True)
         Path(file_or_io).write_text(s, encoding="utf8")
         return
     file_or_io.write(s)
 
 
 def dumps_yaml(obj: Any, standard_format: bool = True, check_roundtrip: bool = True,
                **kwargs) -> str:
@@ -62,15 +65,15 @@
     if check_roundtrip:
         re_obj = loads_yaml(yaml_str)
 
         if re_obj != obj:
             print(f"---------- Original object:\n{obj}\n", file=sys.stderr)
             print(f"---------- Reconstructed object:\n{re_obj}\n", file=sys.stderr)
             raise RuntimeError(
-                    "roundtrip failed (original object cannot be reconstructed from yaml, see stderr)")
+                "roundtrip failed (original object cannot be reconstructed from yaml, see stderr)")
     return yaml_str
 
 
 def _dumps_yaml_recursive(
         obj: Any, indent: int = 4, _indent_level: int = 0,
         _is_inside_list: bool = False) -> str:
     """
@@ -79,15 +82,15 @@
     # setup key-value collector and indent level
     indent = " " * (_indent_level * indent)
 
     # check type
     if isinstance(obj, (bool, int, float, type(None))):
         # by yaml standard, if there is only a single objects in the file, append "..." (eod)
         return _convert_single_object_to_yaml_str(
-                obj, remove_eod=_indent_level > 0 or _is_inside_list)
+            obj, remove_eod=_indent_level > 0 or _is_inside_list)
     if isinstance(obj, str):
         # put quotes around strings
         return f"\"{obj}\""
     if is_any_mapping(obj):
         if _is_inside_list:
             # short: dicts inside lists will be kept in the abbreviated form: {key: "value"}
             if len(obj) == 0:
@@ -101,16 +104,16 @@
             dct_strs.append("}")
             return "".join(dct_strs)
         # long: build the dict line by line
         ret_list = []
         for k, v in obj.items():
             kv_sep = "\n" if isinstance(v, abc.Mapping) else " "
             recursive_result = _dumps_yaml_recursive(
-                    v, _indent_level=_indent_level + 1,
-                    _is_inside_list=_is_inside_list)
+                v, _indent_level=_indent_level + 1,
+                _is_inside_list=_is_inside_list)
             ret_list.append(f"{indent}{k}:{kv_sep}{recursive_result}")
         return "\n".join(ret_list)
     if is_any_iterable(obj):
         # iterate lists
         return f"[{', '.join((_dumps_yaml_recursive(v, _is_inside_list=True) for v in obj))}]"
     raise ValueError(f"dict to yaml, value type not understood: {obj}")
```

### Comparing `packg-0.2.16/src/packg/paths.py` & `packg-0.2.18/src/packg/paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,19 +65,19 @@
 
 
 def get_from_environ(env_k: str):
     setup_environ()
     return os.environ[env_k]
 
 
-def print_all_environment_variables():
+def print_all_environment_variables(print_fn=print):
     setup_environ()
-    print(f"Path definitions:")
+    print_fn(f"Path definitions:")
     for env_k in EnvKeys.values():
-        print(f"    {env_k}={os.environ[env_k]}")
+        print_fn(f"    {env_k}={os.environ[env_k]}")
 
 
 def get_data_dir(overwrite_dir: OptionalPathType = None) -> Path:
     return get_path_from_env(EnvKeys.ENV_DATA_DIR, overwrite_dir)
 
 
 def get_result_dir(overwrite_dir: OptionalPathType = None) -> Path:
```

### Comparing `packg-0.2.16/src/packg/strings.py` & `packg-0.2.18/src/packg/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,31 +92,31 @@
 
     def _shorten_keys(keys: List[str]) -> List[Tuple[str, str]]:
         """For a given list of flat keys, find the shortest non-common prefix for each key.
         Returns a list of tuples (short_key, long_key)
         """
         if len(keys) == 0:
             return []
-        longest_len = max([len(key) for key in keys])
+        longest_len = max(len(key) for key in keys)
         remaining_keys = deepcopy(keys)
         done_keys = []
         for k in range(1, longest_len + 1):
             # for a cutoff length k, sort the cut keys into buckets
             cut_keys = defaultdict(list)
             for key in remaining_keys:
                 short_key = key[:k]
                 cut_keys[short_key].append(key)
 
             # buckets with size 1 are done, for other buckets the cutoff needs to increase
             remaining_keys = []
-            for short_key, keys in cut_keys.items():
-                if len(keys) == 1:
-                    done_keys.append((short_key, keys[0]))
+            for short_key, t_keys in cut_keys.items():
+                if len(t_keys) == 1:
+                    done_keys.append((short_key, t_keys[0]))
                 else:
-                    remaining_keys.extend(keys)
+                    remaining_keys.extend(t_keys)
 
             if len(remaining_keys) == 0:
                 break
         else:
             raise ValueError("Could not find abbreviations")  # should not happen ever
         return done_keys
```

### Comparing `packg-0.2.16/src/packg/system.py` & `packg-0.2.18/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg/tensors.py` & `packg-0.2.18/src/packg/tensors.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg/typext.py` & `packg-0.2.18/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.16/src/packg.egg-info/PKG-INFO` & `packg-0.2.18/src/packg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.16
+Version: 0.2.18
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.16 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.18 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.16/src/packg.egg-info/SOURCES.txt` & `packg-0.2.18/src/packg.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 src/packg/__init__.py
 src/packg/caching.py
 src/packg/constclass.py
+src/packg/debugging.py
 src/packg/dtime.py
 src/packg/import_from_source.py
 src/packg/log.py
 src/packg/misc.py
 src/packg/paths.py
 src/packg/strings.py
 src/packg/system.py
@@ -18,11 +19,12 @@
 src/packg.egg-info/SOURCES.txt
 src/packg.egg-info/dependency_links.txt
 src/packg.egg-info/requires.txt
 src/packg.egg-info/top_level.txt
 src/packg.egg-info/zip-safe
 src/packg/iotools/__init__.py
 src/packg/iotools/compressed.py
+src/packg/iotools/gitmatcher.py
 src/packg/iotools/jsonext.py
 src/packg/iotools/jsonext_encoder.py
 src/packg/iotools/misc.py
 src/packg/iotools/yamlext.py
```

