# Comparing `tmp/stdatm-0.2.0.tar.gz` & `tmp/stdatm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdatm-0.2.0.tar", max compression
+gzip compressed data, was "stdatm-0.3.0.tar", max compression
```

## Comparing `stdatm-0.2.0.tar` & `stdatm-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-02-16 10:36:32.394670 stdatm-0.2.0/LICENSE
--rw-r--r--   0        0        0       50 2022-02-16 10:36:32.394670 stdatm-0.2.0/README.md
--rw-r--r--   0        0        0     2326 2022-02-16 10:36:39.314671 stdatm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1113 2022-02-16 10:36:32.394670 stdatm-0.2.0/src/stdatm/__init__.py
--rw-r--r--   0        0        0    17987 2022-02-16 10:36:32.394670 stdatm-0.2.0/src/stdatm/atmosphere.py
--rw-r--r--   0        0        0      765 2022-02-16 10:36:40.425725 stdatm-0.2.0/setup.py
--rw-r--r--   0        0        0     1114 2022-02-16 10:36:40.426201 stdatm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-06 08:21:38.389067 stdatm-0.3.0/LICENSE
+-rw-r--r--   0        0        0       50 2023-07-06 08:21:38.389067 stdatm-0.3.0/README.md
+-rw-r--r--   0        0        0     2567 2023-07-06 08:21:57.981546 stdatm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1183 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/__init__.py
+-rw-r--r--   0        0        0    14500 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/atmosphere.py
+-rw-r--r--   0        0        0     7111 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/atmosphere_partials.py
+-rw-r--r--   0        0        0     6822 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/partials_state_parameters.py
+-rw-r--r--   0        0        0     8954 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/speed_parameters.py
+-rw-r--r--   0        0        0     4447 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/state_parameters.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 stdatm-0.3.0/PKG-INFO
```

### Comparing `stdatm-0.2.0/LICENSE` & `stdatm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stdatm-0.2.0/pyproject.toml` & `stdatm-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stdatm"
-version = "v0.2.0"
+version = "0.3.0"
 description = "Numpy-oriented Standard Atmosphere model"
 readme = "README.md"
 authors = [
     "Christophe DAVID <christophe.david@onera.fr>",
 ]
 license = "GPL-3.0-only"
 classifiers = [
@@ -13,47 +13,58 @@
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
 packages = [
     { include = "stdatm", from = "src" },
 ]
 exclude = ["**/tests/**"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-numpy = "^1.17.3"
-scipy = "^1.4.1"
+python = "^3.8"
+numpy = "^1.22.0"
+scipy = "^1.9.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 coverage = { version = "^6.0", extras = ["toml"] }
-pre-commit = "^2.14.1"
-black = { version = "22.1.0" }
-flake8 = "^4.0.1"
+
+[tool.poetry.group.benchmark.dependencies]
+pytest-profiling = "^1.7.0"
+snakeviz = "^2.1.1"
+pytest-benchmark = { version = "^4", extras = ["histogram"] }
+
+[tool.poetry.group.doc.dependencies]
 sphinx = "^4.1.2"
 sphinx-rtd-theme = "^1.0"
 sphinxcontrib-bibtex = "^2.3.0"
-pytest-profiling = "^1.7.0"
-snakeviz = "^2.1.1"
-pytest-benchmark = { version = "^3.4.1", extras = ["histogram"] }
+
+[tool.poetry.group.lint.dependencies]
+pre-commit = "^2.14.1"
+black = { version = "23.3.0" }
+flake8 = "^4.0.1"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 100
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov stdatm --cov-report term-missing --cov-report html --verbose --benchmark-disable --benchmark-autosave"
```

### Comparing `stdatm-0.2.0/src/stdatm/__init__.py` & `stdatm-0.3.0/src/stdatm/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pkg_resources import DistributionNotFound, get_distribution
 
 from .atmosphere import Atmosphere, AtmosphereSI  # noqa: F401
+from .atmosphere_partials import AtmosphereWithPartials  # noqa: F401
 
 try:
     # Change here if project is renamed and does not equal the package name
     dist_name = "StdAtm"
     __version__ = get_distribution(dist_name).version
 except DistributionNotFound:
     __version__ = "unknown"
```

### Comparing `stdatm-0.2.0/PKG-INFO` & `stdatm-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: stdatm
-Version: 0.2.0
+Version: 0.3.0
 Summary: Numpy-oriented Standard Atmosphere model
 License: GPL-3.0-only
 Author: Christophe DAVID
 Author-email: christophe.david@onera.fr
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: numpy (>=1.17.3,<2.0.0)
-Requires-Dist: scipy (>=1.4.1,<2.0.0)
+Requires-Dist: numpy (>=1.22.0,<2.0.0)
+Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # StdAtm
 Numpy-oriented Standard Atmosphere model
```

