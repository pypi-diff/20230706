# Comparing `tmp/lummao-0.5.0.tar.gz` & `tmp/lummao-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lummao-0.5.0.tar", last modified: Thu Jul  6 02:11:57 2023, max compression
+gzip compressed data, was "lummao-0.5.1.tar", last modified: Thu Jul  6 06:41:25 2023, max compression
```

## Comparing `lummao-0.5.0.tar` & `lummao-0.5.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.436658 lummao-0.5.0/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.384896 lummao-0.5.0/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.396391 lummao-0.5.0/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     2096 2023-07-06 02:10:34.000000 lummao-0.5.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner     (501) staff       (20)     1994 2023-07-06 02:10:34.000000 lummao-0.5.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner     (501) staff       (20)      177 2023-07-06 02:10:34.000000 lummao-0.5.0/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)    35149 2023-07-06 02:10:34.000000 lummao-0.5.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      276 2023-07-06 02:10:34.000000 lummao-0.5.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3603 2023-07-06 02:11:57.436888 lummao-0.5.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3252 2023-07-06 02:10:34.000000 lummao-0.5.0/README.md
--rw-r--r--   0 runner     (501) staff       (20)     5179 2023-07-06 02:10:34.000000 lummao-0.5.0/autobuild.xml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.396981 lummao-0.5.0/extern/
--rw-r--r--   0 runner     (501) staff       (20)   907858 2023-07-06 02:10:34.000000 lummao-0.5.0/extern/json.hh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.403378 lummao-0.5.0/extras/
--rw-r--r--   0 runner     (501) staff       (20)       11 2023-07-06 02:10:34.000000 lummao-0.5.0/extras/README.md
--rwxr-xr-x   0 runner     (501) staff       (20)      268 2023-07-06 02:10:34.000000 lummao-0.5.0/extras/hello_shellsl.lsl
--rw-r--r--   0 runner     (501) staff       (20)     5162 2023-07-06 02:10:34.000000 lummao-0.5.0/extras/lslwsgi.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2486 2023-07-06 02:10:34.000000 lummao-0.5.0/extras/shellsl
--rw-r--r--   0 runner     (501) staff       (20)     1254 2023-07-06 02:10:34.000000 lummao-0.5.0/extras/web_server.lsl
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.407405 lummao-0.5.0/lummao/
--rw-r--r--   0 runner     (501) staff       (20)     1605 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      575 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/cli.py
--rw-r--r--   0 runner     (501) staff       (20)      388 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)     4459 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/goto.py
--rw-r--r--   0 runner     (501) staff       (20)     1840 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/http.py
--rw-r--r--   0 runner     (501) staff       (20)    14879 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/lslexecutils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.412463 lummao-0.5.0/lummao/vendor/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.419607 lummao-0.5.0/lummao/vendor/lslopt/
--rw-r--r--   0 runner     (501) staff       (20)    35147 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/COPYING
--rw-r--r--   0 runner     (501) staff       (20)      267 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/README.md
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    74695 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/lslbasefuncs.py
--rw-r--r--   0 runner     (501) staff       (20)     4362 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/lslcommon.py
--rw-r--r--   0 runner     (501) staff       (20)    10688 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/lslextrafuncs.py
--rw-r--r--   0 runner     (501) staff       (20)      933 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/lslfuncs.py
--rw-r--r--   0 runner     (501) staff       (20)    24163 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/lsljson.py
--rw-r--r--   0 runner     (501) staff       (20)     3394 2023-07-06 02:10:35.000000 lummao-0.5.0/lummao/vendor/lslopt/strutil.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.411867 lummao-0.5.0/lummao.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3603 2023-07-06 02:11:57.000000 lummao-0.5.0/lummao.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1745 2023-07-06 02:11:57.000000 lummao-0.5.0/lummao.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-06 02:11:57.000000 lummao-0.5.0/lummao.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       47 2023-07-06 02:11:57.000000 lummao-0.5.0/lummao.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-06 02:11:57.000000 lummao-0.5.0/lummao.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-06 02:11:57.000000 lummao-0.5.0/lummao.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2023-07-06 02:11:57.000000 lummao-0.5.0/lummao.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      157 2023-07-06 02:10:35.000000 lummao-0.5.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       53 2023-07-06 02:10:35.000000 lummao-0.5.0/requirements-test.txt
--rw-r--r--   0 runner     (501) staff       (20)      262 2023-07-06 02:11:57.438001 lummao-0.5.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2784 2023-07-06 02:10:35.000000 lummao-0.5.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.423085 lummao-0.5.0/src/
--rw-r--r--   0 runner     (501) staff       (20)     3629 2023-07-06 02:10:35.000000 lummao-0.5.0/src/compiler.cc
--rw-r--r--   0 runner     (501) staff       (20)    22825 2023-07-06 02:10:35.000000 lummao-0.5.0/src/json_ir_pass.cc
--rw-r--r--   0 runner     (501) staff       (20)     4211 2023-07-06 02:10:35.000000 lummao-0.5.0/src/json_ir_pass.hh
--rw-r--r--   0 runner     (501) staff       (20)    23791 2023-07-06 02:10:35.000000 lummao-0.5.0/src/python_pass.cc
--rw-r--r--   0 runner     (501) staff       (20)     2723 2023-07-06 02:10:35.000000 lummao-0.5.0/src/python_pass.hh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.425056 lummao-0.5.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-06 02:10:35.000000 lummao-0.5.0/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1736 2023-07-06 02:10:35.000000 lummao-0.5.0/tests/test_conformance.py
--rw-r--r--   0 runner     (501) staff       (20)     4372 2023-07-06 02:10:35.000000 lummao-0.5.0/tests/test_harnesses.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-06 02:11:57.436159 lummao-0.5.0/tests/test_resources/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-06 02:10:35.000000 lummao-0.5.0/tests/test_resources/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      229 2023-07-06 02:10:35.000000 lummao-0.5.0/tests/test_resources/continue_like_jump_with_ret.lsl
--rw-r--r--   0 runner     (501) staff       (20)      136 2023-07-06 02:10:35.000000 lummao-0.5.0/tests/test_resources/detected_touch.lsl
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-07-06 02:10:35.000000 lummao-0.5.0/tests/test_resources/function_mocking.lsl
--rw-r--r--   0 runner     (501) staff       (20)      253 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/hoist_decl_unstructured_jump.lsl
--rw-r--r--   0 runner     (501) staff       (20)      477 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/http_request.lsl
--rw-r--r--   0 runner     (501) staff       (20)       95 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/jump_out_of_while_true.lsl
--rw-r--r--   0 runner     (501) staff       (20)    20547 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/lsl_conformance.lsl
--rw-r--r--   0 runner     (501) staff       (20)    26804 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/lsl_conformance.py
--rw-r--r--   0 runner     (501) staff       (20)    13851 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/lsl_conformance2.lsl
--rw-r--r--   0 runner     (501) staff       (20)    18444 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/lsl_conformance2.py
--rw-r--r--   0 runner     (501) staff       (20)       62 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/one_error.lsl
--rw-r--r--   0 runner     (501) staff       (20)      153 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/statements.lsl
--rw-r--r--   0 runner     (501) staff       (20)      310 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/statements.py
--rw-r--r--   0 runner     (501) staff       (20)      182 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/timers.lsl
--rw-r--r--   0 runner     (501) staff       (20)       86 2023-07-06 02:10:36.000000 lummao-0.5.0/tests/test_resources/two_errors.lsl
--rw-r--r--   0 runner     (501) staff       (20)      142 2023-07-06 02:10:36.000000 lummao-0.5.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:25.716251 lummao-0.5.1/
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.937569 lummao-0.5.1/.github/
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.953194 lummao-0.5.1/.github/workflows/
+-rw-rw-rw-   0        0        0     2096 2023-07-06 06:41:08.000000 lummao-0.5.1/.github/workflows/pypi_publish.yml
+-rw-rw-rw-   0        0        0     1994 2023-07-06 06:41:08.000000 lummao-0.5.1/.github/workflows/pytest.yml
+-rw-rw-rw-   0        0        0      177 2023-07-06 06:41:08.000000 lummao-0.5.1/.gitignore
+-rw-rw-rw-   0        0        0    35149 2023-07-06 06:41:08.000000 lummao-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-07-06 06:41:08.000000 lummao-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3929 2023-07-06 06:41:25.716251 lummao-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3490 2023-07-06 06:41:08.000000 lummao-0.5.1/README.md
+-rw-rw-rw-   0        0        0     5179 2023-07-06 06:41:08.000000 lummao-0.5.1/autobuild.xml
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.953194 lummao-0.5.1/extern/
+-rw-rw-rw-   0        0        0   907858 2023-07-06 06:41:08.000000 lummao-0.5.1/extern/json.hh
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.953194 lummao-0.5.1/extras/
+-rw-rw-rw-   0        0        0       11 2023-07-06 06:41:08.000000 lummao-0.5.1/extras/README.md
+-rw-rw-rw-   0        0        0      255 2023-07-06 06:41:08.000000 lummao-0.5.1/extras/hello_shellsl.lsl
+-rw-rw-rw-   0        0        0     5143 2023-07-06 06:41:08.000000 lummao-0.5.1/extras/lslwsgi.py
+-rw-rw-rw-   0        0        0     1254 2023-07-06 06:41:08.000000 lummao-0.5.1/extras/web_server.lsl
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.968822 lummao-0.5.1/lummao/
+-rw-rw-rw-   0        0        0     1605 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/__init__.py
+-rw-rw-rw-   0        0        0      575 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/cli.py
+-rw-rw-rw-   0        0        0      388 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/exceptions.py
+-rw-rw-rw-   0        0        0     4459 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/goto.py
+-rw-rw-rw-   0        0        0     1840 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/http.py
+-rw-rw-rw-   0        0        0    14879 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/lslexecutils.py
+-rw-rw-rw-   0        0        0     2490 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/shellsl.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.968822 lummao-0.5.1/lummao/vendor/
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.968822 lummao-0.5.1/lummao/vendor/lslopt/
+-rw-rw-rw-   0        0        0    35147 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/COPYING
+-rw-rw-rw-   0        0        0      267 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/README.md
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/__init__.py
+-rw-rw-rw-   0        0        0    74695 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/lslbasefuncs.py
+-rw-rw-rw-   0        0        0     4362 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/lslcommon.py
+-rw-rw-rw-   0        0        0    10688 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/lslextrafuncs.py
+-rw-rw-rw-   0        0        0      933 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/lslfuncs.py
+-rw-rw-rw-   0        0        0    24163 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/lsljson.py
+-rw-rw-rw-   0        0        0     3394 2023-07-06 06:41:08.000000 lummao-0.5.1/lummao/vendor/lslopt/strutil.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.968822 lummao-0.5.1/lummao.egg-info/
+-rw-rw-rw-   0        0        0     3929 2023-07-06 06:41:24.000000 lummao-0.5.1/lummao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1748 2023-07-06 06:41:24.000000 lummao-0.5.1/lummao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:41:24.000000 lummao-0.5.1/lummao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-06 06:41:24.000000 lummao-0.5.1/lummao.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 06:41:24.000000 lummao-0.5.1/lummao.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2023-07-06 06:41:24.000000 lummao-0.5.1/lummao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 06:41:24.000000 lummao-0.5.1/lummao.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      157 2023-07-06 06:41:08.000000 lummao-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-07-06 06:41:08.000000 lummao-0.5.1/requirements-test.txt
+-rw-rw-rw-   0        0        0      274 2023-07-06 06:41:25.716251 lummao-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2837 2023-07-06 06:41:08.000000 lummao-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.984443 lummao-0.5.1/src/
+-rw-rw-rw-   0        0        0     3629 2023-07-06 06:41:08.000000 lummao-0.5.1/src/compiler.cc
+-rw-rw-rw-   0        0        0    22825 2023-07-06 06:41:08.000000 lummao-0.5.1/src/json_ir_pass.cc
+-rw-rw-rw-   0        0        0     4211 2023-07-06 06:41:08.000000 lummao-0.5.1/src/json_ir_pass.hh
+-rw-rw-rw-   0        0        0    23791 2023-07-06 06:41:08.000000 lummao-0.5.1/src/python_pass.cc
+-rw-rw-rw-   0        0        0     2723 2023-07-06 06:41:08.000000 lummao-0.5.1/src/python_pass.hh
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:24.984443 lummao-0.5.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1736 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_conformance.py
+-rw-rw-rw-   0        0        0     4372 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_harnesses.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:41:25.716251 lummao-0.5.1/tests/test_resources/
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/__init__.py
+-rw-rw-rw-   0        0        0      229 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/continue_like_jump_with_ret.lsl
+-rw-rw-rw-   0        0        0      136 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/detected_touch.lsl
+-rw-rw-rw-   0        0        0       84 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/function_mocking.lsl
+-rw-rw-rw-   0        0        0      253 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/hoist_decl_unstructured_jump.lsl
+-rw-rw-rw-   0        0        0      477 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/http_request.lsl
+-rw-rw-rw-   0        0        0       95 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/jump_out_of_while_true.lsl
+-rw-rw-rw-   0        0        0    20547 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/lsl_conformance.lsl
+-rw-rw-rw-   0        0        0    26804 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/lsl_conformance.py
+-rw-rw-rw-   0        0        0    13851 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/lsl_conformance2.lsl
+-rw-rw-rw-   0        0        0    18444 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/lsl_conformance2.py
+-rw-rw-rw-   0        0        0       62 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/one_error.lsl
+-rw-rw-rw-   0        0        0      153 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/statements.lsl
+-rw-rw-rw-   0        0        0      310 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/statements.py
+-rw-rw-rw-   0        0        0      182 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/timers.lsl
+-rw-rw-rw-   0        0        0       86 2023-07-06 06:41:08.000000 lummao-0.5.1/tests/test_resources/two_errors.lsl
+-rw-rw-rw-   0        0        0      142 2023-07-06 06:41:08.000000 lummao-0.5.1/tox.ini
```

### Comparing `lummao-0.5.0/.github/workflows/pypi_publish.yml` & `lummao-0.5.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/.github/workflows/pytest.yml` & `lummao-0.5.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/LICENSE` & `lummao-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/PKG-INFO` & `lummao-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: lummao
-Version: 0.5.0
-Summary: Toolkit for compiling and executing the Linden Scripting Language as Python
-Home-page: https://github.com/SaladDais/Lummao
-Author: Salad Dais
-Author-email: SaladDais@users.noreply.github.com
-License: GPLv3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Lummao
 
 [Lummao](https://github.com/SaladDais/Lummao) is a toolkit for compiling and executing the Linden Scripting Language as Python. 
 It aims to ease testing of LSL code by leveraging Python's existing ecosystem for debugging and testing. Think of it as the less opinionated,
 stupider cousin of [LSLForge's unit testing framework](https://github.com/raysilent/lslforge/blob/master/lslforge/eclipse/lslforge/html/unit-test.html).
 
 The runtime is largely handled by the excellent implementation of LSL's basic operations and library functions
@@ -33,34 +21,40 @@
 
 ```bash
 pip install -e .
 ```
 
 ## How
 
-For a real-world example, see <https://github.com/SaladDais/SLGraphPather> or <https://github.com/SaladDais/SickJoke>'s
-tests and test coverage reporting.
+For a real-world example of local LSL testing with Lummao, see <https://github.com/SaladDais/SLGraphPather> or
+<https://github.com/SaladDais/SickJoke>'s tests and test coverage reporting.
 
 Along with the python API, a helper `lummao` script is provided that takes in an LSL file and outputs a python file.
 It can be invoked like `lummao input.lsl output.py`.
 
+If you just want to run an LSL script from the command-line, the `shellsl` command will be installed alongside `lummao`,
+and can be run from the commandline like so:
+
+```
+$ shellsl tests/test_resources/lsl_conformance.lsl
+All tests passed
+```
+
 ## Why
 
 If you've ever written a sufficiently complicated system in LSL, you know how annoying it is to debug your scripts
 or be sure if they're even correct. Clearly the sanest way to bring sanity to your workflow is to convert your LSL
-scripts to Python, so you can mock LSL library functions and use Python debuggers. Hence the name "Lummao".
+scripts to Python, so you can mock LSL library functions and use Python debuggers. Hence, the name "Lummao".
 
 ## TODO
 
 * Symbol shadowing behavior is not correct. Python has very different shadowing rules.
 * Provide mock helpers for: 
 * * inter-script communication
-* * HTTP
 * * auto-stubs for all functions
-* * state-aware event queueing
 
 ## License
 
 GPLv3
 
 ### Licensing Clarifications
```

### Comparing `lummao-0.5.0/README.md` & `lummao-0.5.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,88 @@
-# Lummao
-
-[Lummao](https://github.com/SaladDais/Lummao) is a toolkit for compiling and executing the Linden Scripting Language as Python. 
-It aims to ease testing of LSL code by leveraging Python's existing ecosystem for debugging and testing. Think of it as the less opinionated,
-stupider cousin of [LSLForge's unit testing framework](https://github.com/raysilent/lslforge/blob/master/lslforge/eclipse/lslforge/html/unit-test.html).
-
-The runtime is largely handled by the excellent implementation of LSL's basic operations and library functions
-from Sei Lisa's [LSL-PyOptimizer](https://github.com/Sei-Lisa/LSL-PyOptimizer).
-See [vendor/lslopt](https://github.com/SaladDais/Lummao/tree/master/lummao/vendor/lslopt) for Lummao's vendored copy of LSL-Pyoptimizer.
-
-To see an example input script and its Python output, see the [`test_resources` directory](https://github.com/SaladDais/Lummao/tree/master/tests/test_resources).
-
-## Setup
-
-```bash
-pip install --upgrade pip
-pip install lummao
-```
-
-### From source
-
-```bash
-pip install -e .
-```
-
-## How
-
-For a real-world example, see <https://github.com/SaladDais/SLGraphPather> or <https://github.com/SaladDais/SickJoke>'s
-tests and test coverage reporting.
-
-Along with the python API, a helper `lummao` script is provided that takes in an LSL file and outputs a python file.
-It can be invoked like `lummao input.lsl output.py`.
-
-## Why
-
-If you've ever written a sufficiently complicated system in LSL, you know how annoying it is to debug your scripts
-or be sure if they're even correct. Clearly the sanest way to bring sanity to your workflow is to convert your LSL
-scripts to Python, so you can mock LSL library functions and use Python debuggers. Hence the name "Lummao".
-
-## TODO
-
-* Symbol shadowing behavior is not correct. Python has very different shadowing rules.
-* Provide mock helpers for: 
-* * inter-script communication
-* * HTTP
-* * auto-stubs for all functions
-* * state-aware event queueing
-
-## License
-
-GPLv3
-
-### Licensing Clarifications
-
-The output of the compiler necessarily links against the GPL-licensed runtime code from LSL-PyOptimizer for
-functionality, and LSL-PyOptimizer does not provide a library exception in its license.
-You should assume that any LSL converted to Python by the compiler and any testcases you write exercising
-them must _also_ be distributable under the GPL.
-
-In short: If or when you distribute your testcases, you must _also_ allow distribution of their direct
-dependencies (your LSL scripts) under the terms of the GPL. This does not necessarily
-change the license of your LSL scripts themselves, or require consumers of your scripts to license
-their own scripts under the GPL. It is perfectly possible to have an otherwise MIT-licensed or proprietary
-library with a GPL-licensed test suite. No distribution of testcases == no requirement to distribute under the GPL.
-
-Suggested reading to understand your rights and obligations under the GPL when using a GPL-licensed test suite:
-
-* https://www.gnu.org/licenses/gpl-3.0.html
-* https://opensource.stackexchange.com/questions/7503/implications-of-using-gpl-licenced-code-only-during-testing
-* https://opensource.stackexchange.com/questions/4112/using-gpl-library-in-unit-test-suite-of-open-source-library
+Metadata-Version: 2.1
+Name: lummao
+Version: 0.5.1
+Summary: Toolkit for compiling and executing the Linden Scripting Language as Python
+Home-page: https://github.com/SaladDais/Lummao
+Author: Salad Dais
+Author-email: SaladDais@users.noreply.github.com
+License: GPLv3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Lummao
+
+[Lummao](https://github.com/SaladDais/Lummao) is a toolkit for compiling and executing the Linden Scripting Language as Python. 
+It aims to ease testing of LSL code by leveraging Python's existing ecosystem for debugging and testing. Think of it as the less opinionated,
+stupider cousin of [LSLForge's unit testing framework](https://github.com/raysilent/lslforge/blob/master/lslforge/eclipse/lslforge/html/unit-test.html).
+
+The runtime is largely handled by the excellent implementation of LSL's basic operations and library functions
+from Sei Lisa's [LSL-PyOptimizer](https://github.com/Sei-Lisa/LSL-PyOptimizer).
+See [vendor/lslopt](https://github.com/SaladDais/Lummao/tree/master/lummao/vendor/lslopt) for Lummao's vendored copy of LSL-Pyoptimizer.
+
+To see an example input script and its Python output, see the [`test_resources` directory](https://github.com/SaladDais/Lummao/tree/master/tests/test_resources).
+
+## Setup
+
+```bash
+pip install --upgrade pip
+pip install lummao
+```
+
+### From source
+
+```bash
+pip install -e .
+```
+
+## How
+
+For a real-world example of local LSL testing with Lummao, see <https://github.com/SaladDais/SLGraphPather> or
+<https://github.com/SaladDais/SickJoke>'s tests and test coverage reporting.
+
+Along with the python API, a helper `lummao` script is provided that takes in an LSL file and outputs a python file.
+It can be invoked like `lummao input.lsl output.py`.
+
+If you just want to run an LSL script from the command-line, the `shellsl` command will be installed alongside `lummao`,
+and can be run from the commandline like so:
+
+```
+$ shellsl tests/test_resources/lsl_conformance.lsl
+All tests passed
+```
+
+## Why
+
+If you've ever written a sufficiently complicated system in LSL, you know how annoying it is to debug your scripts
+or be sure if they're even correct. Clearly the sanest way to bring sanity to your workflow is to convert your LSL
+scripts to Python, so you can mock LSL library functions and use Python debuggers. Hence, the name "Lummao".
+
+## TODO
+
+* Symbol shadowing behavior is not correct. Python has very different shadowing rules.
+* Provide mock helpers for: 
+* * inter-script communication
+* * auto-stubs for all functions
+
+## License
+
+GPLv3
+
+### Licensing Clarifications
+
+The output of the compiler necessarily links against the GPL-licensed runtime code from LSL-PyOptimizer for
+functionality, and LSL-PyOptimizer does not provide a library exception in its license.
+You should assume that any LSL converted to Python by the compiler and any testcases you write exercising
+them must _also_ be distributable under the GPL.
+
+In short: If or when you distribute your testcases, you must _also_ allow distribution of their direct
+dependencies (your LSL scripts) under the terms of the GPL. This does not necessarily
+change the license of your LSL scripts themselves, or require consumers of your scripts to license
+their own scripts under the GPL. It is perfectly possible to have an otherwise MIT-licensed or proprietary
+library with a GPL-licensed test suite. No distribution of testcases == no requirement to distribute under the GPL.
+
+Suggested reading to understand your rights and obligations under the GPL when using a GPL-licensed test suite:
+
+* https://www.gnu.org/licenses/gpl-3.0.html
+* https://opensource.stackexchange.com/questions/7503/implications-of-using-gpl-licenced-code-only-during-testing
+* https://opensource.stackexchange.com/questions/4112/using-gpl-library-in-unit-test-suite-of-open-source-library
```

### Comparing `lummao-0.5.0/autobuild.xml` & `lummao-0.5.1/autobuild.xml`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/extern/json.hh` & `lummao-0.5.1/extern/json.hh`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/extras/lslwsgi.py` & `lummao-0.5.1/extras/lslwsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,12 +125,11 @@
     app.before_request(wsgi_wrapper.handle_request)
     # Can't use reloader because it tries to reload the LSL!
     app.run(
         host=os.environ.get("SERVER_NAME", "localhost"),
         port=_get_server_port(),
         use_reloader=False,
     )
-    app.run_task()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lummao-0.5.0/extras/shellsl` & `lummao-0.5.1/lummao/shellsl.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         stdout, stderr = p.communicate()
         if stderr:
             print(stderr.decode("utf8"), file=sys.stderr)
         self.script.cashquery = p.returncode
         return stdout.decode("utf8").rstrip("\n")
 
 
-async def main():
+def shellsl_main():
     with open(sys.argv[1], "rb") as f:
         lsl_bytes = f.read()
     # replace shebang line if present
     if lsl_bytes.startswith(b"#!"):
         lsl_bytes = b"\n" + b"\n".join(lsl_bytes.split(b"\n")[1:])
     script = lummao.compile_script(LSL_HEADER + lsl_bytes)
 
@@ -65,12 +65,12 @@
     http_extender = HTTPRequestScriptExtender()
     http_extender.extend_script(script)
     timer_extender = TimerScriptExtender()
     timer_extender.extend_script(script)
     datetime_extender = DateTimeScriptExtender()
     datetime_extender.extend_script(script)
 
-    await script.execute_until_complete()
+    asyncio.run(script.execute_until_complete())
 
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    shellsl_main()
```

### Comparing `lummao-0.5.0/extras/web_server.lsl` & `lummao-0.5.1/extras/web_server.lsl`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/__init__.py` & `lummao-0.5.1/lummao/__init__.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/cli.py` & `lummao-0.5.1/lummao/cli.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/goto.py` & `lummao-0.5.1/lummao/goto.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/http.py` & `lummao-0.5.1/lummao/http.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/lslexecutils.py` & `lummao-0.5.1/lummao/lslexecutils.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/vendor/lslopt/COPYING` & `lummao-0.5.1/lummao/vendor/lslopt/COPYING`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/vendor/lslopt/lslbasefuncs.py` & `lummao-0.5.1/lummao/vendor/lslopt/lslbasefuncs.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/vendor/lslopt/lslcommon.py` & `lummao-0.5.1/lummao/vendor/lslopt/lslcommon.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/vendor/lslopt/lslextrafuncs.py` & `lummao-0.5.1/lummao/vendor/lslopt/lslextrafuncs.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/vendor/lslopt/lslfuncs.py` & `lummao-0.5.1/lummao/vendor/lslopt/lslfuncs.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/vendor/lslopt/lsljson.py` & `lummao-0.5.1/lummao/vendor/lslopt/lsljson.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao/vendor/lslopt/strutil.py` & `lummao-0.5.1/lummao/vendor/lslopt/strutil.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/lummao.egg-info/PKG-INFO` & `lummao-0.5.1/lummao.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,88 @@
-Metadata-Version: 2.1
-Name: lummao
-Version: 0.5.0
-Summary: Toolkit for compiling and executing the Linden Scripting Language as Python
-Home-page: https://github.com/SaladDais/Lummao
-Author: Salad Dais
-Author-email: SaladDais@users.noreply.github.com
-License: GPLv3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Lummao
-
-[Lummao](https://github.com/SaladDais/Lummao) is a toolkit for compiling and executing the Linden Scripting Language as Python. 
-It aims to ease testing of LSL code by leveraging Python's existing ecosystem for debugging and testing. Think of it as the less opinionated,
-stupider cousin of [LSLForge's unit testing framework](https://github.com/raysilent/lslforge/blob/master/lslforge/eclipse/lslforge/html/unit-test.html).
-
-The runtime is largely handled by the excellent implementation of LSL's basic operations and library functions
-from Sei Lisa's [LSL-PyOptimizer](https://github.com/Sei-Lisa/LSL-PyOptimizer).
-See [vendor/lslopt](https://github.com/SaladDais/Lummao/tree/master/lummao/vendor/lslopt) for Lummao's vendored copy of LSL-Pyoptimizer.
-
-To see an example input script and its Python output, see the [`test_resources` directory](https://github.com/SaladDais/Lummao/tree/master/tests/test_resources).
-
-## Setup
-
-```bash
-pip install --upgrade pip
-pip install lummao
-```
-
-### From source
-
-```bash
-pip install -e .
-```
-
-## How
-
-For a real-world example, see <https://github.com/SaladDais/SLGraphPather> or <https://github.com/SaladDais/SickJoke>'s
-tests and test coverage reporting.
-
-Along with the python API, a helper `lummao` script is provided that takes in an LSL file and outputs a python file.
-It can be invoked like `lummao input.lsl output.py`.
-
-## Why
-
-If you've ever written a sufficiently complicated system in LSL, you know how annoying it is to debug your scripts
-or be sure if they're even correct. Clearly the sanest way to bring sanity to your workflow is to convert your LSL
-scripts to Python, so you can mock LSL library functions and use Python debuggers. Hence the name "Lummao".
-
-## TODO
-
-* Symbol shadowing behavior is not correct. Python has very different shadowing rules.
-* Provide mock helpers for: 
-* * inter-script communication
-* * HTTP
-* * auto-stubs for all functions
-* * state-aware event queueing
-
-## License
-
-GPLv3
-
-### Licensing Clarifications
-
-The output of the compiler necessarily links against the GPL-licensed runtime code from LSL-PyOptimizer for
-functionality, and LSL-PyOptimizer does not provide a library exception in its license.
-You should assume that any LSL converted to Python by the compiler and any testcases you write exercising
-them must _also_ be distributable under the GPL.
-
-In short: If or when you distribute your testcases, you must _also_ allow distribution of their direct
-dependencies (your LSL scripts) under the terms of the GPL. This does not necessarily
-change the license of your LSL scripts themselves, or require consumers of your scripts to license
-their own scripts under the GPL. It is perfectly possible to have an otherwise MIT-licensed or proprietary
-library with a GPL-licensed test suite. No distribution of testcases == no requirement to distribute under the GPL.
-
-Suggested reading to understand your rights and obligations under the GPL when using a GPL-licensed test suite:
-
-* https://www.gnu.org/licenses/gpl-3.0.html
-* https://opensource.stackexchange.com/questions/7503/implications-of-using-gpl-licenced-code-only-during-testing
-* https://opensource.stackexchange.com/questions/4112/using-gpl-library-in-unit-test-suite-of-open-source-library
+Metadata-Version: 2.1
+Name: lummao
+Version: 0.5.1
+Summary: Toolkit for compiling and executing the Linden Scripting Language as Python
+Home-page: https://github.com/SaladDais/Lummao
+Author: Salad Dais
+Author-email: SaladDais@users.noreply.github.com
+License: GPLv3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Lummao
+
+[Lummao](https://github.com/SaladDais/Lummao) is a toolkit for compiling and executing the Linden Scripting Language as Python. 
+It aims to ease testing of LSL code by leveraging Python's existing ecosystem for debugging and testing. Think of it as the less opinionated,
+stupider cousin of [LSLForge's unit testing framework](https://github.com/raysilent/lslforge/blob/master/lslforge/eclipse/lslforge/html/unit-test.html).
+
+The runtime is largely handled by the excellent implementation of LSL's basic operations and library functions
+from Sei Lisa's [LSL-PyOptimizer](https://github.com/Sei-Lisa/LSL-PyOptimizer).
+See [vendor/lslopt](https://github.com/SaladDais/Lummao/tree/master/lummao/vendor/lslopt) for Lummao's vendored copy of LSL-Pyoptimizer.
+
+To see an example input script and its Python output, see the [`test_resources` directory](https://github.com/SaladDais/Lummao/tree/master/tests/test_resources).
+
+## Setup
+
+```bash
+pip install --upgrade pip
+pip install lummao
+```
+
+### From source
+
+```bash
+pip install -e .
+```
+
+## How
+
+For a real-world example of local LSL testing with Lummao, see <https://github.com/SaladDais/SLGraphPather> or
+<https://github.com/SaladDais/SickJoke>'s tests and test coverage reporting.
+
+Along with the python API, a helper `lummao` script is provided that takes in an LSL file and outputs a python file.
+It can be invoked like `lummao input.lsl output.py`.
+
+If you just want to run an LSL script from the command-line, the `shellsl` command will be installed alongside `lummao`,
+and can be run from the commandline like so:
+
+```
+$ shellsl tests/test_resources/lsl_conformance.lsl
+All tests passed
+```
+
+## Why
+
+If you've ever written a sufficiently complicated system in LSL, you know how annoying it is to debug your scripts
+or be sure if they're even correct. Clearly the sanest way to bring sanity to your workflow is to convert your LSL
+scripts to Python, so you can mock LSL library functions and use Python debuggers. Hence, the name "Lummao".
+
+## TODO
+
+* Symbol shadowing behavior is not correct. Python has very different shadowing rules.
+* Provide mock helpers for: 
+* * inter-script communication
+* * auto-stubs for all functions
+
+## License
+
+GPLv3
+
+### Licensing Clarifications
+
+The output of the compiler necessarily links against the GPL-licensed runtime code from LSL-PyOptimizer for
+functionality, and LSL-PyOptimizer does not provide a library exception in its license.
+You should assume that any LSL converted to Python by the compiler and any testcases you write exercising
+them must _also_ be distributable under the GPL.
+
+In short: If or when you distribute your testcases, you must _also_ allow distribution of their direct
+dependencies (your LSL scripts) under the terms of the GPL. This does not necessarily
+change the license of your LSL scripts themselves, or require consumers of your scripts to license
+their own scripts under the GPL. It is perfectly possible to have an otherwise MIT-licensed or proprietary
+library with a GPL-licensed test suite. No distribution of testcases == no requirement to distribute under the GPL.
+
+Suggested reading to understand your rights and obligations under the GPL when using a GPL-licensed test suite:
+
+* https://www.gnu.org/licenses/gpl-3.0.html
+* https://opensource.stackexchange.com/questions/7503/implications-of-using-gpl-licenced-code-only-during-testing
+* https://opensource.stackexchange.com/questions/4112/using-gpl-library-in-unit-test-suite-of-open-source-library
```

### Comparing `lummao-0.5.0/lummao.egg-info/SOURCES.txt` & `lummao-0.5.1/lummao.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 tox.ini
 .github/workflows/pypi_publish.yml
 .github/workflows/pytest.yml
 extern/json.hh
 extras/README.md
 extras/hello_shellsl.lsl
 extras/lslwsgi.py
-extras/shellsl
 extras/web_server.lsl
 lummao/__init__.py
 lummao/cli.py
 lummao/exceptions.py
 lummao/goto.py
 lummao/http.py
 lummao/lslexecutils.py
+lummao/shellsl.py
 lummao.egg-info/PKG-INFO
 lummao.egg-info/SOURCES.txt
 lummao.egg-info/dependency_links.txt
 lummao.egg-info/entry_points.txt
 lummao.egg-info/not-zip-safe
 lummao.egg-info/requires.txt
 lummao.egg-info/top_level.txt
```

### Comparing `lummao-0.5.0/setup.py` & `lummao-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,10 +85,11 @@
             py_limited_api=True,
             autobuild_deps=["tailslide"],
         )
     ],
     entry_points={
         'console_scripts': {
             'lummao = lummao.cli:cli_main',
+            'shellsl = lummao.shellsl:shellsl_main',
         }
     },
 )
```

### Comparing `lummao-0.5.0/src/compiler.cc` & `lummao-0.5.1/src/compiler.cc`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/src/json_ir_pass.cc` & `lummao-0.5.1/src/json_ir_pass.cc`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/src/json_ir_pass.hh` & `lummao-0.5.1/src/json_ir_pass.hh`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/src/python_pass.cc` & `lummao-0.5.1/src/python_pass.cc`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/src/python_pass.hh` & `lummao-0.5.1/src/python_pass.hh`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/tests/test_conformance.py` & `lummao-0.5.1/tests/test_conformance.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/tests/test_harnesses.py` & `lummao-0.5.1/tests/test_harnesses.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/tests/test_resources/lsl_conformance.lsl` & `lummao-0.5.1/tests/test_resources/lsl_conformance.lsl`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/tests/test_resources/lsl_conformance.py` & `lummao-0.5.1/tests/test_resources/lsl_conformance.py`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/tests/test_resources/lsl_conformance2.lsl` & `lummao-0.5.1/tests/test_resources/lsl_conformance2.lsl`

 * *Files identical despite different names*

### Comparing `lummao-0.5.0/tests/test_resources/lsl_conformance2.py` & `lummao-0.5.1/tests/test_resources/lsl_conformance2.py`

 * *Files identical despite different names*

