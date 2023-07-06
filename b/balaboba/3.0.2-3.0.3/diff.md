# Comparing `tmp/balaboba-3.0.2.tar.gz` & `tmp/balaboba-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balaboba-3.0.2.tar", max compression
+gzip compressed data, was "balaboba-3.0.3.tar", max compression
```

## Comparing `balaboba-3.0.2.tar` & `balaboba-3.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-06-10 08:45:42.647279 balaboba-3.0.2/LICENSE
--rw-r--r--   0        0        0     1041 2023-06-10 08:45:42.647279 balaboba-3.0.2/README.md
--rw-r--r--   0        0        0      128 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/__init__.py
--rw-r--r--   0        0        0     2935 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/_balaboba.py
--rw-r--r--   0        0        0     1442 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/_http.py
--rw-r--r--   0        0        0      147 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/_text_type.py
--rw-r--r--   0        0        0        0 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/py.typed
--rw-r--r--   0        0        0     2818 2023-06-10 08:45:42.651279 balaboba-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 balaboba-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 15:25:24.985129 balaboba-3.0.3/LICENSE
+-rw-r--r--   0        0        0      896 2023-07-06 15:25:24.985129 balaboba-3.0.3/README.md
+-rw-r--r--   0        0        0      128 2023-07-06 15:25:24.985129 balaboba-3.0.3/balaboba/__init__.py
+-rw-r--r--   0        0        0     3303 2023-07-06 15:25:24.985129 balaboba-3.0.3/balaboba/_balaboba.py
+-rw-r--r--   0        0        0     1442 2023-07-06 15:25:24.985129 balaboba-3.0.3/balaboba/_http.py
+-rw-r--r--   0        0        0      147 2023-07-06 15:25:24.985129 balaboba-3.0.3/balaboba/_text_type.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:25:24.985129 balaboba-3.0.3/balaboba/py.typed
+-rw-r--r--   0        0        0     3195 2023-07-06 15:25:24.985129 balaboba-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 balaboba-3.0.3/PKG-INFO
```

### Comparing `balaboba-3.0.2/LICENSE` & `balaboba-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `balaboba-3.0.2/README.md` & `balaboba-3.0.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -13,21 +13,14 @@
 
 ## Installation
 
 ```bash
 python -m pip install -U balaboba
 ```
 
-## Usage example
+## Documentation
 
-```python
-from balaboba import Balaboba
-
-bb = Balaboba()
-text_types = bb.get_text_types(language="en")
-response = bb.balaboba("Hello", text_type=text_types[0])
-print(response)
-```
+<https://balaboba.readthedocs.io/>
 
 ## License
 
 [MIT](https://github.com/monosans/balaboba/blob/main/LICENSE)
```

### Comparing `balaboba-3.0.2/balaboba/_balaboba.py` & `balaboba-3.0.3/balaboba/_balaboba.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,72 +12,92 @@
 if sys.version_info < (3, 8):  # pragma: <3.8 cover
     from typing_extensions import Literal
 else:  # pragma: >=3.8 cover
     from typing import Literal
 
 
 class Balaboba:
-    """Wrapper for Yandex Balaboba."""
+    """Wrapper for Yandex Balaboba.
+
+    Examples:
+        ```python
+        >>> from balaboba import Balaboba
+        >>>
+        >>> bb = Balaboba()
+        >>> text_types = bb.get_text_types(language="en")
+        >>> print(text_types)
+        >>> response = bb.balaboba("Hello", text_type=text_types[0])
+        >>> print(response)
+        ```
+    """
 
     __slots__ = ("_session",)
 
     def __init__(self, session: Optional[Session] = None) -> None:
-        """Wrapper for Yandex Balaboba."""
         self._session = HTTPSession(session)
 
     @property
     def session(self) -> Optional[Session]:
         return self._session.session
 
     @session.setter
     def session(self, session: Optional[Session]) -> None:
         self._session.session = session
 
-    def get_text_types(self, language: Literal["en", "ru"] = "ru") -> List[TextType]:
+    def get_text_types(
+        self, language: Literal["en", "ru"] = "ru"
+    ) -> List[TextType]:
         endpoint = "intros" if language == "ru" else "intros_eng"
         response = self._session.get_response(
-            method="GET", endpoint=endpoint, headers=self._get_text_types_headers()
+            method="GET",
+            endpoint=endpoint,
+            headers=self._get_text_types_headers(),
         )
         return [TextType(*intro) for intro in response["intros"]]
 
     def balaboba(self, query: str, text_type: Union[TextType, int]) -> str:
-        intro = text_type.number if isinstance(text_type, TextType) else text_type
+        intro = (
+            text_type.number if isinstance(text_type, TextType) else text_type
+        )
         response = self._session.get_response(
             method="POST",
             endpoint="text3",
             json={"query": query, "intro": intro, "filter": 1},
             headers=self._get_balaboba_headers(query, intro),
         )
         return "{}{}".format(response["query"], response["text"])
 
     def _get_text_types_headers(self) -> Dict[str, str]:
         return {
             "User-Agent": (
-                "Mozilla/5.0 (Windows NT 10.0; rv:114.0) Gecko/20100101 Firefox/114.0"
+                "Mozilla/5.0 (Windows NT 10.0; rv:114.0)"
+                " Gecko/20100101 Firefox/114.0"
             ),
             "Accept-Language": "en-US,en;q=0.5",
             "Referer": "https://yandex.ru/lab/yalm",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "TE": "trailers",
         }
 
-    def _get_balaboba_headers(self, query: str, text_type: int) -> Dict[str, str]:
+    def _get_balaboba_headers(
+        self, query: str, text_type: int
+    ) -> Dict[str, str]:
         return {
             "User-Agent": (
-                "Mozilla/5.0 (Windows NT 10.0; rv:114.0) Gecko/20100101 Firefox/114.0"
+                "Mozilla/5.0 (Windows NT 10.0; rv:114.0)"
+                " Gecko/20100101 Firefox/114.0"
             ),
             "Accept-Language": "en-US,en;q=0.5",
             "Referer": f"https://yandex.ru/lab/yalm?style={text_type}",
             "X-Requested-With": "XMLHttpRequest",
             "X-Retpath-Y": (
-                "https://yandex.ru/lab/yalm?style={}&input={}&skipCurtain=1".format(
-                    text_type, urllib.parse.quote_plus(query)
-                )
+                "https://yandex.ru/lab/yalm?style={}&input={}&skipCurtain=1"
+                .format(text_type, urllib.parse.quote_plus(query))
             ),
             "Origin": "https://yandex.ru",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "TE": "trailers",
         }
```

### Comparing `balaboba-3.0.2/balaboba/_http.py` & `balaboba-3.0.3/balaboba/_http.py`

 * *Files identical despite different names*

### Comparing `balaboba-3.0.2/pyproject.toml` & `balaboba-3.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "balaboba"
-version = "3.0.2"
+version = "3.0.3"
 description = "Wrapper for Yandex Balaboba"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/balaboba"
+documentation = "https://balaboba.readthedocs.io/"
 keywords = ["yalm"]
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Natural Language :: English",
     "Natural Language :: Russian",
@@ -28,23 +29,32 @@
 python = "^3.7"
 requests = "^2.28"
 typing-extensions = { version = ">=3.7.4.3,<5", python = "<3.8" }
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 covdefaults = "2.3.0"
-mypy = "1.3.0"
+mypy = "1.4.1"
 pre-commit = "2.21.0"
-pytest = "7.3.1"
-coverage = { version = "7.2.7", extras = ["toml"] }
-ruff = "0.0.272"
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
+ruff = "0.0.277"
 types-requests = "2.31.0.1"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.18"
+mkdocstrings = { version = "0.22.0", extras = ["python"] }
+
 [tool.black]
 target-version = ["py37"]
+line-length = 80
 skip-magic-trailing-comma = true
 preview = true
 
 [tool.coverage.report]
 exclude_lines = ["^\\s*@(?:abc\\.)?abstractmethod$"]
 
 [tool.coverage.run]
@@ -56,27 +66,29 @@
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
 
 [tool.pytest.ini_options]
 addopts = ["--strict-config", "--strict-markers"]
 xfail_strict = true
 
 [tool.ruff]
 target-version = "py37"
+line-length = 80
 select = ["ALL"]
 ignore = [
     "ANN",
     "BLE001",
     "C901",
     "COM",
     "D100",
@@ -96,42 +108,49 @@
     "D407",
     "D415",
     "D417",
     "DJ008",
     "ERA001",
     "FBT002",
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
     "TCH003",
     "TID252",
     "TRY400",
-    "UP006",
-    "UP007",
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
 
 [tool.ruff.flake8-unused-arguments]
 ignore-variadic-names = true
 
 [tool.ruff.isort]
 combine-as-imports = true
 required-imports = ["from __future__ import annotations"]
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.pyupgrade]
+keep-runtime-typing = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `balaboba-3.0.2/PKG-INFO` & `balaboba-3.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balaboba
-Version: 3.0.2
+Version: 3.0.3
 Summary: Wrapper for Yandex Balaboba
 Home-page: https://github.com/monosans/balaboba
 License: MIT
 Keywords: yalm
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
@@ -27,14 +27,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: typing-extensions (>=3.7.4.3,<5) ; python_version < "3.8"
+Project-URL: Documentation, https://balaboba.readthedocs.io/
 Project-URL: Repository, https://github.com/monosans/balaboba
 Description-Content-Type: text/markdown
 
 # balaboba
 
 [![CI](https://github.com/monosans/balaboba/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/balaboba/actions/workflows/ci.yml)
 [![Downloads](https://static.pepy.tech/badge/balaboba)](https://pepy.tech/project/balaboba)
@@ -49,22 +50,15 @@
 
 ## Installation
 
 ```bash
 python -m pip install -U balaboba
 ```
 
-## Usage example
+## Documentation
 
-```python
-from balaboba import Balaboba
-
-bb = Balaboba()
-text_types = bb.get_text_types(language="en")
-response = bb.balaboba("Hello", text_type=text_types[0])
-print(response)
-```
+<https://balaboba.readthedocs.io/>
 
 ## License
 
 [MIT](https://github.com/monosans/balaboba/blob/main/LICENSE)
```

