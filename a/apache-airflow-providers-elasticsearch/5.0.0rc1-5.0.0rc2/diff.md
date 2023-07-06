# Comparing `tmp/apache-airflow-providers-elasticsearch-5.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-elasticsearch-5.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-elasticsearch-5.0.0rc1.tar", last modified: Wed Jul  5 07:29:59 2023, max compression
+gzip compressed data, was "apache-airflow-providers-elasticsearch-5.0.0rc2.tar", last modified: Thu Jul  6 04:50:43 2023, max compression
```

## Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1.tar` & `apache-airflow-providers-elasticsearch-5.0.0rc2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.248184 apache-airflow-providers-elasticsearch-5.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5739 2023-07-05 07:29:59.248779 apache-airflow-providers-elasticsearch-5.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4046 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.153473 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.154748 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.203164 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-07-05 07:19:39.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2871 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.210183 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6474 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.220252 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py
--rw-r--r--   0 root         (0) root         (0)    19313 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.245375 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5739 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      868 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2048 2023-07-05 07:29:59.250722 apache-airflow-providers-elasticsearch-5.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.082125 apache-airflow-providers-elasticsearch-5.0.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-06 04:50:43.082798 apache-airflow-providers-elasticsearch-5.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4046 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.003037 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.004258 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.038172 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-05 18:50:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.044001 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6474 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/elasticsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.054490 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_json_formatter.py
+-rw-r--r--   0 root         (0) root         (0)    19313 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:43.079094 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      868 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:42.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-06 04:50:43.084834 apache-airflow-providers-elasticsearch-5.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-07-06 04:50:41.000000 apache-airflow-providers-elasticsearch-5.0.0rc2/setup.py
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/LICENSE` & `apache-airflow-providers-elasticsearch-5.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/MANIFEST.in` & `apache-airflow-providers-elasticsearch-5.0.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/PKG-INFO` & `apache-airflow-providers-elasticsearch-5.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-elasticsearch
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-elasticsearch package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.0.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.0.0rc1``
+Release: ``5.0.0rc2``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/README.rst` & `apache-airflow-providers-elasticsearch-5.0.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.0.0rc1``
+Release: ``5.0.0rc2``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/get_provider_info.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/hooks/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_json_formatter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/airflow/providers/elasticsearch/log/es_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO` & `apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-elasticsearch
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-elasticsearch package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.0.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.0.0rc1``
+Release: ``5.0.0rc2``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt` & `apache-airflow-providers-elasticsearch-5.0.0rc2/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/pyproject.toml` & `apache-airflow-providers-elasticsearch-5.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/setup.cfg` & `apache-airflow-providers-elasticsearch-5.0.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.elasticsearch.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.elasticsearch
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-elasticsearch-5.0.0rc1/setup.py` & `apache-airflow-providers-elasticsearch-5.0.0rc2/setup.py`

 * *Files identical despite different names*

