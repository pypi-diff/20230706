# Comparing `tmp/sp_variant-3.2.1.tar.gz` & `tmp/sp_variant-3.2.2.tar.gz`

## Comparing `sp_variant-3.2.1.tar` & `sp_variant-3.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sp_variant-3.2.1/.editorconfig
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sp_variant-3.2.1/mkdocs.yml
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 sp_variant-3.2.1/tox.ini
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sp_variant-3.2.1/.reuse/dep5
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.2.1/LICENSES/BSD-2-Clause.txt
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 sp_variant-3.2.1/data/common/scripts/add-storpool-repo.sh
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 sp_variant-3.2.1/data/common/scripts/storpool_variant.sh
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sp_variant-3.2.1/data/debian/repo/storpool-keyring.gpg
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sp_variant-3.2.1/data/debian/repo/storpool.sources
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 sp_variant-3.2.1/data/redhat/repo/RPM-GPG-KEY-StorPool
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sp_variant-3.2.1/data/redhat/repo/storpool-centos.repo
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.2.1/docs/api.md
--rw-r--r--   0        0        0    16967 2020-02-02 00:00:00.000000 sp_variant-3.2.1/docs/changes.md
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.2.1/docs/index.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sp_variant-3.2.1/examples/build-repo-overrides.toml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/config/ruff-all/pyproject.toml
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/config/ruff-base/pyproject.toml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/requirements/docs.txt
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/requirements/ruff.txt
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/requirements/test-mypy.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/requirements/test-tox-stages.txt
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/requirements/test-unit.txt
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/requirements/tools.txt
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_build_repo/__init__.py
--rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_build_repo/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_build_repo/py.typed
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_build_repo/subst.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_variant/__init__.py
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_variant/__main__.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_variant/defs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_variant/py.typed
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_variant/variant.py
--rw-r--r--   0        0        0    29586 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_variant/vbuild.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/sp_variant/yaiparser.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/test_docker/__init__.py
--rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/test_docker/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/unit_tests/__init__.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/unit_tests/test_subst.py
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/unit_tests/test_variant.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sp_variant-3.2.1/python/unit_tests/test_yaiparser.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sp_variant-3.2.1/.gitignore
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.2.1/README.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sp_variant-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 sp_variant-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sp_variant-3.2.2/.editorconfig
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sp_variant-3.2.2/mkdocs.yml
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 sp_variant-3.2.2/tox.ini
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sp_variant-3.2.2/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.2.2/LICENSES/BSD-2-Clause.txt
+-rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 sp_variant-3.2.2/data/common/scripts/add-storpool-repo.sh
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 sp_variant-3.2.2/data/common/scripts/storpool_variant.sh
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sp_variant-3.2.2/data/debian/repo/storpool-keyring.gpg
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sp_variant-3.2.2/data/debian/repo/storpool.sources
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 sp_variant-3.2.2/data/redhat/repo/RPM-GPG-KEY-StorPool
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sp_variant-3.2.2/data/redhat/repo/storpool-centos.repo
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.2.2/docs/api.md
+-rw-r--r--   0        0        0    17426 2020-02-02 00:00:00.000000 sp_variant-3.2.2/docs/changes.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sp_variant-3.2.2/docs/index.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sp_variant-3.2.2/examples/build-repo-overrides.toml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/requirements/docs.txt
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/requirements/ruff.txt
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/requirements/test-mypy.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/requirements/test-tox-stages.txt
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/requirements/test-unit.txt
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/requirements/tools.txt
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_build_repo/__init__.py
+-rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_build_repo/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_build_repo/py.typed
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_build_repo/subst.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_variant/__init__.py
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_variant/__main__.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_variant/defs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_variant/py.typed
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_variant/variant.py
+-rw-r--r--   0        0        0    29586 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_variant/vbuild.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/sp_variant/yaiparser.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/test_docker/__init__.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/test_docker/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/unit_tests/__init__.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/unit_tests/test_subst.py
+-rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/unit_tests/test_variant.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sp_variant-3.2.2/python/unit_tests/test_yaiparser.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sp_variant-3.2.2/.gitignore
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.2.2/README.md
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 sp_variant-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 sp_variant-3.2.2/PKG-INFO
```

### Comparing `sp_variant-3.2.1/.editorconfig` & `sp_variant-3.2.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/mkdocs.yml` & `sp_variant-3.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/tox.ini` & `sp_variant-3.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/LICENSES/BSD-2-Clause.txt` & `sp_variant-3.2.2/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/data/debian/repo/storpool-keyring.gpg` & `sp_variant-3.2.2/data/debian/repo/storpool-keyring.gpg`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/data/redhat/repo/RPM-GPG-KEY-StorPool` & `sp_variant-3.2.2/data/redhat/repo/RPM-GPG-KEY-StorPool`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/data/redhat/repo/storpool-centos.repo` & `sp_variant-3.2.2/data/redhat/repo/storpool-centos.repo`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/docs/changes.md` & `sp_variant-3.2.2/docs/changes.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,30 @@
 All notable changes to the sp-variant project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.2.2] - 2023-07-06
+
+### Fixes
+
+- docs:
+    - fix the 3.2.1 GitHub commit log URL
+
+### Additions
+
+- docs:
+    - add a navigational bar-like list of URLs at the top of the index page
+    - use a link reference for the StorPool support team e-mail address
+- python:
+    - add the repo.storpool.com URL as the project homepage, keep the GitHub one as
+      "Source Code"
+
 ## [3.2.1] - 2023-07-06
 
 ### Fixes
 
 - python:
     - drop the unneeded `hatch-requirements-txt` PEP 517 build dependency
 
@@ -431,16 +447,17 @@
 
 ## [1.3.0] - 2021-09-15
 
 ### Started
 
 - First public release.
 
-[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.2.1...main
-[3.2.0]: https://github.com/storpool/sp-variant/compare/release/3.2.0...release/3.2.1
+[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.2.2...main
+[3.2.2]: https://github.com/storpool/sp-variant/compare/release/3.2.1...release/3.2.2
+[3.2.1]: https://github.com/storpool/sp-variant/compare/release/3.2.0...release/3.2.1
 [3.2.0]: https://github.com/storpool/sp-variant/compare/release/3.1.2...release/3.2.0
 [3.1.2]: https://github.com/storpool/sp-variant/compare/release/3.1.1...release/3.1.2
 [3.1.1]: https://github.com/storpool/sp-variant/compare/release/3.1.0...release/3.1.1
 [3.1.0]: https://github.com/storpool/sp-variant/compare/release/3.0.0...release/3.1.0
 [3.0.0]: https://github.com/storpool/sp-variant/compare/release/2.3.3...release/3.0.0
 [2.3.3]: https://github.com/storpool/sp-variant/compare/release/2.3.2...release/2.3.3
 [2.3.2]: https://github.com/storpool/sp-variant/compare/release/2.3.1...release/2.3.2
```

### Comparing `sp_variant-3.2.1/docs/index.md` & `sp_variant-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/config/ruff-base/pyproject.toml` & `sp_variant-3.2.2/python/config/ruff-base/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/sp_build_repo/__main__.py` & `sp_variant-3.2.2/python/sp_build_repo/__main__.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/sp_build_repo/subst.py` & `sp_variant-3.2.2/python/sp_build_repo/subst.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/sp_variant/__main__.py` & `sp_variant-3.2.2/python/sp_variant/__main__.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/sp_variant/defs.py` & `sp_variant-3.2.2/python/sp_variant/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     """Attributes common to a StorPool package repository."""
 
     name: str
     extension: str
     url: str
 
 
-VERSION: Final = "3.2.1"
+VERSION: Final = "3.2.2"
 FORMAT_VERSION: Final = (1, 4)
 
 REPO_TYPES: Final = [
     RepoType(name="contrib", extension="", url="https://repo.storpool.com/public/"),
     RepoType(
         name="staging",
         extension="-staging",
```

### Comparing `sp_variant-3.2.1/python/sp_variant/variant.py` & `sp_variant-3.2.2/python/sp_variant/variant.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/sp_variant/vbuild.py` & `sp_variant-3.2.2/python/sp_variant/vbuild.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/sp_variant/yaiparser.py` & `sp_variant-3.2.2/python/sp_variant/yaiparser.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/test_docker/__main__.py` & `sp_variant-3.2.2/python/test_docker/__main__.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/unit_tests/test_subst.py` & `sp_variant-3.2.2/python/unit_tests/test_subst.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/unit_tests/test_variant.py` & `sp_variant-3.2.2/python/unit_tests/test_variant.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/python/unit_tests/test_yaiparser.py` & `sp_variant-3.2.2/python/unit_tests/test_yaiparser.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.2.1/README.md` & `sp_variant-3.2.2/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <!--
 SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
 SPDX-License-Identifier: BSD-2-Clause
 -->
 
 # sp-variant - detect the Linux distribution for the StorPool build system
 
+\[[Home][repo-sp-variant] | [GitHub][github] | [PyPI][pypi] | [crates.io][crates-io]\]
+
 The `sp-variant` library is mainly useful within the StorPool internal
 build and QA environment, as well as the first step of installations on
 end-user systems. It examines several files and tries to determine what
 distribution and what version it is running on.
 
 ## Basic command-line usage
 
@@ -41,8 +43,14 @@
 - `build_variants()` - return information about all supported variants
 - `detect()` - get an object describing the detected distribution
 - `get_from()` - get an object describing the specified distribution
 - `get_by_alias_from()` - same, but specify the StorPool builder alias for
   the distribution
 
 For more information, as well as for suggestions and problem reports, please
-contact [the StorPool support team](mailto:support@storpool.com).
+contact [the StorPool support team][sp-support].
+
+[repo-sp-variant]: https://repo.storpool.com/public/doc/sp-variant/ "The sp-variant home page"
+[github]: https://github.com/storpool/sp-variant "The sp-variant GitHub repository"
+[pypi]: https://pypi.org/project/sp-variant/ "The sp-variant PyPI project page"
+[crates-io]: https://crates.io/crates/sp-variant "The sp-variant Rust crate page"
+[sp-support]: mailto:support@storpool.com "The StorPool support team"
```

### Comparing `sp_variant-3.2.1/pyproject.toml` & `sp_variant-3.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,17 @@
 name = "StorPool"
 email = "support@storpool.com"
 
 [project.scripts]
 sp_variant = "sp_variant.__main__:main"
 
 [project.urls]
-Homepage = "https://github.com/storpool/sp-variant"
+Homepage = "https://repo.storpool.com/public/doc/sp-variant/"
 Changelog = "https://github.com/storpool/sp-variant/blob/main/docs/changes.md"
+"Source Code" = "https://github.com/storpool/sp-variant"
 
 [tool.hatch.build]
 include = [
   "/data",
   "/docs",
   ".editorconfig",
   "/examples",
```

### Comparing `sp_variant-3.2.1/PKG-INFO` & `sp_variant-3.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: sp-variant
-Version: 3.2.1
+Version: 3.2.2
 Summary: Detect the Linux distribution for the StorPool build system
-Project-URL: Homepage, https://github.com/storpool/sp-variant
+Project-URL: Homepage, https://repo.storpool.com/public/doc/sp-variant/
 Project-URL: Changelog, https://github.com/storpool/sp-variant/blob/main/docs/changes.md
+Project-URL: Source Code, https://github.com/storpool/sp-variant
 Author-email: StorPool <support@storpool.com>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: DFSG approved
```

