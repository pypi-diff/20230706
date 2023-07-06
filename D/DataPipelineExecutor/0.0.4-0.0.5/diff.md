# Comparing `tmp/DataPipelineExecutor-0.0.4.tar.gz` & `tmp/DataPipelineExecutor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataPipelineExecutor-0.0.4.tar", last modified: Wed Jul  5 09:54:05 2023, max compression
+gzip compressed data, was "DataPipelineExecutor-0.0.5.tar", last modified: Thu Jul  6 09:06:34 2023, max compression
```

## Comparing `DataPipelineExecutor-0.0.4.tar` & `DataPipelineExecutor-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 09:54:05.619722 DataPipelineExecutor-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-06-30 09:37:05.000000 DataPipelineExecutor-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2773 2023-07-05 09:54:05.619722 DataPipelineExecutor-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2316 2023-07-05 09:52:22.000000 DataPipelineExecutor-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 09:54:05.621031 DataPipelineExecutor-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      586 2023-07-05 09:53:17.000000 DataPipelineExecutor-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:54:05.606970 DataPipelineExecutor-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 09:54:05.615633 DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.egg-info/
--rw-rw-rw-   0        0        0     2773 2023-07-05 09:54:05.000000 DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-05 09:54:05.000000 DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 09:54:05.000000 DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-05 09:54:05.000000 DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35008 2023-07-03 14:23:59.000000 DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:06:34.001450 DataPipelineExecutor-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-06-30 09:37:05.000000 DataPipelineExecutor-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2772 2023-07-06 09:06:34.001450 DataPipelineExecutor-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2315 2023-07-06 09:06:02.000000 DataPipelineExecutor-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 09:06:34.001450 DataPipelineExecutor-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      586 2023-07-06 09:06:13.000000 DataPipelineExecutor-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:06:33.994138 DataPipelineExecutor-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 09:06:33.999817 DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.egg-info/
+-rw-rw-rw-   0        0        0     2772 2023-07-06 09:06:33.000000 DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-07-06 09:06:33.000000 DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 09:06:33.000000 DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-06 09:06:33.000000 DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35008 2023-07-03 14:23:59.000000 DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.py
```

### Comparing `DataPipelineExecutor-0.0.4/LICENSE.txt` & `DataPipelineExecutor-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DataPipelineExecutor-0.0.4/PKG-INFO` & `DataPipelineExecutor-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataPipelineExecutor
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to execute Copy and Stored Procedure tasks on data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -92,15 +92,15 @@
 Cluster = 
 Database =
 ClientID =
 ClientSecret = 
 AuthorityID = 
 ```
 
-Fornmat for sink_config:
+Format for sink_config:
 ```shell
 [SQL]
 Server = 
 Database = 
 Username =
 Password =
 Driver =
```

### Comparing `DataPipelineExecutor-0.0.4/README.md` & `DataPipelineExecutor-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 Cluster = 
 Database =
 ClientID =
 ClientSecret = 
 AuthorityID = 
 ```
 
-Fornmat for sink_config:
+Format for sink_config:
 ```shell
 [SQL]
 Server = 
 Database = 
 Username =
 Password =
 Driver =
```

### Comparing `DataPipelineExecutor-0.0.4/setup.py` & `DataPipelineExecutor-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='DataPipelineExecutor',
-    version='0.0.4',
+    version='0.0.5',
     description='A package to execute Copy and Stored Procedure tasks on data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     py_modules=["DataPipelineExecutor"],
     package_dir={'':'src'},
     classifiers=(
         "Programming Language :: Python :: 3",
```

### Comparing `DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.egg-info/PKG-INFO` & `DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataPipelineExecutor
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to execute Copy and Stored Procedure tasks on data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -92,15 +92,15 @@
 Cluster = 
 Database =
 ClientID =
 ClientSecret = 
 AuthorityID = 
 ```
 
-Fornmat for sink_config:
+Format for sink_config:
 ```shell
 [SQL]
 Server = 
 Database = 
 Username =
 Password =
 Driver =
```

### Comparing `DataPipelineExecutor-0.0.4/src/DataPipelineExecutor.py` & `DataPipelineExecutor-0.0.5/src/DataPipelineExecutor.py`

 * *Files identical despite different names*

