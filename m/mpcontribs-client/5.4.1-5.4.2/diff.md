# Comparing `tmp/mpcontribs-client-5.4.1.tar.gz` & `tmp/mpcontribs-client-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.4.1.tar", last modified: Fri Jun 30 18:13:28 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.4.2.tar", last modified: Thu Jul  6 21:52:37 2023, max compression
```

## Comparing `mpcontribs-client-5.4.1.tar` & `mpcontribs-client-5.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.856181 mpcontribs-client-5.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 18:13:28.856181 mpcontribs-client-5.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    87020 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:13:28.856181 mpcontribs-client-5.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.337099 mpcontribs-client-5.4.2/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.337099 mpcontribs-client-5.4.2/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    87020 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.337099 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 21:52:37.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/tests/test_client.py
```

### Comparing `mpcontribs-client-5.4.1/LICENSE` & `mpcontribs-client-5.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/PKG-INFO` & `mpcontribs-client-5.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.4.1
+Version: 5.4.2
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.4.1/README.md` & `mpcontribs-client-5.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/mpcontribs/client/__init__.py` & `mpcontribs-client-5.4.2/mpcontribs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.4.2/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.4.1
+Version: 5.4.2
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.4.1/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.4.2/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/deployment.txt` & `mpcontribs-client-5.4.2/requirements/deployment.txt`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
@@ -235,15 +235,15 @@
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydantic-core
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.1/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.4.2/requirements/macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.2/requirements/macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.4.2/requirements/macos-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.2/requirements/macos-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.4.2/requirements/macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.2/requirements/macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/setup.py` & `mpcontribs-client-5.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.1/tests/test_client.py` & `mpcontribs-client-5.4.2/tests/test_client.py`

 * *Files identical despite different names*

