# Comparing `tmp/pyproject_ops-0.2.3.tar.gz` & `tmp/pyproject_ops-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_ops-0.2.3.tar", last modified: Mon Jul  3 16:36:32 2023, max compression
+gzip compressed data, was "pyproject_ops-0.3.1.tar", last modified: Thu Jul  6 01:54:33 2023, max compression
```

## Comparing `pyproject_ops-0.2.3.tar` & `pyproject_ops-0.3.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.354181 pyproject_ops-0.2.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)    10513 2023-07-03 16:36:32.353953 pyproject_ops-0.2.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     9359 2023-07-03 16:35:56.000000 pyproject_ops-0.2.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.350668 pyproject_ops-0.2.3/pyproject_ops/
--rw-r--r--   0 sanhehu    (501) staff       (20)      423 2023-06-03 06:48:33.000000 pyproject_ops-0.2.3/pyproject_ops/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-03 16:32:58.000000 pyproject_ops-0.2.3/pyproject_ops/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-03 05:51:29.000000 pyproject_ops-0.2.3/pyproject_ops/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5122 2023-06-15 00:58:04.000000 pyproject_ops-0.2.3/pyproject_ops/cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      163 2023-05-22 19:51:02.000000 pyproject_ops-0.2.3/pyproject_ops/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.351620 pyproject_ops-0.2.3/pyproject_ops/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/pyproject_ops/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      219 2023-04-27 16:12:50.000000 pyproject_ops-0.2.3/pyproject_ops/helpers.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      154 2023-05-23 00:56:49.000000 pyproject_ops-0.2.3/pyproject_ops/logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      144 2023-05-23 01:06:08.000000 pyproject_ops-0.2.3/pyproject_ops/operation_system.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1020 2023-06-03 06:39:10.000000 pyproject_ops-0.2.3/pyproject_ops/ops.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      657 2023-05-22 19:25:03.000000 pyproject_ops-0.2.3/pyproject_ops/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      470 2023-06-03 06:22:27.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4237 2023-07-03 16:34:10.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_aws_lambda.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1305 2023-06-03 06:09:59.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_build.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1206 2023-06-03 06:02:21.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_config_management.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13420 2023-06-03 05:59:35.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_deps.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3399 2023-06-03 05:59:07.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_docs.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12633 2023-06-14 13:22:05.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-03 06:38:24.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_publish.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2416 2023-06-14 13:23:14.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_tests.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1997 2023-06-03 05:56:13.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_venv.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.352092 pyproject_ops-0.2.3/pyproject_ops/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 pyproject_ops-0.2.3/pyproject_ops/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 pyproject_ops-0.2.3/pyproject_ops/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.353241 pyproject_ops-0.2.3/pyproject_ops/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-23 00:53:52.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3224 2023-06-03 06:06:50.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-06-03 06:50:12.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/jsonutils.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-23 00:53:57.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/nested_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-23 00:54:59.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.351470 pyproject_ops-0.2.3/pyproject_ops.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)    10513 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1354 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/entry_points.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1399 2023-07-03 16:33:24.000000 pyproject_ops-0.2.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 pyproject_ops-0.2.3/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-23 02:18:02.000000 pyproject_ops-0.2.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-03 06:28:54.000000 pyproject_ops-0.2.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-06-03 07:40:12.000000 pyproject_ops-0.2.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:58:31.000000 pyproject_ops-0.2.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-03 16:36:32.354234 pyproject_ops-0.2.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7839 2023-06-14 13:30:02.000000 pyproject_ops-0.2.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.353624 pyproject_ops-0.2.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-06-03 07:45:37.000000 pyproject_ops-0.2.3/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1733 2023-06-03 07:14:18.000000 pyproject_ops-0.2.3/tests/test_pyproject_ops.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 01:54:33.269998 pyproject_ops-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-23 02:11:51.000000 pyproject_ops-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-05-23 02:11:51.000000 pyproject_ops-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-23 02:11:51.000000 pyproject_ops-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10865 2023-07-06 01:54:33.269790 pyproject_ops-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9711 2023-07-06 01:45:18.000000 pyproject_ops-0.3.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 01:54:33.266678 pyproject_ops-0.3.1/pyproject_ops/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      423 2023-06-03 06:48:33.000000 pyproject_ops-0.3.1/pyproject_ops/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 01:45:48.000000 pyproject_ops-0.3.1/pyproject_ops/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-03 05:51:29.000000 pyproject_ops-0.3.1/pyproject_ops/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5122 2023-06-15 00:58:04.000000 pyproject_ops-0.3.1/pyproject_ops/cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      163 2023-05-22 19:51:02.000000 pyproject_ops-0.3.1/pyproject_ops/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 01:54:33.267521 pyproject_ops-0.3.1/pyproject_ops/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-23 02:11:51.000000 pyproject_ops-0.3.1/pyproject_ops/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      219 2023-04-27 16:12:50.000000 pyproject_ops-0.3.1/pyproject_ops/helpers.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      154 2023-05-23 00:56:49.000000 pyproject_ops-0.3.1/pyproject_ops/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      144 2023-05-23 01:06:08.000000 pyproject_ops-0.3.1/pyproject_ops/operation_system.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1091 2023-07-06 01:44:30.000000 pyproject_ops-0.3.1/pyproject_ops/ops.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      657 2023-05-22 19:25:03.000000 pyproject_ops-0.3.1/pyproject_ops/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      470 2023-06-03 06:22:27.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1193 2023-07-06 01:45:13.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_aws_glue.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4237 2023-07-03 16:34:10.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_aws_lambda.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1305 2023-06-03 06:09:59.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_build.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1206 2023-06-03 06:02:21.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_config_management.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    14245 2023-07-06 01:51:13.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_deps.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3399 2023-06-03 05:59:07.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_docs.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12633 2023-06-14 13:22:05.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-03 06:38:24.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_publish.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2416 2023-06-14 13:23:14.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_tests.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1997 2023-06-03 05:56:13.000000 pyproject_ops-0.3.1/pyproject_ops/pyproject_venv.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 01:54:33.267910 pyproject_ops-0.3.1/pyproject_ops/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 pyproject_ops-0.3.1/pyproject_ops/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 pyproject_ops-0.3.1/pyproject_ops/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 01:54:33.269127 pyproject_ops-0.3.1/pyproject_ops/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-23 00:53:52.000000 pyproject_ops-0.3.1/pyproject_ops/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3224 2023-06-03 06:06:50.000000 pyproject_ops-0.3.1/pyproject_ops/vendor/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-06-03 06:50:12.000000 pyproject_ops-0.3.1/pyproject_ops/vendor/jsonutils.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-23 00:53:57.000000 pyproject_ops-0.3.1/pyproject_ops/vendor/nested_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-23 00:54:59.000000 pyproject_ops-0.3.1/pyproject_ops/vendor/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 pyproject_ops-0.3.1/pyproject_ops/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 01:54:33.267402 pyproject_ops-0.3.1/pyproject_ops.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10865 2023-07-06 01:54:33.000000 pyproject_ops-0.3.1/pyproject_ops.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1390 2023-07-06 01:54:33.000000 pyproject_ops-0.3.1/pyproject_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 01:54:33.000000 pyproject_ops-0.3.1/pyproject_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-07-06 01:54:33.000000 pyproject_ops-0.3.1/pyproject_ops.egg-info/entry_points.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-07-06 01:54:33.000000 pyproject_ops-0.3.1/pyproject_ops.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-07-06 01:54:33.000000 pyproject_ops-0.3.1/pyproject_ops.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1628 2023-07-06 01:51:46.000000 pyproject_ops-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 pyproject_ops-0.3.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-23 02:18:02.000000 pyproject_ops-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-03 06:28:54.000000 pyproject_ops-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-06-03 07:40:12.000000 pyproject_ops-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:58:31.000000 pyproject_ops-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 01:54:33.270044 pyproject_ops-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7839 2023-06-14 13:30:02.000000 pyproject_ops-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 01:54:33.269477 pyproject_ops-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-06-03 07:45:37.000000 pyproject_ops-0.3.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1771 2023-07-06 01:51:32.000000 pyproject_ops-0.3.1/tests/test_pyproject_ops.py
```

### Comparing `pyproject_ops-0.2.3/LICENSE.txt` & `pyproject_ops-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/PKG-INFO` & `pyproject_ops-0.3.1/pyproject_ops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: pyproject_ops
-Version: 0.2.3
+Name: pyproject-ops
+Version: 0.3.1
 Summary: Python project Ops automation.
 Home-page: https://github.com/MacHu-GWU/pyproject_ops-project
-Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.3#downloads
+Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -113,14 +113,17 @@
 - ``.venv/bin``: ``PyProjectOps.dir_venv_bin``, The bin folder in virtualenv.
 - ``.venv/bin/pip``: ``PyProjectOps.path_venv_bin_pip``, The pip command in virtualenv.
 - ``.venv/bin/pytest``: ``PyProjectOps.path_venv_bin_pytest``, The pytest command in virtualenv.
 - ``.venv/bin/python``: ``PyProjectOps.path_sys_executable``, The current Python interpreter path.
 - ``.venv/bin/python``: ``PyProjectOps.path_venv_bin_python``, The python executable in virtualenv.
 - ``.venv/bin/twine``: ``PyProjectOps.path_bin_twine``, The twine CLI command path.
 - ``build``: ``PyProjectOps.dir_build``, The build folder for Python or artifacts build.
+- ``build/glue``: ``PyProjectOps.dir_build_glue``, The AWS glue artifacts build folder.
+- ``build/glue/extra_py_files``: ``PyProjectOps.dir_build_glue_extra_py_files``, The AWS glue extra Python files build folder.
+- ``build/glue/extra_py_files.zip``: ``PyProjectOps.path_build_glue_extra_py_files_zip``, The AWS glue extra Python files zip file path.
 - ``build/lambda``: ``PyProjectOps.dir_build_lambda``, The AWS Lambda artifacts build folder.
 - ``build/lambda/layer.zip``: ``PyProjectOps.path_build_lambda_layer_zip``, The AWS Lambda layer zip file path.
 - ``build/lambda/python``: ``PyProjectOps.dir_build_lambda_python``, The AWS Lambda layer build folder. This folder contains the dependencies.
 - ``build/lambda/python/aws``: ``PyProjectOps.path_build_lambda_bin_aws``, This is the AWS CLI executable path in Lambda layer.
 - ``build/lambda/source.zip``: ``PyProjectOps.path_build_lambda_source_zip``, The AWS Lambda source code deployment package zip file path.
 - ``config``: ``PyProjectOps.dir_config``, The folder that stores the config files.
 - ``config/config.json``: ``PyProjectOps.path_config_json``, Path to the JSON file that stores the non-sensitive config.
```

### Comparing `pyproject_ops-0.2.3/README.rst` & `pyproject_ops-0.3.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 - ``.venv/bin``: ``PyProjectOps.dir_venv_bin``, The bin folder in virtualenv.
 - ``.venv/bin/pip``: ``PyProjectOps.path_venv_bin_pip``, The pip command in virtualenv.
 - ``.venv/bin/pytest``: ``PyProjectOps.path_venv_bin_pytest``, The pytest command in virtualenv.
 - ``.venv/bin/python``: ``PyProjectOps.path_sys_executable``, The current Python interpreter path.
 - ``.venv/bin/python``: ``PyProjectOps.path_venv_bin_python``, The python executable in virtualenv.
 - ``.venv/bin/twine``: ``PyProjectOps.path_bin_twine``, The twine CLI command path.
 - ``build``: ``PyProjectOps.dir_build``, The build folder for Python or artifacts build.
+- ``build/glue``: ``PyProjectOps.dir_build_glue``, The AWS glue artifacts build folder.
+- ``build/glue/extra_py_files``: ``PyProjectOps.dir_build_glue_extra_py_files``, The AWS glue extra Python files build folder.
+- ``build/glue/extra_py_files.zip``: ``PyProjectOps.path_build_glue_extra_py_files_zip``, The AWS glue extra Python files zip file path.
 - ``build/lambda``: ``PyProjectOps.dir_build_lambda``, The AWS Lambda artifacts build folder.
 - ``build/lambda/layer.zip``: ``PyProjectOps.path_build_lambda_layer_zip``, The AWS Lambda layer zip file path.
 - ``build/lambda/python``: ``PyProjectOps.dir_build_lambda_python``, The AWS Lambda layer build folder. This folder contains the dependencies.
 - ``build/lambda/python/aws``: ``PyProjectOps.path_build_lambda_bin_aws``, This is the AWS CLI executable path in Lambda layer.
 - ``build/lambda/source.zip``: ``PyProjectOps.path_build_lambda_source_zip``, The AWS Lambda source code deployment package zip file path.
 - ``config``: ``PyProjectOps.dir_config``, The folder that stores the config files.
 - ``config/config.json``: ``PyProjectOps.path_config_json``, Path to the JSON file that stores the non-sensitive config.
```

### Comparing `pyproject_ops-0.2.3/pyproject_ops/cli.py` & `pyproject_ops-0.3.1/pyproject_ops/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/ops.py` & `pyproject_ops-0.3.1/pyproject_ops/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 from .pyproject_tests import PyProjectTests
 from .pyproject_docs import PyProjectDocs
 from .pyproject_build import PyProjectBuild
 from .pyproject_publish import PyProjectPublish
 from .pyproject_config_management import PyProjectConfigManagement
 from .pyproject_aws import PyProjectAWS
 from .pyproject_aws_lambda import PyProjectAWSLambda
+from .pyproject_aws_glue import PyProjectAWSGlue
 
 
 @dataclasses.dataclass
 class PyProjectOps(
     PyProjectPaths,
     PyProjectVenv,
     PyProjectDeps,
     PyProjectTests,
     PyProjectDocs,
     PyProjectBuild,
     PyProjectPublish,
     PyProjectConfigManagement,
     PyProjectAWS,
     PyProjectAWSLambda,
+    PyProjectAWSGlue,
 ):
     """
     The namespace for all the pyproject_ops automation methods.
     """
     def __post_init__(self):
         self._validate_paths()
         self._validate_python_version()
```

### Comparing `pyproject_ops-0.2.3/pyproject_ops/paths.py` & `pyproject_ops-0.3.1/pyproject_ops/paths.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_aws_lambda.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_aws_lambda.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_build.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_build.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_config_management.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_config_management.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_deps.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_deps.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 @dataclasses.dataclass
 class PyProjectDeps:
     """
     Namespace class for dependencies management related automation.
     """
+
     def poetry_lock(self: "PyProjectOps"):
         """
         Run:
 
         .. code-block:: bash
 
             poetry lock
@@ -444,7 +445,34 @@
             self.path_requirements_dev,
             self.path_requirements_test,
             self.path_requirements_doc,
             self.path_requirements_automation,
         ]:
             args = [f"{self.path_venv_bin_pip}", "install", "-r", f"{path}"]
             self._run_pip_install(args, quiet)
+
+    def pip_install_awsglue(
+        self: "PyProjectOps",
+        glue_version: str = "4.0",
+        quiet: bool = False,
+    ):
+        """
+        Pip install the awsglue Python library.
+
+        Reference:
+
+        - aws-glue-libs: https://github.com/awslabs/aws-glue-libs
+        - VCS Support - Git: https://pip.pypa.io/en/stable/topics/vcs-support/#git
+        """
+        glue_version_to_git_tag_mapper = {
+            "4.0": "v4.0",
+            "3.0": "v3.0",
+            "2.0": "v1.0-and-v2.0",
+            "1.0": "v1.0-and-v2.0",
+        }
+        git_tag = glue_version_to_git_tag_mapper[glue_version]
+        args = [
+            f"{self.path_venv_bin_pip}",
+            "install",
+            f"git+https://github.com/awslabs/aws-glue-libs.git@{git_tag}",
+        ]
+        self._run_pip_install(args, quiet)
```

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_docs.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_docs.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_paths.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_paths.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_publish.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_publish.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_tests.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_tests.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/pyproject_venv.py` & `pyproject_ops-0.3.1/pyproject_ops/pyproject_venv.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/vendor/build_dist.py` & `pyproject_ops-0.3.1/pyproject_ops/vendor/build_dist.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/vendor/jsonutils.py` & `pyproject_ops-0.3.1/pyproject_ops/vendor/jsonutils.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/vendor/nested_logger.py` & `pyproject_ops-0.3.1/pyproject_ops/vendor/nested_logger.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops/vendor/pytest_cov_helper.py` & `pyproject_ops-0.3.1/pyproject_ops/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/pyproject_ops.egg-info/PKG-INFO` & `pyproject_ops-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: pyproject-ops
-Version: 0.2.3
+Name: pyproject_ops
+Version: 0.3.1
 Summary: Python project Ops automation.
 Home-page: https://github.com/MacHu-GWU/pyproject_ops-project
-Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.3#downloads
+Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -113,14 +113,17 @@
 - ``.venv/bin``: ``PyProjectOps.dir_venv_bin``, The bin folder in virtualenv.
 - ``.venv/bin/pip``: ``PyProjectOps.path_venv_bin_pip``, The pip command in virtualenv.
 - ``.venv/bin/pytest``: ``PyProjectOps.path_venv_bin_pytest``, The pytest command in virtualenv.
 - ``.venv/bin/python``: ``PyProjectOps.path_sys_executable``, The current Python interpreter path.
 - ``.venv/bin/python``: ``PyProjectOps.path_venv_bin_python``, The python executable in virtualenv.
 - ``.venv/bin/twine``: ``PyProjectOps.path_bin_twine``, The twine CLI command path.
 - ``build``: ``PyProjectOps.dir_build``, The build folder for Python or artifacts build.
+- ``build/glue``: ``PyProjectOps.dir_build_glue``, The AWS glue artifacts build folder.
+- ``build/glue/extra_py_files``: ``PyProjectOps.dir_build_glue_extra_py_files``, The AWS glue extra Python files build folder.
+- ``build/glue/extra_py_files.zip``: ``PyProjectOps.path_build_glue_extra_py_files_zip``, The AWS glue extra Python files zip file path.
 - ``build/lambda``: ``PyProjectOps.dir_build_lambda``, The AWS Lambda artifacts build folder.
 - ``build/lambda/layer.zip``: ``PyProjectOps.path_build_lambda_layer_zip``, The AWS Lambda layer zip file path.
 - ``build/lambda/python``: ``PyProjectOps.dir_build_lambda_python``, The AWS Lambda layer build folder. This folder contains the dependencies.
 - ``build/lambda/python/aws``: ``PyProjectOps.path_build_lambda_bin_aws``, This is the AWS CLI executable path in Lambda layer.
 - ``build/lambda/source.zip``: ``PyProjectOps.path_build_lambda_source_zip``, The AWS Lambda source code deployment package zip file path.
 - ``config``: ``PyProjectOps.dir_config``, The folder that stores the config files.
 - ``config/config.json``: ``PyProjectOps.path_config_json``, Path to the JSON file that stores the non-sensitive config.
```

### Comparing `pyproject_ops-0.2.3/pyproject_ops.egg-info/SOURCES.txt` & `pyproject_ops-0.3.1/pyproject_ops.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 pyproject_ops/compat.py
 pyproject_ops/helpers.py
 pyproject_ops/logger.py
 pyproject_ops/operation_system.py
 pyproject_ops/ops.py
 pyproject_ops/paths.py
 pyproject_ops/pyproject_aws.py
+pyproject_ops/pyproject_aws_glue.py
 pyproject_ops/pyproject_aws_lambda.py
 pyproject_ops/pyproject_build.py
 pyproject_ops/pyproject_config_management.py
 pyproject_ops/pyproject_deps.py
 pyproject_ops/pyproject_docs.py
 pyproject_ops/pyproject_paths.py
 pyproject_ops/pyproject_publish.py
```

### Comparing `pyproject_ops-0.2.3/release-history.rst` & `pyproject_ops-0.3.1/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2023-07-05)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add AWS glue related paths. add ``pip_install_awsglue`` command to install ``awsglue`` package.
+
+
 0.2.3 (2023-07-03)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - add ``dir_lambda_app_vendor_python_lib`` path.
```

### Comparing `pyproject_ops-0.2.3/requirements-doc.txt` & `pyproject_ops-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/setup.py` & `pyproject_ops-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.3/tests/test_pyproject_ops.py` & `pyproject_ops-0.3.1/tests/test_pyproject_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         _ = pyops._try_poetry_export
         _ = pyops.pip_install
         _ = pyops.pip_install_dev
         _ = pyops.pip_install_test
         _ = pyops.pip_install_doc
         _ = pyops.pip_install_automation
         _ = pyops.pip_install_all
+        _ = pyops.pip_install_awsglue
 
 
 class PyProjectTests:
     def test(self):
         _ = pyops.run_unit_test
         _ = pyops.run_cov_test
```

