# Comparing `tmp/ansible-doc-extractor-0.1.8.tar.gz` & `tmp/ansible-doc-extractor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-doc-extractor-0.1.8.tar", last modified: Fri Jan 21 09:37:19 2022, max compression
+gzip compressed data, was "ansible-doc-extractor-0.1.9.tar", last modified: Fri Dec  2 09:42:06 2022, max compression
```

## Comparing `ansible-doc-extractor-0.1.8.tar` & `ansible-doc-extractor-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.355151 ansible-doc-extractor-0.1.8/
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.337151 ansible-doc-extractor-0.1.8/.github/
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.352151 ansible-doc-extractor-0.1.8/.github/workflows/
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)      699 2022-01-20 08:24:13.000000 ansible-doc-extractor-0.1.8/.github/workflows/ci.yml
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       87 2022-01-20 08:24:19.000000 ansible-doc-extractor-0.1.8/.gitignore
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)    35149 2022-01-19 09:43:08.000000 ansible-doc-extractor-0.1.8/LICENSE
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     7604 2022-01-21 09:37:19.355151 ansible-doc-extractor-0.1.8/PKG-INFO
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     6848 2022-01-20 08:24:19.000000 ansible-doc-extractor-0.1.8/README.rst
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     1010 2022-01-21 09:37:19.356151 ansible-doc-extractor-0.1.8/setup.cfg
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       58 2022-01-19 09:43:08.000000 ansible-doc-extractor-0.1.8/setup.py
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.337151 ansible-doc-extractor-0.1.8/src/
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.353151 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-19 09:43:08.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/__init__.py
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     4990 2022-01-21 07:33:28.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/cli.py
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.355151 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/templates/
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     3416 2022-01-20 08:24:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/templates/module.md.j2
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     3582 2022-01-19 09:43:08.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/templates/module.rst.j2
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.354151 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     7604 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)      658 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)        1 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       74 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/entry_points.txt
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       75 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/requires.txt
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       22 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/top_level.txt
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)        1 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/zip-safe
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.345151 ansible-doc-extractor-0.1.8/tests/
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.345151 ansible-doc-extractor-0.1.8/tests/integration/
-drwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-21 09:37:19.355151 ansible-doc-extractor-0.1.8/tests/integration/basic/
--rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)    11990 2022-01-20 08:24:13.000000 ansible-doc-extractor-0.1.8/tests/integration/basic/ad_auth_provider.py
--rwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)       76 2022-01-20 08:24:13.000000 ansible-doc-extractor-0.1.8/tests/integration/basic/run.sh
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.439947 ansible-doc-extractor-0.1.9/
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.396947 ansible-doc-extractor-0.1.9/.github/
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.432947 ansible-doc-extractor-0.1.9/.github/workflows/
+-rw-r--r--   0 juremedvesek  (1000) juremedvesek  (1000)      726 2022-12-02 09:05:31.000000 ansible-doc-extractor-0.1.9/.github/workflows/ci.yml
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       87 2022-02-25 13:50:10.000000 ansible-doc-extractor-0.1.9/.gitignore
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)    35149 2022-01-19 09:43:08.000000 ansible-doc-extractor-0.1.9/LICENSE
+-rw-r--r--   0 juremedvesek  (1000) juremedvesek  (1000)     7915 2022-12-02 09:42:06.439947 ansible-doc-extractor-0.1.9/PKG-INFO
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     6848 2022-02-25 13:50:10.000000 ansible-doc-extractor-0.1.9/README.rst
+-rw-r--r--   0 juremedvesek  (1000) juremedvesek  (1000)     1308 2022-12-02 09:42:06.441948 ansible-doc-extractor-0.1.9/setup.cfg
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       58 2022-01-19 09:43:08.000000 ansible-doc-extractor-0.1.9/setup.py
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.396947 ansible-doc-extractor-0.1.9/src/
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.432947 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-01-19 09:43:08.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/__init__.py
+-rw-r--r--   0 juremedvesek  (1000) juremedvesek  (1000)     4990 2022-12-02 09:41:09.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/cli.py
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.439947 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/templates/
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     3416 2022-02-25 13:50:10.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/templates/module.md.j2
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     3582 2022-02-25 13:50:10.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/templates/module.rst.j2
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.438948 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)     7915 2022-12-02 09:42:06.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/PKG-INFO
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)      658 2022-12-02 09:42:06.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)        1 2022-12-02 09:42:06.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       74 2022-12-02 09:42:06.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/entry_points.txt
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       75 2022-12-02 09:42:06.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/requires.txt
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)       22 2022-12-02 09:42:06.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/top_level.txt
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)        1 2022-01-21 09:37:19.000000 ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/zip-safe
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.404947 ansible-doc-extractor-0.1.9/tests/
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.404947 ansible-doc-extractor-0.1.9/tests/integration/
+drwxr-xr-x   0 juremedvesek  (1000) juremedvesek  (1000)        0 2022-12-02 09:42:06.439947 ansible-doc-extractor-0.1.9/tests/integration/basic/
+-rw-rw-r--   0 juremedvesek  (1000) juremedvesek  (1000)    11990 2022-01-20 08:24:13.000000 ansible-doc-extractor-0.1.9/tests/integration/basic/ad_auth_provider.py
+-rwxrwxr-x   0 juremedvesek  (1000) juremedvesek  (1000)       76 2022-01-20 08:24:13.000000 ansible-doc-extractor-0.1.9/tests/integration/basic/run.sh
```

### Comparing `ansible-doc-extractor-0.1.8/.github/workflows/ci.yml` & `ansible-doc-extractor-0.1.9/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ---
 name: CI
 on:
   push:
-    branches: [ main ]
+    branches: [ master ]
   pull_request:
+    branches: [ master ]
   schedule:
     # Run test at 03:04 UTC on mon,wed,fri
     - cron: "3 4 * * 1,3,5"
 
 jobs:
   integration:
     name: Integration tests
     strategy:
       matrix:
-        python: [ "3.6", "3.7", "3.8", "3.9" ]
+        python: ["3.7", "3.8", "3.9", "3.10" ]
     runs-on: ubuntu-latest
     steps:
       - name: Get code
         uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python }}
         uses: actions/setup-python@v2
```

### Comparing `ansible-doc-extractor-0.1.8/LICENSE` & `ansible-doc-extractor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-doc-extractor-0.1.8/PKG-INFO` & `ansible-doc-extractor-0.1.9/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: ansible-doc-extractor
-Version: 0.1.8
-Summary: Extract Ansible module documentation
-Home-page: UNKNOWN
-Author: XLAB Steampunk
-Author-email: steampunk@xlab.si
-License: UNKNOWN
-Keywords: ansible,documentation
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Provides-Extra: ansible
-Provides-Extra: base
-Provides-Extra: core
-License-File: LICENSE
-
 Ansible Collection API Documentation Extractor
 ==============================================
 
 This package contains code for Ansible collection documentation extractor. Its
 main audience are Ansible collection maintainers that would like to publish
 API docs in the HTML form without having to manually copy the data already
 present in the module's metadata.
@@ -113,9 +90,7 @@
    $ python3 -m venv venv
    $ . venv/bin/activate
    (venv) $ pip install -e .
 
 To test the extractor, we can run::
 
    $ ansible-doc-extractor
-
-
```

### Comparing `ansible-doc-extractor-0.1.8/README.rst` & `ansible-doc-extractor-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: ansible-doc-extractor
+Version: 0.1.9
+Summary: Extract Ansible module documentation
+Home-page: https://github.com/xlab-steampunk/ansible-doc-extractor
+Author: XLAB Steampunk
+Author-email: steampunk@xlab.si
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/xlab-steampunk/ansible-doc-extractor/issues
+Keywords: ansible,documentation
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Provides-Extra: ansible
+Provides-Extra: base
+Provides-Extra: core
+License-File: LICENSE
+
 Ansible Collection API Documentation Extractor
 ==============================================
 
 This package contains code for Ansible collection documentation extractor. Its
 main audience are Ansible collection maintainers that would like to publish
 API docs in the HTML form without having to manually copy the data already
 present in the module's metadata.
@@ -90,7 +118,9 @@
    $ python3 -m venv venv
    $ . venv/bin/activate
    (venv) $ pip install -e .
 
 To test the extractor, we can run::
 
    $ ansible-doc-extractor
+
+
```

### Comparing `ansible-doc-extractor-0.1.8/setup.cfg` & `ansible-doc-extractor-0.1.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -11,26 +11,33 @@
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+url = https://github.com/xlab-steampunk/ansible-doc-extractor
+project_urls = 
+	Bug Tracker = https://github.com/xlab-steampunk/ansible-doc-extractor/issues
 
 [options]
 package_dir = 
 	= src
 packages = find:
 zip_safe = True
 include_package_data = True
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	jinja2
 	PyYAML
+python_requires = >=3.6
 
 [options.extras_require]
 ansible = 
 	ansible
 base = 
 	ansible-base
 core =
```

### Comparing `ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/cli.py` & `ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/templates/module.md.j2` & `ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/templates/module.md.j2`

 * *Files identical despite different names*

### Comparing `ansible-doc-extractor-0.1.8/src/ansible_doc_extractor/templates/module.rst.j2` & `ansible-doc-extractor-0.1.9/src/ansible_doc_extractor/templates/module.rst.j2`

 * *Files identical despite different names*

### Comparing `ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/PKG-INFO` & `ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: ansible-doc-extractor
-Version: 0.1.8
+Version: 0.1.9
 Summary: Extract Ansible module documentation
-Home-page: UNKNOWN
+Home-page: https://github.com/xlab-steampunk/ansible-doc-extractor
 Author: XLAB Steampunk
 Author-email: steampunk@xlab.si
 License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/xlab-steampunk/ansible-doc-extractor/issues
 Keywords: ansible,documentation
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
 Provides-Extra: ansible
 Provides-Extra: base
 Provides-Extra: core
 License-File: LICENSE
 
 Ansible Collection API Documentation Extractor
 ==============================================
```

### Comparing `ansible-doc-extractor-0.1.8/src/ansible_doc_extractor.egg-info/SOURCES.txt` & `ansible-doc-extractor-0.1.9/src/ansible_doc_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-doc-extractor-0.1.8/tests/integration/basic/ad_auth_provider.py` & `ansible-doc-extractor-0.1.9/tests/integration/basic/ad_auth_provider.py`

 * *Files identical despite different names*

