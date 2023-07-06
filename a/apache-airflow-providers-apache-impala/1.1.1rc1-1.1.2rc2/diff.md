# Comparing `tmp/apache-airflow-providers-apache-impala-1.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-impala-1.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-impala-1.1.1rc1.tar", last modified: Tue Jun 20 11:41:19 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-impala-1.1.2rc2.tar", last modified: Thu Jul  6 04:50:13 2023, max compression
```

## Comparing `apache-airflow-providers-apache-impala-1.1.1rc1.tar` & `apache-airflow-providers-apache-impala-1.1.2rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.429555 apache-airflow-providers-apache-impala-1.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6768 2023-06-20 11:41:19.430172 apache-airflow-providers-apache-impala-1.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5192 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.363952 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.365284 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.366795 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.397920 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.403483 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/impala.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.426877 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6768 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-impala-1.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1892 2023-06-20 11:41:19.432158 apache-airflow-providers-apache-impala-1.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.808405 apache-airflow-providers-apache-impala-1.1.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-07-06 04:50:13.808966 apache-airflow-providers-apache-impala-1.1.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.726298 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.727558 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.728786 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.763440 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-06 04:42:33.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.769763 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/impala.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.805664 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-06 04:50:13.810962 apache-airflow-providers-apache-impala-1.1.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/LICENSE` & `apache-airflow-providers-apache-impala-1.1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-impala-1.1.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/README.rst` & `apache-airflow-providers-apache-impala-1.1.2rc2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: apache-airflow-providers-apache-impala
+Version: 1.1.2rc2
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-impala package
+Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Author: Apache Software Foundation
+Author-email: dev@airflow.apache.org
+License: Apache License 2.0
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/changelog.html
+Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
+Project-URL: Source Code, https://github.com/apache/airflow
+Project-URL: Slack Chat, https://s.apache.org/airflow-slack
+Project-URL: Twitter, https://twitter.com/ApacheAirflow
+Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Framework :: Apache Airflow
+Classifier: Framework :: Apache Airflow :: Provider
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Monitoring
+Requires-Python: ~=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: common.sql
+Provides-Extra: kerberos
+License-File: LICENSE
+License-File: NOTICE
+
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -12,31 +48,48 @@
 .. Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
+ .. Licensed to the Apache Software Foundation (ASF) under one
+    or more contributor license agreements.  See the NOTICE file
+    distributed with this work for additional information
+    regarding copyright ownership.  The ASF licenses this file
+    to you under the Apache License, Version 2.0 (the
+    "License"); you may not use this file except in compliance
+    with the License.  You may obtain a copy of the License at
+
+ ..   http://www.apache.org/licenses/LICENSE-2.0
+
+ .. Unless required by applicable law or agreed to in writing,
+    software distributed under the License is distributed on an
+    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+    KIND, either express or implied.  See the License for the
+    specific language governing permissions and limitations
+    under the License.
+
 
 Package ``apache-airflow-providers-apache-impala``
 
-Release: ``1.1.1rc1``
+Release: ``1.1.2rc2``
 
 
 `Apache Impala <https://impala.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.impala`` provider. All classes for this provider package
 are in ``airflow.providers.apache.impala`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -69,70 +122,9 @@
 
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
- .. Licensed to the Apache Software Foundation (ASF) under one
-    or more contributor license agreements.  See the NOTICE file
-    distributed with this work for additional information
-    regarding copyright ownership.  The ASF licenses this file
-    to you under the Apache License, Version 2.0 (the
-    "License"); you may not use this file except in compliance
-    with the License.  You may obtain a copy of the License at
-
- ..   http://www.apache.org/licenses/LICENSE-2.0
-
- .. Unless required by applicable law or agreed to in writing,
-    software distributed under the License is distributed on an
-    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-    KIND, either express or implied.  See the License for the
-    specific language governing permissions and limitations
-    under the License.
-
-.. NOTE TO CONTRIBUTORS:
-   Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
-   and you want to add an explanation to the users on how they are supposed to deal with them.
-   The changelog is updated and maintained semi-automatically by release manager.
-
-Changelog
----------
-
-1.1.1
-.....
-
-.. note::
-  This release dropped support for Python 3.7
-
-Misc
-~~~~
-
-* ``Add note about dropping Python 3.7 for kafka and impala (#32017)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-
-1.1.0
-.....
-
-.. note::
-  This release of provider is only available for Airflow 2.4+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
-
-Misc
-~~~~
-
-* ``Bump minimum Airflow version in providers (#30917)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Add full automation for min Airflow version for providers (#30994)``
-   * ``Add mechanism to suspend providers (#30422)``
-   * ``Use '__version__' in providers not 'version' (#31393)``
-   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
-   * ``Prepare docs for May 2023 wave of Providers (#31252)``
-
-1.0.0
-.....
-
-Initial version of the provider.
+The changelog for the provider package can be found in the
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/__init__.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/get_provider_info.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-impala",
         "name": "Apache Impala",
         "description": "`Apache Impala <https://impala.apache.org/>`__.\n",
         "suspended": False,
-        "versions": ["1.1.1", "1.1.0", "1.0.0"],
+        "versions": ["1.1.2", "1.1.1", "1.1.0", "1.0.0"],
         "dependencies": ["impyla>=0.18.0,<1.0", "apache-airflow>=2.4.0"],
         "integrations": [
             {
                 "integration-name": "Apache Impala",
                 "external-doc-url": "https://impala.apache.org",
                 "tags": ["apache"],
             }
@@ -45,8 +45,9 @@
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.apache.impala.hooks.impala.ImpalaHook",
                 "connection-type": "impala",
             }
         ],
+        "additional-extras": [{"name": "kerberos", "dependencies": ["kerberos>=1.3.0"]}],
     }
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/__init__.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/impala.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/impala.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/pyproject.toml` & `apache-airflow-providers-apache-impala-1.1.2rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/setup.cfg` & `apache-airflow-providers-apache-impala-1.1.2rc2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -53,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.impala.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.impala
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1rc1/setup.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-impala package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.1.1"
+version = "1.1.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-impala setup."""
     setup(
         version=version,
-        extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
+        extras_require={
+            "common.sql": ["apache-airflow-providers-common-sql"],
+            "kerberos": ["kerberos>=1.3.0"],
+        },
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.apache.impala",
                 "airflow.providers.apache.impala.*",
                 "airflow.providers.apache.impala_vendor",
                 "airflow.providers.apache.impala_vendor.*",
             ],
```

