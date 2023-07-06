# Comparing `tmp/aiobalaboba-3.0.2.tar.gz` & `tmp/aiobalaboba-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobalaboba-3.0.2.tar", max compression
+gzip compressed data, was "aiobalaboba-3.0.3.tar", max compression
```

## Comparing `aiobalaboba-3.0.2.tar` & `aiobalaboba-3.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/LICENSE
--rw-r--r--   0        0        0     1158 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/README.md
--rw-r--r--   0        0        0      141 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/__init__.py
--rw-r--r--   0        0        0     3022 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/_balaboba.py
--rw-r--r--   0        0        0     1582 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/_http.py
--rw-r--r--   0        0        0      147 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/_text_type.py
--rw-r--r--   0        0        0        0 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/py.typed
--rw-r--r--   0        0        0     2883 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 aiobalaboba-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/LICENSE
+-rw-r--r--   0        0        0      929 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/README.md
+-rw-r--r--   0        0        0      141 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/aiobalaboba/__init__.py
+-rw-r--r--   0        0        0     3537 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/aiobalaboba/_balaboba.py
+-rw-r--r--   0        0        0     1582 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/aiobalaboba/_http.py
+-rw-r--r--   0        0        0      147 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/aiobalaboba/_text_type.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/aiobalaboba/py.typed
+-rw-r--r--   0        0        0     3263 2023-07-06 15:25:34.003155 aiobalaboba-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 aiobalaboba-3.0.3/PKG-INFO
```

### Comparing `aiobalaboba-3.0.2/LICENSE` & `aiobalaboba-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobalaboba-3.0.2/aiobalaboba/_balaboba.py` & `aiobalaboba-3.0.3/aiobalaboba/_balaboba.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,20 +12,37 @@
 if sys.version_info < (3, 8):  # pragma: <3.8 cover
     from typing_extensions import Literal
 else:  # pragma: >=3.8 cover
     from typing import Literal
 
 
 class Balaboba:
-    """Asynchronous wrapper for Yandex Balaboba."""
+    """Asynchronous wrapper for Yandex Balaboba.
+
+    Examples:
+        ```python
+        >>> import asyncio
+        >>>
+        >>> from aiobalaboba import Balaboba
+        >>>
+        >>>
+        >>> async def main():
+        ...     bb = Balaboba()
+        ...     text_types = await bb.get_text_types(language="en")
+        ...     print(text_types)
+        ...     response = await bb.balaboba("Hello", text_type=text_types[0])
+        ...     print(response)
+        >>>
+        >>> asyncio.run(main())
+        ```
+    """
 
     __slots__ = ("_session",)
 
     def __init__(self, session: Optional[ClientSession] = None) -> None:
-        """Asynchronous wrapper for Yandex Balaboba."""
         self._session = HTTPSession(session)
 
     @property
     def session(self) -> Optional[ClientSession]:
         return self._session.session
 
     @session.setter
@@ -33,53 +50,62 @@
         self._session.session = session
 
     async def get_text_types(
         self, language: Literal["en", "ru"] = "ru"
     ) -> List[TextType]:
         endpoint = "intros" if language == "ru" else "intros_eng"
         response = await self._session.get_response(
-            method="GET", endpoint=endpoint, headers=self._get_text_types_headers()
+            method="GET",
+            endpoint=endpoint,
+            headers=self._get_text_types_headers(),
         )
         return [TextType(*intro) for intro in response["intros"]]
 
-    async def balaboba(self, query: str, text_type: Union[TextType, int]) -> str:
-        intro = text_type.number if isinstance(text_type, TextType) else text_type
+    async def balaboba(
+        self, query: str, text_type: Union[TextType, int]
+    ) -> str:
+        intro = (
+            text_type.number if isinstance(text_type, TextType) else text_type
+        )
         response = await self._session.get_response(
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

### Comparing `aiobalaboba-3.0.2/aiobalaboba/_http.py` & `aiobalaboba-3.0.3/aiobalaboba/_http.py`

 * *Files identical despite different names*

### Comparing `aiobalaboba-3.0.2/pyproject.toml` & `aiobalaboba-3.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "aiobalaboba"
-version = "3.0.2"
+version = "3.0.3"
 description = "Asynchronous wrapper for Yandex Balaboba"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/aiobalaboba"
+documentation = "https://aiobalaboba.readthedocs.io/"
 keywords = ["yalm"]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Natural Language :: English",
@@ -29,23 +30,32 @@
 python = "^3.7"
 aiohttp = "^3.8"
 typing-extensions = { version = ">=3.7.4.3,<5", python = "<3.8" }
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 covdefaults = "2.3.0"
-mypy = "1.3.0"
+mypy = "1.4.1"
 pre-commit = "2.21.0"
-pytest = "7.3.1"
+pytest = "7.4.0"
 pytest-asyncio = "0.21.0"
-coverage = { version = "7.2.7", extras = ["toml"] }
-ruff = "0.0.272"
+pytest-cov = "4.1.0"
+ruff = "0.0.277"
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
@@ -57,28 +67,30 @@
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
 asyncio_mode = "auto"
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
@@ -98,42 +110,49 @@
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

### Comparing `aiobalaboba-3.0.2/PKG-INFO` & `aiobalaboba-3.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobalaboba
-Version: 3.0.2
+Version: 3.0.3
 Summary: Asynchronous wrapper for Yandex Balaboba
 Home-page: https://github.com/monosans/aiobalaboba
 License: MIT
 Keywords: yalm
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
@@ -28,14 +28,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: typing-extensions (>=3.7.4.3,<5) ; python_version < "3.8"
+Project-URL: Documentation, https://aiobalaboba.readthedocs.io/
 Project-URL: Repository, https://github.com/monosans/aiobalaboba
 Description-Content-Type: text/markdown
 
 # aiobalaboba
 
 [![CI](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/aiobalaboba/actions/workflows/ci.yml)
 [![Downloads](https://static.pepy.tech/badge/aiobalaboba)](https://pepy.tech/project/aiobalaboba)
@@ -50,28 +51,15 @@
 
 ## Installation
 
 ```bash
 python -m pip install -U aiobalaboba
 ```
 
-## Usage example
+## Documentation
 
-```python
-import asyncio
-
-from aiobalaboba import Balaboba
-
-
-async def main():
-    bb = Balaboba()
-    text_types = await bb.get_text_types(language="en")
-    response = await bb.balaboba("Hello", text_type=text_types[0])
-    print(response)
-
-asyncio.run(main())
-```
+<https://aiobalaboba.readthedocs.io/>
 
 ## License
 
 [MIT](https://github.com/monosans/aiobalaboba/blob/main/LICENSE)
```

