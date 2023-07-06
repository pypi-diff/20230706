# Comparing `tmp/sp-variant-3.1.2.tar.gz` & `tmp/sp_variant-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sp-variant-3.1.2.tar", last modified: Fri Mar 17 06:49:06 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sp-variant-3.1.2.tar` & `sp_variant-3.2.0.tar`

### file list

```diff
@@ -1,74 +1,44 @@
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.738447 sp-variant-3.1.2/
--rw-r--r--   0 roam      (1000) roam      (1000)      611 2023-03-02 06:49:02.000000 sp-variant-3.1.2/.editorconfig
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/.reuse/
--rw-r--r--   0 roam      (1000) roam      (1000)      376 2023-03-02 06:49:02.000000 sp-variant-3.1.2/.reuse/dep5
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/LICENSES/
--rw-r--r--   0 roam      (1000) roam      (1000)     1267 2023-03-02 06:49:02.000000 sp-variant-3.1.2/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      430 2023-03-17 06:47:57.000000 sp-variant-3.1.2/MANIFEST.in
--rw-r--r--   0 roam      (1000) roam      (1000)     3429 2023-03-17 06:49:06.738447 sp-variant-3.1.2/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     2064 2023-03-02 06:49:02.000000 sp-variant-3.1.2/README.md
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.730446 sp-variant-3.1.2/data/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.730446 sp-variant-3.1.2/data/common/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/data/common/scripts/
--rwxr-xr-x   0 roam      (1000) roam      (1000)      238 2023-03-02 06:49:02.000000 sp-variant-3.1.2/data/common/scripts/add-storpool-repo.sh
--rwxr-xr-x   0 roam      (1000) roam      (1000)      212 2023-03-02 06:49:02.000000 sp-variant-3.1.2/data/common/scripts/storpool_variant.sh
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.730446 sp-variant-3.1.2/data/debian/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/data/debian/repo/
--rw-r--r--   0 roam      (1000) roam      (1000)     2289 2021-09-06 17:50:36.000000 sp-variant-3.1.2/data/debian/repo/storpool-keyring.gpg
--rw-r--r--   0 roam      (1000) roam      (1000)      284 2023-03-02 06:49:02.000000 sp-variant-3.1.2/data/debian/repo/storpool.sources
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.730446 sp-variant-3.1.2/data/redhat/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/data/redhat/repo/
--rw-r--r--   0 roam      (1000) roam      (1000)     3171 2021-09-06 17:50:36.000000 sp-variant-3.1.2/data/redhat/repo/RPM-GPG-KEY-StorPool
--rw-r--r--   0 roam      (1000) roam      (1000)      579 2023-03-02 06:49:02.000000 sp-variant-3.1.2/data/redhat/repo/storpool-centos.repo
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/docs/
--rw-r--r--   0 roam      (1000) roam      (1000)    13615 2023-03-17 06:47:57.000000 sp-variant-3.1.2/docs/changes.md
--rw-r--r--   0 roam      (1000) roam      (1000)     2064 2023-03-16 21:50:09.000000 sp-variant-3.1.2/docs/index.md
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/examples/
--rw-r--r--   0 roam      (1000) roam      (1000)      346 2023-03-02 06:49:02.000000 sp-variant-3.1.2/examples/build-repo-overrides.toml
--rw-r--r--   0 roam      (1000) roam      (1000)     1126 2023-03-16 21:50:09.000000 sp-variant-3.1.2/mkdocs.yml
--rw-r--r--   0 roam      (1000) roam      (1000)     3183 2023-03-17 06:47:57.000000 sp-variant-3.1.2/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/config/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/config/ruff-all/
--rw-r--r--   0 roam      (1000) roam      (1000)      180 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/config/ruff-all/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/config/ruff-base/
--rw-r--r--   0 roam      (1000) roam      (1000)     1323 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/config/ruff-base/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/config/ruff-most/
--rw-r--r--   0 roam      (1000) roam      (1000)      698 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/config/ruff-most/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/requirements/
--rw-r--r--   0 roam      (1000) roam      (1000)      222 2023-03-16 21:50:09.000000 sp-variant-3.1.2/python/requirements/docs.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      306 2023-03-16 21:50:09.000000 sp-variant-3.1.2/python/requirements/test-mypy.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      230 2023-03-16 17:04:36.000000 sp-variant-3.1.2/python/requirements/test-tox-stages.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      166 2023-03-16 17:04:36.000000 sp-variant-3.1.2/python/requirements/test-unit.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      280 2023-03-16 17:04:36.000000 sp-variant-3.1.2/python/requirements/tools.txt
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/sp_build_repo/
--rw-r--r--   0 roam      (1000) roam      (1000)      348 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/sp_build_repo/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)    12535 2023-03-16 19:44:23.000000 sp-variant-3.1.2/python/sp_build_repo/__main__.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-09-14 21:00:48.000000 sp-variant-3.1.2/python/sp_build_repo/py.typed
--rw-r--r--   0 roam      (1000) roam      (1000)     4377 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/sp_build_repo/subst.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.734447 sp-variant-3.1.2/python/sp_variant/
--rw-r--r--   0 roam      (1000) roam      (1000)      457 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/sp_variant/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)    13247 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/sp_variant/__main__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     5039 2023-03-17 06:47:57.000000 sp-variant-3.1.2/python/sp_variant/defs.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-09-07 11:46:24.000000 sp-variant-3.1.2/python/sp_variant/py.typed
--rw-r--r--   0 roam      (1000) roam      (1000)     5655 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/sp_variant/variant.py
--rw-r--r--   0 roam      (1000) roam      (1000)    28608 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/sp_variant/vbuild.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4484 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/sp_variant/yaiparser.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.738447 sp-variant-3.1.2/python/sp_variant.egg-info/
--rw-r--r--   0 roam      (1000) roam      (1000)     3429 2023-03-17 06:49:06.000000 sp-variant-3.1.2/python/sp_variant.egg-info/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     1468 2023-03-17 06:49:06.000000 sp-variant-3.1.2/python/sp_variant.egg-info/SOURCES.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-03-17 06:49:06.000000 sp-variant-3.1.2/python/sp_variant.egg-info/dependency_links.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       56 2023-03-17 06:49:06.000000 sp-variant-3.1.2/python/sp_variant.egg-info/entry_points.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       11 2023-03-17 06:49:06.000000 sp-variant-3.1.2/python/sp_variant.egg-info/top_level.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-03-17 06:26:15.000000 sp-variant-3.1.2/python/sp_variant.egg-info/zip-safe
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.738447 sp-variant-3.1.2/python/test_docker/
--rw-r--r--   0 roam      (1000) roam      (1000)      172 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/test_docker/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)    16713 2023-03-16 17:04:36.000000 sp-variant-3.1.2/python/test_docker/__main__.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-17 06:49:06.738447 sp-variant-3.1.2/python/unit_tests/
--rw-r--r--   0 roam      (1000) roam      (1000)      160 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/unit_tests/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2504 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/unit_tests/test_subst.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4807 2023-03-16 17:04:36.000000 sp-variant-3.1.2/python/unit_tests/test_variant.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2998 2023-03-02 06:49:02.000000 sp-variant-3.1.2/python/unit_tests/test_yaiparser.py
--rw-r--r--   0 roam      (1000) roam      (1000)       96 2023-03-17 06:49:06.738447 sp-variant-3.1.2/setup.cfg
--rwxr-xr-x   0 roam      (1000) roam      (1000)      251 2023-03-02 06:49:02.000000 sp-variant-3.1.2/setup.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2020 2023-03-16 21:50:09.000000 sp-variant-3.1.2/tox.ini
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sp_variant-3.2.0/.editorconfig
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sp_variant-3.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 sp_variant-3.2.0/tox.ini
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sp_variant-3.2.0/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.2.0/LICENSES/BSD-2-Clause.txt
+-rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 sp_variant-3.2.0/data/common/scripts/add-storpool-repo.sh
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 sp_variant-3.2.0/data/common/scripts/storpool_variant.sh
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sp_variant-3.2.0/data/debian/repo/storpool-keyring.gpg
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sp_variant-3.2.0/data/debian/repo/storpool.sources
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 sp_variant-3.2.0/data/redhat/repo/RPM-GPG-KEY-StorPool
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sp_variant-3.2.0/data/redhat/repo/storpool-centos.repo
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.2.0/docs/api.md
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 sp_variant-3.2.0/docs/changes.md
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.2.0/docs/index.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sp_variant-3.2.0/examples/build-repo-overrides.toml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/requirements/docs.txt
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/requirements/ruff.txt
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/requirements/test-mypy.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/requirements/test-tox-stages.txt
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/requirements/test-unit.txt
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/requirements/tools.txt
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_build_repo/__init__.py
+-rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_build_repo/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_build_repo/py.typed
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_build_repo/subst.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_variant/__init__.py
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_variant/__main__.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_variant/defs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_variant/py.typed
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_variant/variant.py
+-rw-r--r--   0        0        0    29586 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_variant/vbuild.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/sp_variant/yaiparser.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/test_docker/__init__.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/test_docker/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/unit_tests/__init__.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/unit_tests/test_subst.py
+-rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/unit_tests/test_variant.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sp_variant-3.2.0/python/unit_tests/test_yaiparser.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sp_variant-3.2.0/.gitignore
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.2.0/README.md
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 sp_variant-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 sp_variant-3.2.0/PKG-INFO
```

### Comparing `sp-variant-3.1.2/.editorconfig` & `sp_variant-3.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `sp-variant-3.1.2/LICENSES/BSD-2-Clause.txt` & `sp_variant-3.2.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `sp-variant-3.1.2/PKG-INFO` & `sp_variant-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sp-variant
-Version: 3.1.2
+Version: 3.2.0
 Summary: Detect the Linux distribution for the StorPool build system
-Author-email: StorPool <support@storpool.com>
-License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/storpool/sp-variant
 Project-URL: Changelog, https://github.com/storpool/sp-variant/blob/main/docs/changes.md
+Author-email: StorPool <support@storpool.com>
+License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: DFSG approved
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sp-variant-3.1.2/README.md` & `sp_variant-3.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sp-variant-3.1.2/data/debian/repo/storpool-keyring.gpg` & `sp_variant-3.2.0/data/debian/repo/storpool-keyring.gpg`

 * *Files identical despite different names*

### Comparing `sp-variant-3.1.2/data/redhat/repo/RPM-GPG-KEY-StorPool` & `sp_variant-3.2.0/data/redhat/repo/RPM-GPG-KEY-StorPool`

 * *Files identical despite different names*

### Comparing `sp-variant-3.1.2/data/redhat/repo/storpool-centos.repo` & `sp_variant-3.2.0/data/redhat/repo/storpool-centos.repo`

 * *Files identical despite different names*

### Comparing `sp-variant-3.1.2/docs/changes.md` & `sp_variant-3.2.0/docs/changes.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,85 @@
 SPDX-License-Identifier: BSD-2-Clause
 -->
 
 # Changelog
 
 All notable changes to the sp-variant project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.2.0] - 2023-07-06
+
+### Fixes
+
+- data:
+    - drop the `Architectures` line from the Debian sources list file so that
+      `add-storpool-repo` can also be used on arm64 hosts
+    - mark Debian 9.x (stretch) as no longer supported
+    - drop the `mcelog` package definition for Debian, it was only ever
+      present in the unsupported Debian 9.x and Ubuntu 16.04
+    - refer to the OpenSSL 3.x package for Debian unstable and Ubuntu 22.04
+    - reflect the removal of the `libcgroup-tools` and `python2-simplejson`
+      packages in CentOS 9.x
+    - add a 0644 default to the `--mode` argument of `sp_build_repo.subst`
+- python:
+    - add a no-op `_diag_to_stderr` property setter to avoid mypy errors on
+      (wrong, deprecated) attempts to set that field. Those attempts are
+      ignored anyway since the changes in version 3.1.2, but let mypy know
+      that they are still not completely forbidden.
+
+### Additions
+
+- data:
+    - add Debian 12.x (bookworm), mark Debian unstable as Debian 13.x (trixie)
+    - add Ubuntu 23.04 (Lunar Lobster) as an unsupported variant
+- docs:
+    - add a raw Python API reference
+- python:
+    - install the OS packages defined for each variant during the Docker test
+- rust:
+    - add the `get_all_variants()` and `get_all_variants_in_order()`
+      functions that return all known StorPool build variants
+    - derive `Copy` for some structs and enums
+    - derive `PartialEq` and `Eq` for most structs
+    - allow the Makefile Rust build infrastructure to not pass the `--offline`
+      option to Cargo if the `NO_CARGO_OFFLINE` environment variable is set
+    - run the Cargo tests in the Makefile `test` target
+
+### Other changes
+
+- data:
+    - drop the definitions for the temporary, intermediate, non-LTS
+      Ubuntu 21.10 version
+- docs:
+    - point to version 1.1.0 of the "Keep a Changelog" specification
+- python:
+    - switch from `setuptools` to `hatchling` for the PEP 517 build
+    - use Ruff 0.0.277 in the test suite:
+        - override some checks related to the use of the `subprocess` library
+        - override a "too many parameters" check for the click-decorated main
+          function of `sp_build_repo`
+        - globally disable the "performance penalty for try/except in loops" check;
+          we want our exceptions to provide as much context as possible, including
+          the values of the loop variables
+    - pin the Ruff version to avoid failures due to newly-added future checks
+    - use Ruff's isort implementation to format the source files and
+      rename the `black` and `black-reformat` Tox testing environments to
+      `format` and `reformat` respectively
+    - hide some imports behind `TYPE_CHECKING` checks
+    - use `ClassVar` as needed for singleton data holder classes
+    - narrow down the "run Ruff" stage specification in the `test-stages` definition
+    - drop the `flake8` and `pylint` Tox test environments, rely on Ruff
+    - use `click.Path` in `sp_build_repo` and `test_docker`
+- rust:
+    - import the `VariantError` struct directly in the test suite
+
 ## [3.1.2] - 2023-03-17
 
 ### Semi-incompatible changes
 
 - python:
     - deprecate the `defs.Config._diag_to_stderr` member variable;
       replace it with a read-only property that always returns true and
@@ -358,15 +424,16 @@
 
 ## [1.3.0] - 2021-09-15
 
 ### Started
 
 - First public release.
 
-[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.1.2...main
+[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.2.0...main
+[3.2.0]: https://github.com/storpool/sp-variant/compare/release/3.1.2...release/3.2.0
 [3.1.2]: https://github.com/storpool/sp-variant/compare/release/3.1.1...release/3.1.2
 [3.1.1]: https://github.com/storpool/sp-variant/compare/release/3.1.0...release/3.1.1
 [3.1.0]: https://github.com/storpool/sp-variant/compare/release/3.0.0...release/3.1.0
 [3.0.0]: https://github.com/storpool/sp-variant/compare/release/2.3.3...release/3.0.0
 [2.3.3]: https://github.com/storpool/sp-variant/compare/release/2.3.2...release/2.3.3
 [2.3.2]: https://github.com/storpool/sp-variant/compare/release/2.3.1...release/2.3.2
 [2.3.1]: https://github.com/storpool/sp-variant/compare/release/2.3.0...release/2.3.1
```

### Comparing `sp-variant-3.1.2/docs/index.md` & `sp_variant-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sp-variant-3.1.2/mkdocs.yml` & `sp_variant-3.2.0/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,25 @@
 repo_name: sp-variant
 site_author: storpool
 site_url: https://storpool.com/
 site_dir: site/docs
 nav:
   - 'index.md'
   - 'Changelog': 'changes.md'
+  - 'API Reference': 'api.md'
 markdown_extensions:
   - toc:
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.inlinehilite:
   - pymdownx.superfences:
 plugins:
   - mkdocstrings:
       handlers:
         python:
-          paths: [src]
+          paths: [python]
           options:
             heading_level: 3
             show_root_heading: true
   - search
 watch:
   - 'python/sp_variant'
```

### Comparing `sp-variant-3.1.2/python/config/ruff-base/pyproject.toml` & `sp_variant-3.2.0/python/config/ruff-base/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -20,31 +20,45 @@
 
   # The multi-line docstring summary starts on the same line
   "D213",
 
   # Too restrictive.
   "EM",
 
-  # We have different ideas about the ordering of the typing classes.
-  "I",
+  # We want to report exceptions with as much context as possible.
+  "PERF203",
 
   # Maybe we shall fix the use of magic values... some sunny day.
   "PLR2004",
 
   # Too restrictive for now.
   "TRY003",
 ]
 
+[tool.ruff.isort]
+force-single-line = true
+known-first-party = ["sp_build_repo", "sp_variant", "test_docker"]
+lines-after-imports = 2
+single-line-exclusions = ["defs", "typing"]
+
 [tool.ruff.per-file-ignores]
 # This is a command-line tool. Console output is part of its task.
 # Also, it needs to be able to run typedload on Python < 3.10, so it cannot
 # leverage the full power of X | Y unions, X | None optional values, etc.
-"*/sp_build_repo/__main__.py" = ["T201", "UP006", "UP007"]
+# We also make sure to use `subprocess` responsibly.
+"*/sp_build_repo/__main__.py" = ["S603", "S607", "T201", "UP006", "UP007"]
 
 # This is a command-line tool. Console output is part of its task.
-"*/sp_variant/__main__.py" = ["T201"]
+# We also make sure to use `subprocess` responsibly.
+"*/sp_variant/__main__.py" = ["S603", "S607", "T201"]
+
+# We only run commands defined in our variants structure.
+"*/sp_variant/variant.py" = ["S603", "S607"]
 
 # The "update a named tuple / dictionary functions need to use typing.Any.
 "*/sp_variant/vbuild.py" = ["ANN401"]
 
+# We make sure to use `subprocess` responsibly.
+"*/test_docker/__main__.py" = ["S603", "S607"]
+
 # This is a test suite.
 "*/unit_tests/*.py" = ["S101", "T201"]
```

### Comparing `sp-variant-3.1.2/python/sp_build_repo/__main__.py` & `sp_variant-3.2.0/python/sp_build_repo/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Build the "add StorPool repository" archive."""
 
 from __future__ import annotations
 
 import dataclasses
-import functools
 import datetime
+import functools
 import pathlib
 import shutil
 import subprocess
 import sys
-
-from typing import Dict, Final, Optional
+from typing import TYPE_CHECKING, Dict, Optional
 
 import cfg_diag
 import click
 import jinja2
 import typedload.dataloader
 
 from sp_variant import defs
 from sp_variant import variant
 from sp_variant import vbuild
 
+
+if TYPE_CHECKING:
+    from typing import ClassVar, Final
+
+
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 
 @dataclasses.dataclass
@@ -95,16 +99,16 @@
     overrides: Overrides
     runtime: pathlib.Path
 
 
 class Singles:
     """Keep some singleton objects in a controlled way."""
 
-    _jinja2_env: dict[str, jinja2.Environment] = {}
-    _jinja2_loaders: dict[str, jinja2.BaseLoader] = {}
+    _jinja2_env: ClassVar[dict[str, jinja2.Environment]] = {}
+    _jinja2_loaders: ClassVar[dict[str, jinja2.BaseLoader]] = {}
 
     @classmethod
     def jinja2_env(cls, path: pathlib.Path) -> jinja2.Environment:
         """Instantiate a Jinja2 environment if necessary."""
         if (abspath := str(path.absolute())) in cls._jinja2_env:
             return cls._jinja2_env[abspath]
 
@@ -312,15 +316,14 @@
 
 @functools.lru_cache(maxsize=2)
 def typed_loader(*, failonextra: bool = False) -> typedload.dataloader.Loader:
     """Prepare a loader that can parse annotated types."""
     return typedload.dataloader.Loader(pep563=True, failonextra=failonextra)
 
 
-# pylint: disable-next=too-complex
 def parse_overrides(path: pathlib.Path) -> Overrides:
     """Parse the TOML overrides file."""
     if path is None:
         return Overrides(repo={})
 
     try:
         raw: Final = tomllib.loads(path.read_text(encoding="UTF-8"))
@@ -347,55 +350,83 @@
         sys.exit(f"Invalid format for the {path} overrides file: {err}")
 
 
 @click.command(name="build")
 @click.option(
     "-d",
     "--datadir",
-    type=pathlib.Path,
+    type=click.Path(
+        exists=True,
+        file_okay=False,
+        dir_okay=True,
+        writable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
     required=True,
     help="The directory to place the repo file in",
 )
 @click.option(
     "-D",
     "--destdir",
-    type=pathlib.Path,
+    type=click.Path(
+        exists=True,
+        file_okay=False,
+        dir_okay=True,
+        writable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
     required=True,
     help="The directory to place the repo file in",
 )
 @click.option(
     "-o",
     "--overrides",
-    type=pathlib.Path,
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
     help="The path to a TOML configuration overrides file",
 )
 @click.option(
     "-r",
     "--runtime",
-    type=pathlib.Path,
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        executable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
     required=True,
     help="The storpool_variant executable to use",
 )
 @click.option(
     "--no-date",
     is_flag=True,
     help="Do not include the current date in the directory name",
 )
 @click.pass_context
-def cmd_build(
+def cmd_build(  # noqa: PLR0913
     ctx: click.Context,
     *,
     datadir: pathlib.Path,
     destdir: pathlib.Path,
     overrides: pathlib.Path,
     runtime: pathlib.Path,
     no_date: bool,
 ) -> None:
     """Build the StorPool repository archive and output its name."""
-    # pylint: disable=too-many-arguments
     cfg_hold: Final = ctx.find_object(ConfigHolder)
     assert isinstance(cfg_hold, ConfigHolder)  # noqa: S101  # mypy needs this
     cfg: Final = Config(
         datadir=datadir,
         destdir=destdir,
         no_date=no_date,
         overrides=parse_overrides(overrides),
@@ -419,8 +450,8 @@
     ctx.obj.verbose = verbose
 
 
 main.add_command(cmd_build)
 
 
 if __name__ == "__main__":
-    main()  # pylint: disable=no-value-for-parameter,missing-kwoa
+    main()
```

### Comparing `sp-variant-3.1.2/python/sp_build_repo/subst.py` & `sp_variant-3.2.0/python/sp_build_repo/subst.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,41 @@
 # SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Substitute variant data using Jinja2 templates."""
 
 from __future__ import annotations
 
-import argparse
 import dataclasses
 import functools
 import json
 import pathlib
-
-from typing import Final
+import typing
 
 import cfg_diag
+import click
 import jinja2
 import trivver
 
 from sp_variant import defs
 from sp_variant import variant
 
 
+if typing.TYPE_CHECKING:
+    from typing import Final
+
+
 @dataclasses.dataclass(frozen=True)
 class Config(cfg_diag.Config):
     """Runtime configuration for the variant substitution tool."""
 
     output: pathlib.Path
     output_mode: int
     template: pathlib.Path
 
 
-def parse_args() -> Config:
-    """Parse the command-line arguments."""
-    parser: Final = argparse.ArgumentParser(prog="sp_var_subst")
-    parser.add_argument(
-        "-m",
-        "--mode",
-        type=lambda value: int(value, 8),
-        help="the octal permissions mode of the output file",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=pathlib.Path,
-        required=True,
-        help="the output file to generate",
-    )
-    parser.add_argument(
-        "-t",
-        "--template",
-        type=pathlib.Path,
-        required=True,
-        help="the template to render",
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="verbose operation; display diagnostic messages",
-    )
-
-    args: Final = parser.parse_args()
-
-    return Config(
-        output=args.output,
-        output_mode=args.mode,
-        template=args.template,
-        verbose=args.verbose,
-    )
-
-
 def regex_un_x(value: str) -> str:
     """Un-re.X a regular expression... somewhat."""
     return (
         value.replace(" ", "")
         .replace("\t", "")
         .replace("\n", "")
         .replace("\\s", "[[:space:]]")
@@ -138,15 +101,79 @@
     cfg.diag(lambda: f"Generating the {cfg.output} output file")
     cfg.output.write_text(result, encoding="UTF-8")
     cfg.output.chmod(cfg.output_mode)
 
     cfg.diag(lambda: f"Rendered {cfg.template} into {cfg.output}")
 
 
-def main() -> None:
+class OctalInteger(click.ParamType):
+    """Convert a string value to an integer using base 8."""
+
+    name = "octal"
+
+    def convert(
+        self, value: str | int, param: click.Parameter | None, ctx: click.Context | None
+    ) -> int:
+        """Convert a string to an integer using base 8."""
+        if isinstance(value, int):
+            return value
+
+        try:
+            return int(value, 8)
+        except ValueError as err:
+            self.fail(f"{value!r} is not a valid integer: {err}", param, ctx)
+
+
+OCTAL_INTEGER: Final = OctalInteger()
+
+
+@click.command(name="subst")
+@click.option(
+    "-m",
+    "--mode",
+    type=OCTAL_INTEGER,
+    default=0o644,
+    help="the octal permissions mode of the output file",
+)
+@click.option(
+    "-o",
+    "--output",
+    type=click.Path(
+        dir_okay=False, file_okay=True, writable=True, resolve_path=True, path_type=pathlib.Path
+    ),
+    required=True,
+    help="the output file to generate",
+)
+@click.option(
+    "-t",
+    "--template",
+    type=click.Path(
+        exists=True,
+        dir_okay=False,
+        file_okay=True,
+        readable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
+    required=True,
+    help="the template to render",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    type=bool,
+    is_flag=True,
+    help="verbose operation; display diagnostic messages",
+)
+def main(*, mode: int, output: pathlib.Path, template: pathlib.Path, verbose: bool) -> None:
     """Parse command-line arguments, substitute data."""
-    cfg: Final = parse_args()
+    cfg: Final = Config(
+        output=output,
+        output_mode=mode,
+        template=template,
+        verbose=verbose,
+    )
     substitute(cfg)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sp-variant-3.1.2/python/sp_variant/__main__.py` & `sp_variant-3.2.0/python/sp_variant/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 import argparse
 import json
 import pathlib
 import shlex
 import subprocess
 import sys
-
-from typing import Any, Callable, Final, TYPE_CHECKING
+import typing
 
 from . import defs
 from . import variant
 from . import vbuild
 
 
-if TYPE_CHECKING:
-    # pylint: disable-next=protected-access,invalid-name
+if typing.TYPE_CHECKING:
+    from typing import Any, Callable, Final
+
     SubPAction: Final = argparse._SubParsersAction[argparse.ArgumentParser]  # noqa: SLF001
 
 
 CMD_LIST_BRIEF: Final = [
     ("pkgfile", "install"),
 ]
```

### Comparing `sp-variant-3.1.2/python/sp_variant/defs.py` & `sp_variant-3.2.0/python/sp_variant/defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # SPDX-License-Identifier: BSD-2-Clause
 """Common definitions for the OS/distribution variant detection library."""
 
 from __future__ import annotations
 
 import dataclasses
 import sys
+from typing import TYPE_CHECKING, NamedTuple
 
-from typing import Any, Final, NamedTuple, Pattern, TYPE_CHECKING
 
 if TYPE_CHECKING:
     import pathlib
+    from typing import Any, Final, Pattern
 
 
 class Detect(NamedTuple):
     """Where (and what for) to look when figuring out which variant this is."""
 
     filename: str
     regex: Pattern[str]
@@ -122,15 +123,15 @@
     """Attributes common to a StorPool package repository."""
 
     name: str
     extension: str
     url: str
 
 
-VERSION: Final = "3.1.2"
+VERSION: Final = "3.2.0"
 FORMAT_VERSION: Final = (1, 4)
 
 REPO_TYPES: Final = [
     RepoType(name="contrib", extension="", url="https://repo.storpool.com/public/"),
     RepoType(
         name="staging",
         extension="-staging",
@@ -152,16 +153,14 @@
     """Invalid parameters passed to the variant routines."""
 
 
 @dataclasses.dataclass(frozen=True)
 class Config:
     """Runtime configuration for the sp-variant library functions."""
 
-    # pylint: disable=too-many-instance-attributes
-
     args: list[str] | None = None
     command: str | None = None
     noop: bool = False
     repodir: pathlib.Path | None = None
     repotype: RepoType = REPO_TYPES[0]
     verbose: bool = False
 
@@ -171,26 +170,29 @@
             print(msg, file=sys.stderr)  # noqa: T201
 
     @property
     def _diag_to_stderr(self) -> bool:
         """We always send the diagnostic messages to stderr now."""
         return True
 
+    @_diag_to_stderr.setter
+    def _diag_to_stderr(self, value: bool) -> None:
+        """Simulate setting the property, do nothing instead."""
+
     # OK, this is a bit ugly. It's going away soon.
     def _do_setattr(self, name: str, value: Any) -> None:  # noqa: ANN401
         """Ignore any attempts to set the `_diag_to_stderr` member."""
         if name == "_diag_to_stderr":
             return
 
         _config_orig_setattr(self, name, value)
 
 
 # Let us not do this ever again.
 _config_orig_setattr = Config.__setattr__
-# pylint: disable-next=protected-access
 Config.__setattr__ = Config._do_setattr  # type: ignore[method-assign,assignment]
 
 
 def jsonify(obj: Any) -> Any:  # noqa: ANN401  # this needs to operate on, well, anything
     """Return a more readable representation of an object."""
     if type(obj).__name__.endswith("Pattern") and hasattr(obj, "pattern"):
         return jsonify(obj.pattern)
```

### Comparing `sp-variant-3.1.2/python/sp_variant/variant.py` & `sp_variant-3.2.0/python/sp_variant/variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 
 from __future__ import annotations
 
 import errno
 import pathlib
 import shlex
 import subprocess
-
-from typing import Final, Iterable
+import typing
 
 from . import defs
 from . import vbuild
 from . import yaiparser
-
 from .defs import (
+    VERSION,
     Config,
     Variant,
     VariantError,
-    VERSION,
 )
-
 from .vbuild import update_namedtuple
 
 
+if typing.TYPE_CHECKING:
+    from typing import Final, Iterable
+
+
 class VariantKeyError(VariantError):
     """A variant with an unknown name was requested."""
 
 
 class VariantFileError(VariantError):
     """A filesystem-related error occurred."""
 
@@ -82,15 +83,15 @@
 
 
 def _detect_from_files(cfg: Config) -> Variant | None:
     """Try to match the contents of some variant-specific files."""
     cfg.diag("Trying non-os-release-based heuristics")
     for var in vbuild.DETECT_ORDER:
         cfg.diag(f"- trying {var.name}")
-        try:  # pylint: disable=too-many-try-statements
+        try:
             cfg.diag(f"  - {var.detect.filename}")
             for line in pathlib.Path(var.detect.filename).read_text(encoding=SAFEENC).splitlines():
                 if var.detect.regex.match(line):
                     cfg.diag(f"  - found it: {line}")
                     return var
         except OSError as err:
             if err.errno != errno.ENOENT:
```

### Comparing `sp-variant-3.1.2/python/sp_variant/vbuild.py` & `sp_variant-3.2.0/python/sp_variant/vbuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,45 @@
 # SPDX-License-Identifier: BSD-2-Clause
 """Build the hierarchical structure of variant definitions."""
 
 from __future__ import annotations
 
 import pathlib
 import re
-
-from typing import Any, Callable, Final, NamedTuple, TypeVar
+from typing import TYPE_CHECKING, NamedTuple
 
 from . import defs
 
-CMD_NOOP: Final[list[str]] = ["true"]
 
-_TNamedTuple = TypeVar("_TNamedTuple", bound=NamedTuple)  # pylint: disable=invalid-name
+if TYPE_CHECKING:
+    from typing import Any, Callable, Final, TypeVar
+
+    _TNamedTuple = TypeVar("_TNamedTuple", bound=NamedTuple)
+
+
+CMD_NOOP: Final[list[str]] = ["true"]
 
 _VARIANT_DEF: Final[list[defs.Variant | defs.VariantUpdate]] = [
     defs.Variant(
-        name="DEBIAN12",
-        descr="Debian 12.x (bookworm/unstable)",
+        name="DEBIAN13",
+        descr="Debian 13.x (trixie/unstable)",
         parent="",
         family="debian",
         detect=defs.Detect(
             filename="/etc/os-release",
             regex=re.compile(
                 r"""^
                     PRETTY_NAME= .*
                     Debian \s+ GNU/Linux \s+
-                    (?: bookworm | 12 ) (?: \s | / )
+                    (?: trixie | 13 ) (?: \s | / )
                 """,
                 re.X,
             ),
             os_id="debian",
-            os_version_regex=re.compile(r"^12$"),
+            os_version_regex=re.compile(r"^13$"),
         ),
         supported=defs.Supported(repo=False),
         commands=defs.Commands(
             package=defs.CommandsPackage(
                 update_db=["apt-get", "-q", "-y", "update"],
                 install=[
                     "env",
@@ -107,29 +111,56 @@
         ),
         package={
             "BINDINGS_PYTHON": "python3",
             "BINDINGS_PYTHON_CONFGET": "python3-confget",
             "BINDINGS_PYTHON_SIMPLEJSON": "python3-simplejson",
             "CGROUP": "cgroup-tools",
             "CPUPOWER": "linux-cpupower",
-            "LIBSSL": "libssl1.1",
-            "MCELOG": "mcelog",
+            "LIBSSL": "libssl3",
+            "MCELOG": "bash",
         },
         systemd_lib="lib/systemd/system",
         file_ext="deb",
         initramfs_flavor="update-initramfs",
         builder=defs.Builder(
-            alias="debian12",
+            alias="debian13",
             base_image="debian:unstable",
             branch="debian/unstable",
             kernel_package="linux-headers",
             utf8_locale="C.UTF-8",
         ),
     ),
     defs.VariantUpdate(
+        name="DEBIAN12",
+        descr="Debian 12.x (bookworm)",
+        parent="DEBIAN13",
+        detect=defs.Detect(
+            filename="/etc/os-release",
+            regex=re.compile(
+                r"""^
+                    PRETTY_NAME= .*
+                    Debian \s+ GNU/Linux \s+
+                    (?: bookworm | 12 ) (?: \s | / )
+                """,
+                re.X,
+            ),
+            os_id="debian",
+            os_version_regex=re.compile(r"^12$"),
+        ),
+        updates={
+            "supported": {"repo": True},
+            "repo": {"codename": "bookworm"},
+            "builder": {
+                "alias": "debian12",
+                "base_image": "debian:bookworm",
+                "branch": "debian/bookworm",
+            },
+        },
+    ),
+    defs.VariantUpdate(
         name="DEBIAN11",
         descr="Debian 11.x (bullseye)",
         parent="DEBIAN12",
         detect=defs.Detect(
             filename="/etc/os-release",
             regex=re.compile(
                 r"""^
@@ -141,14 +172,17 @@
             ),
             os_id="debian",
             os_version_regex=re.compile(r"^11$"),
         ),
         updates={
             "supported": {"repo": True},
             "repo": {"codename": "bullseye"},
+            "package": {
+                "LIBSSL": "libssl1.1",
+            },
             "builder": {
                 "alias": "debian11",
                 "base_image": "debian:bullseye",
                 "branch": "debian/bullseye",
             },
         },
     ),
@@ -200,98 +234,102 @@
                 """,
                 re.X,
             ),
             os_id="debian",
             os_version_regex=re.compile(r"^9$"),
         ),
         updates={
+            "supported": {"repo": False},
             "repo": {
                 "codename": "stretch",
                 "req_packages": ["apt-transport-https", "ca-certificates"],
             },
             "builder": {
                 "alias": "debian9",
                 "base_image": "debian:stretch",
                 "branch": "debian/stretch",
             },
         },
     ),
     defs.VariantUpdate(
-        name="UBUNTU2204",
-        descr="Ubuntu 22.04 LTS (Jammy Jellyfish)",
+        name="UBUNTU2304",
+        descr="Ubuntu 23.04 LTS (Lunar Lobster)",
         parent="DEBIAN12",
         detect=defs.Detect(
             filename="/etc/os-release",
             regex=re.compile(
-                r"^ PRETTY_NAME= .* (?: Ubuntu \s+ 22 \. 04 | Mint \s+ 21 ) ",
+                r"^ PRETTY_NAME= .* Ubuntu \s+ 23 \. 04 ",
                 re.X,
             ),
             os_id="ubuntu",
-            os_version_regex=re.compile(r"^22\.04$"),
+            os_version_regex=re.compile(r"^23\.04$"),
         ),
         updates={
-            "supported": {"repo": True},
             "repo": {
                 "vendor": "ubuntu",
-                "codename": "jammy",
+                "codename": "lunar",
             },
             "package": {
                 "CPUPOWER": "linux-tools-generic",
-                "MCELOG": "bash",
             },
             "builder": {
-                "alias": "ubuntu-22.04",
-                "base_image": "ubuntu:jammy",
-                "branch": "ubuntu/jammy",
+                "alias": "ubuntu-23.04",
+                "base_image": "ubuntu:lunar",
+                "branch": "ubuntu/lunar",
             },
         },
     ),
     defs.VariantUpdate(
-        name="UBUNTU2110",
-        descr="Ubuntu 21.10 LTS (Impish Indri)",
-        parent="UBUNTU2204",
+        name="UBUNTU2204",
+        descr="Ubuntu 22.04 LTS (Jammy Jellyfish)",
+        parent="UBUNTU2304",
         detect=defs.Detect(
             filename="/etc/os-release",
             regex=re.compile(
-                r"^ PRETTY_NAME= .* (?: Ubuntu \s+ 21 \. 10 ) ",
+                r"^ PRETTY_NAME= .* (?: Ubuntu \s+ 22 \. 04 | Mint \s+ 21 ) ",
                 re.X,
             ),
             os_id="ubuntu",
-            os_version_regex=re.compile(r"^21\.10$"),
+            os_version_regex=re.compile(r"^22\.04$"),
         ),
         updates={
+            "supported": {"repo": True},
             "repo": {
                 "vendor": "ubuntu",
-                "codename": "impish",
+                "codename": "jammy",
             },
             "builder": {
-                "alias": "ubuntu-21.10",
-                "base_image": "ubuntu:impish",
-                "branch": "ubuntu/impish",
+                "alias": "ubuntu-22.04",
+                "base_image": "ubuntu:jammy",
+                "branch": "ubuntu/jammy",
             },
         },
     ),
     defs.VariantUpdate(
         name="UBUNTU2004",
         descr="Ubuntu 20.04 LTS (Focal Fossa)",
-        parent="UBUNTU2110",
+        parent="UBUNTU2204",
         detect=defs.Detect(
             filename="/etc/os-release",
             regex=re.compile(
                 r"^ PRETTY_NAME= .* (?: Ubuntu \s+ 20 \. 04 | Mint \s+ 20 ) ",
                 re.X,
             ),
             os_id="ubuntu",
             os_version_regex=re.compile(r"^20\.04$"),
         ),
         updates={
+            "supported": {"repo": True},
             "repo": {
                 "vendor": "ubuntu",
                 "codename": "focal",
             },
+            "package": {
+                "LIBSSL": "libssl1.1",
+            },
             "min_sys_python": "3.8",
             "builder": {
                 "alias": "ubuntu-20.04",
                 "base_image": "ubuntu:focal",
                 "branch": "ubuntu/focal",
             },
         },
@@ -431,33 +469,33 @@
 
 if [ -n "$to_install" ]; then
     dnf install -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib --setopt=localpkg_gpgcheck=0 -- $to_install
 fi
 if [ -n "$to_reinstall" ]; then
     dnf reinstall -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib --setopt=localpkg_gpgcheck=0 -- $to_reinstall
 fi
-""",  # noqa: E501  pylint: disable=line-too-long
+""",  # noqa: E501
                 ],
             ),
         ),
         min_sys_python="2.7",
         repo=defs.YumRepo(
             yumdef="redhat/repo/storpool-centos.repo",
             keyring="redhat/repo/RPM-GPG-KEY-StorPool",
         ),
         package={
             "KMOD": "kmod",
-            "LIBCGROUP": "libcgroup-tools",
+            "LIBCGROUP": "bash",
             "LIBUDEV": "systemd-libs",
             "OPENSSL": "openssl-libs",
             "PERL_AUTODIE": "perl-autodie",
             "PERL_FILE_PATH": "perl-File-Path",
             "PERL_LWP_PROTO_HTTPS": "perl-LWP-Protocol-https",
             "PERL_SYS_SYSLOG": "perl-Sys-Syslog",
-            "PYTHON_SIMPLEJSON": "python2-simplejson",
+            "PYTHON_SIMPLEJSON": "bash",
             "PROCPS": "procps-ng",
             "UDEV": "systemd",
         },
         systemd_lib="usr/lib/systemd/system",
         file_ext="rpm",
         initramfs_flavor="mkinitrd",
         builder=defs.Builder(
@@ -476,14 +514,18 @@
             filename="/etc/redhat-release",
             regex=re.compile(r"^ AlmaLinux \s .* \s 8 \. (?: [4-9] | [1-9][0-9] )", re.X),
             os_id="alma",
             os_version_regex=re.compile(r"^8(?:$|\.[4-9]|\.[1-9][0-9])"),
         ),
         updates={
             "supported": {"repo": True},
+            "package": {
+                "LIBCGROUP": "libcgroup-tools",
+                "PYTHON_SIMPLEJSON": "python2-simplejson",
+            },
             "commands": {
                 "package": {
                     "install": [
                         "dnf",
                         "--disablerepo=*",
                         "--enablerepo=appstream",
                         "--enablerepo=baseos",
@@ -512,15 +554,15 @@
 
 if [ -n "$to_install" ]; then
     dnf install -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib,powertools --setopt=localpkg_gpgcheck=0 -- $to_install
 fi
 if [ -n "$to_reinstall" ]; then
     dnf reinstall -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib,powertools --setopt=localpkg_gpgcheck=0 -- $to_reinstall
 fi
-""",  # noqa: E501  pylint: disable=line-too-long
+""",  # noqa: E501
                     ],
                 },
             },
             "builder": {
                 "alias": "alma8",
                 "base_image": "almalinux:8",
                 "branch": "",
@@ -584,15 +626,15 @@
 
 if [ -n "$to_install" ]; then
     yum install -y --disablerepo='*' --enablerepo=base,updates,storpool-contrib --setopt=localpkg_gpgcheck=0 -- $to_install
 fi
 if [ -n "$to_reinstall" ]; then
     yum reinstall -y --disablerepo='*' --enablerepo=base,updates,storpool-contrib --setopt=localpkg_gpgcheck=0 -- $to_reinstall
 fi
-""",  # noqa: E501  pylint: disable=line-too-long
+""",  # noqa: E501
                     ],
                 },
             },
             "builder": {
                 "alias": "centos7",
                 "base_image": "centos:7",
                 "branch": "centos/7",
@@ -699,15 +741,15 @@
 
 if [ -n "$to_install" ]; then
     dnf install -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib,codeready-builder-for-rhel-8-x86_64-rpms --setopt=localpkg_gpgcheck=0 -- $to_install
 fi
 if [ -n "$to_reinstall" ]; then
     dnf reinstall -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib,codeready-builder-for-rhel-8-x86_64-rpms --setopt=localpkg_gpgcheck=0 -- $to_reinstall
 fi
-""",  # noqa: E501  pylint: disable=line-too-long
+""",  # noqa: E501
                     ]
                 },
             },
             "builder": {
                 "alias": "rhel8",
                 "base_image": "redhat/ubi8:reg",
                 "branch": "",
@@ -893,9 +935,8 @@
             else var
         )
         VARIANTS[var.name] = current
         order.append(var.name)
 
     order.reverse()
     DETECT_ORDER.extend([VARIANTS[name] for name in order])
-    # pylint: disable-next=consider-using-f-string
     cfg.diag("Detect order: {names}".format(names=" ".join(var.name for var in DETECT_ORDER)))
```

### Comparing `sp-variant-3.1.2/python/sp_variant/yaiparser.py` & `sp_variant-3.2.0/python/sp_variant/yaiparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 # SPDX-License-Identifier: BSD-2-Clause
 """Yet Another INI-style-file Parser."""
 
 from __future__ import annotations
 
 import pathlib
 import re
-
-from typing import Final
+import typing
 
 from . import defs
 
 
+if typing.TYPE_CHECKING:
+    from typing import Final
+
+
 class VariantYAIError(defs.VariantError):
     """An error that occurred while parsing an INI-like file."""
 
 
 _RE_YAIP_LINE = re.compile(
     r"""
     ^ (?:
@@ -76,15 +79,14 @@
             )
 
         return (varname, quoted)
 
     def _parse_line_unquoted(self, line: str, varname: str, quoted: str) -> tuple[str, str] | None:
         """Escape any characters preceded by a backslash."""
         res = ""
-        # pylint: disable-next=while-used
         while quoted:
             try:
                 idx = quoted.index("\\")
             except ValueError:
                 res += quoted
                 break
```

### Comparing `sp-variant-3.1.2/python/test_docker/__main__.py` & `sp_variant-3.2.0/python/test_docker/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 import asyncio.subprocess as aprocess
 import dataclasses
 import json
 import pathlib
 import subprocess
 import sys
 import tempfile
-
-from typing import Final, NamedTuple
+from typing import TYPE_CHECKING, NamedTuple
 
 import cfg_diag
 import click
 import utf8_locale
 
 
+if TYPE_CHECKING:
+    from typing import Final
+
+
 @dataclasses.dataclass(frozen=True)
 class Config(cfg_diag.Config):
     """Runtime configuration for the Docker test runner."""
 
     images_filter: tuple[str, ...]
     repo_file: pathlib.Path
     utf8_env: dict[str, str]
@@ -128,28 +131,27 @@
 ) -> tuple[bytes | None, list[str]]:
     """Read the lines output by `storpool_variant detect`, see if they look okay."""
     assert proc.stdout is not None  # noqa: S101  # mypy needs this
 
     first_line = None
     rest = b""
     errors: Final = []
-    try:  # pylint: disable=too-many-try-statements
+    try:
         try:
             first_line = await proc.stdout.readline()
-        except Exception as err:  # pylint: disable=broad-except  # noqa: BLE001
+        except Exception as err:  # noqa: BLE001
             errors.append(f"Could not read the first line: {err}")
         cfg.diag(lambda: f"{image}: first line {first_line!r}")
 
         if first_line:
             first_line = first_line.rstrip(b"\n")
-            # pylint: disable-next=while-used
             while True:
                 try:
                     more = await proc.stdout.readline()
-                except Exception as err:  # pylint: disable=broad-except  # noqa: BLE001
+                except Exception as err:  # noqa: BLE001
                     errors.append(f"Could not read a further line: {err}")
                     break
                 cfg.diag(lambda: f"{image}: more {more!r}")  # noqa: B023
 
                 if not more:
                     break
                 rest += b"\n" + more.rstrip(b"\n")
@@ -270,15 +272,14 @@
     assert proc.stdout is not None  # noqa: S101  # mypy needs this
     assert proc.stderr is not None  # noqa: S101  # mypy needs this
 
     async def read_stream(stype: str, stream: asyncio.StreamReader) -> bytes:
         """Read lines from a stream, output them, gather them."""
         cfg.diag(lambda: f"{image}: waiting for {stype} lines")
         res = b""
-        # pylint: disable-next=while-used
         while True:
             if not (line := await stream.readline()):
                 cfg.diag(lambda: f"{image}: no more {stype}")
                 break
 
             cfg.diag(lambda: f"{image}: read a {stype} line: {line!r}")
             res += line
@@ -350,18 +351,23 @@
     fi
 }
 
 # Make sure LC_ALL is set to a valid UTF-8-capable locale
 echo 'Checking whether LC_ALL specifies a valid UTF-8-capable locale'
 check_locale 'The LC_ALL environment variable' "$LC_ALL"
 
+tempf="$(mktemp -t current-variant.json.XXXXXX)"
+trap "rm -f -- '$tempf'" HUP INT TERM EXIT
+echo "Stashing the `sp_variant show current` output into $tempf"
+/sp/storpool_variant show current > "$tempf"
+
 # Parsing JSON without jq? Yeah, sure, why not...
 echo 'Checking for a Debian-like variant'
 unset is_debian
-if /sp/storpool_variant show current | tr "\n" ' ' | grep -Eqe '"family"[[:space:]]*:[[:space:]]*"debian"'; then
+if tr "\n" ' ' < "$tempf" | grep -Eqe '"family"[[:space:]]*:[[:space:]]*"debian"'; then
     is_debian=1
     echo 'Running apt-get update'
     apt-get update
 elif [ "$(/sp/storpool_variant detect)" = 'CENTOS8' ]; then
     echo 'Running dnf swap centos-linux-repos centos-stream-repos'
     dnf --disablerepo '*' --enablerepo extras -y swap centos-linux-repos centos-stream-repos
 else
@@ -371,19 +377,19 @@
 echo 'Running add-storpool-repo'
 /sp/add-storpool-repo.sh
 
 echo 'Installing jq'
 /sp/storpool_variant command run -- package.install jq
 
 echo 'Checking whether builder.utf8_locale specifies a valid UTF-8-capable locale'
-u8loc="$(/sp/storpool_variant show current | jq -r '.variant.builder.utf8_locale')"
+u8loc="$(jq -r '.variant.builder.utf8_locale' < "$tempf")"
 check_locale 'The builder.utf8_locale setting' "$u8loc"
 
 echo 'Checking whether StorPool has a package repository for this variant'
-supp_repo="$(/sp/storpool_variant show current | jq -r '.variant.supported.repo')"
+supp_repo="$(jq -r '.variant.supported.repo' < "$tempf")"
 case "$supp_repo" in
     true)
         supp_repo='1'
         ;;
 
     false)
         supp_repo=''
@@ -427,19 +433,33 @@
         echo 'Ignoring the package query failure for an unsupported repository'
     else
         echo 'Querying for the sp-python3 package failed' 1>&2
         exit 1
     fi
 fi
 
+pkg_count="$(jq '.variant.package | length' < "$tempf")"
+echo "Trying to install $pkg_count packages"
+
+failed=''
+for pkg in $(jq -r '.variant.package | to_entries[] | .value' < "$tempf"); do
+    if ! /sp/storpool_variant command run -- package.install "$pkg"; then
+        failed="$failed $pkg"
+    fi
+done
+if [ -n "$failed" ]; then
+    echo "Could not install some packages:$failed" 1>&2
+    exit 1
+fi
+
 echo 'Done, it seems'
-""",  # noqa: E501  pylint: disable=line-too-long
+""",
             encoding="UTF-8",
         )
-    except Exception as err:  # pylint: disable=broad-except  # noqa: BLE001
+    except Exception as err:  # noqa: BLE001
         return [f"Could not create {addsh}: {err}"]
     try:
         addsh.chmod(0o755)
     except OSError as err:
         return [f"Could not set the permissions mode on {addsh}: {err}"]
 
     cfg.diag_("Spawning the add-repo containers")
@@ -489,15 +509,22 @@
     type=str,
     multiple=True,
     help="Only process images with names containing this string; may be specified multiple times",
 )
 @click.option(
     "-r",
     "--repo-file",
-    type=pathlib.Path,
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
+    ),
     required=True,
     help="The add-storpool-repo archive to test",
 )
 @click.option(
     "-v",
     "--verbose",
     is_flag=True,
@@ -520,8 +547,8 @@
         cfg.diag(lambda: f"About to test {len(images)} containers: {sorted(images.keys())}")
         ordered: Final = sorted(images.items())
 
         asyncio.run(run_tests(cfg, spdir, ordered, var_data))
 
 
 if __name__ == "__main__":
-    main()  # pylint: disable=missing-kwoa
+    main()
```

### Comparing `sp-variant-3.1.2/python/unit_tests/test_subst.py` & `sp_variant-3.2.0/python/unit_tests/test_subst.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Test the variant data template rendering tool."""
 
 import pathlib
 import tempfile
-
-from typing import Final
+import typing
 
 from sp_build_repo import subst
 
 
+if typing.TYPE_CHECKING:
+    from typing import Final
+
+
 def test_subst() -> None:
     """Test the substitution tool."""
     with tempfile.TemporaryDirectory() as tempd_obj:
         tempd: Final = pathlib.Path(tempd_obj)
         cfg: Final = subst.Config(
             output=tempd / "data.txt",
             output_mode=0o612,
@@ -29,15 +32,15 @@
 {% endfor %}
 
 Let's examine some variants:
 
 {% for name, var in variants|dictvsort %}
 Variant: {{ var.name }} alias: {{ var.builder.alias }} family: {{ var.family }} update: {{ var.commands.package.update_db }}
 {% endfor %}
-""",  # noqa: E501  pylint: disable=line-too-long
+""",  # noqa: E501
             encoding="UTF-8",
         )
 
         subst.substitute(cfg)
 
         assert cfg.output.is_file()
         assert (cfg.output.stat().st_mode & 0o7777) == 0o612
```

### Comparing `sp-variant-3.1.2/python/unit_tests/test_variant.py` & `sp_variant-3.2.0/python/unit_tests/test_variant.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 """Test the functions in the sp.variant module."""
 
 from __future__ import annotations
 
 import dataclasses
 import pathlib
 import sys
-
+import typing
 from unittest import mock
 
-from typing import Final, IO
-
 import pytest
 
 from sp_variant import defs
 from sp_variant import variant
 from sp_variant import vbuild
 
 
+if typing.TYPE_CHECKING:
+    from typing import IO, Final
+
+
 _MSG_NOT_SEEN = "This should not be seen"
 _MSG_SEEN = "This should be seen"
 
 
 def test_get() -> None:
     """Test the operation of get_variant()."""
     assert variant.get_variant("CENTOS7").name == "CENTOS7"
@@ -99,20 +101,19 @@
             return
 
         assert output == [(_MSG_SEEN, sys.stderr)]
         output.clear()
 
     def init_cfg(*, verbose: bool, diag_to_stderr: bool = True) -> defs.Config:
         """Initialize a defs.Config object in the specified way."""
-        # pylint: disable=protected-access
         cfg = defs.Config(verbose=verbose)
         assert cfg._diag_to_stderr  # noqa: SLF001
 
         if not diag_to_stderr:
-            cfg._diag_to_stderr = False  # type: ignore[misc]  # noqa: SLF001
+            cfg._diag_to_stderr = False  # noqa: SLF001
             # It... did not change... right?
             assert cfg._diag_to_stderr  # noqa: SLF001
 
         # We cannot just set random properties, can we?
         with pytest.raises(dataclasses.FrozenInstanceError):
             cfg.random_property = 616  # type: ignore[attr-defined]
         assert not hasattr(cfg, "random_property")
```

### Comparing `sp-variant-3.1.2/python/unit_tests/test_yaiparser.py` & `sp_variant-3.2.0/python/unit_tests/test_yaiparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 # SPDX-License-Identifier: BSD-2-Clause
 """Test the os-release parser class."""
 
 from __future__ import annotations
 
 import pathlib
 import tempfile
-
-from typing import Final
+import typing
 
 import pytest
 
 from sp_variant import defs
 from sp_variant import yaiparser
 
 
+if typing.TYPE_CHECKING:
+    from typing import Final
+
+
 _LINES_BAD: Final = [
     "NAME='",
     "NAME=\"foo'",
     "FOO BAR=baz",
     "FOO=bar\\",
     'FOO="meow\\"',
 ]
@@ -97,15 +100,15 @@
 def test_parse() -> None:
     """Test the functionality of _YAIParser.parse() and .get()."""
     with tempfile.TemporaryDirectory() as tempd_obj:
         tempd: Final = pathlib.Path(tempd_obj)
         cfile: Final = tempd / "os-release"
         cfile.write_text(_CFG_TEXT, encoding="UTF-8")
 
-        yai: Final = yaiparser.YAIParser(str(cfile))  # pylint: disable=W0212
+        yai: Final = yaiparser.YAIParser(str(cfile))
         data: Final = yai.parse()
 
         for name, value in _CFG_EXPECTED:
             res_raw = data.get(name)
             assert res_raw == value, repr((name, value, res_raw))
 
             res_ret = yai.get(name)
```

### Comparing `sp-variant-3.1.2/tox.ini` & `sp_variant-3.2.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,68 @@
 # SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 [tox]
 envlist =
   ruff
-  black
-  pep8
+  format
   mypy
-  pylint
+  reuse
   unit-tests
 isolated_build = True
 
 [defs]
 pyfiles =
   python/sp_build_repo
   python/sp_variant
   python/test_docker
-  setup.py
   python/unit_tests
 
 [testenv:ruff]
 skip_install = True
 tags =
   check
 deps =
-  ruff >= 0.0.256, < 0.1
-commands =
-  ruff check --config python/config/ruff-most/pyproject.toml -- {[defs]pyfiles}
-
-[testenv:ruff-all]
-skip_install = True
-tags =
-  check
-deps =
-  ruff == 0.0.256
+  -r python/requirements/ruff.txt
 commands =
   ruff check --config python/config/ruff-all/pyproject.toml -- {[defs]pyfiles}
 
-[testenv:black]
+[testenv:format]
 skip_install = True
 tags =
   check
 deps =
+  -r python/requirements/ruff.txt
   black >= 23, < 24
 commands =
+  ruff check --config python/config/ruff-base/pyproject.toml --select=I --diff -- {[defs]pyfiles}
   black --check {[defs]pyfiles}
 
-[testenv:black-reformat]
+[testenv:reformat]
 skip_install = True
 tags =
   format
   manual
 deps =
+  -r python/requirements/ruff.txt
   black >= 23, < 24
 commands =
+  ruff check --config python/config/ruff-base/pyproject.toml --select=I --fix -- {[defs]pyfiles}
   black {[defs]pyfiles}
 
-[testenv:pep8]
-skip_install = True
-tags =
-  check
-deps =
-  flake8 >= 6, < 7
-commands =
-  flake8 {[defs]pyfiles}
-
 [testenv:mypy]
 skip_install = True
 tags =
   check
 deps =
   -r python/requirements/test-mypy.txt
   mypy >= 1, < 2
 commands =
   mypy {[defs]pyfiles}
 
-[testenv:pylint]
-skip_install = True
-tags =
-  check
-deps =
-  -r python/requirements/test-unit.txt
-  pylint >= 2.16, < 2.17
-commands =
-  pylint {[defs]pyfiles}
-
 [testenv:unit-tests]
 tags =
   tests
 deps =
   -r python/requirements/test-unit.txt
 commands =
   pytest {posargs} python/unit_tests
@@ -106,15 +80,14 @@
   sh -c 'pyupgrade --py38-plus python/sp_build_repo/*.py python/sp_variant/*.py python/test_docker/*.py python/unit_tests/*.py'
 
 # This should only be run when the working tree is clean
 [testenv:reuse]
 skip_install = True
 tags =
   check
-  manual
 deps =
   reuse >= 1, < 2
 commands =
   reuse lint
 
 [testenv:docs]
 skip_install = True
```

