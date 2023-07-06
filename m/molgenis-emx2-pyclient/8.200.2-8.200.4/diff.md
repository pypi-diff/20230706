# Comparing `tmp/molgenis_emx2_pyclient-8.200.2.tar.gz` & `tmp/molgenis_emx2_pyclient-8.200.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.200.2.tar", last modified: Wed Jul  5 08:53:36 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.200.4.tar", last modified: Wed Jul  5 18:07:33 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.200.2.tar` & `molgenis_emx2_pyclient-8.200.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:53:36.752142 molgenis_emx2_pyclient-8.200.2/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-07-05 08:45:34.000000 molgenis_emx2_pyclient-8.200.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-05 08:53:36.752142 molgenis_emx2_pyclient-8.200.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-05 08:45:34.000000 molgenis_emx2_pyclient-8.200.2/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-05 08:45:34.000000 molgenis_emx2_pyclient-8.200.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-05 08:45:34.000000 molgenis_emx2_pyclient-8.200.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:53:36.752142 molgenis_emx2_pyclient-8.200.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:53:36.752142 molgenis_emx2_pyclient-8.200.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:53:36.752142 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-05 08:45:34.000000 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-07-05 08:45:34.000000 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:53:36.752142 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-05 08:53:36.000000 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-05 08:53:36.000000 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:53:36.000000 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-05 08:53:36.000000 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-05 08:53:36.000000 molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 08:47:09.000000 molgenis_emx2_pyclient-8.200.2/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:07:33.382009 molgenis_emx2_pyclient-8.200.4/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-07-05 17:59:43.000000 molgenis_emx2_pyclient-8.200.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-05 18:07:33.382009 molgenis_emx2_pyclient-8.200.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-05 17:59:44.000000 molgenis_emx2_pyclient-8.200.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-05 17:59:44.000000 molgenis_emx2_pyclient-8.200.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-05 17:59:44.000000 molgenis_emx2_pyclient-8.200.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 18:07:33.382009 molgenis_emx2_pyclient-8.200.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:07:33.378009 molgenis_emx2_pyclient-8.200.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:07:33.378009 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-05 17:59:44.000000 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-07-05 17:59:44.000000 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:07:33.382009 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-05 18:07:33.000000 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-05 18:07:33.000000 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 18:07:33.000000 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-05 18:07:33.000000 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-05 18:07:33.000000 molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 18:01:13.000000 molgenis_emx2_pyclient-8.200.4/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.200.2/LICENSE` & `molgenis_emx2_pyclient-8.200.4/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.200.2/PKG-INFO` & `molgenis_emx2_pyclient-8.200.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.200.2
+Version: 8.200.4
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.200.2/README.md` & `molgenis_emx2_pyclient-8.200.4/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.200.2/pyproject.toml` & `molgenis_emx2_pyclient-8.200.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.200.2/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.200.4/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.200.2
+Version: 8.200.4
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

