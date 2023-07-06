# Comparing `tmp/pdns_exporter-0.2.0.tar.gz` & `tmp/pdns_exporter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdns_exporter-0.2.0.tar", last modified: Sat Oct  2 14:48:54 2021, max compression
+gzip compressed data, was "pdns_exporter-0.3.0.tar", last modified: Thu Jul  6 18:42:58 2023, max compression
```

## Comparing `pdns_exporter-0.2.0.tar` & `pdns_exporter-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-02 14:48:54.004841 pdns_exporter-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-10-02 14:48:40.000000 pdns_exporter-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-10-02 14:48:40.000000 pdns_exporter-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4236 2021-10-02 14:48:54.004841 pdns_exporter-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3673 2021-10-02 14:48:40.000000 pdns_exporter-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-02 14:48:54.004841 pdns_exporter-0.2.0/pdns_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-02 14:48:40.000000 pdns_exporter-0.2.0/pdns_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2021-10-02 14:48:40.000000 pdns_exporter-0.2.0/pdns_exporter/exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-10-02 14:48:40.000000 pdns_exporter-0.2.0/pdns_exporter/settings.conf
--rw-r--r--   0 runner    (1001) docker     (121)     5603 2021-10-02 14:48:40.000000 pdns_exporter-0.2.0/pdns_exporter/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-02 14:48:54.004841 pdns_exporter-0.2.0/pdns_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4236 2021-10-02 14:48:53.000000 pdns_exporter-0.2.0/pdns_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-10-02 14:48:53.000000 pdns_exporter-0.2.0/pdns_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-02 14:48:53.000000 pdns_exporter-0.2.0/pdns_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-02 14:48:53.000000 pdns_exporter-0.2.0/pdns_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-02 14:48:53.000000 pdns_exporter-0.2.0/pdns_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-02 14:48:53.000000 pdns_exporter-0.2.0/pdns_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-02 14:48:54.004841 pdns_exporter-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-10-02 14:48:53.000000 pdns_exporter-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:42:58.573041 pdns_exporter-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-06 18:42:58.573041 pdns_exporter-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:42:58.569041 pdns_exporter-0.3.0/pdns_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/pdns_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/pdns_exporter/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/pdns_exporter/settings.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/pdns_exporter/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:42:58.569041 pdns_exporter-0.3.0/pdns_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-06 18:42:58.000000 pdns_exporter-0.3.0/pdns_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-06 18:42:58.000000 pdns_exporter-0.3.0/pdns_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:42:58.000000 pdns_exporter-0.3.0/pdns_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-06 18:42:58.000000 pdns_exporter-0.3.0/pdns_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 18:42:58.000000 pdns_exporter-0.3.0/pdns_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 18:42:58.000000 pdns_exporter-0.3.0/pdns_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:42:58.573041 pdns_exporter-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-06 18:42:58.000000 pdns_exporter-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:42:58.569041 pdns_exporter-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-06 18:42:49.000000 pdns_exporter-0.3.0/tests/test_webapp.py
```

### Comparing `pdns_exporter-0.2.0/LICENSE` & `pdns_exporter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdns_exporter-0.2.0/PKG-INFO` & `pdns_exporter-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pdns_exporter
-Version: 0.2.0
+Version: 0.3.0
 Summary: PowerDNS records exporter
 Home-page: https://github.com/dmachard/python-pdns-exporter
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
-License: UNKNOWN
 Keywords: powerdns pdns database exporter mysql zone bind
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python PowerDNS Records Exporter
 
-![powerdns auth 4.4.x](https://img.shields.io/badge/pdns%204.4.x-tested-green) ![powerdns auth 4.5.x](https://img.shields.io/badge/pdns%204.5.x-tested-green) 
+![powerdns auth 4.8.x](https://img.shields.io/badge/pdns%204.8.x-tested-green) ![powerdns auth 4.7.x](https://img.shields.io/badge/pdns%204.7.x-tested-green) ![powerdns auth 4.6.x](https://img.shields.io/badge/pdns%204.6.x-tested-green) ![powerdns auth 4.5.x](https://img.shields.io/badge/pdns%204.5.x-tested-green) ![powerdns auth 4.4.x](https://img.shields.io/badge/pdns%204.4.x-tested-green)
 
-This tool can be used to export PowerDNS records database in several ways:
+This tool can be usedto export PowerDNS records database in several ways:
 - bind zone format
 - metrics for Prometheus
 
 ## Installation
 
 ### PyPI
 
@@ -150,9 +149,7 @@
 | | |
 | ------------- | ------------- |
 | Author | Denis Machard <d.machard@gmail.com> |
 | PyPI | https://pypi.org/project/python-pdns-exporter/ |
 | Github | https://github.com/dmachard/python-pdns-exporter|
 | DockerHub | https://hub.docker.com/r/dmachard/pdns-exporter |
 | | |
-
-
```

### Comparing `pdns_exporter-0.2.0/README.md` & `pdns_exporter-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Python PowerDNS Records Exporter
 
-![powerdns auth 4.4.x](https://img.shields.io/badge/pdns%204.4.x-tested-green) ![powerdns auth 4.5.x](https://img.shields.io/badge/pdns%204.5.x-tested-green) 
+![powerdns auth 4.8.x](https://img.shields.io/badge/pdns%204.8.x-tested-green) ![powerdns auth 4.7.x](https://img.shields.io/badge/pdns%204.7.x-tested-green) ![powerdns auth 4.6.x](https://img.shields.io/badge/pdns%204.6.x-tested-green) ![powerdns auth 4.5.x](https://img.shields.io/badge/pdns%204.5.x-tested-green) ![powerdns auth 4.4.x](https://img.shields.io/badge/pdns%204.4.x-tested-green)
 
-This tool can be used to export PowerDNS records database in several ways:
+This tool can be usedto export PowerDNS records database in several ways:
 - bind zone format
 - metrics for Prometheus
 
 ## Installation
 
 ### PyPI
```

### Comparing `pdns_exporter-0.2.0/pdns_exporter/exporter.py` & `pdns_exporter-0.3.0/pdns_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pdns_exporter-0.2.0/pdns_exporter/webapp.py` & `pdns_exporter-0.3.0/pdns_exporter/webapp.py`

 * *Files identical despite different names*

### Comparing `pdns_exporter-0.2.0/pdns_exporter.egg-info/PKG-INFO` & `pdns_exporter-0.3.0/pdns_exporter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pdns-exporter
-Version: 0.2.0
+Version: 0.3.0
 Summary: PowerDNS records exporter
 Home-page: https://github.com/dmachard/python-pdns-exporter
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
-License: UNKNOWN
 Keywords: powerdns pdns database exporter mysql zone bind
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python PowerDNS Records Exporter
 
-![powerdns auth 4.4.x](https://img.shields.io/badge/pdns%204.4.x-tested-green) ![powerdns auth 4.5.x](https://img.shields.io/badge/pdns%204.5.x-tested-green) 
+![powerdns auth 4.8.x](https://img.shields.io/badge/pdns%204.8.x-tested-green) ![powerdns auth 4.7.x](https://img.shields.io/badge/pdns%204.7.x-tested-green) ![powerdns auth 4.6.x](https://img.shields.io/badge/pdns%204.6.x-tested-green) ![powerdns auth 4.5.x](https://img.shields.io/badge/pdns%204.5.x-tested-green) ![powerdns auth 4.4.x](https://img.shields.io/badge/pdns%204.4.x-tested-green)
 
-This tool can be used to export PowerDNS records database in several ways:
+This tool can be usedto export PowerDNS records database in several ways:
 - bind zone format
 - metrics for Prometheus
 
 ## Installation
 
 ### PyPI
 
@@ -150,9 +149,7 @@
 | | |
 | ------------- | ------------- |
 | Author | Denis Machard <d.machard@gmail.com> |
 | PyPI | https://pypi.org/project/python-pdns-exporter/ |
 | Github | https://github.com/dmachard/python-pdns-exporter|
 | DockerHub | https://hub.docker.com/r/dmachard/pdns-exporter |
 | | |
-
-
```

### Comparing `pdns_exporter-0.2.0/setup.py` & `pdns_exporter-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
     
 KEYWORDS = ('powerdns pdns database exporter mysql zone bind')
 
 setuptools.setup(
     name="pdns_exporter",
-    version="0.2.0",
+    version="0.3.0",
     author="Denis MACHARD",
     author_email="d.machard@gmail.com",
     description="PowerDNS records exporter",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/dmachard/python-pdns-exporter",
     packages=['pdns_exporter'],
```

