# Comparing `tmp/testdwg-0.4.9.tar.gz` & `tmp/testdwg-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-0.4.9.tar", max compression
+gzip compressed data, was "testdwg-1.0.6.tar", max compression
```

## Comparing `testdwg-0.4.9.tar` & `testdwg-1.0.6.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-04 15:03:33.177599 testdwg-0.4.9/README.md
--rw-r--r--   0        0        0      305 2023-07-04 15:03:47.001868 testdwg-0.4.9/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-04 15:03:33.177599 testdwg-0.4.9/testdwg/__init__.py
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 10:53:41.324177 testdwg-1.0.6/LICENSE
+-rw-r--r--   0        0        0        9 2023-07-06 10:53:41.324177 testdwg-1.0.6/README.md
+-rw-r--r--   0        0        0      639 2023-07-06 10:53:59.908355 testdwg-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-06 10:53:41.324177 testdwg-1.0.6/testdwg/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-06 10:53:41.324177 testdwg-1.0.6/testdwg/main.py
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 testdwg-1.0.6/PKG-INFO
```

