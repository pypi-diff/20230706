# Comparing `tmp/spyral_cli-1.0.6.tar.gz` & `tmp/spyral_cli-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-1.0.6.tar", max compression
+gzip compressed data, was "spyral_cli-1.0.7.tar", max compression
```

## Comparing `spyral_cli-1.0.6.tar` & `spyral_cli-1.0.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      691 2023-07-05 15:33:45.110669 spyral_cli-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.6/src/spyral/__init__.py
--rw-r--r--   0        0        0     7007 2023-07-05 15:32:14.537063 spyral_cli-1.0.6/src/spyral/cli.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-07-06 13:33:29.779202 spyral_cli-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.7/src/spyral/__init__.py
+-rw-r--r--   0        0        0     7083 2023-07-06 08:53:53.525992 spyral_cli-1.0.7/src/spyral/cli.py
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 spyral_cli-1.0.7/PKG-INFO
```

### Comparing `spyral_cli-1.0.6/pyproject.toml` & `spyral_cli-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyral-cli"
-version = "1.0.6"
+version = "1.0.7"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "spyral", from = "src" },
 ]
 
@@ -14,20 +14,20 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 typer = "^0.9.0"
 psutil = "^5.9.5"
 rich = "^13.4.2"
 plotext = "^5.2.8"
 backports-strenum = "^1.2.4"
+pandas = "^2.0.3"
+numpy = "^1.25.0"
 
 [tool.poetry.group.plot]
 [tool.poetry.group.plot.dependencies]
 matplotlib = "^3.7.1"
-pandas = "^2.0.3"
-numpy = "^1.25.0"
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spyral_cli-1.0.6/src/spyral/cli.py` & `spyral_cli-1.0.7/src/spyral/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,17 @@
     png = "png"
 
 
 @app.command()
 def plot(
     csv: Path = typer.Argument(..., dir_okay=False, exists=True),
     formats: List[Format] = ["pdf"],
-    output: Path = Path.cwd(),
+    output: Path = typer.Option(
+        Path.cwd(), "--output", "-o", file_okay=False, exists=True
+    ),
 ):
     console = rich.console.Console()
     with console.status("Importing plotting modules"):
         import matplotlib
 
         matplotlib.use("Agg")
         import matplotlib.pyplot as plt
```

### Comparing `spyral_cli-1.0.6/PKG-INFO` & `spyral_cli-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backports-strenum (>=1.2.4,<2.0.0)
+Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: plotext (>=5.2.8,<6.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

