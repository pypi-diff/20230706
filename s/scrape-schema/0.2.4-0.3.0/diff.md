# Comparing `tmp/scrape_schema-0.2.4.tar.gz` & `tmp/scrape_schema-0.3.0.tar.gz`

## Comparing `scrape_schema-0.2.4.tar` & `scrape_schema-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,12 @@
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/__init__.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/_base_configs.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/_logger.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/_type_caster.py
--rw-r--r--   0        0        0    19756 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/exceptions.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/callbacks/parsel.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/fields/mock.py
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/fields/parsel.py
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/LICENSE
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/README.md
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 scrape_schema-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/_logger.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/_typing.py
+-rw-r--r--   0        0        0    14556 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/base.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/field.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/nested.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/scrape_schema/type_caster.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/README.md
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 scrape_schema-0.3.0/PKG-INFO
```

### Comparing `scrape_schema-0.2.4/scrape_schema/_type_caster.py` & `scrape_schema-0.3.0/scrape_schema/type_caster.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
-from typing import Any, ByteString, Iterable, Type, Union
+from typing import Any, Type, Union
 
-from scrape_schema._logger import logger
-from scrape_schema.base import get_args, get_origin
+from scrape_schema._logger import _logger
+from scrape_schema._typing import get_args, get_origin
 
 NoneType = type(None)
 
 
 class TypeCaster:
     def _typing_to_builtin(self, type_hint: Type) -> Type:
         origin = get_origin(type_hint)
@@ -21,67 +21,67 @@
 
     def cast(self, type_hint: Type, value: Any) -> Any:
         if sys.version_info >= (3, 9):
             type_hint = self._typing_to_builtin(type_hint)
 
         origin = get_origin(type_hint)
         args = get_args(type_hint)
-        logger.info(
-            "`{}` Cast type start. `value={}`, type_annotation={}, `origin={}`, `args={}`",
+        _logger.debug(
+            "`%s` Cast type start. `value=%s`, type_annotation=%s, `origin=%s`, `args=%s`",
             self.__class__.__name__,
             value,
             type_hint,
             origin,
             args,
         )
         # None
         if value is None and type_hint is not bool:
             return value
 
         if origin is not None and args:
             # list
             if origin is list:
-                logger.debug(
-                    "List cast {} -> arg={}, value={}",
+                _logger.debug(
+                    "List cast %s %s -> %s",
                     self.__class__.__name__,
                     args[0],
                     value,
                 )
                 return [self.cast(type_hint=args[0], value=v) for v in value]
             # dict
             elif origin is dict:
                 key_type, value_type = args
-                logger.debug(
-                    "Dict cast {} -> key={}, value={}  `{}`",
+                _logger.debug(
+                    "Dict cast %s key=%s, value=%s -> %s",
                     self.__class__.__name__,
                     key_type.__name__,
                     value_type.__name__,
                     value,
                 )
                 return {
                     self.cast(type_hint=key_type, value=k): self.cast(
                         type_hint=value_type, value=v
                     )
                     for k, v in value.items()
                 }
             # Optional
             elif origin is Union:
                 if value is None and NoneType in args:
-                    logger.debug(
-                        "Optional cast {} -> {}", self.__class__.__name__, value
+                    _logger.debug(
+                        "Optional cast %s -> %s", self.__class__.__name__, value
                     )
                     return None
                 # in python3.8 raise TypeError: issubclass() arg 1 must be a class
                 # example _cast_type(Optional[List[int]], [])
                 non_none_args = [arg for arg in args if arg is not NoneType]
                 if len(non_none_args) == 1:
                     return self.cast(type_hint=non_none_args[0], value=value)
         # bool cast
         elif type_hint is bool:
-            logger.debug("Cast {} `{}()` -> bool", self.__class__.__name__, value)
+            _logger.debug("Bool cast %s -> %s", self.__class__.__name__, value)
             return bool(value)
         else:
             # direct cast
-            logger.debug(
-                "Cast `{}` := `{}({})`", self.__class__.__name__, type_hint, value
+            _logger.debug(
+                "Direct cast %s %s -> %s", self.__class__.__name__, type_hint, value
             )
             return type_hint(value)
```

### Comparing `scrape_schema-0.2.4/.gitignore` & `scrape_schema-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.4/LICENSE` & `scrape_schema-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.4/pyproject.toml` & `scrape_schema-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,32 +20,29 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Internet",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Text Processing"
 ]
 dependencies = [
-  'colorama',
+  'colorlog',
+  'parsel',
   'typing_extensions; python_version < "3.11"'
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/vypivshiy/scrape-schema#readme"
 Issues = "https://github.com/vypivshiy/scrape-schema/issues"
 Source = "https://github.com/vypivshiy/scrape-schema"
 Examples = "https://github.com/vypivshiy/scrape-schema/examples"
 
 
 [project.optional-dependencies]
-selectolax = ["selectolax"]
-bs4 = ["bs4"]
-parsel = ["parsel"]
-all = ["selectolax", "bs4", "parsel"]
-dev = ["bs4", "selectolax", "flake8", "black", "isort", "pytest", "mypy", "parsel"]
+dev = ["flake8", "black", "isort", "pytest", "mypy", "parsel"]
 ci = ["hatch", "bs4", "selectolax", "flake8", "black", "isort", "pytest", "mypy", "parsel"]
 docs = ["mkdocs-material"]
 
 [tool.hatch.version]
 path = "scrape_schema/__init__.py"
 
 [tool.hatch.envs.docs]
```

