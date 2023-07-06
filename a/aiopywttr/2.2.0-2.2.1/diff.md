# Comparing `tmp/aiopywttr-2.2.0.tar.gz` & `tmp/aiopywttr-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopywttr-2.2.0.tar", max compression
+gzip compressed data, was "aiopywttr-2.2.1.tar", max compression
```

## Comparing `aiopywttr-2.2.0.tar` & `aiopywttr-2.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-20 07:24:39.800123 aiopywttr-2.2.0/LICENSE
--rw-r--r--   0        0        0     1738 2023-04-22 20:08:34.439262 aiopywttr-2.2.0/README.md
--rw-r--r--   0        0        0      183 2023-04-22 19:53:57.019253 aiopywttr-2.2.0/aiopywttr/__init__.py
--rw-r--r--   0        0        0     5591 2023-04-20 07:24:39.800123 aiopywttr-2.2.0/aiopywttr/_wttr.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:39.800123 aiopywttr-2.2.0/aiopywttr/py.typed
--rw-r--r--   0        0        0     3046 2023-04-22 20:17:01.709267 aiopywttr-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3202 1970-01-01 00:00:00.000000 aiopywttr-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/LICENSE
+-rw-r--r--   0        0        0      603 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/README.md
+-rw-r--r--   0        0        0      183 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/aiopywttr/__init__.py
+-rw-r--r--   0        0        0     6104 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/aiopywttr/_wttr.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/aiopywttr/py.typed
+-rw-r--r--   0        0        0     3431 2023-07-06 15:59:22.689695 aiopywttr-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 aiopywttr-2.2.1/PKG-INFO
```

### Comparing `aiopywttr-2.2.0/LICENSE` & `aiopywttr-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopywttr-2.2.0/aiopywttr/_wttr.py` & `aiopywttr-2.2.1/aiopywttr/_wttr.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,40 @@
 from typing import Any, Optional
 
 import pywttr_models
 from aiohttp import ClientResponse, ClientSession
 
 
 class Wttr:
-    """Asynchronous wrapper for wttr.in weather forecast API."""
+    """Asynchronous wrapper for wttr.in weather forecast API.
+
+    Examples:
+        Prints the average temperature in New York today:
+
+        ```python
+        >>> import asyncio
+        >>>
+        >>> import aiopywttr
+        >>>
+        >>>
+        >>> async def main():
+        ...     wttr = aiopywttr.Wttr("New York")
+        ...     forecast = await wttr.en()
+        ...     print(forecast.weather[0].avgtemp_c)
+        >>>
+        >>>
+        >>> asyncio.run(main())
+        ```
+    """
 
     __slots__ = ("location", "session")
 
-    def __init__(self, location: str, session: Optional[ClientSession] = None) -> None:
+    def __init__(
+        self, location: str, session: Optional[ClientSession] = None
+    ) -> None:
         self.location = location
         self.session = session
 
     async def af(self) -> pywttr_models.af.Model:
         return pywttr_models.af.Model.parse_obj(await self._get_json("af"))
 
     async def am(self) -> pywttr_models.am.Model:
@@ -87,15 +108,17 @@
     async def oc(self) -> pywttr_models.oc.Model:
         return pywttr_models.oc.Model.parse_obj(await self._get_json("oc"))
 
     async def pl(self) -> pywttr_models.pl.Model:
         return pywttr_models.pl.Model.parse_obj(await self._get_json("pl"))
 
     async def pt_br(self) -> pywttr_models.pt_br.Model:
-        return pywttr_models.pt_br.Model.parse_obj(await self._get_json("pt-br"))
+        return pywttr_models.pt_br.Model.parse_obj(
+            await self._get_json("pt-br")
+        )
 
     async def ro(self) -> pywttr_models.ro.Model:
         return pywttr_models.ro.Model.parse_obj(await self._get_json("ro"))
 
     async def ru(self) -> pywttr_models.ru.Model:
         return pywttr_models.ru.Model.parse_obj(await self._get_json("ru"))
 
@@ -111,18 +134,22 @@
     async def uk(self) -> pywttr_models.uk.Model:
         return pywttr_models.uk.Model.parse_obj(await self._get_json("uk"))
 
     async def vi(self) -> pywttr_models.vi.Model:
         return pywttr_models.vi.Model.parse_obj(await self._get_json("vi"))
 
     async def zh_cn(self) -> pywttr_models.zh_cn.Model:
-        return pywttr_models.zh_cn.Model.parse_obj(await self._get_json("zh-cn"))
+        return pywttr_models.zh_cn.Model.parse_obj(
+            await self._get_json("zh-cn")
+        )
 
     async def zh_tw(self) -> pywttr_models.zh_tw.Model:
-        return pywttr_models.zh_tw.Model.parse_obj(await self._get_json("zh-tw"))
+        return pywttr_models.zh_tw.Model.parse_obj(
+            await self._get_json("zh-tw")
+        )
 
     async def _get_json(self, lang: str) -> Any:
         if isinstance(self.session, ClientSession) and not self.session.closed:
             response = await self._fetch(lang, self.session)
         else:
             async with ClientSession() as session:
                 response = await self._fetch(lang, session)
```

### Comparing `aiopywttr-2.2.0/pyproject.toml` & `aiopywttr-2.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "aiopywttr"
-version = "2.2.0"
+version = "2.2.1"
 description = "Asynchronous wrapper for wttr.in API"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/aiopywttr"
+documentation = "https://aiopywttr.readthedocs.io/"
 keywords = ["forecast", "weather"]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic :: 1",
     "Framework :: Pydantic",
     "Intended Audience :: Developers",
@@ -30,24 +31,33 @@
 python = "^3.7.2"
 aiohttp = "^3.8"
 pywttr-models = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 covdefaults = "2.3.0"
-mypy = "1.2.0"
+mypy = "1.4.1"
 pre-commit = "2.21.0"
-pydantic = "1.10.7"
-pytest = "7.3.1"
+pydantic = "2.0.2"
+pytest = "7.4.0"
 pytest-asyncio = "0.21.0"
-pytest-cov = "4.0.0"
-ruff = "0.0.262"
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
@@ -59,14 +69,15 @@
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
@@ -74,23 +85,24 @@
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.pytest.ini_options]
+addopts = ["--strict-config", "--strict-markers"]
+asyncio_mode = "auto"
 xfail_strict = true
-addopts = ["--strict-markers", "--strict-config", "--asyncio-mode=auto"]
 
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
@@ -105,23 +117,27 @@
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
@@ -136,13 +152,16 @@
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

