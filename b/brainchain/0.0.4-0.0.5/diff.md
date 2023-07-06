# Comparing `tmp/brainchain-0.0.4.tar.gz` & `tmp/brainchain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.0.4.tar", max compression
+gzip compressed data, was "brainchain-0.0.5.tar", max compression
```

## Comparing `brainchain-0.0.4.tar` & `brainchain-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,11 @@
--rw-r--r--   0        0        0        0 2023-07-06 16:24:54.636075 brainchain-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-07-06 16:24:54.636037 brainchain-0.0.4/brainchain/__init__.py
--rw-r--r--   0        0        0      300 2023-07-06 16:26:29.571125 brainchain-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      319 1970-01-01 00:00:00.000000 brainchain-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.0.5/brainchain/README.md
+-rw-r--r--   0        0        0      104 2023-07-06 16:47:41.411790 brainchain-0.0.5/brainchain/__init__.py
+-rw-r--r--   0        0        0     4983 2023-07-05 23:39:12.540065 brainchain-0.0.5/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.0.5/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.0.5/brainchain/coredata.py
+-rw-r--r--   0        0        0     1713 2023-07-06 15:10:07.036695 brainchain-0.0.5/brainchain/example.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.0.5/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.0.5/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6351 2023-07-05 20:38:03.247634 brainchain-0.0.5/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      530 2023-07-06 16:44:28.277736 brainchain-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.0.5/PKG-INFO
```

