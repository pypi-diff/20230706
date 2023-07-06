# Comparing `tmp/yandil-0.3.2.tar.gz` & `tmp/yandil-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.3.2.tar", max compression
+gzip compressed data, was "yandil-0.3.3.tar", max compression
```

## Comparing `yandil-0.3.2.tar` & `yandil-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1498 2023-07-05 23:46:58.747308 yandil-0.3.2/LICENSE
--rw-r--r--   0        0        0    11594 2023-07-05 23:46:58.747308 yandil-0.3.2/README.md
--rw-r--r--   0        0        0      988 2023-07-05 23:47:54.068124 yandil-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0    11337 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/dependency.py
--rw-r--r--   0        0        0     1505 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3653 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      279 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/instance_and_class_does_not_match_error.py
--rw-r--r--   0        0        0      257 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      301 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     4954 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-07-05 23:46:58.747308 yandil-0.3.2/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 yandil-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-06 15:41:06.050516 yandil-0.3.3/LICENSE
+-rw-r--r--   0        0        0    11594 2023-07-06 15:41:06.050516 yandil-0.3.3/README.md
+-rw-r--r--   0        0        0      988 2023-07-06 15:42:15.159197 yandil-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0    11387 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1505 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3653 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      279 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/instance_and_class_does_not_match_error.py
+-rw-r--r--   0        0        0      257 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      301 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     4954 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 yandil-0.3.3/PKG-INFO
```

### Comparing `yandil-0.3.2/LICENSE` & `yandil-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/README.md` & `yandil-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/pyproject.toml` & `yandil-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.3.2"
+version = "0.3.3"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/DeejayRevok/yandil"
 homepage = "https://github.com/DeejayRevok/yandil"
 keywords = ["dependency injection", "di"]
@@ -34,15 +34,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.2"
+version = "0.3.3"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.3.2/src/yandil/configuration/configuration_container.py` & `yandil-0.3.3/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/container.py` & `yandil-0.3.3/src/yandil/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
 
                 self.__add_children_to_base(cls, base, children_is_primary)
                 orig_classes_args[base_origin_class] = get_args(base)
 
         for base in reference_class.__bases__:
             if self.__should_skip_base(base):
                 continue
-            self.__add_children_to_base(cls, base, children_is_primary)
+            if base not in orig_classes_args:
+                self.__add_children_to_base(cls, base, children_is_primary)
             self.__update_bases_map(
                 cls, children_is_primary, reference_class=base, reference_class_args=orig_classes_args.get(base)
             )
 
     def __should_skip_base(self, base: Type) -> bool:
         return base in self.__EXCLUDED_BASES or base in self.__ABSTRACT_BASES
```

### Comparing `yandil-0.3.2/src/yandil/declarative/decorators.py` & `yandil-0.3.3/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/dependency.py` & `yandil-0.3.3/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/dependency_filler.py` & `yandil-0.3.3/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/discovery/class_discovery.py` & `yandil-0.3.3/src/yandil/discovery/class_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/discovery/module_discovery.py` & `yandil-0.3.3/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.3.3/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.3.3/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/src/yandil/typing_tools.py` & `yandil-0.3.3/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.2/PKG-INFO` & `yandil-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.3.2
+Version: 0.3.3
 Summary: Yet ANother Dependency Injection Library
 Home-page: https://github.com/DeejayRevok/yandil
 License: BSD-3-Clause
 Keywords: dependency injection,di
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
```

