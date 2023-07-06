# Comparing `tmp/hotel-elasticsearch-1.0.4.tar.gz` & `tmp/hotel-elasticsearch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotel-elasticsearch-1.0.4.tar", last modified: Tue Mar  2 21:29:28 2021, max compression
+gzip compressed data, was "hotel-elasticsearch-1.0.5.tar", last modified: Thu Jul  6 21:55:51 2023, max compression
```

## Comparing `hotel-elasticsearch-1.0.4.tar` & `hotel-elasticsearch-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 21:29:28.865582 hotel-elasticsearch-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)      217 2021-03-02 21:29:28.865582 hotel-elasticsearch-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      251 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 21:29:28.861582 hotel-elasticsearch-1.0.4/hotel_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2299 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/app.py
--rw-r--r--   0 runner    (1001) docker     (116)     1260 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/backup.py
--rw-r--r--   0 runner    (1001) docker     (116)      556 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)      936 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     1813 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/dist_locks.py
--rw-r--r--   0 runner    (1001) docker     (116)      844 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (116)     1892 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch/service.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 21:29:28.865582 hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      217 2021-03-02 21:29:28.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      566 2021-03-02 21:29:28.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 21:29:28.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-02 21:29:28.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       40 2021-03-02 21:29:28.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2021-03-02 21:29:28.000000 hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 21:29:28.865582 hotel-elasticsearch-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      523 2021-03-02 21:29:19.000000 hotel-elasticsearch-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:51.732665 hotel-elasticsearch-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 21:55:51.732665 hotel-elasticsearch-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:51.728665 hotel-elasticsearch-1.0.5/hotel_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/dist_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:51.728665 hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 21:55:51.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-06 21:55:51.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:55:51.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 21:55:51.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 21:55:51.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:55:51.000000 hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:55:51.732665 hotel-elasticsearch-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 21:55:41.000000 hotel-elasticsearch-1.0.5/setup.py
```

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch/app.py` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch/app.py`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch/backup.py` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch/backup.py`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch/cluster.py` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch/cluster.py`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch/configuration.py` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch/configuration.py`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch/dist_locks.py` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch/dist_locks.py`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch/dynamodb.py` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch/dynamodb.py`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch/service.py` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch/service.py`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/hotel_elasticsearch.egg-info/SOURCES.txt` & `hotel-elasticsearch-1.0.5/hotel_elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotel-elasticsearch-1.0.4/setup.py` & `hotel-elasticsearch-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # encoding: utf-8
 from setuptools import setup
 
 setup(
     name='hotel-elasticsearch',
-    version='1.0.4',
+    version='1.0.5',
     packages=['hotel_elasticsearch'],
     url='',
     license='',
     author='Kristian Øllegaard',
     author_email='kristian@plecto.com',
     description='',
     install_requires=[
         'PyYAML',
-        'flask',
+        'flask==2.1.3',
         'boto',
         'requests',
         'frigga-snake'
     ],
     entry_points={
         'console_scripts': [
             'hotel-elasticsearch = hotel_elasticsearch.app:run',
```

