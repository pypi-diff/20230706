# Comparing `tmp/in-n-out-0.1.7.tar.gz` & `tmp/in_n_out-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-n-out-0.1.7.tar", last modified: Mon Feb 27 14:02:11 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `in-n-out-0.1.7.tar` & `in_n_out-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.984407 in-n-out-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.976407 in-n-out-0.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.976407 in-n-out-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-27 14:01:49.000000 in-n-out-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-02-27 14:01:49.000000 in-n-out-0.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-27 14:01:49.000000 in-n-out-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-27 14:01:49.000000 in-n-out-0.1.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-02-27 14:02:11.984407 in-n-out-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-02-27 14:01:49.000000 in-n-out-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-27 14:01:49.000000 in-n-out-0.1.7/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.976407 in-n-out-0.1.7/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 14:01:49.000000 in-n-out-0.1.7/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-27 14:01:49.000000 in-n-out-0.1.7/benchmarks/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-27 14:01:49.000000 in-n-out-0.1.7/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-02-27 14:01:49.000000 in-n-out-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 14:02:11.984407 in-n-out-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-27 14:01:49.000000 in-n-out-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.972407 in-n-out-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.980407 in-n-out-0.1.7/src/in_n_out/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-27 14:01:49.000000 in-n-out-0.1.7/src/in_n_out/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-02-27 14:01:49.000000 in-n-out-0.1.7/src/in_n_out/_global.py
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-02-27 14:01:49.000000 in-n-out-0.1.7/src/in_n_out/_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-02-27 14:01:49.000000 in-n-out-0.1.7/src/in_n_out/_type_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-27 14:01:49.000000 in-n-out-0.1.7/src/in_n_out/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 14:01:49.000000 in-n-out-0.1.7/src/in_n_out/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.980407 in-n-out-0.1.7/src/in_n_out.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-02-27 14:02:11.000000 in-n-out-0.1.7/src/in_n_out.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-27 14:02:11.000000 in-n-out-0.1.7/src/in_n_out.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 14:02:11.000000 in-n-out-0.1.7/src/in_n_out.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 14:02:11.000000 in-n-out-0.1.7/src/in_n_out.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-27 14:02:11.000000 in-n-out-0.1.7/src/in_n_out.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-27 14:02:11.000000 in-n-out-0.1.7/src/in_n_out.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.980407 in-n-out-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_type_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/test_type_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:02:11.984407 in-n-out-0.1.7/tests/typesafety/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/typesafety/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-02-27 14:01:49.000000 in-n-out-0.1.7/tests/typesafety/test_types.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 in_n_out-0.1.8/src/in_n_out/__init__.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 in_n_out-0.1.8/src/in_n_out/_global.py
+-rw-r--r--   0        0        0    42643 2020-02-02 00:00:00.000000 in_n_out-0.1.8/src/in_n_out/_store.py
+-rw-r--r--   0        0        0    12587 2020-02-02 00:00:00.000000 in_n_out-0.1.8/src/in_n_out/_type_resolution.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 in_n_out-0.1.8/src/in_n_out/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_n_out-0.1.8/src/in_n_out/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_injection.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_logging.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_processors.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_providers.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_store.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_type_resolution.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/test_type_support.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/typesafety/__init__.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 in_n_out-0.1.8/tests/typesafety/test_types.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 in_n_out-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 in_n_out-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 in_n_out-0.1.8/README.md
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 in_n_out-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 in_n_out-0.1.8/PKG-INFO
```

### Comparing `in-n-out-0.1.7/.gitignore` & `in_n_out-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/LICENSE` & `in_n_out-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/PKG-INFO` & `in_n_out-0.1.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: in-n-out
-Version: 0.1.7
-Summary:  plugable dependency injection and result processing
-Author: Talley Lambert
-Author-email: talley.lambert@gmail.com
-License: BSD 3-Clause License
-Project-URL: homepage, https://github.com/pyapp-kit/in-n-out
-Project-URL: repository, https://github.com/pyapp-kit/in-n-out
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: build
-License-File: LICENSE
-
 # in-n-out
 
 [![License](https://img.shields.io/pypi/l/in-n-out.svg?color=green)](https://github.com/pyapp-kit/in-n-out/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/in-n-out.svg?color=green)](https://pypi.org/project/in-n-out)
 [![Python Version](https://img.shields.io/pypi/pyversions/in-n-out.svg?color=green)](https://python.org)
 [![CI](https://github.com/pyapp-kit/in-n-out/actions/workflows/ci.yml/badge.svg)](https://github.com/pyapp-kit/in-n-out/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/pyapp-kit/in-n-out/branch/main/graph/badge.svg)](https://app.codecov.io/gh/pyapp-kit/in-n-out)
```

### Comparing `in-n-out-0.1.7/src/in_n_out/__init__.py` & `in_n_out-0.1.8/src/in_n_out/__init__.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/src/in_n_out/_global.py` & `in_n_out-0.1.8/src/in_n_out/_global.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     # unfortunately, the best we can do is convert the signature to Callabe[..., R]
     # so we lose the parameter information.  but it seems better than having
     # "missing positional args" errors everywhere on injected functions.
 
 
 @overload
 def inject(
-    func: Literal[None] = None,
+    func: Literal[None] | None = None,
     *,
     providers: bool = True,
     processors: bool = False,
     localns: dict | None = None,
     on_unresolved_required_args: RaiseWarnReturnIgnore | None = None,
     on_unannotated_required_args: RaiseWarnReturnIgnore | None = None,
     guess_self: bool | None = None,
@@ -255,15 +255,15 @@
     store: str | Store | None = None,
 ) -> Callable[P, R]:
     ...
 
 
 @overload
 def inject_processors(
-    func: Literal[None] = None,
+    func: Literal[None] | None = None,
     *,
     hint: object | type[T] | None = None,
     first_processor_only: bool = False,
     raise_exception: bool = False,
     store: str | Store | None = None,
 ) -> Callable[[Callable[P, R]], Callable[P, R]]:
     ...
```

### Comparing `in-n-out-0.1.7/src/in_n_out/_store.py` & `in_n_out-0.1.8/src/in_n_out/_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from inspect import CO_VARARGS, isgeneratorfunction, unwrap
 from logging import getLogger
 from types import CodeType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    ClassVar,
     ContextManager,
     Iterable,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
     Tuple,
@@ -28,16 +29,14 @@
 from ._type_resolution import _resolve_sig_or_inform, resolve_type_hints
 from ._util import _split_union, issubclassable
 
 logger = getLogger("in_n_out")
 
 
 if TYPE_CHECKING:
-    from inspect import Signature
-
     from typing_extensions import ParamSpec
 
     from ._type_resolution import RaiseWarnReturnIgnore
 
     P = ParamSpec("P")
     R = TypeVar("R")
 
@@ -121,15 +120,15 @@
         self._disposers.clear()
 
 
 class Store:
     """A Store is a collection of providers and processors."""
 
     _NULL = _NullSentinel()
-    _instances: dict[str, Store] = {}
+    _instances: ClassVar[dict[str, Store]] = {}
 
     @classmethod
     def create(cls, name: str) -> Store:
         """Create a new Store instance with the given `name`.
 
         This name can be used to refer to the Store in other functions.
 
@@ -405,15 +404,15 @@
         ...     return 42
         """
 
         def _deco(func: ProviderVar) -> ProviderVar:
             try:
                 self.register_provider(func, type_hint=type_hint, weight=weight)
             except ValueError as e:
-                warnings.warn(str(e))
+                warnings.warn(str(e), stacklevel=2)
             return func
 
         return _deco(func) if func is not None else _deco
 
     @overload
     def mark_processor(
         self,
@@ -469,15 +468,15 @@
         ...     print("Processing int:", x)
         """
 
         def _deco(func: ProcessorVar) -> ProcessorVar:
             try:
                 self.register_processor(func, type_hint=type_hint, weight=weight)
             except ValueError as e:
-                warnings.warn(str(e))
+                warnings.warn(str(e), stacklevel=2)
             return func
 
         return _deco(func) if func is not None else _deco
 
     # ------------------------- Callback retrieval ------------------------------
 
     def iter_providers(
@@ -581,15 +580,16 @@
             try:
                 logger.debug("  P: %s", processor)
                 processor(result)
             except Exception as e:  # pragma: no cover
                 if raise_exception:
                     raise e
                 warnings.warn(
-                    f"Processor {processor!r} failed to process result {result!r}: {e}"
+                    f"Processor {processor!r} failed to process result {result!r}: {e}",
+                    stacklevel=2,
                 )
             if first_processor_only:
                 break
 
     # ----------------------Injection decorators ------------------------------------
 
     @overload
@@ -608,15 +608,15 @@
         # unfortunately, the best we can do is convert the signature to Callabe[..., R]
         # so we lose the parameter information.  but it seems better than having
         # "missing positional args" errors everywhere on injected functions.
 
     @overload
     def inject(
         self,
-        func: Literal[None] = None,
+        func: Literal[None] | None = None,
         *,
         providers: bool = True,
         processors: bool = False,
         localns: dict | None = None,
         on_unresolved_required_args: RaiseWarnReturnIgnore | None = None,
         on_unannotated_required_args: RaiseWarnReturnIgnore | None = None,
         guess_self: bool | None = None,
@@ -768,24 +768,23 @@
                 logger.debug(
                     "Executing @injected %s%s with args: %r, kwargs: %r",
                     _fname,
                     sig,
                     args,
                     kwargs,
                 )
-                _sig = cast("Signature", sig)  # mypy thinks sig is still optional
 
                 # use bind_partial to allow the caller to still provide their own args
                 # if desired. (i.e. the injected deps are only used if not provided)
-                bound = _sig.bind_partial(*args, **kwargs)
+                bound = sig.bind_partial(*args, **kwargs)
                 bound.apply_defaults()
 
                 # first, get and call the provider functions for each parameter type:
                 _injected_names: set[str] = set()
-                for param in _sig.parameters.values():
+                for param in sig.parameters.values():
                     if param.name not in bound.arguments:
                         provided = self.provide(param.annotation)
                         if provided is not None:
                             logger.debug(
                                 "  injecting %s: %s = %r",
                                 param.name,
                                 param.annotation,
@@ -810,14 +809,25 @@
                     # show what was injected and raise
                     _argnames = (
                         f"arguments: {_injected_names!r}"
                         if _injected_names
                         else "NO arguments"
                     )
                     logger.exception(e)
+                    for param in sig.parameters.values():
+                        if (
+                            param.name not in bound.arguments
+                            and param.default is param.empty
+                        ):
+                            logger.error(
+                                f"Do not have argument for {param.name}: using "
+                                "providers "
+                                f"{list(self.iter_providers(param.annotation))}"
+                            )
+
                     raise TypeError(
                         f"After injecting dependencies for {_argnames}, {e}"
                     ) from e
 
                 return result
 
             out = _exec
@@ -857,15 +867,15 @@
         raise_exception: bool = False,
     ) -> Callable[P, R]:
         ...
 
     @overload
     def inject_processors(
         self,
-        func: Literal[None] = None,
+        func: Literal[None] | None = None,
         *,
         type_hint: object | type[T] | None = None,
         first_processor_only: bool = False,
         raise_exception: bool = False,
     ) -> Callable[[Callable[P, R]], Callable[P, R]]:
         ...
```

### Comparing `in-n-out-0.1.7/src/in_n_out/_type_resolution.py` & `in_n_out-0.1.8/src/in_n_out/_type_resolution.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/src/in_n_out/_util.py` & `in_n_out-0.1.8/src/in_n_out/_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 import types
 from typing import Any, List, Set, Tuple, Type, Union, cast, get_origin
 
-try:
-    import cython
-except ImportError:  # pragma: no cover
-    _compiled: bool = False
-else:  # pragma: no cover
-    try:
-        _compiled = cython.compiled
-    except AttributeError:
-        _compiled = False
+_compiled: bool = False
 
 
 UNION_TYPES: Set[Any] = {Union}
 if hasattr(types, "UnionType"):
     # doing it this way to deal with python-version specific linting issues
     UNION_TYPES.add(cast(Any, getattr(types, "UnionType")))  # noqa
```

### Comparing `in-n-out-0.1.7/tests/test_benchmarks.py` & `in_n_out-0.1.8/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/tests/test_injection.py` & `in_n_out-0.1.8/tests/test_injection.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,17 +59,16 @@
 
 
 def test_injection_missing():
     @inject
     def f(x: int):
         return x
 
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError, match="After injecting dependencies"):
         f()
-    assert "missing 1 required positional argument" in str(e.value)
     assert f(4) == 4
     with register(providers={int: lambda: 1}):
         assert f() == 1
 
 
 def test_set_processor():
     @inject_processors
```

### Comparing `in-n-out-0.1.7/tests/test_logging.py` & `in_n_out-0.1.8/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/tests/test_processors.py` & `in_n_out-0.1.8/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/tests/test_providers.py` & `in_n_out-0.1.8/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/tests/test_store.py` & `in_n_out-0.1.8/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/tests/test_type_resolution.py` & `in_n_out-0.1.8/tests/test_type_resolution.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/tests/test_type_support.py` & `in_n_out-0.1.8/tests/test_type_support.py`

 * *Files identical despite different names*

### Comparing `in-n-out-0.1.7/tests/typesafety/test_types.py` & `in_n_out-0.1.8/tests/typesafety/test_types.py`

 * *Files identical despite different names*

