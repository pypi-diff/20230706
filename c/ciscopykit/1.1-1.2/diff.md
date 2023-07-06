# Comparing `tmp/ciscopykit-1.1.tar.gz` & `tmp/ciscopykit-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscopykit-1.1.tar", last modified: Wed Jul  5 00:06:56 2023, max compression
+gzip compressed data, was "ciscopykit-1.2.tar", last modified: Thu Jul  6 17:46:05 2023, max compression
```

## Comparing `ciscopykit-1.1.tar` & `ciscopykit-1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.486178 ciscopykit-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 00:06:41.000000 ciscopykit-1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-05 00:06:41.000000 ciscopykit-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-05 00:06:56.486178 ciscopykit-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-05 00:06:41.000000 ciscopykit-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.482177 ciscopykit-1.1/ciscopykit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.486178 ciscopykit-1.1/ciscopykit/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/templates/generate_router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/templates/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.482177 ciscopykit-1.1/ciscopykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:06:56.486178 ciscopykit-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-05 00:06:41.000000 ciscopykit-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:05.307187 ciscopykit-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-06 17:45:46.000000 ciscopykit-1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 17:45:46.000000 ciscopykit-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-06 17:46:05.307187 ciscopykit-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-06 17:45:46.000000 ciscopykit-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:05.307187 ciscopykit-1.2/ciscopykit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:45:46.000000 ciscopykit-1.2/ciscopykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-06 17:45:46.000000 ciscopykit-1.2/ciscopykit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-06 17:45:46.000000 ciscopykit-1.2/ciscopykit/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-06 17:45:46.000000 ciscopykit-1.2/ciscopykit/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-06 17:45:46.000000 ciscopykit-1.2/ciscopykit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:05.307187 ciscopykit-1.2/ciscopykit/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-06 17:45:46.000000 ciscopykit-1.2/ciscopykit/templates/generate_router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:45:46.000000 ciscopykit-1.2/ciscopykit/templates/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:46:05.307187 ciscopykit-1.2/ciscopykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-06 17:46:05.000000 ciscopykit-1.2/ciscopykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 17:46:05.000000 ciscopykit-1.2/ciscopykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:46:05.000000 ciscopykit-1.2/ciscopykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 17:46:05.000000 ciscopykit-1.2/ciscopykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 17:46:05.000000 ciscopykit-1.2/ciscopykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 17:46:05.000000 ciscopykit-1.2/ciscopykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:46:05.307187 ciscopykit-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 17:45:46.000000 ciscopykit-1.2/setup.py
```

### Comparing `ciscopykit-1.1/LICENSE.md` & `ciscopykit-1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.1/README.md` & `ciscopykit-1.2/README.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.1/ciscopykit/app.py` & `ciscopykit-1.2/ciscopykit/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.1/ciscopykit/device.py` & `ciscopykit-1.2/ciscopykit/device.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.1/ciscopykit/interface.py` & `ciscopykit-1.2/ciscopykit/interface.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.1/ciscopykit/templates/generate_router_config.py` & `ciscopykit-1.2/ciscopykit/templates/generate_router_config.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.1/setup.py` & `ciscopykit-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ciscopykit',
-    version='1.1',
+    version='1.2',
     author='devinci-it',
     author_email='vince.dev@icloud.com',
     description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer',
     long_description='''A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.''',
-    url='https://github.com/devinci-it/ciscopykit',
+    url='https://github.com/Vincent-de-Torres-Portfolio/ciscopykit',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

