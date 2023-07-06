# Comparing `tmp/pywttr-2.2.0.tar.gz` & `tmp/pywttr-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywttr-2.2.0.tar", max compression
+gzip compressed data, was "pywttr-2.2.1.tar", max compression
```

## Comparing `pywttr-2.2.0.tar` & `pywttr-2.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-20 07:24:52.970123 pywttr-2.2.0/LICENSE
--rw-r--r--   0        0        0     1612 2023-04-22 20:08:26.179262 pywttr-2.2.0/README.md
--rw-r--r--   0        0        0     2982 2023-04-22 20:16:41.419265 pywttr-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      170 2023-04-22 19:53:35.889252 pywttr-2.2.0/pywttr/__init__.py
--rw-r--r--   0        0        0     5005 2023-04-20 07:24:52.970123 pywttr-2.2.0/pywttr/_wttr.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:52.970123 pywttr-2.2.0/pywttr/py.typed
--rw-r--r--   0        0        0     3023 1970-01-01 00:00:00.000000 pywttr-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 15:59:19.998339 pywttr-2.2.1/LICENSE
+-rw-r--r--   0        0        0      570 2023-07-06 15:59:19.998339 pywttr-2.2.1/README.md
+-rw-r--r--   0        0        0     3363 2023-07-06 15:59:20.002339 pywttr-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-07-06 15:59:20.002339 pywttr-2.2.1/pywttr/__init__.py
+-rw-r--r--   0        0        0     5304 2023-07-06 15:59:20.002339 pywttr-2.2.1/pywttr/_wttr.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:59:20.002339 pywttr-2.2.1/pywttr/py.typed
+-rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 pywttr-2.2.1/PKG-INFO
```

### Comparing `pywttr-2.2.0/LICENSE` & `pywttr-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywttr-2.2.0/pyproject.toml` & `pywttr-2.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "pywttr"
-version = "2.2.0"
+version = "2.2.1"
 description = "Wrapper for wttr.in API"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/pywttr"
+documentation = "https://pywttr.readthedocs.io/"
 keywords = ["forecast", "weather"]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Pydantic :: 1",
     "Framework :: Pydantic",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
@@ -29,24 +30,33 @@
 python = "^3.7.2"
 pywttr-models = "^1.1"
 requests = "^2.28"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 covdefaults = "2.3.0"
-mypy = "1.2.0"
+mypy = "1.4.1"
 pre-commit = "2.21.0"
-pydantic = "1.10.7"
-pytest = "7.3.1"
-pytest-cov = "4.0.0"
-ruff = "0.0.262"
-types-requests = "2.28.11.17"
+pydantic = "2.0.2"
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
+ruff = "0.0.277"
+types-requests = "2.31.0.1"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.18"
+mkdocstrings = { version = "0.22.0", extras = ["python"] }
 
 [tool.black]
 target-version = ["py37"]
+line-length = 80
 skip-magic-trailing-comma = true
 preview = true
 
 [tool.coverage.report]
 exclude_lines = ["^\\s*@(?:abc\\.)?abstractmethod$"]
 
 [tool.coverage.run]
@@ -58,14 +68,15 @@
 disallow_untyped_calls = false
 disallow_untyped_decorators = false
 warn_unreachable = true
 local_partial_types = true
 enable_error_code = [
     "redundant-self",
     "redundant-expr",
+    "possibly-undefined",
     "truthy-bool",
     "truthy-iterable",
     "ignore-without-code",
     "unused-awaitable",
 ]
 strict = true
 plugins = ["pydantic.mypy"]
@@ -73,23 +84,23 @@
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.pytest.ini_options]
+addopts = ["--strict-config", "--strict-markers"]
 xfail_strict = true
-addopts = ["--strict-markers", "--strict-config"]
 
 [tool.ruff]
 target-version = "py37"
+line-length = 80
 select = ["ALL"]
 ignore = [
     "ANN",
-    "B008",
     "BLE001",
     "C901",
     "COM",
     "D100",
     "D101",
     "D102",
     "D103",
@@ -104,23 +115,27 @@
     "D400",
     "D401",
     "D407",
     "D415",
     "D417",
     "DJ008",
     "ERA001",
+    "FBT002",
     "PD901",
+    "PERF203",
     "PLR0911",
     "PLR0912",
     "PLR0913",
     "PLR0915",
     "PT012",
     "RUF001",
     "RUF002",
     "RUF003",
+    "RUF012",
+    "RUF013",
     "S110",
     "S112",
     "S308",
     "S311",
     "SIM105",
     "TCH001",
     "TCH002",
@@ -135,13 +150,16 @@
 [tool.ruff.flake8-unused-arguments]
 ignore-variadic-names = true
 
 [tool.ruff.isort]
 combine-as-imports = true
 required-imports = ["from __future__ import annotations"]
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.ruff.pyupgrade]
 keep-runtime-typing = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pywttr-2.2.0/pywttr/_wttr.py` & `pywttr-2.2.1/pywttr/_wttr.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,33 @@
 from typing import Any, Optional
 
 import pywttr_models
 from requests import Response, Session
 
 
 class Wttr:
-    """Wrapper for wttr.in weather forecast API."""
+    """Wrapper for wttr.in weather forecast API.
+
+    Examples:
+        Prints the average temperature in New York today:
+
+        ```python
+        >>> import pywttr
+        >>>
+        >>> wttr = pywttr.Wttr("New York")
+        >>> forecast = wttr.en()
+        >>> print(forecast.weather[0].avgtemp_c)
+        ```
+    """
 
     __slots__ = ("location", "session")
 
-    def __init__(self, location: str, session: Optional[Session] = None) -> None:
+    def __init__(
+        self, location: str, session: Optional[Session] = None
+    ) -> None:
         self.location = location
         self.session = session
 
     def af(self) -> pywttr_models.af.Model:
         return pywttr_models.af.Model.parse_obj(self._get_json("af"))
 
     def am(self) -> pywttr_models.am.Model:
@@ -127,10 +141,11 @@
             with Session() as session:
                 response = self._fetch(lang, session)
         response.raise_for_status()
         return response.json()
 
     def _fetch(self, lang: str, session: Session) -> Response:
         with session.get(
-            f"https://wttr.in/{self.location}", params={"format": "j1", "lang": lang}
+            f"https://wttr.in/{self.location}",
+            params={"format": "j1", "lang": lang},
         ) as response:
             return response
```

### Comparing `pywttr-2.2.0/PKG-INFO` & `pywttr-2.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywttr
-Version: 2.2.0
+Version: 2.2.1
 Summary: Wrapper for wttr.in API
 Home-page: https://github.com/monosans/pywttr
 License: MIT
 Keywords: forecast,weather
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7.2,<4.0.0
@@ -27,56 +27,34 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: pywttr-models (>=1.1,<2.0)
 Requires-Dist: requests (>=2.28,<3.0)
+Project-URL: Documentation, https://pywttr.readthedocs.io/
 Project-URL: Repository, https://github.com/monosans/pywttr
 Description-Content-Type: text/markdown
 
 # pywttr
 
-[![CI](https://github.com/monosans/pywttr/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pywttr/actions/workflows/ci.yml?query=event%3Apush+branch%3Amain)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pywttr/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pywttr/main)
-[![Coverage](https://img.shields.io/codecov/c/github/monosans/pywttr/main?logo=codecov)](https://codecov.io/gh/monosans/pywttr)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/pywttr?logo=pypi)](https://pypi.org/project/pywttr/)
+[![CI](https://github.com/monosans/pywttr/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/pywttr/actions/workflows/ci.yml)
+[![Downloads](https://static.pepy.tech/badge/pywttr)](https://pepy.tech/project/pywttr)
 
 Wrapper for [wttr.in](https://wttr.in) weather forecast API.
 
 Asynchronous version [here](https://github.com/monosans/aiopywttr).
 
 ## Installation
 
 ```bash
 python -m pip install -U pywttr pywttr-models
 ```
 
-## Example
-
-This example prints the average temperature in New York today.
-
-```python
-import pywttr
-
-wttr = pywttr.Wttr("New York")
-forecast = wttr.en()
-print(forecast.weather[0].avgtemp_c)
-```
-
-Other languages may also be used instead of `en`. For a complete list of supported languages, follow the code completion in your IDE.
-
 ## Documentation
 
-There is no documentation, just follow the example and code completion in your IDE.
-
-All types of objects returned by the wttr.in API are in the `pywttr.models` package.
-
-## Recommended IDEs
-
-- [Visual Studio Code](https://code.visualstudio.com) (with [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python))
-- [PyCharm](https://jetbrains.com/pycharm)
+<https://pywttr.readthedocs.io/>
 
 ## License
 
 [MIT](https://github.com/monosans/pywttr/blob/main/LICENSE)
```

