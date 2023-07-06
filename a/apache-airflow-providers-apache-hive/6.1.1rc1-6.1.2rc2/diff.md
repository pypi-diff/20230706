# Comparing `tmp/apache-airflow-providers-apache-hive-6.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-hive-6.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.1rc1.tar", last modified: Tue Jun 20 11:41:17 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.2rc2.tar", last modified: Thu Jul  6 04:50:11 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hive-6.1.1rc1.tar` & `apache-airflow-providers-apache-hive-6.1.2rc2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.585976 apache-airflow-providers-apache-hive-6.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    19538 2023-06-20 11:41:17.587160 apache-airflow-providers-apache-hive-6.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17873 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.460881 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.462033 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.463236 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.501401 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5668 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.507300 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42441 2023-06-18 13:29:11.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.513956 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.522586 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.528160 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.539416 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.559887 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5279 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0 root         (0) root         (0)     5662 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     6713 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)    11742 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     5564 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.583345 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19538 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2053 2023-06-20 11:41:17.590526 apache-airflow-providers-apache-hive-6.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.873354 apache-airflow-providers-apache-hive-6.1.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6929 2023-07-06 04:50:11.873895 apache-airflow-providers-apache-hive-6.1.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.742202 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.743421 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.744650 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.787671 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-06 04:42:33.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.793479 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42460 2023-07-04 13:46:32.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.800195 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.808843 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.814578 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.827768 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/metastore_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.847924 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py
+-rw-r--r--   0 root         (0) root         (0)     5664 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     6719 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)    11748 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.871107 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6929 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-hive-6.1.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-07-06 04:50:11.875786 apache-airflow-providers-apache-hive-6.1.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/LICENSE` & `apache-airflow-providers-apache-hive-6.1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-hive-6.1.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/__init__.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "6.1.1"
+__version__ = "6.1.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/get_provider_info.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-hive",
         "name": "Apache Hive",
         "description": "`Apache Hive <https://hive.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "6.1.2",
             "6.1.1",
             "6.1.0",
             "6.0.0",
             "5.1.3",
             "5.1.2",
             "5.1.1",
             "5.1.0",
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/__init__.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,15 @@
 from airflow.utils.operator_helpers import AIRFLOW_VAR_NAME_FORMAT_MAPPING
 
 HIVE_QUEUE_PRIORITIES = ["VERY_HIGH", "HIGH", "NORMAL", "LOW", "VERY_LOW"]
 
 
 def get_context_from_env_var() -> dict[Any, Any]:
     """
-    Extract context from env variable, e.g. dag_id, task_id and execution_date,
-    so that they can be used inside BashOperator and PythonOperator.
+    Extract context from env variable, (dag_id, task_id, etc) for use in BashOperator and PythonOperator.
 
     :return: The context of interest.
     """
     return {
         format_map["default"]: os.environ.get(format_map["env_var_format"], "")
         for format_map in AIRFLOW_VAR_NAME_FORMAT_MAPPING.values()
     }
@@ -149,14 +148,16 @@
             if conf.get("core", "security") == "kerberos":
                 template = conn.extra_dejson.get("principal", "hive/_HOST@EXAMPLE.COM")
                 if "_HOST" in template:
                     template = utils.replace_hostname_pattern(utils.get_components(template))
                 proxy_user = self._get_proxy_user()
                 if ";" in template:
                     raise RuntimeError("The principal should not contain the ';' character")
+                if ";" in proxy_user:
+                    raise RuntimeError("The proxy_user should not contain the ';' character")
                 jdbc_url += f";principal={template};{proxy_user}"
             elif self.auth:
                 jdbc_url += ";auth=" + self.auth
 
             jdbc_url = f'"{jdbc_url}"'
 
             cmd_extra += ["-u", jdbc_url]
@@ -184,16 +185,15 @@
             raise Exception(
                 f"The schema used in beeline command ({conn.schema}) should not contain ';' character)"
             )
 
     @staticmethod
     def _prepare_hiveconf(d: dict[Any, Any]) -> list[Any]:
         """
-        This function prepares a list of hiveconf params
-        from a dictionary of key value pairs.
+        Prepares a list of hiveconf params from a dictionary of key value pairs.
 
         :param d:
 
         >>> hh = HiveCliHook()
         >>> hive_conf = {"hive.exec.dynamic.partition": "true",
         ... "hive.exec.dynamic.partition.mode": "nonstrict"}
         >>> hh._prepare_hiveconf(hive_conf)
@@ -208,17 +208,18 @@
         self,
         hql: str,
         schema: str | None = None,
         verbose: bool = True,
         hive_conf: dict[Any, Any] | None = None,
     ) -> Any:
         """
-        Run an hql statement using the hive cli. If hive_conf is specified
-        it should be a dict and the entries will be set as key/value pairs
-        in HiveConf.
+        Run an hql statement using the hive cli.
+
+        If hive_conf is specified it should be a dict and the entries
+        will be set as key/value pairs in HiveConf.
 
         :param hql: an hql (hive query language) statement to run with hive cli
         :param schema: Name of hive schema (database) to use
         :param verbose: Provides additional logging. Defaults to True.
         :param hive_conf: if specified these key value pairs will be passed
             to hive as ``-hiveconf "key"="value"``. Note that they will be
             passed after the ``hive_cli_params`` and thus will override
@@ -648,16 +649,17 @@
     def get_databases(self, pattern: str = "*") -> Any:
         """Get a metastore table object."""
         with self.metastore as client:
             return client.get_databases(pattern)
 
     def get_partitions(self, schema: str, table_name: str, partition_filter: str | None = None) -> list[Any]:
         """
-        Returns a list of all partitions in a table. Works only
-        for tables with less than 32767 (java short max val).
+        Returns a list of all partitions in a table.
+
+        Works only for tables with less than 32767 (java short max val).
         For subpartitioned table, the number might easily exceed this.
 
         >>> hh = HiveMetastoreHook()
         >>> t = 'static_babynames_partitioned'
         >>> parts = hh.get_partitions(schema='airflow', table_name=t)
         >>> len(parts)
         1
@@ -685,17 +687,17 @@
                 return [dict(zip(pnames, p.values)) for p in parts]
 
     @staticmethod
     def _get_max_partition_from_part_specs(
         part_specs: list[Any], partition_key: str | None, filter_map: dict[str, Any] | None
     ) -> Any:
         """
-        Helper method to get max partition of partitions with partition_key
-        from part specs. key:value pair in filter_map will be used to
-        filter out partitions.
+        Helper method to get max partition of partitions with partition_key from part specs.
+
+        key:value pair in filter_map will be used to filter out partitions.
 
         :param part_specs: list of partition specs.
         :param partition_key: partition key name.
         :param filter_map: partition_key:partition_value map used for partition filtering,
                            e.g. {'key1': 'value1', 'key2': 'value2'}.
                            Only partitions matching all partition_key:partition_value
                            pairs will be considered as candidates of max partition.
@@ -732,14 +734,15 @@
         schema: str,
         table_name: str,
         field: str | None = None,
         filter_map: dict[Any, Any] | None = None,
     ) -> Any:
         """
         Returns the maximum value for all partitions with given field in a table.
+
         If only one partition key exist in the table, the key will be used as field.
         filter_map should be a partition_key:partition_value map and will be used to
         filter out partitions.
 
         :param schema: schema name.
         :param table_name: table name.
         :param field: partition key to get max partition from.
@@ -1010,16 +1013,15 @@
 
         self.log.info("Done. Loaded a total of %s rows.", i)
 
     def get_records(
         self, sql: str | list[str], parameters: Iterable | Mapping | None = None, **kwargs
     ) -> Any:
         """
-        Get a set of records from a Hive query. You can optionally pass 'schema' kwarg
-        which specifies target schema and default to 'default'.
+        Get a set of records from a Hive query; optionally pass a 'schema' kwarg to specify target schema.
 
         :param sql: hql to be executed.
         :param parameters: optional configuration passed to get_results
         :return: result of hive execution
 
         >>> hh = HiveServer2Hook()
         >>> sql = "SELECT * FROM airflow.static_babynames LIMIT 100"
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/__init__.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/hive.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     hive_hook = HiveMetastoreHook(metastore_conn_id=metastore_conn_id)
     return hive_hook.max_partition(schema=schema, table_name=table, field=field, filter_map=filter_map)
 
 
 def _closest_date(target_dt, date_list, before_target=None) -> datetime.date | None:
     """
     This function finds the date in a list closest to the target date.
+
     An optional parameter can be given to get the closest before or after.
 
     :param target_dt: The target date
     :param date_list: The list of dates to search
     :param before_target: closest before or after the target
     :returns: The closest date
     """
@@ -72,14 +73,15 @@
 
 
 def closest_ds_partition(
     table, ds, before=True, schema="default", metastore_conn_id="metastore_default"
 ) -> str | None:
     """
     This function finds the date in a list closest to the target date.
+
     An optional parameter can be given to get the closest before or after.
 
     :param table: A hive table name
     :param ds: A datestamp ``%Y-%m-%d`` e.g. ``yyyy-mm-dd``
     :param before: closest before (True), after (False) or either side of ds
     :param schema: table schema
     :param metastore_conn_id: which metastore connection to use
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/__init__.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive_stats.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive_stats.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/__init__.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/__init__.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/metastore_partition.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/metastore_partition.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class MetastorePartitionSensor(SqlSensor):
     """
-    An alternative to the HivePartitionSensor that talk directly to the
-    MySQL db. This was created as a result of observing sub optimal
-    queries generated by the Metastore thrift service when hitting
-    subpartitioned tables. The Thrift service's queries were written in a
-    way that would not leverage the indexes.
+    An alternative to the HivePartitionSensor that talk directly to the MySQL db.
+
+    This was created as a result of observing sub optimal queries generated by the
+    Metastore thrift service when hitting subpartitioned tables. The Thrift service's
+    queries were written in a way that would not leverage the indexes.
 
     :param schema: the schema
     :param table: the table
     :param partition_name: the partition name, as defined in the PARTITIONS
         table of the Metastore. Order of the fields does matter.
         Examples: ``ds=2016-01-01`` or
         ``ds=2016-01-01/sub=foo`` for a sub partitioned table
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/__init__.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class HiveToMySqlOperator(BaseOperator):
     """
-    Moves data from Hive to MySQL, note that for now the data is loaded
-    into memory before being pushed to MySQL, so this operator should
-    be used for smallish amount of data.
+    Moves data from Hive to MySQL.
+
+    Note that for now the data is loaded into memory before being pushed
+    to MySQL, so this operator should be used for smallish amount of data.
 
     :param sql: SQL query to execute against Hive server. (templated)
     :param mysql_table: target MySQL table, use dot notation to target a
         specific database. (templated)
     :param mysql_conn_id: source mysql connection
     :param hiveserver2_conn_id: Reference to the
         :ref:`Hive Server2 thrift service connection id <howto/connection:hiveserver2>`.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class HiveToSambaOperator(BaseOperator):
     """
-    Executes hql code in a specific Hive database and loads the
-    results of the query as a csv to a Samba location.
+    Execute hql code in a specific Hive database and load the results as a csv to a Samba location.
 
     :param hql: the hql to be exported. (templated)
     :param destination_filepath: the file path to where the file will be pushed onto samba
     :param samba_conn_id: reference to the samba destination
     :param hiveserver2_conn_id: Reference to the
         :ref: `Hive Server2 thrift service connection id <howto/connection:hiveserver2>`.
     """
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class MsSqlToHiveOperator(BaseOperator):
     """
-    Moves data from Microsoft SQL Server to Hive. The operator runs
-    your query against Microsoft SQL Server, stores the file locally
-    before loading it into a Hive table. If the ``create`` or
-    ``recreate`` arguments are set to ``True``,
-    a ``CREATE TABLE`` and ``DROP TABLE`` statements are generated.
+    Moves data from Microsoft SQL Server to Hive.
+
+    The operator runs your query against Microsoft SQL Server, stores
+    the file locally before loading it into a Hive table. If the
+    ``create`` or ``recreate`` arguments are set to ``True``, a
+    ``CREATE TABLE`` and ``DROP TABLE`` statements are generated.
+
     Hive data types are inferred from the cursor's metadata.
     Note that the table generated in Hive uses ``STORED AS textfile``
     which isn't the most efficient serialization format. If a
     large amount of data is loaded and/or if the table gets
     queried considerably, you may want to use this operator only to
     stage the data into a temporary table before loading it into its
     final destination using a ``HiveOperator``.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,19 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class MySqlToHiveOperator(BaseOperator):
     """
-    Moves data from MySql to Hive. The operator runs your query against
-    MySQL, stores the file locally before loading it into a Hive table.
+    Moves data from MySql to Hive.
+
+    The operator runs your query against MySQL, stores the file locally
+    before loading it into a Hive table.
+
     If the ``create`` or ``recreate`` arguments are set to ``True``,
     a ``CREATE TABLE`` and ``DROP TABLE`` statements are generated.
     Hive data types are inferred from the cursor's metadata. Note that the
     table generated in Hive uses ``STORED AS textfile``
     which isn't the most efficient serialization format. If a
     large amount of data is loaded and/or if the table gets
     queried considerably, you may want to use this operator only to
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,19 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class S3ToHiveOperator(BaseOperator):
     """
-    Moves data from S3 to Hive. The operator downloads a file from S3,
-    stores the file locally before loading it into a Hive table.
+    Moves data from S3 to Hive.
+
+    The operator downloads a file from S3, stores the file locally
+    before loading it into a Hive table.
+
     If the ``create`` or ``recreate`` arguments are set to ``True``,
     a ``CREATE TABLE`` and ``DROP TABLE`` statements are generated.
     Hive data types are inferred from the cursor's metadata from.
 
     Note that the table generated in Hive uses ``STORED AS textfile``
     which isn't the most efficient serialization format. If a
     large amount of data is loaded and/or if the tables gets
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class VerticaToHiveOperator(BaseOperator):
     """
-    Moves data from Vertica to Hive. The operator runs
-    your query against Vertica, stores the file locally
-    before loading it into a Hive table. If the ``create`` or
-    ``recreate`` arguments are set to ``True``,
+    Moves data from Vertica to Hive.
+
+    The operator runs your query against Vertica, stores the file
+    locally before loading it into a Hive table. If the ``create``
+    or ``recreate`` arguments are set to ``True``,
     a ``CREATE TABLE`` and ``DROP TABLE`` statements are generated.
     Hive data types are inferred from the cursor's metadata.
     Note that the table generated in Hive uses ``STORED AS textfile``
     which isn't the most efficient serialization format. If a
     large amount of data is loaded and/or if the table gets
     queried considerably, you may want to use this operator only to
     stage the data into a temporary table before loading it into its
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/pyproject.toml` & `apache-airflow-providers-apache-hive-6.1.2rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/setup.cfg` & `apache-airflow-providers-apache-hive-6.1.2rc2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -59,10 +60,10 @@
 airflow.plugins = 
 	hive=airflow.providers.apache.hive.plugins.hive:HivePlugin
 
 [files]
 packages = airflow.providers.apache.hive
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1rc1/setup.py` & `apache-airflow-providers-apache-hive-6.1.2rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-hive package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.1.1"
+version = "6.1.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-hive setup."""
     setup(
         version=version,
         extras_require={
```

