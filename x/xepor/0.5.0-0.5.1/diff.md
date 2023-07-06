# Comparing `tmp/xepor-0.5.0.tar.gz` & `tmp/xepor-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xepor-0.5.0.tar", last modified: Sun Mar 20 09:56:33 2022, max compression
+gzip compressed data, was "xepor-0.5.1.tar", last modified: Wed Jul  5 08:46:42 2023, max compression
```

## Comparing `xepor-0.5.0.tar` & `xepor-0.5.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.416414 xepor-0.5.0/
--rw-rw-r--   0 vm        (1000) vm        (1000)      588 2022-02-25 12:52:46.000000 xepor-0.5.0/.coveragerc
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.408414 xepor-0.5.0/.github/
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.412414 xepor-0.5.0/.github/workflows/
--rw-rw-r--   0 vm        (1000) vm        (1000)     1293 2022-03-19 09:49:31.000000 xepor-0.5.0/.github/workflows/python-package.yml
--rw-rw-r--   0 vm        (1000) vm        (1000)      568 2022-03-20 08:28:12.000000 xepor-0.5.0/.gitignore
--rw-rw-r--   0 vm        (1000) vm        (1000)     1694 2022-02-28 08:41:01.000000 xepor-0.5.0/.gitlab-ci.yml
--rw-rw-r--   0 vm        (1000) vm        (1000)       91 2022-02-25 06:44:18.000000 xepor-0.5.0/.gitmodules
--rw-rw-r--   0 vm        (1000) vm        (1000)      490 2022-02-25 12:52:46.000000 xepor-0.5.0/.readthedocs.yml
--rw-rw-r--   0 vm        (1000) vm        (1000)       57 2022-03-17 08:31:40.000000 xepor-0.5.0/AUTHORS.md
--rw-rw-r--   0 vm        (1000) vm        (1000)     2972 2022-03-20 09:49:18.000000 xepor-0.5.0/CHANGELOG.md
--rw-rw-r--   0 vm        (1000) vm        (1000)    12403 2022-03-17 08:40:37.000000 xepor-0.5.0/CONTRIBUTING.rst
--rw-rw-r--   0 vm        (1000) vm        (1000)    11357 2022-02-25 13:32:38.000000 xepor-0.5.0/LICENSE
--rw-rw-r--   0 vm        (1000) vm        (1000)    11357 2022-02-25 12:52:46.000000 xepor-0.5.0/LICENSE.txt
--rw-rw-r--   0 vm        (1000) vm        (1000)     7113 2022-03-20 09:56:33.416414 xepor-0.5.0/PKG-INFO
--rw-rw-r--   0 vm        (1000) vm        (1000)     5556 2022-03-20 09:41:41.000000 xepor-0.5.0/README.md
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.412414 xepor-0.5.0/docs/
--rw-rw-r--   0 vm        (1000) vm        (1000)     1154 2022-02-25 12:52:46.000000 xepor-0.5.0/docs/Makefile
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.412414 xepor-0.5.0/docs/_static/
--rw-rw-r--   0 vm        (1000) vm        (1000)       18 2022-02-25 12:52:46.000000 xepor-0.5.0/docs/_static/.gitignore
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.416414 xepor-0.5.0/docs/api/
--rw-rw-r--   0 vm        (1000) vm        (1000)      137 2022-03-20 08:27:02.000000 xepor-0.5.0/docs/api/modules.rst
--rw-rw-r--   0 vm        (1000) vm        (1000)       57 2022-03-17 08:31:40.000000 xepor-0.5.0/docs/authors.md
--rw-rw-r--   0 vm        (1000) vm        (1000)     2972 2022-03-20 09:49:18.000000 xepor-0.5.0/docs/changelog.md
--rw-rw-r--   0 vm        (1000) vm        (1000)     8741 2022-03-20 08:27:02.000000 xepor-0.5.0/docs/conf.py
--rw-rw-r--   0 vm        (1000) vm        (1000)       33 2022-02-25 12:52:46.000000 xepor-0.5.0/docs/contributing.rst
--rw-rw-r--   0 vm        (1000) vm        (1000)      306 2022-03-20 08:27:02.000000 xepor-0.5.0/docs/index.md
--rw-rw-r--   0 vm        (1000) vm        (1000)       66 2022-03-17 08:11:33.000000 xepor-0.5.0/docs/license.rst
--rw-rw-r--   0 vm        (1000) vm        (1000)     5556 2022-03-20 09:41:41.000000 xepor-0.5.0/docs/readme.md
--rw-rw-r--   0 vm        (1000) vm        (1000)      262 2022-03-20 07:35:43.000000 xepor-0.5.0/docs/requirements.txt
--rw-rw-r--   0 vm        (1000) vm        (1000)      355 2022-03-17 08:38:14.000000 xepor-0.5.0/pyproject.toml
--rw-rw-r--   0 vm        (1000) vm        (1000)     2107 2022-03-20 09:56:33.416414 xepor-0.5.0/setup.cfg
--rw-rw-r--   0 vm        (1000) vm        (1000)      652 2022-03-17 08:37:06.000000 xepor-0.5.0/setup.py
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.408414 xepor-0.5.0/src/
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.416414 xepor-0.5.0/src/xepor/
--rw-rw-r--   0 vm        (1000) vm        (1000)      688 2022-03-20 08:28:16.000000 xepor-0.5.0/src/xepor/__init__.py
--rw-rw-r--   0 vm        (1000) vm        (1000)    17408 2022-03-20 09:41:59.000000 xepor-0.5.0/src/xepor/xepor.py
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.416414 xepor-0.5.0/src/xepor.egg-info/
--rw-rw-r--   0 vm        (1000) vm        (1000)     7113 2022-03-20 09:56:32.000000 xepor-0.5.0/src/xepor.egg-info/PKG-INFO
--rw-rw-r--   0 vm        (1000) vm        (1000)      729 2022-03-20 09:56:33.000000 xepor-0.5.0/src/xepor.egg-info/SOURCES.txt
--rw-rw-r--   0 vm        (1000) vm        (1000)        1 2022-03-20 09:56:32.000000 xepor-0.5.0/src/xepor.egg-info/dependency_links.txt
--rw-rw-r--   0 vm        (1000) vm        (1000)        1 2022-02-25 08:56:56.000000 xepor-0.5.0/src/xepor.egg-info/not-zip-safe
--rw-rw-r--   0 vm        (1000) vm        (1000)      128 2022-03-20 09:56:33.000000 xepor-0.5.0/src/xepor.egg-info/requires.txt
--rw-rw-r--   0 vm        (1000) vm        (1000)        6 2022-03-20 09:56:33.000000 xepor-0.5.0/src/xepor.egg-info/top_level.txt
-drwxrwxr-x   0 vm        (1000) vm        (1000)        0 2022-03-20 09:56:33.416414 xepor-0.5.0/tests/
--rw-rw-r--   0 vm        (1000) vm        (1000)        0 2022-03-19 07:57:11.000000 xepor-0.5.0/tests/__init__.py
--rw-rw-r--   0 vm        (1000) vm        (1000)      991 2022-03-19 07:56:52.000000 xepor-0.5.0/tests/conftest.py
--rw-rw-r--   0 vm        (1000) vm        (1000)     5150 2022-03-20 08:28:16.000000 xepor-0.5.0/tests/test_examples.py
--rw-rw-r--   0 vm        (1000) vm        (1000)     1407 2022-03-19 08:13:26.000000 xepor-0.5.0/tests/test_single.py
--rw-rw-r--   0 vm        (1000) vm        (1000)     2262 2022-03-20 08:28:16.000000 xepor-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-05 08:46:32.000000 xepor-0.5.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.555777 xepor-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-05 08:46:32.000000 xepor-0.5.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-05 08:46:32.000000 xepor-0.5.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-05 08:46:32.000000 xepor-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-05 08:46:32.000000 xepor-0.5.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-05 08:46:32.000000 xepor-0.5.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-05 08:46:32.000000 xepor-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-05 08:46:32.000000 xepor-0.5.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 08:46:32.000000 xepor-0.5.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-05 08:46:32.000000 xepor-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-05 08:46:32.000000 xepor-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 08:46:32.000000 xepor-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 08:46:32.000000 xepor-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-05 08:46:42.559777 xepor-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-05 08:46:32.000000 xepor-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-05 08:46:32.000000 xepor-0.5.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 08:46:32.000000 xepor-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-05 08:46:42.563777 xepor-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-05 08:46:32.000000 xepor-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.555777 xepor-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/src/xepor/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-05 08:46:32.000000 xepor-0.5.1/src/xepor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-07-05 08:46:32.000000 xepor-0.5.1/src/xepor/xepor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/src/xepor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-05 08:46:42.000000 xepor-0.5.1/src/xepor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-05 08:46:42.000000 xepor-0.5.1/src/xepor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:46:42.000000 xepor-0.5.1/src/xepor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:46:42.000000 xepor-0.5.1/src/xepor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 08:46:42.000000 xepor-0.5.1/src/xepor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 08:46:42.000000 xepor-0.5.1/src/xepor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:42.559777 xepor-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:46:32.000000 xepor-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-05 08:46:32.000000 xepor-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-05 08:46:32.000000 xepor-0.5.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-05 08:46:32.000000 xepor-0.5.1/tests/test_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-05 08:46:32.000000 xepor-0.5.1/tox.ini
```

### Comparing `xepor-0.5.0/.coveragerc` & `xepor-0.5.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/.gitignore` & `xepor-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/.gitlab-ci.yml` & `xepor-0.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/CHANGELOG.md` & `xepor-0.5.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 
 % **Note**: This document contains some [MyST](https://myst-parser.readthedocs.io/en/latest/index.html) syntax which is not completely Markdown. For better experience (and cross references to the changed code) you could read this document on [Read the Docs](https://xepor.readthedocs.io/en/latest/changelog.html)
+## Version 0.5.1
+
+- Feature: Add compatibility with mitmproxy 9.x and Python 3.11~3.12.
+  - Since mitmproxy 8.x is not compatible with Python 3.11, therefore updating to mitmproxy 9.x + xepor 0.5.1 is recommended especially for Kali users with rolling updates.
 
 ## Version 0.5.0
 
 **⚠️Breaking Change⚠️**: Incompatible API changes.
 
 - Change: Move some constants inside {class}`~xepor.InterceptedAPI` to seperate enums: {func}`xepor.RouteType`, {func}`xepor.FlowMeta`. ([xepor/xepor@83128e8](https://github.com/xepor/xepor/commit/83128e81f8c181cd23363d27c76209b9de1c49eb))
 - Change: rename `reqtype` in {func}`xepor.InterceptedAPI.route` to `rtype`. The name there before is for historical reason. [xepor/xepor@c6c7e83](https://github.com/xepor/xepor/commit/c6c7e8319aef95de01a0f797d9bb2c01632b7609)
```

### Comparing `xepor-0.5.0/CONTRIBUTING.rst` & `xepor-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/LICENSE` & `xepor-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/LICENSE.txt` & `xepor-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/PKG-INFO` & `xepor-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xepor
-Version: 0.5.0
+Version: 0.5.1
 Summary: Xepor, a web routing framework for reverse engineers and security researchers.
 Home-page: https://github.com/xepor/xepor
 Author: ttimasdf
 Author-email: opensource@rabit.pw
 License: Apache-2.0
 Project-URL: Documentation, https://xepor.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/xepor/xepor
@@ -25,20 +25,20 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-[![Python package](https://github.com/xepor/xepor/actions/workflows/python-package.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/python-package.yml)
+[![Unit Tests](https://github.com/xepor/xepor/actions/workflows/test.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/test.yml)
 [![PyPI-Server](https://img.shields.io/pypi/v/xepor.svg)](https://pypi.org/project/xepor/)
 ![PyPI - Status](https://img.shields.io/pypi/status/xepor)
 [![Documentation Status](https://readthedocs.org/projects/xepor/badge/?version=latest)](https://xepor.readthedocs.io/en/latest/?badge=latest)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
 
 # Xepor
@@ -66,14 +66,20 @@
 2. Sniffing traffic from specific device by iptables + transparent proxy, modify the payload with xepor on the fly.
 3. Cracking cloud based software license. See [examples/krisp/](https://github.com/xepor/xepor-examples/tree/main/krisp/) as an example.
 4. Write complicated web crawler in **\~100 lines of codes**. See [examples/polyv_scrapper/](https://github.com/xepor/xepor-examples/tree/main/polyv_scrapper/) as an example.
 5. ... and many more.
 
 SSL stripping is NOT provided by this project.
 
+# Installation
+
+```bash
+pip install xepor
+```
+
 # Quick start
 
 Take the script from [examples/httpbin](https://github.com/xepor/xepor-examples/tree/main/httpbin/) as an example.
 
 ```bash
 mitmweb --web-host=\* --set connection_strategy=lazy -s example/httpbin/httpbin.py
 ```
@@ -124,10 +130,7 @@
         f"Captured {'successful' if flow.response.status_code < 300 else 'unsuccessful'} login:",
         flow.request.headers.get("Authorization", ""),
     )
 
 
 addons = [api]
 ```
-
-
-
```

### Comparing `xepor-0.5.0/README.md` & `xepor-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Python package](https://github.com/xepor/xepor/actions/workflows/python-package.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/python-package.yml)
+[![Unit Tests](https://github.com/xepor/xepor/actions/workflows/test.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/test.yml)
 [![PyPI-Server](https://img.shields.io/pypi/v/xepor.svg)](https://pypi.org/project/xepor/)
 ![PyPI - Status](https://img.shields.io/pypi/status/xepor)
 [![Documentation Status](https://readthedocs.org/projects/xepor/badge/?version=latest)](https://xepor.readthedocs.io/en/latest/?badge=latest)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
 
 # Xepor
@@ -30,14 +30,20 @@
 2. Sniffing traffic from specific device by iptables + transparent proxy, modify the payload with xepor on the fly.
 3. Cracking cloud based software license. See [examples/krisp/](https://github.com/xepor/xepor-examples/tree/main/krisp/) as an example.
 4. Write complicated web crawler in **\~100 lines of codes**. See [examples/polyv_scrapper/](https://github.com/xepor/xepor-examples/tree/main/polyv_scrapper/) as an example.
 5. ... and many more.
 
 SSL stripping is NOT provided by this project.
 
+# Installation
+
+```bash
+pip install xepor
+```
+
 # Quick start
 
 Take the script from [examples/httpbin](https://github.com/xepor/xepor-examples/tree/main/httpbin/) as an example.
 
 ```bash
 mitmweb --web-host=\* --set connection_strategy=lazy -s example/httpbin/httpbin.py
 ```
@@ -88,8 +94,7 @@
         f"Captured {'successful' if flow.response.status_code < 300 else 'unsuccessful'} login:",
         flow.request.headers.get("Authorization", ""),
     )
 
 
 addons = [api]
 ```
-
```

### Comparing `xepor-0.5.0/docs/Makefile` & `xepor-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/docs/changelog.md` & `xepor-0.5.1/docs/changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 
 % **Note**: This document contains some [MyST](https://myst-parser.readthedocs.io/en/latest/index.html) syntax which is not completely Markdown. For better experience (and cross references to the changed code) you could read this document on [Read the Docs](https://xepor.readthedocs.io/en/latest/changelog.html)
+## Version 0.5.1
+
+- Feature: Add compatibility with mitmproxy 9.x and Python 3.11~3.12.
+  - Since mitmproxy 8.x is not compatible with Python 3.11, therefore updating to mitmproxy 9.x + xepor 0.5.1 is recommended especially for Kali users with rolling updates.
 
 ## Version 0.5.0
 
 **⚠️Breaking Change⚠️**: Incompatible API changes.
 
 - Change: Move some constants inside {class}`~xepor.InterceptedAPI` to seperate enums: {func}`xepor.RouteType`, {func}`xepor.FlowMeta`. ([xepor/xepor@83128e8](https://github.com/xepor/xepor/commit/83128e81f8c181cd23363d27c76209b9de1c49eb))
 - Change: rename `reqtype` in {func}`xepor.InterceptedAPI.route` to `rtype`. The name there before is for historical reason. [xepor/xepor@c6c7e83](https://github.com/xepor/xepor/commit/c6c7e8319aef95de01a0f797d9bb2c01632b7609)
```

### Comparing `xepor-0.5.0/docs/conf.py` & `xepor-0.5.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
+import re
 import sys
 
 # -- Path setup --------------------------------------------------------------
 
 __location__ = os.path.dirname(__file__)
 
 # If extensions (or modules to document with autodoc) are in another directory,
@@ -253,8 +254,17 @@
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "flask": ("https://flask.palletsprojects.com/en/2.0.x/", None),
     "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
 
-print(f"loading configurations for {project} {version} ...", file=sys.stderr)
+# -- linkcheck event listener ------------------------------------------------
+def strip_github_anchor(app, url):
+    if url and (match := re.match(r"(https:\/\/github\.com\/[\w\d._-]+\/[\w\d._-]+\/blob\/.*?)#L\d+(?:-L\d+)?", url)) != None:
+        url = match.group(1)
+    return url
+
+def setup(app):
+    app.connect('linkcheck-process-uri', strip_github_anchor)
+
+print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `xepor-0.5.0/docs/readme.md` & `xepor-0.5.1/docs/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Python package](https://github.com/xepor/xepor/actions/workflows/python-package.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/python-package.yml)
+[![Unit Tests](https://github.com/xepor/xepor/actions/workflows/test.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/test.yml)
 [![PyPI-Server](https://img.shields.io/pypi/v/xepor.svg)](https://pypi.org/project/xepor/)
 ![PyPI - Status](https://img.shields.io/pypi/status/xepor)
 [![Documentation Status](https://readthedocs.org/projects/xepor/badge/?version=latest)](https://xepor.readthedocs.io/en/latest/?badge=latest)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
 
 # Xepor
@@ -30,14 +30,20 @@
 2. Sniffing traffic from specific device by iptables + transparent proxy, modify the payload with xepor on the fly.
 3. Cracking cloud based software license. See [examples/krisp/](https://github.com/xepor/xepor-examples/tree/main/krisp/) as an example.
 4. Write complicated web crawler in **\~100 lines of codes**. See [examples/polyv_scrapper/](https://github.com/xepor/xepor-examples/tree/main/polyv_scrapper/) as an example.
 5. ... and many more.
 
 SSL stripping is NOT provided by this project.
 
+# Installation
+
+```bash
+pip install xepor
+```
+
 # Quick start
 
 Take the script from [examples/httpbin](https://github.com/xepor/xepor-examples/tree/main/httpbin/) as an example.
 
 ```bash
 mitmweb --web-host=\* --set connection_strategy=lazy -s example/httpbin/httpbin.py
 ```
@@ -88,8 +94,7 @@
         f"Captured {'successful' if flow.response.status_code < 300 else 'unsuccessful'} login:",
         flow.request.headers.get("Authorization", ""),
     )
 
 
 addons = [api]
 ```
-
```

### Comparing `xepor-0.5.0/setup.cfg` & `xepor-0.5.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,18 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	importlib-metadata; python_version<"3.8"
-	mitmproxy>=7.0.0,<9.0.0
-	parse>=1.19.0
+	mitmproxy>=7.0.0,<10.0.0
+	parse>=1.19.0,<2.0.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `xepor-0.5.0/setup.py` & `xepor-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/src/xepor/xepor.py` & `xepor-0.5.1/src/xepor/xepor.py`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/src/xepor.egg-info/PKG-INFO` & `xepor-0.5.1/src/xepor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xepor
-Version: 0.5.0
+Version: 0.5.1
 Summary: Xepor, a web routing framework for reverse engineers and security researchers.
 Home-page: https://github.com/xepor/xepor
 Author: ttimasdf
 Author-email: opensource@rabit.pw
 License: Apache-2.0
 Project-URL: Documentation, https://xepor.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/xepor/xepor
@@ -25,20 +25,20 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-[![Python package](https://github.com/xepor/xepor/actions/workflows/python-package.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/python-package.yml)
+[![Unit Tests](https://github.com/xepor/xepor/actions/workflows/test.yml/badge.svg)](https://github.com/xepor/xepor/actions/workflows/test.yml)
 [![PyPI-Server](https://img.shields.io/pypi/v/xepor.svg)](https://pypi.org/project/xepor/)
 ![PyPI - Status](https://img.shields.io/pypi/status/xepor)
 [![Documentation Status](https://readthedocs.org/projects/xepor/badge/?version=latest)](https://xepor.readthedocs.io/en/latest/?badge=latest)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)
 
 # Xepor
@@ -66,14 +66,20 @@
 2. Sniffing traffic from specific device by iptables + transparent proxy, modify the payload with xepor on the fly.
 3. Cracking cloud based software license. See [examples/krisp/](https://github.com/xepor/xepor-examples/tree/main/krisp/) as an example.
 4. Write complicated web crawler in **\~100 lines of codes**. See [examples/polyv_scrapper/](https://github.com/xepor/xepor-examples/tree/main/polyv_scrapper/) as an example.
 5. ... and many more.
 
 SSL stripping is NOT provided by this project.
 
+# Installation
+
+```bash
+pip install xepor
+```
+
 # Quick start
 
 Take the script from [examples/httpbin](https://github.com/xepor/xepor-examples/tree/main/httpbin/) as an example.
 
 ```bash
 mitmweb --web-host=\* --set connection_strategy=lazy -s example/httpbin/httpbin.py
 ```
@@ -124,10 +130,7 @@
         f"Captured {'successful' if flow.response.status_code < 300 else 'unsuccessful'} login:",
         flow.request.headers.get("Authorization", ""),
     )
 
 
 addons = [api]
 ```
-
-
-
```

### Comparing `xepor-0.5.0/src/xepor.egg-info/SOURCES.txt` & `xepor-0.5.1/src/xepor.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 .coveragerc
 .gitignore
 .gitlab-ci.yml
 .gitmodules
+.pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.rst
 LICENSE
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
-.github/workflows/python-package.yml
+.github/workflows/build.yml
+.github/workflows/test.yml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
 docs/conf.py
 docs/contributing.rst
 docs/index.md
 docs/license.rst
```

### Comparing `xepor-0.5.0/tests/conftest.py` & `xepor-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/tests/test_examples.py` & `xepor-0.5.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/tests/test_single.py` & `xepor-0.5.1/tests/test_single.py`

 * *Files identical despite different names*

### Comparing `xepor-0.5.0/tox.ini` & `xepor-0.5.1/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,97 @@
 # Tox configuration file
 # Read more under https://tox.wiki/
 # THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 [tox]
-minversion = 3.15
-envlist = mitmproxy7,mitmproxy8
+minversion = 3.24
+envlist = py{38,39,310,311,312}-mitmproxy{7,8},py{39,310,311,312}-mitmproxy9
 isolated_build = True
 
 
 [testenv]
+basepython =
+    py38: python3.8
+    py39: python3.9
+    py310: python3.10
+    py311: python3.11
+    py312: python3.12
+    docs: python3.11
+    lint: python3.11
+
 description = Invoke pytest to run automated tests
 deps =
     mitmproxy7: mitmproxy>=7.0.0,<8.0.0
     mitmproxy8: mitmproxy>=8.0.0,<9.0.0
+    mitmproxy9: mitmproxy>=9.0.0,<10.0.0
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
 extras =
     testing
 commands =
     pytest {posargs}
 
+# To run `tox -e lint` you need to make sure you have a
+# `.pre-commit-config.yaml` file. See https://pre-commit.com
+[testenv:lint]
+description = Perform static analysis and style checks
+skip_install = True
+deps = pre-commit
+passenv =
+    HOMEPATH
+    PROGRAMDATA
+commands =
+    pre-commit run --all-files {posargs:--show-diff-on-failure}
 
 [testenv:{build,clean}]
 description =
     build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
     clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
 # https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
 skip_install = True
 changedir = {toxinidir}
 deps =
     build: build[virtualenv]
+passenv =
+    SETUPTOOLS_SCM_PRETEND_VERSION
 commands =
-    clean: python -c 'from shutil import rmtree; rmtree("build", True); rmtree("dist", True)'
+    clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
+    clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
     build: python -m build {posargs}
 
 
-[testenv:{docs,apidoc,doctests,linkcheck}]
+[testenv:{docs,doctests,linkcheck}]
 description =
     docs: Invoke sphinx-build to build the docs
-    apidoc: Invoke sphinx-apidoc to build the API docs
     doctests: Invoke sphinx-build to run doctests
     linkcheck: Check for broken links in the documentation
 setenv =
     DOCSDIR = {toxinidir}/docs
     BUILDDIR = {toxinidir}/docs/_build
     docs: BUILD = html
     doctests: BUILD = doctest
     linkcheck: BUILD = linkcheck
 deps =
     -r {toxinidir}/docs/requirements.txt
     # ^  requirements.txt shared with Read The Docs
 commands =
-    apidoc: sphinx-apidoc --implicit-namespaces -f -o "{env:DOCSDIR}/api" "{toxinidir}/src"
     sphinx-build --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
 
 
 [testenv:publish]
 description =
     Publish the package you have been developing to a package index server.
     By default, it uses testpypi. If you really want to publish your package
     to be publicly accessible in PyPI, use the `-- --repository pypi` option.
 skip_install = True
 changedir = {toxinidir}
 passenv =
+    # See: https://twine.readthedocs.io/en/latest/
     TWINE_USERNAME
     TWINE_PASSWORD
     TWINE_REPOSITORY
 deps = twine
 commands =
     python -m twine check dist/*
-    python -m twine upload {posargs:--repository testpypi} dist/*
+    python -m twine upload {posargs:--repository {env:TWINE_REPOSITORY:testpypi}} dist/*
```

