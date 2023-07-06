# Comparing `tmp/servicepytan-0.3.1.tar.gz` & `tmp/servicepytan-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicepytan-0.3.1.tar", last modified: Tue May  2 13:18:42 2023, max compression
+gzip compressed data, was "servicepytan-0.3.2.tar", last modified: Thu Jul  6 15:58:49 2023, max compression
```

## Comparing `servicepytan-0.3.1.tar` & `servicepytan-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.486563 servicepytan-0.3.1/
--rw-rw-rw-   0        0        0      174 2022-09-07 01:39:30.000000 servicepytan-0.3.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3724 2022-09-07 01:39:30.000000 servicepytan-0.3.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2022-09-07 01:39:30.000000 servicepytan-0.3.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1094 2022-09-07 01:39:30.000000 servicepytan-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      273 2022-09-07 01:39:30.000000 servicepytan-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2025 2023-05-02 13:18:42.486563 servicepytan-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2022-11-25 13:47:40.000000 servicepytan-0.3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.432902 servicepytan-0.3.1/docs/
--rw-rw-rw-   0        0        0      654 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/Makefile
--rw-rw-rw-   0        0        0     2103 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/conf.py
--rw-rw-rw-   0        0        0     4259 2022-11-25 13:42:00.000000 servicepytan-0.3.1/docs/index.rst
--rwxrwxrwx   0        0        0      800 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/make.bat
--rw-rw-rw-   0        0        0       80 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/modules.rst
--rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.auth.rst
--rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.data.rst
--rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.dates.rst
--rw-rw-rw-   0        0        0      158 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.requests.rst
--rw-rw-rw-   0        0        0      358 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.rst
--rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.utils.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.451059 servicepytan-0.3.1/servicepytan/
--rw-rw-rw-   0        0        0      952 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/__init__.py
--rw-rw-rw-   0        0        0     1879 2022-09-07 01:39:30.000000 servicepytan-0.3.1/servicepytan/_dates.py
--rw-rw-rw-   0        0        0     4278 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/auth.py
--rw-rw-rw-   0        0        0     4669 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/data.py
--rw-rw-rw-   0        0        0     5475 2023-05-02 13:17:32.000000 servicepytan-0.3.1/servicepytan/reports.py
--rw-rw-rw-   0        0        0     4414 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/requests.py
--rw-rw-rw-   0        0        0      257 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/summary.py
--rw-rw-rw-   0        0        0     4895 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.482137 servicepytan-0.3.1/servicepytan.egg-info/
--rw-rw-rw-   0        0        0     2025 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      809 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-10-25 17:52:15.000000 servicepytan-0.3.1/servicepytan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       62 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      407 2023-05-02 13:18:42.489408 servicepytan-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-05-02 13:18:04.000000 servicepytan-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.485561 servicepytan-0.3.1/tests/
--rw-rw-rw-   0        0        0       43 2022-09-07 01:39:30.000000 servicepytan-0.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0      920 2022-09-07 01:39:30.000000 servicepytan-0.3.1/tests/test_servicepytan.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:58:49.947894 servicepytan-0.3.2/
+-rw-rw-rw-   0        0        0      174 2022-09-07 01:39:30.000000 servicepytan-0.3.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3724 2022-09-07 01:39:30.000000 servicepytan-0.3.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2022-09-07 01:39:30.000000 servicepytan-0.3.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1094 2022-09-07 01:39:30.000000 servicepytan-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2022-09-07 01:39:30.000000 servicepytan-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2025 2023-07-06 15:58:49.947894 servicepytan-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2022-11-25 13:47:40.000000 servicepytan-0.3.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 15:58:49.891222 servicepytan-0.3.2/docs/
+-rw-rw-rw-   0        0        0      654 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/Makefile
+-rw-rw-rw-   0        0        0     2103 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/conf.py
+-rw-rw-rw-   0        0        0     4259 2022-11-25 13:42:00.000000 servicepytan-0.3.2/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/make.bat
+-rw-rw-rw-   0        0        0       80 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/modules.rst
+-rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/servicepytan.auth.rst
+-rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/servicepytan.data.rst
+-rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/servicepytan.dates.rst
+-rw-rw-rw-   0        0        0      158 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/servicepytan.requests.rst
+-rw-rw-rw-   0        0        0      358 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/servicepytan.rst
+-rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.2/docs/servicepytan.utils.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 15:58:49.915579 servicepytan-0.3.2/servicepytan/
+-rw-rw-rw-   0        0        0      952 2023-07-06 15:54:01.000000 servicepytan-0.3.2/servicepytan/__init__.py
+-rw-rw-rw-   0        0        0     1879 2022-09-07 01:39:30.000000 servicepytan-0.3.2/servicepytan/_dates.py
+-rw-rw-rw-   0        0        0     4278 2022-11-25 13:42:00.000000 servicepytan-0.3.2/servicepytan/auth.py
+-rw-rw-rw-   0        0        0     4669 2022-11-25 13:42:00.000000 servicepytan-0.3.2/servicepytan/data.py
+-rw-rw-rw-   0        0        0     5475 2023-05-02 13:17:32.000000 servicepytan-0.3.2/servicepytan/reports.py
+-rw-rw-rw-   0        0        0     4629 2023-07-06 15:53:07.000000 servicepytan-0.3.2/servicepytan/requests.py
+-rw-rw-rw-   0        0        0      257 2022-11-25 13:42:00.000000 servicepytan-0.3.2/servicepytan/summary.py
+-rw-rw-rw-   0        0        0     4895 2022-11-25 13:42:00.000000 servicepytan-0.3.2/servicepytan/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:58:49.943765 servicepytan-0.3.2/servicepytan.egg-info/
+-rw-rw-rw-   0        0        0     2025 2023-07-06 15:58:49.000000 servicepytan-0.3.2/servicepytan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      809 2023-07-06 15:58:49.000000 servicepytan-0.3.2/servicepytan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:58:49.000000 servicepytan-0.3.2/servicepytan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-06 15:58:49.000000 servicepytan-0.3.2/servicepytan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-10-25 17:52:15.000000 servicepytan-0.3.2/servicepytan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       62 2023-07-06 15:58:49.000000 servicepytan-0.3.2/servicepytan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 15:58:49.000000 servicepytan-0.3.2/servicepytan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      407 2023-07-06 15:58:49.955720 servicepytan-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-07-06 15:53:55.000000 servicepytan-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:58:49.946376 servicepytan-0.3.2/tests/
+-rw-rw-rw-   0        0        0       43 2022-09-07 01:39:30.000000 servicepytan-0.3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      920 2022-09-07 01:39:30.000000 servicepytan-0.3.2/tests/test_servicepytan.py
```

### Comparing `servicepytan-0.3.1/CONTRIBUTING.rst` & `servicepytan-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/LICENSE` & `servicepytan-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/PKG-INFO` & `servicepytan-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicepytan
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Library to make it easier to interact with the ServiceTitan API v2
 Home-page: https://github.com/elliotpalmer/servicepytan
 Author: Elliot Palmer
 Author-email: elliot@ecoplumbers.com
 License: MIT license
 Keywords: servicepytan
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `servicepytan-0.3.1/README.rst` & `servicepytan-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/docs/Makefile` & `servicepytan-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/docs/conf.py` & `servicepytan-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/docs/index.rst` & `servicepytan-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/docs/make.bat` & `servicepytan-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/servicepytan/__init__.py` & `servicepytan-0.3.2/servicepytan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     >>> import servicepytan
     >>> servicetitan_endpoint = servicepytan.Endpoint("jpm","jobs")
     >>> data = servicetitan_endpoint.get_one(id=12345678)
 """
 
 __author__ = """Elliot Palmer"""
 __email__ = 'elliot@ecoplumbers.com'
-__version__ = '0.3.0'
+__version__ = '0.3.2'
 
 # MODULES
 import requests
 import json
 
 # GLOBALS
 AUTH_ROOT = "https://auth.servicetitan.io"
```

### Comparing `servicepytan-0.3.1/servicepytan/_dates.py` & `servicepytan-0.3.2/servicepytan/_dates.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/servicepytan/auth.py` & `servicepytan-0.3.2/servicepytan/auth.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/servicepytan/data.py` & `servicepytan-0.3.2/servicepytan/data.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/servicepytan/reports.py` & `servicepytan-0.3.2/servicepytan/reports.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/servicepytan/requests.py` & `servicepytan-0.3.2/servicepytan/requests.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,18 +15,19 @@
   def __init__(self, folder, endpoint, conn=None):
     """Inits Endpoint with folder, endpoint and allows for getting necessary credentials from the config file."""
     self.folder = folder
     self.endpoint = endpoint
     self.conn = conn
 
   # Main Request Types
-  def get_one(self, id, modifier=""):
+  def get_one(self, id, modifier="", query={}):
     """Retrieve one record using the record id. Modifier is used for further endpoints."""
     url = endpoint_url(self.folder, self.endpoint, id=id, modifier=modifier, conn=self.conn)
-    return request_json(url, options={}, payload="", conn=self.conn, request_type="GET")
+    options = check_default_options(query)
+    return request_json(url, options=options, payload="", conn=self.conn, request_type="GET")
 
   def get_many(self, query={}):
     """Retrieve one page of results with query options to customize."""
     url = endpoint_url(self.folder, self.endpoint, conn=self.conn)
     options = check_default_options(query)
     return request_json(url, options, payload="", conn=self.conn, request_type="GET")
   
@@ -63,29 +64,29 @@
     return request_json(url, options={}, payload="", conn=self.conn, request_type="DEL")
 
   def delete_subitem(self, id, modifier_id, modifier):
     """Method that corresponds to a DEL request for deleting objects with subitems"""
     url = endpoint_url(self.folder, self.endpoint, id=id, modifier=f"{modifier}/{modifier_id}", conn=self.conn)
     return request_json(url, options={}, payload="", conn=self.conn, request_type="DEL")
 
-  def export_one(self, export_endpoint, export_from=""):
+  def export_one(self, export_endpoint, export_from="", include_recent_changes=False):
     """Export Doc String"""
     url = endpoint_url(self.folder, "export", id="", modifier=f"{export_endpoint}", conn=self.conn)
-    return request_json(url, options={"from": export_from}, payload="", conn=self.conn, request_type="GET")
+    return request_json(url, options={"from": export_from, "includeRecentChanges": include_recent_changes}, payload="", conn=self.conn, request_type="GET")
 
-  def export_all(self, export_endpoint, export_from=""):
+  def export_all(self, export_endpoint, export_from="", include_recent_changes=False):
     """Export All Doc String"""
     counter = 1
     print(f"{export_endpoint} {counter}: {export_from}")
-    response = self.export_one(export_endpoint, export_from)
+    response = self.export_one(export_endpoint, export_from, include_recent_changes)
     data = response["data"]
     if data == []: return []
     has_more = response["hasMore"]
     while has_more:
       counter += 1
       export_from = response["continueFrom"]
       print(f"{export_endpoint} {counter}: {export_from}")
-      response = self.export_one(export_endpoint, export_from)
+      response = self.export_one(export_endpoint, export_from, include_recent_changes)
       data.extend(response["data"])
       has_more = response["hasMore"]
     print(f"Export Data Complete. {len(data)} rows exported.")
     return data
```

### Comparing `servicepytan-0.3.1/servicepytan/utils.py` & `servicepytan-0.3.2/servicepytan/utils.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/servicepytan.egg-info/PKG-INFO` & `servicepytan-0.3.2/servicepytan.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicepytan
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Library to make it easier to interact with the ServiceTitan API v2
 Home-page: https://github.com/elliotpalmer/servicepytan
 Author: Elliot Palmer
 Author-email: elliot@ecoplumbers.com
 License: MIT license
 Keywords: servicepytan
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `servicepytan-0.3.1/servicepytan.egg-info/SOURCES.txt` & `servicepytan-0.3.2/servicepytan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.1/setup.py` & `servicepytan-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='servicepytan',
     name='servicepytan',
     packages=find_packages(include=['servicepytan', 'servicepytan.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/elliotpalmer/servicepytan',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False,
 )
```

### Comparing `servicepytan-0.3.1/tests/test_servicepytan.py` & `servicepytan-0.3.2/tests/test_servicepytan.py`

 * *Files identical despite different names*

