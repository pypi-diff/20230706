# Comparing `tmp/scanoss-1.6.0.tar.gz` & `tmp/scanoss-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanoss-1.6.0.tar", last modified: Fri Jun 16 17:04:30 2023, max compression
+gzip compressed data, was "scanoss-1.6.1.tar", last modified: Thu Jul  6 14:43:39 2023, max compression
```

## Comparing `scanoss-1.6.0.tar` & `scanoss-1.6.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 17:04:04.000000 scanoss-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-16 17:04:04.000000 scanoss-1.6.0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-16 17:04:30.286773 scanoss-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-16 17:04:04.000000 scanoss-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 17:04:04.000000 scanoss-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-16 17:04:30.286773 scanoss-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.278772 scanoss-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/common/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/v2/scanoss_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/components/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.278772 scanoss-1.6.0/src/scanoss/api/cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/cryptography/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/dependencies/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/scanning/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/scanning/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/vulnerabilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34052 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/csvoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/cyclonedx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 17:04:18.000000 scanoss-1.6.0/src/scanoss/data/build_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/data/spdx-exceptions.json
--rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/data/spdx-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/filecount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scancodedeps.py
--rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanossapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanossbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanossgrpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/spdxlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/threadeddependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/threadedscanning.py
--rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/winnowing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.737285 scanoss-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 14:43:09.000000 scanoss-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-06 14:43:09.000000 scanoss-1.6.1/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-06 14:43:39.737285 scanoss-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-06 14:43:09.000000 scanoss-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 14:43:09.000000 scanoss-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-06 14:43:39.737285 scanoss-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.725284 scanoss-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.729284 scanoss-1.6.1/src/scanoss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/common/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/common/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/common/v2/scanoss_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/components/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/components/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/components/v2/scanoss_components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.725284 scanoss-1.6.1/src/scanoss/api/cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/cryptography/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/dependencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/dependencies/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/dependencies/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/scanning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/scanning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/scanning/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/scanning/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/vulnerabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/vulnerabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss/api/vulnerabilities/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/vulnerabilities/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34052 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/csvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/cyclonedx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.737285 scanoss-1.6.1/src/scanoss/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 14:43:27.000000 scanoss-1.6.1/src/scanoss/data/build_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/data/spdx-exceptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/data/spdx-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/filecount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/scancodedeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/scanossapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/scanossbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/scanossgrpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/spdxlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/threadeddependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/threadedscanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-07-06 14:43:09.000000 scanoss-1.6.1/src/scanoss/winnowing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:43:39.733285 scanoss-1.6.1/src/scanoss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-06 14:43:39.000000 scanoss-1.6.1/src/scanoss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-06 14:43:39.000000 scanoss-1.6.1/src/scanoss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:43:39.000000 scanoss-1.6.1/src/scanoss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 14:43:39.000000 scanoss-1.6.1/src/scanoss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 14:43:39.000000 scanoss-1.6.1/src/scanoss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 14:43:39.000000 scanoss-1.6.1/src/scanoss.egg-info/top_level.txt
```

### Comparing `scanoss-1.6.0/LICENSE` & `scanoss-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/PACKAGE.md` & `scanoss-1.6.1/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/PKG-INFO` & `scanoss-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.6.0
+Version: 1.6.1
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.6.0/README.md` & `scanoss-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/setup.cfg` & `scanoss-1.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 	grpcio>1.42.0
 	protobuf>3.19.1
 	pypac
 	pyOpenSSL
 
 [options.extras_require]
 fast_winnowing = 
-	scanoss_winnowing
+	scanoss_winnowing>=0.2.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = data/*.txt, data/*.json
```

### Comparing `scanoss-1.6.0/src/scanoss/__init__.py` & `scanoss-1.6.1/src/scanoss/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
 
-__version__ = '1.6.0'
+__version__ = '1.6.1'
```

### Comparing `scanoss-1.6.0/src/scanoss/api/__init__.py` & `scanoss-1.6.1/src/scanoss/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/common/__init__.py` & `scanoss-1.6.1/src/scanoss/api/common/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/common/v2/__init__.py` & `scanoss-1.6.1/src/scanoss/api/common/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/common/v2/scanoss_common_pb2.py` & `scanoss-1.6.1/src/scanoss/api/common/v2/scanoss_common_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/components/__init__.py` & `scanoss-1.6.1/src/scanoss/api/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/components/v2/__init__.py` & `scanoss-1.6.1/src/scanoss/api/components/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2.py` & `scanoss-1.6.1/src/scanoss/api/components/v2/scanoss_components_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py` & `scanoss-1.6.1/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py` & `scanoss-1.6.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py` & `scanoss-1.6.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/dependencies/__init__.py` & `scanoss-1.6.1/src/scanoss/api/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/dependencies/v2/__init__.py` & `scanoss-1.6.1/src/scanoss/api/dependencies/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py` & `scanoss-1.6.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py` & `scanoss-1.6.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/scanning/__init__.py` & `scanoss-1.6.1/src/scanoss/api/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/scanning/v2/__init__.py` & `scanoss-1.6.1/src/scanoss/api/scanning/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py` & `scanoss-1.6.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py` & `scanoss-1.6.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/vulnerabilities/__init__.py` & `scanoss-1.6.1/src/scanoss/api/vulnerabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/__init__.py` & `scanoss-1.6.1/src/scanoss/api/vulnerabilities/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py` & `scanoss-1.6.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py` & `scanoss-1.6.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/cli.py` & `scanoss-1.6.1/src/scanoss/cli.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/components.py` & `scanoss-1.6.1/src/scanoss/components.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/csvoutput.py` & `scanoss-1.6.1/src/scanoss/csvoutput.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                 detected = {}
                 if id_details == 'dependency':
                     dependencies = d.get("dependencies")
                     if not dependencies:
                         self.print_stderr(f'Warning: No Dependencies found for {f}: {file_details}')
                         continue
                     for deps in dependencies:
+                        detected = {}
                         purl = deps.get("purl")
                         if not purl:
                             self.print_stderr(f'Warning: No PURL found for {f}: {deps}')
                             continue
                         detected['purls'] = purl
                         for field in ['component', 'version', 'latest', 'url']:
                             detected[field] = deps.get(field, '')
@@ -86,14 +87,27 @@
                                 name = lic.get("name")
                                 if name and name not in dc:  # Only save the license name once
                                     dc.append(name)
                         if not dc or len(dc) == 0:
                             detected['licenses'] = ''
                         else:
                             detected['licenses'] = ';'.join(dc)
+                        # inventory_id,path,usage,detected_component,detected_license,detected_version,detected_latest,purl
+                        csv_dict.append({'inventory_id': row_id, 'path': f, 'detected_usage': id_details,
+                                         'detected_component': detected.get('component'),
+                                         'detected_license': detected.get('licenses'),
+                                         'detected_version': detected.get('version'),
+                                         'detected_latest': detected.get('latest'),
+                                         'detected_purls': detected.get('purls'),
+                                         'detected_url': detected.get('url'),
+                                         'detected_path': detected.get('file', ''),
+                                         'detected_match': matched, 'detected_lines': lines,
+                                         'detected_oss_lines': oss_lines
+                                         })
+                        row_id = row_id + 1
                 else:
                     purls = d.get('purl')
                     if not purls:
                         self.print_stderr(f'Warning: Purl block missing for {f}: {file_details}')
                         continue
                     pa = []
                     for p in purls:
@@ -112,24 +126,27 @@
                             name = lic.get("name")
                             if name and name not in dc:  # Only save the license name once
                                 dc.append(lic.get("name"))
                     if not dc or len(dc) == 0:
                         detected['licenses'] = ''
                     else:
                         detected['licenses'] = ';'.join(dc)
-                # inventory_id,path,usage,detected_component,detected_license,detected_version,detected_latest,purl
-                csv_dict.append({'inventory_id': row_id, 'path': f, 'detected_usage': id_details,
-                                 'detected_component': detected.get('component'),
-                                 'detected_license': detected.get('licenses'),
-                                 'detected_version': detected.get('version'), 'detected_latest': detected.get('latest'),
-                                 'detected_purls': detected.get('purls'), 'detected_url': detected.get('url'),
-                                 'detected_path': detected.get('file', ''),
-                                 'detected_match': matched, 'detected_lines': lines, 'detected_oss_lines': oss_lines
-                                 })
-                row_id = row_id + 1
+                    # inventory_id,path,usage,detected_component,detected_license,detected_version,detected_latest,purl
+                    csv_dict.append({'inventory_id': row_id, 'path': f, 'detected_usage': id_details,
+                                     'detected_component': detected.get('component'),
+                                     'detected_license': detected.get('licenses'),
+                                     'detected_version': detected.get('version'),
+                                     'detected_latest': detected.get('latest'),
+                                     'detected_purls': detected.get('purls'),
+                                     'detected_url': detected.get('url'),
+                                     'detected_path': detected.get('file', ''),
+                                     'detected_match': matched, 'detected_lines': lines,
+                                     'detected_oss_lines': oss_lines
+                                     })
+                    row_id = row_id + 1
         return csv_dict
 
     def produce_from_file(self, json_file: str, output_file: str = None) -> bool:
         """
         Parse plain/raw input JSON file and produce CSV output
         :param json_file:
         :param output_file:
```

### Comparing `scanoss-1.6.0/src/scanoss/cyclonedx.py` & `scanoss-1.6.1/src/scanoss/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/data/spdx-exceptions.json` & `scanoss-1.6.1/src/scanoss/data/spdx-exceptions.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/data/spdx-licenses.json` & `scanoss-1.6.1/src/scanoss/data/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/filecount.py` & `scanoss-1.6.1/src/scanoss/filecount.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/scancodedeps.py` & `scanoss-1.6.1/src/scanoss/scancodedeps.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/scanner.py` & `scanoss-1.6.1/src/scanoss/scanner.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/scanossapi.py` & `scanoss-1.6.1/src/scanoss/scanossapi.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/scanossbase.py` & `scanoss-1.6.1/src/scanoss/scanossbase.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/scanossgrpc.py` & `scanoss-1.6.1/src/scanoss/scanossgrpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/scantype.py` & `scanoss-1.6.1/src/scanoss/scantype.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/spdxlite.py` & `scanoss-1.6.1/src/scanoss/spdxlite.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/threadeddependencies.py` & `scanoss-1.6.1/src/scanoss/threadeddependencies.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/threadedscanning.py` & `scanoss-1.6.1/src/scanoss/threadedscanning.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss/winnowing.py` & `scanoss-1.6.1/src/scanoss/winnowing.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.6.0/src/scanoss.egg-info/PKG-INFO` & `scanoss-1.6.1/src/scanoss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.6.0
+Version: 1.6.1
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.6.0/src/scanoss.egg-info/SOURCES.txt` & `scanoss-1.6.1/src/scanoss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

