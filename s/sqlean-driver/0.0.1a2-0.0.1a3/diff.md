# Comparing `tmp/sqlean_driver-0.0.1a2.tar.gz` & `tmp/sqlean_driver-0.0.1a3.tar.gz`

## Comparing `sqlean_driver-0.0.1a2.tar` & `sqlean_driver-0.0.1a3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/.github/dependabot.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/.github/semantic.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/src/sqlean_driver/__about__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/src/sqlean_driver/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/tests/__init__.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/tests/test_driver.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/LICENSE.txt
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/README.md
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/.github/dependabot.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/.github/semantic.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/src/sqlean_driver/__about__.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/src/sqlean_driver/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/tests/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/tests/conftest.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/tests/test_driver.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/LICENSE.txt
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/README.md
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 sqlean_driver-0.0.1a3/PKG-INFO
```

### Comparing `sqlean_driver-0.0.1a2/.github/dependabot.yaml` & `sqlean_driver-0.0.1a3/.github/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `sqlean_driver-0.0.1a2/.github/workflows/release.yaml` & `sqlean_driver-0.0.1a3/.github/workflows/release.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -44,8 +44,8 @@
                 with:
                     file: dist/*.whl
                     tag: ${{ github.ref }}
                     overwrite: true
                     file_glob: true
             
             -   name: Publish
-                uses: pypa/gh-action-pypi-publish@v1.8.6
+                uses: pypa/gh-action-pypi-publish@v1.8.7
```

### Comparing `sqlean_driver-0.0.1a2/.github/workflows/test.yaml` & `sqlean_driver-0.0.1a3/.github/workflows/test.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -25,32 +25,54 @@
               env:
                 PIP_CONSTRAINT: .github/workflows/constraints.txt
               run: |
                 pipx install hatch
             - name: Run lint
               run: |
                 hatch run lint:style-gh
+
+    typing:
+      name: Typing
+      runs-on: ubuntu-latest
+      steps:
+          - uses: actions/checkout@v3
+          - uses: actions/setup-python@v4
+            with:
+                cache: pip
+                python-version: "3.11"
+          - name: Install dependencies
+            env:
+              PIP_CONSTRAINT: .github/workflows/constraints.txt
+            run: |
+              pipx install hatch
+          - name: Run typing
+            run: |
+              hatch run typing:check
+
     test:
-        name: Pytest
+        name: Pytest (Python ${{ matrix.python-version }}, SQLAlchemy ${{ matrix.sqlalchemy-version }})
         runs-on: ubuntu-latest
         strategy:
             matrix:
                 python-version: ["3.8", "3.9", "3.10", "3.11"]
+                sqlalchemy-version: ["1", "2"]
         steps:
             - uses: actions/checkout@v3
             - uses: actions/setup-python@v4
               with:
                   cache: pip
                   python-version: ${{ matrix.python-version }}
             - name: Install dependencies
               env:
                 PIP_CONSTRAINT: .github/workflows/constraints.txt
               run: |
                 pipx install hatch
             - name: Run tests
+              env:
+                SQLALCHEMY_VERSION: ${{ matrix.sqlalchemy-version }}
               run: |
                 hatch run test-cov
             - uses: actions/upload-artifact@v3
               with:
                 name: coverage-data
                 path: ".coverage.*"
```

### Comparing `sqlean_driver-0.0.1a2/src/sqlean_driver/__init__.py` & `sqlean_driver-0.0.1a3/src/sqlean_driver/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,39 @@
 
 import typing as t
 from importlib.metadata import version
 
 from sqlalchemy.dialects.sqlite.pysqlite import SQLiteDialect_pysqlite
 
 if t.TYPE_CHECKING:
+    from types import ModuleType
+
     from sqlalchemy.engine.url import URL
 
 
 __version__ = version(__package__)
 
 
 class SQLeanDialect(SQLiteDialect_pysqlite):
     """A dialect for SQLite that uses sqlean.py as the DBAPI."""
 
     driver = "sqlean"
     supports_statement_cache = True
 
     @classmethod
-    def import_dbapi(cls: type[SQLeanDialect]) -> type:
+    def dbapi(cls: type[SQLeanDialect]) -> ModuleType:  # type: ignore[override]
         """Return the DBAPI module."""
         import sqlean
 
         return sqlean
 
     def on_connect_url(self: SQLeanDialect, url: URL) -> t.Callable[[t.Any], t.Any] | None:
         """Return a callable that will be executed on connect."""
-        extensions = url.query.get("extensions", "").split(",")
+        query = url.query.get("extensions", ())
+        extensions = query if isinstance(query, tuple) else query.split(",")
+
         if "all" in extensions:
-            self.dbapi.extensions.enable_all()
+            self.dbapi.extensions.enable_all()  # type: ignore[attr-defined]
         else:
-            self.dbapi.extensions.enable(*extensions)
+            self.dbapi.extensions.enable(*extensions)  # type: ignore[attr-defined]
 
         return super().on_connect_url(url)
```

### Comparing `sqlean_driver-0.0.1a2/tests/test_driver.py` & `sqlean_driver-0.0.1a3/tests/test_driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Test the driver class."""
 
 from __future__ import annotations
 
 import typing as t
+from types import ModuleType
 
 import pytest
-from sqlalchemy import create_engine, text
+from sqlalchemy import column, create_engine, func, select
+from sqlalchemy.exc import OperationalError
 
 if t.TYPE_CHECKING:
     from sqlalchemy.engine import Engine
+    from sqlalchemy.sql.selectable import Select
 
 
 @pytest.fixture()
 def engine() -> Engine:
     """Return a SQLAlchemy engine."""
     url = "sqlite+sqlean:///:memory:"
     return create_engine(url)
@@ -21,51 +24,76 @@
 def test_driver_name(engine: Engine):
     """Test that the URL works."""
     assert engine.dialect.driver == "sqlean"
 
 
 def test_driver_dbapi(engine: Engine):
     """Test that the DBAPI is sqlean."""
+    assert isinstance(engine.dialect.dbapi, ModuleType)
     assert engine.dialect.dbapi.__name__ == "sqlean"
 
 
 def test_sql(engine: Engine):
     """Test that the SQL works."""
     with engine.connect() as conn:
-        result = conn.execute(text("SELECT 1"))
+        result = conn.execute(select(1))
     assert result.fetchone() == (1,)
 
 
+def test_no_extensions(engine: Engine):
+    """Test that the extensions are not loaded."""
+    with pytest.raises(OperationalError), engine.connect() as conn:
+        conn.execute(
+            select(
+                func.median(column("value")),
+            ).select_from(
+                func.generate_series(1, 99).alias("generate_series_1"),
+            ),
+        )
+
+
 @pytest.mark.parametrize(
     ("extensions", "query", "expected"),
     [
         (
             "all",
-            """
-            select
-                hex(md5('hello' || value)) as crypto,
-                median(value) as stats
-            from generate_series(1, 99)
-            """,
+            select(
+                func.hex(func.md5(func.concat("hello", column("value")))).label("crypto"),
+                func.median(column("value")).label("stats"),
+            ).select_from(
+                func.generate_series(1, 99).alias("generate_series_1"),
+            ),
             ("203AD5FFA1D7C650AD681FDFF3965CD2", 50),
         ),
-        ("stats", "select median(value) from generate_series(1, 99)", (50,)),
-        ("crypto", "select hex(md5('hello'))", ("5D41402ABC4B2A76B9719D911017C592",)),
-        ("ipaddr", "select ipfamily('192.168.1.1')", (4,)),
+        (
+            "stats",
+            select(
+                func.median(column("value")),
+            ).select_from(
+                func.generate_series(1, 99).alias("generate_series_1"),
+            ),
+            (50,),
+        ),
+        ("crypto", select(func.hex(func.md5("hello"))), ("5D41402ABC4B2A76B9719D911017C592",)),
+        (
+            "ipaddr",
+            select(func.ipfamily("192.168.1.1")),
+            (4,),
+        ),
         (
             "ipaddr,crypto",
-            """select
-                ipnetwork('192.168.16.12/24') as network,
-                hex(md5('hello')) as hash
-            """,
+            select(
+                func.ipnetwork("192.168.16.12/24").label("network"),
+                func.hex(func.md5("hello")).label("hash"),
+            ),
             ("192.168.16.0/24", "5D41402ABC4B2A76B9719D911017C592"),
         ),
     ],
     ids=["all", "stats", "crypto", "ipaddr", "multiple"],
 )
-def test_extensions(extensions: str, query: str, expected: tuple):
+def test_extensions(extensions: str, query: Select, expected: tuple):
     """Test that the extensions work."""
     url = f"sqlite+sqlean:///:memory:?extensions={extensions}"
     engine = create_engine(url)
     with engine.connect() as conn:
-        result = conn.execute(text(query))
+        result = conn.execute(query)
     assert result.fetchone() == expected
```

### Comparing `sqlean_driver-0.0.1a2/.gitignore` & `sqlean_driver-0.0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlean_driver-0.0.1a2/LICENSE.txt` & `sqlean_driver-0.0.1a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlean_driver-0.0.1a2/README.md` & `sqlean_driver-0.0.1a3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,40 +20,40 @@
 ```console
 pip install sqlean-driver
 ```
 
 ## Usage
 
 ```python
-from sqlalchemy import create_engine, text
+from sqlalchemy import create_engine, func, select
 
 engine = create_engine("sqlite+sqlean:///:memory:?extensions=all")
 
 with engine.connect() as conn:
-    result = conn.execute(text("SELECT ipfamily('192.168.1.1')"))
+    result = conn.execute(select(func.ipfamily("192.168.1.1")))
     print(result.scalar())  # 4
 ```
 
 ### Extensions
 
 By default, `sqlean.py` disables all [SQLite extensions](https://github.com/nalgeon/sqlean.py#extensions). To enable all of them, pass `extensions=all` as a query parameter to the connection string. Or use a comma-separated list of extensions to enable only some of them, e.g. `extensions=ipaddr,crypto`.
 
 ### Alternatives
 
-Note that you don't strictly need this driver to use `sqlean.py`. You can supply `sqlean` as the [`module`](https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine.params.module) parameter:
+Note that you don't strictly need this driver to use `sqlean.py` with SQLAlchemy. You can supply `sqlean` as the [`module`](https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine.params.module) parameter to `create_engine`:
 
 ```python
 import sqlean
-from sqlalchemy import create_engine, text
+from sqlalchemy import create_engine, func, select
 
 sqlean.extensions.enable_all()
 engine = create_engine("sqlite:///:memory:", module=sqlean)
 
 with engine.connect() as conn:
-    result = conn.execute(text("SELECT ipfamily('192.168.1.1')"))
+    result = conn.execute(select(func.ipfamily("192.168.1.1")))
     print(result.scalar())  # 4
 ```
 
 ## Development
 
 This project uses [Hatch](https://hatch.pypa.io/) to manage the development environment, so make sure you have it installed.
 
@@ -65,10 +65,16 @@
 
 ### Run linter
 
 ```console
 hatch run lint:style
 ```
 
+### Run type checker
+
+```console
+hatch run typing:check
+```
+
 ## License
 
 `sqlean-driver` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `sqlean_driver-0.0.1a2/pyproject.toml` & `sqlean_driver-0.0.1a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -39,40 +39,54 @@
 Issues = "https://github.com/edgarrmondragon/sqlean-driver/issues"
 Source = "https://github.com/edgarrmondragon/sqlean-driver"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.envs.default]
-dependencies = ["coverage[toml]>=6.5", "pytest"]
+dependencies = ["coverage[toml]>=6.5", "pytest", "sqlalchemy=={env:SQLALCHEMY_VERSION:1}.*"]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-xml = "coverage xml"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
+[tool.hatch.envs.typing]
+dependencies = ["mypy>=1.0.0", "pytest"]
+[tool.hatch.envs.typing.scripts]
+check = "mypy --install-types --non-interactive {args:src/sqlean_driver tests}"
+
 [tool.hatch.envs.lint]
 detached = true
 dependencies = ["black>=23.1.0", "mypy>=1.0.0", "ruff>=0.0.243"]
 [tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/sqlean_driver tests}"
 style = ["ruff check {args:.}", "black --check --diff {args:.}"]
 style-gh = ["ruff check {args:.} --format github", "black --check --diff {args:.}"]
 fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
-all = ["style", "typing"]
 
 [tool.black]
 target-version = ["py38"]
 line-length = 100
 skip-string-normalization = true
 
+[tool.mypy]
+warn_unreachable = true
+warn_unused_configs = true
+warn_unused_ignores = true
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "sqlean.*",
+]
+
 [tool.pytest]
 addopts = ["-vv"]
 
 [tool.ruff]
 line-length = 100
 select = [
   "ALL",
```

### Comparing `sqlean_driver-0.0.1a2/PKG-INFO` & `sqlean_driver-0.0.1a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlean-driver
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: SQLAlchemy dialect for the sqlean.py SQLite wrapper
 Project-URL: Documentation, https://github.com/edgarrmondragon/sqlean-driver#readme
 Project-URL: Issues, https://github.com/edgarrmondragon/sqlean-driver/issues
 Project-URL: Source, https://github.com/edgarrmondragon/sqlean-driver
 Author-email: Edgar Ramírez Mondragón <edgarrm358@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -45,40 +45,40 @@
 ```console
 pip install sqlean-driver
 ```
 
 ## Usage
 
 ```python
-from sqlalchemy import create_engine, text
+from sqlalchemy import create_engine, func, select
 
 engine = create_engine("sqlite+sqlean:///:memory:?extensions=all")
 
 with engine.connect() as conn:
-    result = conn.execute(text("SELECT ipfamily('192.168.1.1')"))
+    result = conn.execute(select(func.ipfamily("192.168.1.1")))
     print(result.scalar())  # 4
 ```
 
 ### Extensions
 
 By default, `sqlean.py` disables all [SQLite extensions](https://github.com/nalgeon/sqlean.py#extensions). To enable all of them, pass `extensions=all` as a query parameter to the connection string. Or use a comma-separated list of extensions to enable only some of them, e.g. `extensions=ipaddr,crypto`.
 
 ### Alternatives
 
-Note that you don't strictly need this driver to use `sqlean.py`. You can supply `sqlean` as the [`module`](https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine.params.module) parameter:
+Note that you don't strictly need this driver to use `sqlean.py` with SQLAlchemy. You can supply `sqlean` as the [`module`](https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine.params.module) parameter to `create_engine`:
 
 ```python
 import sqlean
-from sqlalchemy import create_engine, text
+from sqlalchemy import create_engine, func, select
 
 sqlean.extensions.enable_all()
 engine = create_engine("sqlite:///:memory:", module=sqlean)
 
 with engine.connect() as conn:
-    result = conn.execute(text("SELECT ipfamily('192.168.1.1')"))
+    result = conn.execute(select(func.ipfamily("192.168.1.1")))
     print(result.scalar())  # 4
 ```
 
 ## Development
 
 This project uses [Hatch](https://hatch.pypa.io/) to manage the development environment, so make sure you have it installed.
 
@@ -90,10 +90,16 @@
 
 ### Run linter
 
 ```console
 hatch run lint:style
 ```
 
+### Run type checker
+
+```console
+hatch run typing:check
+```
+
 ## License
 
 `sqlean-driver` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

