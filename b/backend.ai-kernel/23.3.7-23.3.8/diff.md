# Comparing `tmp/backend.ai-kernel-23.3.7.tar.gz` & `tmp/backend.ai-kernel-23.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-23.3.7.tar", last modified: Mon Jul  3 16:26:21 2023, max compression
+gzip compressed data, was "backend.ai-kernel-23.3.8.tar", last modified: Thu Jul  6 04:38:09 2023, max compression
```

## Comparing `backend.ai-kernel-23.3.7.tar` & `backend.ai-kernel-23.3.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.918465 backend.ai-kernel-23.3.7/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.918465 backend.ai-kernel-23.3.7/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.922465 backend.ai-kernel-23.3.7/ai/backend/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.922465 backend.ai-kernel-23.3.7/ai/backend/kernel/app/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39380 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.922465 backend.ai-kernel-23.3.7/ai/backend/kernel/c/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.922465 backend.ai-kernel-23.3.7/ai/backend/kernel/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.922465 backend.ai-kernel-23.3.7/ai/backend/kernel/git/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.922465 backend.ai-kernel-23.3.7/ai/backend/kernel/golang/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/golang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.922465 backend.ai-kernel-23.3.7/ai/backend/kernel/haskell/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/haskell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/intrinsic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/java/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/julia/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/lua/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/lua/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/nodejs/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/nodejs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/octave/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/octave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/php/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/php/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/python/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/python/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/r/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/r/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/r_server_ms/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/r_server_ms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/rust/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/rust/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/service_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/aws_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/aws_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/aws_polly/inproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/h2o/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/h2o/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:26:21.926466 backend.ai-kernel-23.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-03 16:26:21.000000 backend.ai-kernel-23.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42169 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/golang/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/golang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/haskell/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/haskell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/intrinsic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.652316 backend.ai-kernel-23.3.8/ai/backend/kernel/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/lua/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/lua/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/nodejs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/nodejs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/octave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/octave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/php/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/php/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/python/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/r/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/r/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/r_server_ms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/r_server_ms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/rust/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/service_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/inproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/h2o/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/h2o/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:09.656317 backend.ai-kernel-23.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-06 04:38:09.000000 backend.ai-kernel-23.3.8/setup.py
```

### Comparing `backend.ai-kernel-23.3.7/PKG-INFO` & `backend.ai-kernel-23.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.7
+Version: 23.3.8
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/__main__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/app/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/app/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/base.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import concurrent.futures
 import json
 import logging
 import os
+import resource
 import signal
 import sys
 import time
 import urllib.error
 import urllib.request
 import uuid
 from abc import ABCMeta, abstractmethod
@@ -38,15 +39,15 @@
     init_sshd_service,
     prepare_sshd_service,
     prepare_ttyd_service,
 )
 from .jupyter_client import aexecute_interactive
 from .logging import BraceStyleAdapter, setup_logger
 from .service import ServiceParser
-from .utils import wait_local_port_open
+from .utils import scan_proc_stats, wait_local_port_open
 
 log = BraceStyleAdapter(logging.getLogger())
 
 
 async def pipe_output(stream, outsock, target, log_fd):
     assert target in ("stdout", "stderr")
     target = target.encode("ascii")
@@ -576,14 +577,68 @@
 
         The default interface is jupyter kernel. To use different interface,
         `Runner` subclass should implement its own `complete` method.
         """
         if hasattr(self, "kernel_mgr") and self.kernel_mgr is not None:
             await self.kernel_mgr.interrupt_kernel()
 
+    async def log_oom(self):
+        log.warning("Out-of-memory detected!")
+        prev_pid_set = {}
+        for history in self._pid_set_history:  # merge the history
+            prev_pid_set.update(history)
+        for _ in range(30):
+            current_pid_set = scan_proc_stats()
+            terminated_pid_list = sorted(set(prev_pid_set.keys()) - set(current_pid_set.keys()))
+            if not terminated_pid_list:
+                await asyncio.sleep(0.5)
+                continue
+            else:
+                break
+        else:
+            log.warning("failed to get the information of oom-killed processes")
+            return
+        pgsize = resource.getpagesize()
+        for pid, pstat in map(lambda p: (p, prev_pid_set[p]), terminated_pid_list):
+            process_tree = []
+            count = 0
+            while True:
+                if count > 0:
+                    indent = ("   " * (count - 1)) + "└─ "
+                else:
+                    indent = ""
+                cmdline = pstat["cmdline"].replace(b"\0", b" ").decode("utf8")
+                elapsed_time = "{:,.2f}".format(time.monotonic() - pstat["starttime"])
+                vm_size = "{:,}".format(pstat["vsize"] // (2**20))
+                rss = "{:,}".format((pstat["rss"] * pgsize) // (2**20))
+                process_tree.append(
+                    f"{indent}{pid} (running for {elapsed_time}s, vm: {vm_size}m, rss:"
+                    f" {rss}m): {cmdline}"
+                )
+                ppid = pstat["ppid"]
+                if ppid == 0 or ppid == pid:
+                    break
+                pid = ppid
+                pstat = prev_pid_set[ppid]
+                count += 1
+            log.warning(
+                "detected potentially oom-killed process:\n{}",
+                "\n".join(process_tree),
+            )
+
+    async def log_event(self, data):
+        match data["type"]:
+            case "oom":
+                await self.log_oom()
+            case _:
+                log.info(
+                    "Agent-notified event: {}",
+                    data,
+                )
+
     async def _send_status(self):
         data = {
             "started_at": self.started_at,
         }
         await self.outsock.send_multipart(
             [
                 b"status",
@@ -893,14 +948,24 @@
         await self.outsock.send_multipart(
             [
                 b"apps-result",
                 json.dumps(result).encode("utf8"),
             ]
         )
 
+    async def _monitor_processes(self):
+        while True:
+            self._pid_set_history.append(scan_proc_stats())
+            if len(self._pid_set_history) > 2:
+                self._pid_set_history.pop(0)
+            try:
+                await asyncio.sleep(2)
+            except asyncio.CancelledError:
+                return
+
     async def main_loop(self, cmdargs):
         log.debug("starting user input server...")
         user_input_server = await asyncio.start_unix_server(
             self.handle_user_input, "/tmp/bai-user-input.sock"
         )
         log.debug("initializing krunner...")
         await self._init_with_loop()
@@ -908,14 +973,17 @@
         await self._init_jupyter_kernel()
 
         user_bootstrap_path = Path("/home/work/bootstrap.sh")
         if user_bootstrap_path.is_file():
             log.debug("running user bootstrap script...")
             await self._bootstrap(user_bootstrap_path)
 
+        self._pid_set_history = []
+        monitor_proc_task = asyncio.create_task(self._monitor_processes())
+
         log.debug("starting intrinsic services: sshd, ttyd ...")
         intrinsic_spawn_coros = []
         intrinsic_spawn_coros.append(
             self._start_service(
                 {
                     "name": "sshd",
                     "port": self.intrinsic_host_ports_mapping.get("sshd", 2200),
@@ -963,14 +1031,17 @@
                 elif op_type == "complete":  # auto-completion
                     data = json.loads(text)
                     await self._complete(data)
                 elif op_type == "interrupt":
                     await self._interrupt()
                 elif op_type == "status":
                     await self._send_status()
+                elif op_type == "event":
+                    data = json.loads(text)
+                    asyncio.create_task(self.log_event(data))
                 elif op_type == "start-model-service":  # activate a service port
                     data = json.loads(text)
                     asyncio.create_task(self.start_model_service(data))
                 elif op_type == "start-service":  # activate a service port
                     data = json.loads(text)
                     asyncio.create_task(self._start_service_and_feed_result(data))
                 elif op_type == "shutdown-service":  # shutdown the service by its name
@@ -985,8 +1056,10 @@
                 await asyncio.sleep(0)
             except Exception:
                 log.exception("main_loop: unexpected error")
                 # we need to continue anyway unless we are shutting down
                 continue
         user_input_server.close()
         await user_input_server.wait_closed()
+        monitor_proc_task.cancel()
+        await monitor_proc_task
         await self.shutdown()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/c/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/c/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/compat.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/cpp/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/git/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/git/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/golang/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/golang/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/haskell/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/haskell/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/intrinsic.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/intrinsic.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/java/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/java/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/julia/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/julia/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/jupyter_client.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/jupyter_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/logging.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/lua/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/lua/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/nodejs/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/nodejs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/octave/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/octave/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/php/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/php/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/python/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/python/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/canvas.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/canvas.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/color.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/color.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/python/drawing/turtle.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/python/drawing/turtle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/python/sitecustomize.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/python/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/python/types.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/python/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/r/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/r/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/r_server_ms/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/r_server_ms/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/rust/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/rust/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/scheme/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/service.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/service_actions.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/service_actions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/terminal.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/terminal.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/aws_polly/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/aws_polly/inproc.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/aws_polly/inproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/ai/backend/kernel/vendor/h2o/__init__.py` & `backend.ai-kernel-23.3.8/ai/backend/kernel/vendor/h2o/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/PKG-INFO` & `backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.7
+Version: 23.3.8
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-23.3.7/backend.ai_kernel.egg-info/SOURCES.txt` & `backend.ai-kernel-23.3.8/backend.ai_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/backend_shim.py` & `backend.ai-kernel-23.3.8/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.7/setup.py` & `backend.ai-kernel-23.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,11 +72,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.7
+    'version': """23.03.8
 """,
     'zip_safe': False,
 })
```

