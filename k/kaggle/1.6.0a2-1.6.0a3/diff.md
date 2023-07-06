# Comparing `tmp/kaggle-1.6.0a2.tar.gz` & `tmp/kaggle-1.6.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaggle-1.6.0a2.tar", last modified: Tue Jun 13 00:13:46 2023, max compression
+gzip compressed data, was "kaggle-1.6.0a3.tar", last modified: Thu Jul  6 16:58:38 2023, max compression
```

## Comparing `kaggle-1.6.0a2.tar` & `kaggle-1.6.0a3.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    11541 2023-06-13 00:13:37.000000 kaggle-1.6.0a2/LICENSE
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       19 2023-06-13 00:13:37.000000 kaggle-1.6.0a2/MANIFEST.in
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/PKG-INFO
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    35072 2023-06-13 00:13:37.000000 kaggle-1.6.0a2/README.md
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.872311 kaggle-1.6.0a2/kaggle/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      799 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/__init__.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.876311 kaggle-1.6.0a2/kaggle/api/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      742 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/api/__init__.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)   196727 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/api/kaggle_api.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)   153689 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/api/kaggle_api_extended.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    25458 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/api_client.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    74254 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/cli.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     8858 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/configuration.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/kaggle/models/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1849 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/__init__.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     4851 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/collaborator.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     7424 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/dataset_column.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    12281 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/dataset_new_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     9991 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/dataset_new_version_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    10114 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/dataset_update_settings_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     4342 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/error.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     6915 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/kaggle_models_extended.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    19316 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/kernel_push_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     4077 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/license.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     5051 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/model_instance_new_version_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     9699 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/model_instance_update_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    12103 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/model_new_instance_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    10055 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/model_new_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     9096 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/model_update_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     2895 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/result.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     5439 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/upload_file.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    13927 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/rest.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/kaggle/tests/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      596 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/tests/__init__.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1782 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/tests/test_authenticate.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.872311 kaggle-1.6.0a2/kaggle.egg-info/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/PKG-INFO
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1077 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/SOURCES.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)        1 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/dependency_links.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       43 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/entry_points.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       78 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/requires.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)        7 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/top_level.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       79 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/setup.cfg
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1680 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/
+-rw-r--r--   0 root         (0) root         (0)    11541 2023-07-06 16:58:34.000000 kaggle-1.6.0a3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 16:58:34.000000 kaggle-1.6.0a3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35600 2023-07-06 16:58:34.000000 kaggle-1.6.0a3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.605670 kaggle-1.6.0a3/kaggle/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.609670 kaggle-1.6.0a3/kaggle/api/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   189890 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api/kaggle_api.py
+-rw-r--r--   0 root         (0) root         (0)   156655 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api/kaggle_api_extended.py
+-rw-r--r--   0 root         (0) root         (0)    25458 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    74101 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9163 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.613670 kaggle-1.6.0a3/kaggle/models/
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/api_blob_type.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/collaborator.py
+-rw-r--r--   0 root         (0) root         (0)     5166 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/create_inbox_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     7424 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_column.py
+-rw-r--r--   0 root         (0) root         (0)    12558 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_new_request.py
+-rw-r--r--   0 root         (0) root         (0)     9991 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_new_version_request.py
+-rw-r--r--   0 root         (0) root         (0)    10114 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/dataset_update_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/kaggle_models_extended.py
+-rw-r--r--   0 root         (0) root         (0)    20199 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/kernel_push_request.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/license.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_instance_new_version_request.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_instance_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    12103 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_new_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    10055 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_new_request.py
+-rw-r--r--   0 root         (0) root         (0)     9096 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/model_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/result.py
+-rw-r--r--   0 root         (0) root         (0)     7844 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/start_blob_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/start_blob_upload_response.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/models/upload_file.py
+-rw-r--r--   0 root         (0) root         (0)    13927 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/kaggle/test/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/kaggle/test/test_authenticate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:58:38.609670 kaggle-1.6.0a3/kaggle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 16:58:38.000000 kaggle-1.6.0a3/kaggle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-06 16:58:38.617671 kaggle-1.6.0a3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-07-06 16:58:35.000000 kaggle-1.6.0a3/setup.py
```

### Comparing `kaggle-1.6.0a2/LICENSE` & `kaggle-1.6.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/PKG-INFO` & `kaggle-1.6.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a2
+Version: 1.6.0a3
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a2/README.md` & `kaggle-1.6.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ## Commands
 
 The command line tool supports the following commands:
 
 ``` 
 kaggle competitions {list, files, download, submit, submissions, leaderboard}
-kaggle datasets {list, files, download, create, version, init}
+kaggle datasets {list, files, download, create, version, init, metadata, status}
 kaggle kernels {list, init, push, pull, output, status}
 kaggle models {get, list, init, create, delete, update}
 kaggle models instances {get, init, create, delete, update}
 kaggle models instances versions {init, create, download, delete}
 kaggle models instances {get, init, create, delete, update}
 kaggle config {view, set, unset}
 ```
@@ -235,20 +235,21 @@
     metadata            Download metadata about a dataset
     status              Get the creation status for a dataset
 ```
 
 ##### List datasets
 
 ```
-usage: kaggle datasets list [-h] [--sort-by SORT_BY] [--size SIZE] [--file-type FILE_TYPE] [--license LICENSE_NAME] [--tags TaG_IDS] [-s SEARCH] [-m] [--user USER] [-p PAGE] [-v]
+usage: kaggle datasets list [-h] [--sort-by SORT_BY] [--min-size MIN_SIZE] [--max-size MAX_SIZE] [--file-type FILE_TYPE] [--license LICENSE_NAME] [--tags TAG_IDS] [-s SEARCH] [-m] [--user USER] [-p PAGE] [-v]
 
 optional arguments:
   -h, --help            show this help message and exit
   --sort-by SORT_BY     Sort list results. Default is 'hottest'. Valid options are 'hottest', 'votes', 'updated', and 'active'
-  --size SIZE           Search for datasets of a specific size. Default is 'all'. Valid options are 'all', 'small', 'medium', and 'large'
+  --max-size MAX_SIZE   Specify the maximum size of the dataset to return (bytes)
+  --min-size MIN_SIZE   Specify the minimum size of the dataset to return (bytes)
   --file-type FILE_TYPE Search for datasets with a specific file type. Default is 'all'. Valid options are 'all', 'csv', 'sqlite', 'json', and 'bigQuery'. Please note that bigQuery datasets cannot be downloaded
   --license LICENSE_NAME 
                         Search for datasets with a specific license. Default is 'all'. Valid options are 'all', 'cc', 'gpl', 'odb', and 'other'
   --tags TAG_IDS        Search for datasets that have specific tags. Tag list should be comma separated                      
   -s SEARCH, --search SEARCH
                         Term(s) to search for
   -m, --mine            Display only my items
@@ -264,34 +265,40 @@
 `kaggle datasets list --sort-by votes`
 
 ##### List files for a dataset
 
 ```
 usage: kaggle datasets files [-h] [-v] [dataset]
 
+required arguments:
+  dataset               Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options), or <owner>/<dataset-name>/<version-number> for a specific version
+
 optional arguments:
   -h, --help  show this help message and exit
-  dataset     Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options)
   -v, --csv   Print results in CSV format (if not set print in table format)
 ```
 
 Example:
 
 `kaggle datasets files zillow/zecon`
 
+`kaggle datasets files zillow/zecon/3`
+
 ##### Download dataset files
 
 ```
 usage: kaggle datasets download [-h] [-f FILE_NAME] [-p PATH] [-w] [--unzip]
                                 [-o] [-q]
                                 [dataset]
 
+required arguments:
+  dataset               Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options), or <owner>/<dataset-name>/<version-number> for a specific version
+
 optional arguments:
   -h, --help            show this help message and exit
-  dataset               Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options)
   -f FILE_NAME, --file FILE_NAME
                         File name, all files downloaded if not provided
                         (use "kaggle datasets files -d <dataset>" to show options)
   -p PATH, --path PATH  Folder where file(s) will be downloaded, defaults to current working directory
   -w, --wp              Download files to current working path
   --unzip               Unzip the downloaded file. Will delete the zip file when completed.
   -o, --force           Skip check whether local version of file is up to date, force file download
@@ -299,27 +306,29 @@
 ```
 
 
 Examples:
 
 `kaggle datasets download zillow/zecon`
 
+`kaggle datasets download zillow/zecon/3`
+
 `kaggle datasets download zillow/zecon -f State_time_series.csv`
 
 Please note that BigQuery datasets cannot be downloaded.
 
 ##### Initialize metadata file for dataset creation
 
 ```
 usage: kaggle datasets init [-h] [-p FOLDER]
 
 optional arguments:
   -h, --help            show this help message and exit
   -p FOLDER, --path FOLDER
-                        Folder for upload, containing data files and a special dataset-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Dataset-Metadata). Defaults to current working directory
+                        Folder where the special dataset-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Dataset-Metadata) will be created. Defaults to current working directory
 ```
 
 Example:
 
 `kaggle datasets init -p /path/to/dataset`
 
 ##### Create a new dataset
@@ -372,33 +381,37 @@
 
 
 ##### Download metadata for an existing dataset
 
 ```
 usage: kaggle datasets metadata [-h] [-p PATH] [dataset]
 
+required arguments:
+  dataset               Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options)
+
 optional arguments:
   -h, --help            show this help message and exit
-  dataset               Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options)
   -p PATH, --path PATH  Location to download dataset metadata to. Defaults to current working directory
 ```
 
 Example:
 
 `kaggle datasets metadata -p /path/to/download zillow/zecon`
 
 
 ##### Get dataset creation status 
 
 ```
 usage: kaggle datasets status [-h] [dataset]
 
+required arguments:
+  dataset     Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options)
+
 optional arguments:
   -h, --help  show this help message and exit
-  dataset     Dataset URL suffix in format <owner>/<dataset-name> (use "kaggle datasets list" to show options)
 ```
 
 Example:
 
 `kaggle datasets status zillow/zecon`
 
 
@@ -463,35 +476,35 @@
 
 ```
 usage: kaggle kernels init [-h] [-p FOLDER]
 
 optional arguments:
   -h, --help            show this help message and exit
   -p FOLDER, --path FOLDER
-                        Folder for upload, containing data files and a special kernel-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Kernel-Metadata). Defaults to current working directory
+                        Folder where the special kernel-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Kernel-Metadata) will be created. Defaults to current working directory
 ```
 
 Example:
 
-`kaggle kernels init -p /path/to/kernel`
+`kaggle kernels init -p /path/to/folder`
   
 ##### Push a kernel
 
 ```
 usage: kaggle kernels push [-h] -p FOLDER
 
 optional arguments:
   -h, --help            show this help message and exit
   -p FOLDER, --path FOLDER
                         Folder for upload, containing data files and a special kernel-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Kernel-Metadata). Defaults to current working directory
 ```
 
 Example:
 
-`kaggle kernels push -p /path/to/kernel`
+`kaggle kernels push -p /path/to/folder`
 
 ##### Pull a kernel
 
 ```
 usage: kaggle kernels pull [-h] [-p PATH] [-w] [-m] [kernel]
 
 optional arguments:
@@ -507,17 +520,19 @@
 `kaggle kernels pull rtatman/list-of-5-day-challenges -p /path/to/dest`
 
 ##### Retrieve a kernel's output
 
 ```
 usage: kaggle kernels output [-h] [-p PATH] [-w] [-o] [-q] [kernel]
 
+required arguments:
+  kernel      Kernel URL suffix in format <owner>/<kernel-name> (use "kaggle kernels list" to show options)
+
 optional arguments:
   -h, --help            show this help message and exit
-  kernel                Kernel URL suffix in format <owner>/<kernel-name> (use "kaggle kernels list" to show options)
   -p PATH, --path PATH  Folder where file(s) will be downloaded, defaults to current working directory
   -w, --wp              Download files to current working path
   -o, --force           Skip check whether local version of file is up to date, force file download
   -q, --quiet           Suppress printing information about the upload/download progress
 ```
 
 Example:
@@ -525,17 +540,19 @@
 `kaggle kernels output mrisdal/exploring-survival-on-the-titanic -p /path/to/dest`
 
 ##### Get the status of the latest kernel run
 
 ```
 usage: kaggle kernels status [-h] [kernel]
 
+required arguments:
+  kernel      Kernel URL suffix in format <owner>/<kernel-name> (use "kaggle kernels list" to show options)
+
 optional arguments:
   -h, --help  show this help message and exit
-  kernel      Kernel URL suffix in format <owner>/<kernel-name> (use "kaggle kernels list" to show options)
 ```
 
 Example:
 
 `kaggle kernels status mrisdal/exploring-survival-on-the-titanic`
 
 ### Models
@@ -630,17 +647,19 @@
 `kaggle models create -p /path/to/model`
 
 ##### Delete model
 
 ```
 usage: kaggle models delete [-h] [model]
 
+required arguments:
+  model       Model URL suffix in format <owner>/<model-name>
+
 optional arguments:
   -h, --help  show this help message and exit
-  model       Model URL suffix in format <owner>/<model-name>
 ```
 
 Example:
 
 `kaggle models delete tensorflow/toxicity`
 
 ##### Update a model
@@ -733,17 +752,19 @@
 `kaggle models instances create -p /path/to/modelinstance`
 
 ##### Delete model instance
 
 ```
 usage: kaggle models instances delete [-h] [modelInstance]
 
+required arguments:
+  modelInstance         Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>
+
 optional arguments:
   -h, --help     show this help message and exit
-  modelInstance  Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>
 ```
 
 Example:
 
 `kaggle models instances delete tensorflow/toxicity/tfjs/default`
 
 ##### Update a model instance
@@ -782,17 +803,19 @@
 ```
 
 ##### Create a new model instance version
 
 ```
 usage: kaggle models instances versions create [-h] [modelInstance] [-p FOLDER] [-n NOTES]
 
+required arguments:
+  modelInstance         Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>
+
 optional arguments:
   -h, --help            show this help message and exit
-  modelInstance         Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>
   -p FOLDER, --path FOLDER
                         Folder containing the model files to upload
   -n, --version-notes NOTES
                         Version notes to record for this new version
   -q, --quiet           Suppress printing information about the upload progress
   -r {skip,zip,tar}, --dir-mode {skip,zip,tar}
                         What to do with directories: "skip" - ignore; "zip" - compressed upload; "tar" - uncompressed upload
@@ -803,17 +826,19 @@
 `kaggle models instances versions create tensorflow/toxicity/tfjs/default -p /path/to/files -n "updated weights"`
 
 ##### Download a model instance version
 
 ```
 usage: kaggle models instances versions download [-h] [-p PATH] [--untar] [-f] [-q] [modelInstanceVersion]
 
+required arguments:
+  modelInstanceVersion  Model Instance version URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>/<version_number>
+
 optional arguments:
   -h, --help            show this help message and exit
-  modelInstanceVersion  Model Instance version URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>/<version_number>
   -p PATH, --path PATH  Folder where file(s) will be downloaded, defaults to current working directory
   --untar               Untar the downloaded file. Will delete the tar file when completed.
   -f, --force           Skip check whether local version of file is up to date, force file download
   -q, --quiet           Suppress printing information about the download progress
 ```
 
 
@@ -822,17 +847,19 @@
 `kaggle models instances versions download tensorflow/toxicity/tfjs/default/1`
 
 ##### Delete model instance
 
 ```
 usage: kaggle models instances versions delete [-h] [modelInstanceVersion]
 
+required arguments:
+  modelInstanceVersion  Model Instance version URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>/<version_number>
+
 optional arguments:
   -h, --help            show this help message and exit
-  modelInstanceVersion  Model Instance version URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>/<version_number>
 ```
 
 Example:
 
 `kaggle models instances versions delete tensorflow/toxicity/tfjs/default/1`
 
 ### Config
```

### Comparing `kaggle-1.6.0a2/kaggle/__init__.py` & `kaggle-1.6.0a3/kaggle/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/api/__init__.py` & `kaggle-1.6.0a3/kaggle/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/api/kaggle_api.py` & `kaggle-1.6.0a3/kaggle/api/kaggle_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -829,15 +829,15 @@
         >>> thread = api.competitions_submissions_upload(file, guid, content_length, last_modified_date_utc, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param file file: Competition submission file (required)
         :param str guid: Location where submission should be uploaded (required)
         :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
+        :param int last_modified_date_utc: Last modified date of file in seconds since epoch in UTC (required)
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.competitions_submissions_upload_with_http_info(file, guid, content_length, last_modified_date_utc, **kwargs)  # noqa: E501
@@ -853,15 +853,15 @@
         >>> thread = api.competitions_submissions_upload_with_http_info(file, guid, content_length, last_modified_date_utc, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param file file: Competition submission file (required)
         :param str guid: Location where submission should be uploaded (required)
         :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
+        :param int last_modified_date_utc: Last modified date of file in seconds since epoch in UTC (required)
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['file', 'guid', 'content_length', 'last_modified_date_utc']  # noqa: E501
         all_params.append('async_req')
@@ -949,15 +949,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.competitions_submissions_url(id, content_length, last_modified_date_utc, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: Competition name, as it appears in the competition's URL (required)
         :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
+        :param int last_modified_date_utc: Last modified date of file in seconds since epoch in UTC (required)
         :param str file_name: Competition submission file name
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -973,15 +973,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.competitions_submissions_url_with_http_info(id, content_length, last_modified_date_utc, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str id: Competition name, as it appears in the competition's URL (required)
         :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
+        :param int last_modified_date_utc: Last modified date of file in seconds since epoch in UTC (required)
         :param str file_name: Competition submission file name
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id', 'content_length', 'last_modified_date_utc', 'file_name']  # noqa: E501
@@ -1055,14 +1055,111 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def create_inbox_file(self, create_inbox_file_request, **kwargs):  # noqa: E501
+        """Creates (aka \&quot;drops\&quot;) a new file into the inbox.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_inbox_file(create_inbox_file_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param CreateInboxFileRequest create_inbox_file_request: (required)
+        :return: Result
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.create_inbox_file_with_http_info(create_inbox_file_request, **kwargs)  # noqa: E501
+        else:
+            (data) = self.create_inbox_file_with_http_info(create_inbox_file_request, **kwargs)  # noqa: E501
+            return data
+
+    def create_inbox_file_with_http_info(self, create_inbox_file_request, **kwargs):  # noqa: E501
+        """Creates (aka \&quot;drops\&quot;) a new file into the inbox.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_inbox_file_with_http_info(create_inbox_file_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param CreateInboxFileRequest create_inbox_file_request: (required)
+        :return: Result
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['create_inbox_file_request']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_inbox_file" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'create_inbox_file_request' is set
+        if ('create_inbox_file_request' not in params or
+                params['create_inbox_file_request'] is None):
+            raise ValueError("Missing the required parameter `create_inbox_file_request` when calling `create_inbox_file`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'create_inbox_file_request' in params:
+            body_params = params['create_inbox_file_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/inbox/files/create', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Result',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def datasets_create_new(self, dataset_new_request, **kwargs):  # noqa: E501
         """Create a new dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.datasets_create_new(dataset_new_request, async_req=True)
         >>> result = thread.get()
@@ -1728,14 +1825,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.datasets_list_files(owner_slug, dataset_slug, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner_slug: Dataset owner (required)
         :param str dataset_slug: Dataset name (required)
+        :param str dataset_version_number: Dataset version number
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.datasets_list_files_with_http_info(owner_slug, dataset_slug, **kwargs)  # noqa: E501
@@ -1750,20 +1848,21 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.datasets_list_files_with_http_info(owner_slug, dataset_slug, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner_slug: Dataset owner (required)
         :param str dataset_slug: Dataset name (required)
+        :param str dataset_version_number: Dataset version number
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['owner_slug', 'dataset_slug']  # noqa: E501
+        all_params = ['owner_slug', 'dataset_slug', 'dataset_version_number']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1788,14 +1887,16 @@
         path_params = {}
         if 'owner_slug' in params:
             path_params['ownerSlug'] = params['owner_slug']  # noqa: E501
         if 'dataset_slug' in params:
             path_params['datasetSlug'] = params['dataset_slug']  # noqa: E501
 
         query_params = []
+        if 'dataset_version_number' in params:
+            query_params.append(('datasetVersionNumber', params['dataset_version_number']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1919,228 +2020,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def datasets_upload_file(self, file_name, content_length, last_modified_date_utc, **kwargs):  # noqa: E501
-        """Get URL and token to start uploading a data file  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.datasets_upload_file(file_name, content_length, last_modified_date_utc, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str file_name: Dataset file name (required)
-        :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
-        :return: Result
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.datasets_upload_file_with_http_info(file_name, content_length, last_modified_date_utc, **kwargs)  # noqa: E501
-        else:
-            (data) = self.datasets_upload_file_with_http_info(file_name, content_length, last_modified_date_utc, **kwargs)  # noqa: E501
-            return data
-
-    def datasets_upload_file_with_http_info(self, file_name, content_length, last_modified_date_utc, **kwargs):  # noqa: E501
-        """Get URL and token to start uploading a data file  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.datasets_upload_file_with_http_info(file_name, content_length, last_modified_date_utc, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str file_name: Dataset file name (required)
-        :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
-        :return: Result
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['file_name', 'content_length', 'last_modified_date_utc']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method datasets_upload_file" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'file_name' is set
-        if ('file_name' not in params or
-                params['file_name'] is None):
-            raise ValueError("Missing the required parameter `file_name` when calling `datasets_upload_file`")  # noqa: E501
-        # verify the required parameter 'content_length' is set
-        if ('content_length' not in params or
-                params['content_length'] is None):
-            raise ValueError("Missing the required parameter `content_length` when calling `datasets_upload_file`")  # noqa: E501
-        # verify the required parameter 'last_modified_date_utc' is set
-        if ('last_modified_date_utc' not in params or
-                params['last_modified_date_utc'] is None):
-            raise ValueError("Missing the required parameter `last_modified_date_utc` when calling `datasets_upload_file`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'content_length' in params:
-            path_params['contentLength'] = params['content_length']  # noqa: E501
-        if 'last_modified_date_utc' in params:
-            path_params['lastModifiedDateUtc'] = params['last_modified_date_utc']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-        if 'file_name' in params:
-            form_params.append(('fileName', params['file_name']))  # noqa: E501
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['multipart/form-data'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['basicAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/datasets/upload/file/{contentLength}/{lastModifiedDateUtc}', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='Result',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def datasets_view(self, owner_slug, dataset_slug, **kwargs):  # noqa: E501
-        """Show details about a dataset  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.datasets_view(owner_slug, dataset_slug, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str owner_slug: Dataset owner (required)
-        :param str dataset_slug: Dataset name (required)
-        :return: Result
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.datasets_view_with_http_info(owner_slug, dataset_slug, **kwargs)  # noqa: E501
-        else:
-            (data) = self.datasets_view_with_http_info(owner_slug, dataset_slug, **kwargs)  # noqa: E501
-            return data
-
-    def datasets_view_with_http_info(self, owner_slug, dataset_slug, **kwargs):  # noqa: E501
-        """Show details about a dataset  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.datasets_view_with_http_info(owner_slug, dataset_slug, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str owner_slug: Dataset owner (required)
-        :param str dataset_slug: Dataset name (required)
-        :return: Result
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['owner_slug', 'dataset_slug']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method datasets_view" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'owner_slug' is set
-        if ('owner_slug' not in params or
-                params['owner_slug'] is None):
-            raise ValueError("Missing the required parameter `owner_slug` when calling `datasets_view`")  # noqa: E501
-        # verify the required parameter 'dataset_slug' is set
-        if ('dataset_slug' not in params or
-                params['dataset_slug'] is None):
-            raise ValueError("Missing the required parameter `dataset_slug` when calling `datasets_view`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'owner_slug' in params:
-            path_params['ownerSlug'] = params['owner_slug']  # noqa: E501
-        if 'dataset_slug' in params:
-            path_params['datasetSlug'] = params['dataset_slug']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['basicAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/datasets/view/{ownerSlug}/{datasetSlug}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='Result',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def delete_model(self, owner_slug, model_slug, **kwargs):  # noqa: E501
         """Delete a model  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_model(owner_slug, model_slug, async_req=True)
         >>> result = thread.get()
@@ -4026,361 +3913,345 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def models_upload_file(self, file_name, content_length, last_modified_date_utc, **kwargs):  # noqa: E501
-        """Get URL and token to start uploading a model file  # noqa: E501
+    def update_model(self, owner_slug, model_slug, model_update_request, **kwargs):  # noqa: E501
+        """Update a model  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_upload_file(file_name, content_length, last_modified_date_utc, async_req=True)
+        >>> thread = api.update_model(owner_slug, model_slug, model_update_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str file_name: Model file name (required)
-        :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
+        :param str owner_slug: Model owner (required)
+        :param str model_slug: Model name (required)
+        :param ModelUpdateRequest model_update_request: Information for updating a model (required)
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.models_upload_file_with_http_info(file_name, content_length, last_modified_date_utc, **kwargs)  # noqa: E501
+            return self.update_model_with_http_info(owner_slug, model_slug, model_update_request, **kwargs)  # noqa: E501
         else:
-            (data) = self.models_upload_file_with_http_info(file_name, content_length, last_modified_date_utc, **kwargs)  # noqa: E501
+            (data) = self.update_model_with_http_info(owner_slug, model_slug, model_update_request, **kwargs)  # noqa: E501
             return data
 
-    def models_upload_file_with_http_info(self, file_name, content_length, last_modified_date_utc, **kwargs):  # noqa: E501
-        """Get URL and token to start uploading a model file  # noqa: E501
+    def update_model_with_http_info(self, owner_slug, model_slug, model_update_request, **kwargs):  # noqa: E501
+        """Update a model  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.models_upload_file_with_http_info(file_name, content_length, last_modified_date_utc, async_req=True)
+        >>> thread = api.update_model_with_http_info(owner_slug, model_slug, model_update_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str file_name: Model file name (required)
-        :param int content_length: Content length of file in bytes (required)
-        :param int last_modified_date_utc: Last modified date of file in milliseconds since epoch in UTC (required)
+        :param str owner_slug: Model owner (required)
+        :param str model_slug: Model name (required)
+        :param ModelUpdateRequest model_update_request: Information for updating a model (required)
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['file_name', 'content_length', 'last_modified_date_utc']  # noqa: E501
+        all_params = ['owner_slug', 'model_slug', 'model_update_request']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method models_upload_file" % key
+                    " to method update_model" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'file_name' is set
-        if ('file_name' not in params or
-                params['file_name'] is None):
-            raise ValueError("Missing the required parameter `file_name` when calling `models_upload_file`")  # noqa: E501
-        # verify the required parameter 'content_length' is set
-        if ('content_length' not in params or
-                params['content_length'] is None):
-            raise ValueError("Missing the required parameter `content_length` when calling `models_upload_file`")  # noqa: E501
-        # verify the required parameter 'last_modified_date_utc' is set
-        if ('last_modified_date_utc' not in params or
-                params['last_modified_date_utc'] is None):
-            raise ValueError("Missing the required parameter `last_modified_date_utc` when calling `models_upload_file`")  # noqa: E501
+        # verify the required parameter 'owner_slug' is set
+        if ('owner_slug' not in params or
+                params['owner_slug'] is None):
+            raise ValueError("Missing the required parameter `owner_slug` when calling `update_model`")  # noqa: E501
+        # verify the required parameter 'model_slug' is set
+        if ('model_slug' not in params or
+                params['model_slug'] is None):
+            raise ValueError("Missing the required parameter `model_slug` when calling `update_model`")  # noqa: E501
+        # verify the required parameter 'model_update_request' is set
+        if ('model_update_request' not in params or
+                params['model_update_request'] is None):
+            raise ValueError("Missing the required parameter `model_update_request` when calling `update_model`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'content_length' in params:
-            path_params['contentLength'] = params['content_length']  # noqa: E501
-        if 'last_modified_date_utc' in params:
-            path_params['lastModifiedDateUtc'] = params['last_modified_date_utc']  # noqa: E501
+        if 'owner_slug' in params:
+            path_params['ownerSlug'] = params['owner_slug']  # noqa: E501
+        if 'model_slug' in params:
+            path_params['modelSlug'] = params['model_slug']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
-        if 'file_name' in params:
-            form_params.append(('fileName', params['file_name']))  # noqa: E501
 
         body_params = None
+        if 'model_update_request' in params:
+            body_params = params['model_update_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['multipart/form-data'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/models/upload/file/{contentLength}/{lastModifiedDateUtc}', 'POST',
+            '/models/{ownerSlug}/{modelSlug}/update', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Result',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_model(self, owner_slug, model_slug, model_update_request, **kwargs):  # noqa: E501
+    def update_model_instance(self, owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs):  # noqa: E501
         """Update a model  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_model(owner_slug, model_slug, model_update_request, async_req=True)
+        >>> thread = api.update_model_instance(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner_slug: Model owner (required)
         :param str model_slug: Model name (required)
-        :param ModelUpdateRequest model_update_request: Information for updating a model (required)
+        :param str framework: Model instance framework (required)
+        :param str instance_slug: Model instance slug (required)
+        :param ModelInstanceUpdateRequest model_instance_update_request: Information for updating a model instance (required)
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.update_model_with_http_info(owner_slug, model_slug, model_update_request, **kwargs)  # noqa: E501
+            return self.update_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs)  # noqa: E501
         else:
-            (data) = self.update_model_with_http_info(owner_slug, model_slug, model_update_request, **kwargs)  # noqa: E501
+            (data) = self.update_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs)  # noqa: E501
             return data
 
-    def update_model_with_http_info(self, owner_slug, model_slug, model_update_request, **kwargs):  # noqa: E501
+    def update_model_instance_with_http_info(self, owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs):  # noqa: E501
         """Update a model  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_model_with_http_info(owner_slug, model_slug, model_update_request, async_req=True)
+        >>> thread = api.update_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner_slug: Model owner (required)
         :param str model_slug: Model name (required)
-        :param ModelUpdateRequest model_update_request: Information for updating a model (required)
+        :param str framework: Model instance framework (required)
+        :param str instance_slug: Model instance slug (required)
+        :param ModelInstanceUpdateRequest model_instance_update_request: Information for updating a model instance (required)
         :return: Result
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['owner_slug', 'model_slug', 'model_update_request']  # noqa: E501
+        all_params = ['owner_slug', 'model_slug', 'framework', 'instance_slug', 'model_instance_update_request']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_model" % key
+                    " to method update_model_instance" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'owner_slug' is set
         if ('owner_slug' not in params or
                 params['owner_slug'] is None):
-            raise ValueError("Missing the required parameter `owner_slug` when calling `update_model`")  # noqa: E501
+            raise ValueError("Missing the required parameter `owner_slug` when calling `update_model_instance`")  # noqa: E501
         # verify the required parameter 'model_slug' is set
         if ('model_slug' not in params or
                 params['model_slug'] is None):
-            raise ValueError("Missing the required parameter `model_slug` when calling `update_model`")  # noqa: E501
-        # verify the required parameter 'model_update_request' is set
-        if ('model_update_request' not in params or
-                params['model_update_request'] is None):
-            raise ValueError("Missing the required parameter `model_update_request` when calling `update_model`")  # noqa: E501
+            raise ValueError("Missing the required parameter `model_slug` when calling `update_model_instance`")  # noqa: E501
+        # verify the required parameter 'framework' is set
+        if ('framework' not in params or
+                params['framework'] is None):
+            raise ValueError("Missing the required parameter `framework` when calling `update_model_instance`")  # noqa: E501
+        # verify the required parameter 'instance_slug' is set
+        if ('instance_slug' not in params or
+                params['instance_slug'] is None):
+            raise ValueError("Missing the required parameter `instance_slug` when calling `update_model_instance`")  # noqa: E501
+        # verify the required parameter 'model_instance_update_request' is set
+        if ('model_instance_update_request' not in params or
+                params['model_instance_update_request'] is None):
+            raise ValueError("Missing the required parameter `model_instance_update_request` when calling `update_model_instance`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'owner_slug' in params:
             path_params['ownerSlug'] = params['owner_slug']  # noqa: E501
         if 'model_slug' in params:
             path_params['modelSlug'] = params['model_slug']  # noqa: E501
+        if 'framework' in params:
+            path_params['framework'] = params['framework']  # noqa: E501
+        if 'instance_slug' in params:
+            path_params['instanceSlug'] = params['instance_slug']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'model_update_request' in params:
-            body_params = params['model_update_request']
+        if 'model_instance_update_request' in params:
+            body_params = params['model_instance_update_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/models/{ownerSlug}/{modelSlug}/update', 'POST',
+            '/models/{ownerSlug}/{modelSlug}/{framework}/{instanceSlug}/update', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Result',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_model_instance(self, owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs):  # noqa: E501
-        """Update a model  # noqa: E501
+    def upload_file(self, start_blob_upload_request, **kwargs):  # noqa: E501
+        """Start uploading a file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_model_instance(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, async_req=True)
+        >>> thread = api.upload_file(start_blob_upload_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str owner_slug: Model owner (required)
-        :param str model_slug: Model name (required)
-        :param str framework: Model instance framework (required)
-        :param str instance_slug: Model instance slug (required)
-        :param ModelInstanceUpdateRequest model_instance_update_request: Information for updating a model instance (required)
-        :return: Result
+        :param StartBlobUploadRequest start_blob_upload_request: (required)
+        :return: StartBlobUploadResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.update_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs)  # noqa: E501
+            return self.upload_file_with_http_info(start_blob_upload_request, **kwargs)  # noqa: E501
         else:
-            (data) = self.update_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs)  # noqa: E501
+            (data) = self.upload_file_with_http_info(start_blob_upload_request, **kwargs)  # noqa: E501
             return data
 
-    def update_model_instance_with_http_info(self, owner_slug, model_slug, framework, instance_slug, model_instance_update_request, **kwargs):  # noqa: E501
-        """Update a model  # noqa: E501
+    def upload_file_with_http_info(self, start_blob_upload_request, **kwargs):  # noqa: E501
+        """Start uploading a file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, model_instance_update_request, async_req=True)
+        >>> thread = api.upload_file_with_http_info(start_blob_upload_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str owner_slug: Model owner (required)
-        :param str model_slug: Model name (required)
-        :param str framework: Model instance framework (required)
-        :param str instance_slug: Model instance slug (required)
-        :param ModelInstanceUpdateRequest model_instance_update_request: Information for updating a model instance (required)
-        :return: Result
+        :param StartBlobUploadRequest start_blob_upload_request: (required)
+        :return: StartBlobUploadResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['owner_slug', 'model_slug', 'framework', 'instance_slug', 'model_instance_update_request']  # noqa: E501
+        all_params = ['start_blob_upload_request']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_model_instance" % key
+                    " to method upload_file" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'owner_slug' is set
-        if ('owner_slug' not in params or
-                params['owner_slug'] is None):
-            raise ValueError("Missing the required parameter `owner_slug` when calling `update_model_instance`")  # noqa: E501
-        # verify the required parameter 'model_slug' is set
-        if ('model_slug' not in params or
-                params['model_slug'] is None):
-            raise ValueError("Missing the required parameter `model_slug` when calling `update_model_instance`")  # noqa: E501
-        # verify the required parameter 'framework' is set
-        if ('framework' not in params or
-                params['framework'] is None):
-            raise ValueError("Missing the required parameter `framework` when calling `update_model_instance`")  # noqa: E501
-        # verify the required parameter 'instance_slug' is set
-        if ('instance_slug' not in params or
-                params['instance_slug'] is None):
-            raise ValueError("Missing the required parameter `instance_slug` when calling `update_model_instance`")  # noqa: E501
-        # verify the required parameter 'model_instance_update_request' is set
-        if ('model_instance_update_request' not in params or
-                params['model_instance_update_request'] is None):
-            raise ValueError("Missing the required parameter `model_instance_update_request` when calling `update_model_instance`")  # noqa: E501
+        # verify the required parameter 'start_blob_upload_request' is set
+        if ('start_blob_upload_request' not in params or
+                params['start_blob_upload_request'] is None):
+            raise ValueError("Missing the required parameter `start_blob_upload_request` when calling `upload_file`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'owner_slug' in params:
-            path_params['ownerSlug'] = params['owner_slug']  # noqa: E501
-        if 'model_slug' in params:
-            path_params['modelSlug'] = params['model_slug']  # noqa: E501
-        if 'framework' in params:
-            path_params['framework'] = params['framework']  # noqa: E501
-        if 'instance_slug' in params:
-            path_params['instanceSlug'] = params['instance_slug']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'model_instance_update_request' in params:
-            body_params = params['model_instance_update_request']
+        if 'start_blob_upload_request' in params:
+            body_params = params['start_blob_upload_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/models/{ownerSlug}/{modelSlug}/{framework}/{instanceSlug}/update', 'POST',
+            '/blobs/upload', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='Result',  # noqa: E501
+            response_type='StartBlobUploadResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `kaggle-1.6.0a2/kaggle/api/kaggle_api_extended.py` & `kaggle-1.6.0a3/kaggle/api/kaggle_api_extended.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,34 +34,34 @@
 from __future__ import print_function
 import csv
 from datetime import datetime
 import io
 import json
 import os
 from os.path import expanduser
-from os.path import isfile
 import sys
 import shutil
 import tarfile
 import zipfile
 import tempfile
 from ..api_client import ApiClient
 from kaggle.configuration import Configuration
 from .kaggle_api import KaggleApi
+from ..models.api_blob_type import ApiBlobType
 from ..models.collaborator import Collaborator
+from ..models.create_inbox_file_request import CreateInboxFileRequest
 from ..models.dataset_column import DatasetColumn
 from ..models.dataset_new_request import DatasetNewRequest
 from ..models.dataset_new_version_request import DatasetNewVersionRequest
 from ..models.dataset_update_settings_request import DatasetUpdateSettingsRequest
 from ..models.kaggle_models_extended import Competition
 from ..models.kaggle_models_extended import Dataset
 from ..models.kaggle_models_extended import DatasetNewResponse
 from ..models.kaggle_models_extended import DatasetNewVersionResponse
 from ..models.kaggle_models_extended import File
-from ..models.kaggle_models_extended import FileUploadInfo
 from ..models.kaggle_models_extended import Kernel
 from ..models.kaggle_models_extended import KernelPushResponse
 from ..models.kaggle_models_extended import LeaderboardEntry
 from ..models.kaggle_models_extended import ListFilesResult
 from ..models.kaggle_models_extended import Metadata
 from ..models.kaggle_models_extended import Model
 from ..models.kaggle_models_extended import ModelNewResponse
@@ -71,46 +71,68 @@
 from ..models.kernel_push_request import KernelPushRequest
 from ..models.license import License
 from ..models.model_new_request import ModelNewRequest
 from ..models.model_new_instance_request import ModelNewInstanceRequest
 from ..models.model_instance_new_version_request import ModelInstanceNewVersionRequest
 from ..models.model_update_request import ModelUpdateRequest
 from ..models.model_instance_update_request import ModelInstanceUpdateRequest
+from ..models.start_blob_upload_request import StartBlobUploadRequest
 from ..models.upload_file import UploadFile
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from ..rest import ApiException
 import six
 from slugify import slugify
 from tqdm import tqdm
 import bleach
+import time
 
 try:
     unicode  # Python 2
 except NameError:
     unicode = str  # Python 3
 
 
+class DirectoryArchive(object):
+
+    def __init__(self, fullpath, format):
+        self._fullpath = fullpath
+        self._format = format
+        self.name = None
+        self.path = None
+
+    def __enter__(self):
+        self._temp_dir = tempfile.mkdtemp()
+        _, dir_name = os.path.split(self._fullpath)
+        self.path = shutil.make_archive(os.path.join(self._temp_dir, dir_name),
+                                        self._format, self._fullpath)
+        _, self.name = os.path.split(self.path)
+
+    def __exit__(self, *args):
+        shutil.rmtree(self._temp_dir)
+
+
 class KaggleApi(KaggleApi):
-    __version__ = '1.6.0a2'
+    __version__ = '1.6.0a3'
 
     CONFIG_NAME_PROXY = 'proxy'
     CONFIG_NAME_COMPETITION = 'competition'
     CONFIG_NAME_PATH = 'path'
     CONFIG_NAME_USER = 'username'
     CONFIG_NAME_KEY = 'key'
     CONFIG_NAME_SSL_CA_CERT = 'ssl_ca_cert'
 
     HEADER_API_VERSION = 'X-Kaggle-ApiVersion'
     DATASET_METADATA_FILE = 'dataset-metadata.json'
     OLD_DATASET_METADATA_FILE = 'datapackage.json'
     KERNEL_METADATA_FILE = 'kernel-metadata.json'
     MODEL_METADATA_FILE = 'model-metadata.json'
     MODEL_INSTANCE_METADATA_FILE = 'model-instance-metadata.json'
+    MAX_NUM_INBOX_FILES_TO_UPLOAD = 1000
 
     config_dir = os.environ.get('KAGGLE_CONFIG_DIR') or os.path.join(
         expanduser('~'), '.kaggle')
     if not os.path.exists(config_dir):
         os.makedirs(config_dir)
 
     config_file = 'kaggle.json'
@@ -705,15 +727,15 @@
         response = self.process_response(
             self.competitions_data_download_file_with_http_info(
                 id=competition, file_name=file_name, _preload_content=False))
         url = response.retries.history[0].redirect_location.split('?')[0]
         outfile = os.path.join(effective_path, url.split('/')[-1])
 
         if force or self.download_needed(response, outfile, quiet):
-            self.download_file(response, outfile, quiet)
+            self.download_file(response, outfile, quiet, not force)
 
     def competition_download_files(self,
                                    competition,
                                    path=None,
                                    force=False,
                                    quiet=True):
         """ downloads all competition files.
@@ -735,15 +757,15 @@
             self.competitions_data_download_files_with_http_info(
                 id=competition, _preload_content=False))
         url = response.retries.history[0].redirect_location.split('?')[0]
         outfile = os.path.join(effective_path,
                                competition + '.' + url.split('.')[-1])
 
         if force or self.download_needed(response, outfile, quiet):
-            self.download_file(response, outfile, quiet)
+            self.download_file(response, outfile, quiet, not force)
 
     def competition_download_cli(self,
                                  competition,
                                  competition_opt=None,
                                  file_name=None,
                                  path=None,
                                  force=False,
@@ -980,35 +1002,14 @@
             if csv_display:
                 self.print_csv(datasets, fields)
             else:
                 self.print_table(datasets, fields)
         else:
             print('No datasets found')
 
-    def dataset_view(self, dataset):
-        """ view metadata for a dataset.
-
-            Parameters
-            ==========
-            dataset: the string identified of the dataset
-                     should be in format [owner]/[dataset-name]
-        """
-        if '/' in dataset:
-            self.validate_dataset_string(dataset)
-            dataset_urls = dataset.split('/')
-            owner_slug = dataset_urls[0]
-            dataset_slug = dataset_urls[1]
-        else:
-            owner_slug = self.get_config_value(self.CONFIG_NAME_USER)
-            dataset_slug = dataset
-
-        result = self.process_response(
-            self.datasets_view_with_http_info(owner_slug, dataset_slug))
-        return Dataset(result)
-
     def dataset_metadata_prep(self, dataset, path):
         if dataset is None:
             raise ValueError('A dataset must be specified')
         if '/' in dataset:
             self.validate_dataset_string(dataset)
             dataset_urls = dataset.split('/')
             owner_slug = dataset_urls[0]
@@ -1087,25 +1088,22 @@
              Parameters
             ==========
             dataset: the string identified of the dataset
                      should be in format [owner]/[dataset-name]
         """
         if dataset is None:
             raise ValueError('A dataset must be specified')
-        if '/' in dataset:
-            self.validate_dataset_string(dataset)
-            dataset_urls = dataset.split('/')
-            owner_slug = dataset_urls[0]
-            dataset_slug = dataset_urls[1]
-        else:
-            owner_slug = self.get_config_value(self.CONFIG_NAME_USER)
-            dataset_slug = dataset
+        owner_slug, dataset_slug, dataset_version_number = self.split_dataset_string(
+            dataset)
+
         dataset_list_files_result = self.process_response(
-            self.datasets_list_files_with_http_info(owner_slug=owner_slug,
-                                                    dataset_slug=dataset_slug))
+            self.datasets_list_files_with_http_info(
+                owner_slug=owner_slug,
+                dataset_slug=dataset_slug,
+                dataset_version_number=dataset_version_number))
         return ListFilesResult(dataset_list_files_result)
 
     def dataset_list_files_cli(self,
                                dataset,
                                dataset_opt=None,
                                csv_display=False):
         """ a wrapper to dataset_list_files for the client
@@ -1200,15 +1198,15 @@
                 owner_slug=owner_slug,
                 dataset_slug=dataset_slug,
                 file_name=file_name,
                 _preload_content=False))
         url = response.retries.history[0].redirect_location.split('?')[0]
         outfile = os.path.join(effective_path, url.split('/')[-1])
         if force or self.download_needed(response, outfile, quiet):
-            self.download_file(response, outfile, quiet)
+            self.download_file(response, outfile, quiet, not force)
             return True
         else:
             return False
 
     def dataset_download_files(self,
                                dataset,
                                path=None,
@@ -1224,37 +1222,32 @@
             path: the path to download the dataset to
             force: force the download if the file already exists (default False)
             quiet: suppress verbose output (default is True)
             unzip: if True, unzip files upon download (default is False)
         """
         if dataset is None:
             raise ValueError('A dataset must be specified')
-        if '/' in dataset:
-            self.validate_dataset_string(dataset)
-            dataset_urls = dataset.split('/')
-            owner_slug = dataset_urls[0]
-            dataset_slug = dataset_urls[1]
-        else:
-            owner_slug = self.get_config_value(self.CONFIG_NAME_USER)
-            dataset_slug = dataset
-
+        owner_slug, dataset_slug, dataset_version_number = self.split_dataset_string(
+            dataset)
         if path is None:
             effective_path = self.get_default_download_dir(
                 'datasets', owner_slug, dataset_slug)
         else:
             effective_path = path
 
         response = self.process_response(
-            self.datasets_download_with_http_info(owner_slug=owner_slug,
-                                                  dataset_slug=dataset_slug,
-                                                  _preload_content=False))
+            self.datasets_download_with_http_info(
+                owner_slug=owner_slug,
+                dataset_slug=dataset_slug,
+                dataset_version_number=dataset_version_number,
+                _preload_content=False))
 
         outfile = os.path.join(effective_path, dataset_slug + '.zip')
         if force or self.download_needed(response, outfile, quiet):
-            self.download_file(response, outfile, quiet)
+            self.download_file(response, outfile, quiet, not force)
             downloaded = True
         else:
             downloaded = False
 
         if downloaded:
             outfile = os.path.join(effective_path, dataset_slug + '.zip')
             if unzip:
@@ -1304,46 +1297,38 @@
         else:
             self.dataset_download_file(dataset,
                                        file_name,
                                        path=path,
                                        force=force,
                                        quiet=quiet)
 
-    def upload_file(self, path, quiet, entity='dataset'):
+    def _upload_blob(self, path, quiet, blob_type):
         """ upload a file
 
             Parameters
             ==========
             path: the complete path to upload
             quiet: suppress verbose output (default is False)
-            dataset: whether is a dataset file, otherwise it's a model file
-            entity: dataset or model
+            blob_type (ApiBlobType): To which entity the file/blob refers
         """
         file_name = os.path.basename(path)
         content_length = os.path.getsize(path)
-        last_modified_date_utc = int(os.path.getmtime(path))
-        result = None
+        last_modified_epoch_seconds = int(os.path.getmtime(path))
 
-        if entity == 'dataset':
-            result = FileUploadInfo(
-                self.process_response(
-                    self.datasets_upload_file_with_http_info(
-                        file_name, content_length, last_modified_date_utc)))
-        elif entity == 'model':
-            result = FileUploadInfo(
-                self.process_response(
-                    self.models_upload_file_with_http_info(
-                        file_name, content_length, last_modified_date_utc)))
-        else:
-            raise ValueError('Invalid entity to upload: ' + entity)
-
-        success = self.upload_complete(path, result.createUrl, quiet)
+        request = StartBlobUploadRequest(
+            blob_type,
+            file_name,
+            content_length,
+            last_modified_epoch_seconds=last_modified_epoch_seconds)
+        response = self.process_response(
+            self.upload_file_with_http_info(request))
+        success = self.upload_complete(path, response.create_url, quiet)
 
         if success:
-            return result.token
+            return response.token
         return None
 
     def dataset_create_version(self,
                                folder,
                                version_notes,
                                quiet=False,
                                convert_to_csv=True,
@@ -1388,16 +1373,16 @@
             version_notes=version_notes,
             subtitle=subtitle,
             description=description,
             files=[],
             convert_to_csv=convert_to_csv,
             category_ids=keywords,
             delete_old_versions=delete_old_versions)
-        self.upload_files(request, resources, folder, 'dataset', quiet,
-                          dir_mode)
+        self.upload_files(request, resources, folder, ApiBlobType.DATASET,
+                          quiet, dir_mode)
 
         if id_no:
             result = DatasetNewVersionResponse(
                 self.process_response(
                     self.datasets_create_version_by_id_with_http_info(
                         id_no, request)))
         else:
@@ -1438,20 +1423,21 @@
         result = self.dataset_create_version(
             folder,
             version_notes,
             quiet=quiet,
             convert_to_csv=convert_to_csv,
             delete_old_versions=delete_old_versions,
             dir_mode=dir_mode)
-        if result.invalidTags:
+
+        if result is None:
+            print('Dataset version creation error: See previous output')
+        elif result.invalidTags:
             print(
                 ('The following are not valid tags and could not be added to '
                  'the dataset: ') + str(result.invalidTags))
-        if result is None:
-            print('Dataset version creation error: See previous output')
         elif result.status.lower() == 'ok':
             print(
                 'Dataset version is being created. Please check progress at ' +
                 result.url)
         else:
             print('Dataset version creation error: ' + result.error)
 
@@ -1553,16 +1539,16 @@
                                     license_name=license_name,
                                     subtitle=subtitle,
                                     description=description,
                                     files=[],
                                     is_private=not public,
                                     convert_to_csv=convert_to_csv,
                                     category_ids=keywords)
-        self.upload_files(request, resources, folder, 'dataset', quiet,
-                          dir_mode)
+        self.upload_files(request, resources, folder, ApiBlobType.DATASET,
+                          quiet, dir_mode)
         result = DatasetNewResponse(
             self.process_response(
                 self.datasets_create_new_with_http_info(request)))
 
         return result
 
     def dataset_create_new_cli(self,
@@ -1592,49 +1578,89 @@
                       'progress at ' + result.url)
             else:
                 print('Your private Dataset is being created. Please check '
                       'progress at ' + result.url)
         else:
             print('Dataset creation error: ' + result.error)
 
-    def download_file(self, response, outfile, quiet=True, chunk_size=1048576):
+    def download_file(self,
+                      response,
+                      outfile,
+                      quiet=True,
+                      resume=False,
+                      chunk_size=1048576):
         """ download a file to an output file based on a chunk size
 
             Parameters
             ==========
             response: the response to download
             outfile: the output file to download to
             quiet: suppress verbose output (default is True)
             chunk_size: the size of the chunk to stream
+            resume: whether to resume an existing download
         """
 
         outpath = os.path.dirname(outfile)
         if not os.path.exists(outpath):
             os.makedirs(outpath)
         size = int(response.headers['Content-Length'])
         size_read = 0
+        open_mode = 'wb'
+        remote_date = datetime.strptime(response.headers['Last-Modified'],
+                                        '%a, %d %b %Y %X %Z')
+        remote_date_timestamp = time.mktime(remote_date.timetuple())
+
         if not quiet:
             print('Downloading ' + os.path.basename(outfile) + ' to ' +
                   outpath)
+
+        file_exists = os.path.isfile(outfile)
+        resumable = 'Accept-Ranges' in response.headers and response.headers[
+            'Accept-Ranges'] == 'bytes'
+
+        if resume and resumable and file_exists:
+            size_read = os.path.getsize(outfile)
+            open_mode = 'ab'
+
+            if not quiet:
+                print("... resuming from %d bytes (%d bytes left) ..." % (
+                    size_read,
+                    size - size_read,
+                ))
+
+            request_history = response.retries.history[0]
+            response = self.api_client.request(
+                request_history.method,
+                request_history.redirect_location,
+                headers={'Range': 'bytes=%d-' % (size_read, )},
+                _preload_content=False)
+
         with tqdm(total=size,
+                  initial=size_read,
                   unit='B',
                   unit_scale=True,
                   unit_divisor=1024,
                   disable=quiet) as pbar:
-            with open(outfile, 'wb') as out:
+            with open(outfile, open_mode) as out:
                 while True:
                     data = response.read(chunk_size)
                     if not data:
                         break
                     out.write(data)
+                    os.utime(outfile,
+                             times=(remote_date_timestamp - 1,
+                                    remote_date_timestamp - 1))
                     size_read = min(size, size_read + chunk_size)
                     pbar.update(len(data))
             if not quiet:
                 print('\n', end='')
 
+            os.utime(outfile,
+                     times=(remote_date_timestamp, remote_date_timestamp))
+
     def kernels_list(self,
                      page=1,
                      page_size=20,
                      dataset=None,
                      competition=None,
                      parent_kernel=None,
                      search=None,
@@ -1749,15 +1775,15 @@
         fields = ['ref', 'title', 'author', 'lastRunTime', 'totalVotes']
         if kernels:
             if csv_display:
                 self.print_csv(kernels, fields)
             else:
                 self.print_table(kernels, fields)
         else:
-            print('No kernels found')
+            print('Not found')
 
     def kernels_initialize(self, folder):
         """ create a new kernel in a specified folder from template, including
             json metadata that grabs values from the configuration.
              Parameters
             ==========
             folder: the path of the folder
@@ -1783,14 +1809,16 @@
             'kernel_type':
             'Pick one of: {' +
             ','.join(x for x in self.valid_push_kernel_types) + '}',
             'is_private':
             'true',
             'enable_gpu':
             'false',
+            'enable_tpu':
+            'false',
             'enable_internet':
             'true',
             'dataset_sources': [],
             'competition_sources': [],
             'kernel_sources': [],
             'model_sources': [],
         }
@@ -1915,14 +1943,15 @@
             slug=slug,
             new_title=self.get_or_default(meta_data, 'title', None),
             text=script_body,
             language=language,
             kernel_type=kernel_type,
             is_private=self.get_or_default(meta_data, 'is_private', None),
             enable_gpu=self.get_or_default(meta_data, 'enable_gpu', None),
+            enable_tpu=self.get_or_default(meta_data, 'enable_tpu', None),
             enable_internet=self.get_or_default(meta_data, 'enable_internet',
                                                 None),
             dataset_data_sources=dataset_sources,
             competition_data_sources=self.get_or_default(
                 meta_data, 'competition_sources', []),
             kernel_data_sources=kernel_sources,
             model_data_sources=model_sources,
@@ -2089,14 +2118,16 @@
             data['code_file'] = file_name
             data['language'] = server_metadata['language']
             data['kernel_type'] = server_metadata['kernelType']
             self.set_if_present(server_metadata, 'isPrivate', data,
                                 'is_private')
             self.set_if_present(server_metadata, 'enableGpu', data,
                                 'enable_gpu')
+            self.set_if_present(server_metadata, 'enableTpu', data,
+                                'enable_tpu')
             self.set_if_present(server_metadata, 'enableInternet', data,
                                 'enable_internet')
             self.set_if_present(server_metadata, 'categoryIds', data,
                                 'keywords')
             self.set_if_present(server_metadata, 'datasetDataSources', data,
                                 'dataset_sources')
             self.set_if_present(server_metadata, 'kernelDataSources', data,
@@ -2241,32 +2272,30 @@
     def model_get(self, model):
         """ call to get a model from the API
              Parameters
             ==========
             model: the string identified of the model
                      should be in format [owner]/[model-name]
         """
-        if model is None:
-            raise ValueError('A model must be specified')
         owner_slug, model_slug = self.split_model_string(model)
 
         model_get_result = self.process_response(
             self.get_model_with_http_info(owner_slug, model_slug))
         return model_get_result
 
-    def model_get_cli(self, model, folder=None, model_opt=None):
+    def model_get_cli(self, model, folder=None):
         """ wrapper for client for model_get, with additional
             model_opt to get a model from the API
              Parameters
             ==========
+            model: the string identified of the model
+                     should be in format [owner]/[model-name]
             folder: the folder to download the model metadata file
-            model_opt: an alternative to model
         """
-        m = model or model_opt
-        model = self.model_get(m)
+        model = self.model_get(model)
         if folder is None:
             self.print_obj(model)
         else:
             meta_file = os.path.join(folder, self.MODEL_METADATA_FILE)
 
             data = {}
             data['id'] = model['id']
@@ -2419,14 +2448,16 @@
                 'Default title detected, please change values before uploading'
             )
         if slug == 'INSERT_SLUG_HERE':
             raise ValueError(
                 'Default slug detected, please change values before uploading')
         if not isinstance(is_private, bool):
             raise ValueError('model.isPrivate must be a boolean')
+        if publish_time:
+            self.validate_date(publish_time)
 
         request = ModelNewRequest(owner_slug=owner_slug,
                                   slug=slug,
                                   title=title,
                                   subtitle=subtitle,
                                   is_private=is_private,
                                   description=description,
@@ -2456,32 +2487,33 @@
     def model_delete(self, model):
         """ call to delete a model from the API
              Parameters
             ==========
             model: the string identified of the model
                      should be in format [owner]/[model-name]
         """
-        if model is None:
-            raise ValueError('A model must be specified')
         owner_slug, model_slug = self.split_model_string(model)
 
+        if not self.confirmation():
+            print('Deletion cancelled')
+            exit(0)
+
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_with_http_info(owner_slug, model_slug)))
         return res
 
-    def model_delete_cli(self, model, model_opt=None):
-        """ wrapper for client for model_delete, with additional
-            model_opt to get a model from the API
+    def model_delete_cli(self, model):
+        """ wrapper for client for model_delete
              Parameters
             ==========
-            model_opt: an alternative to model
+            model: the string identified of the model
+                     should be in format [owner]/[model-name]
         """
-        m = model or model_opt
-        result = self.model_delete(m)
+        result = self.model_delete(model)
 
         if result.hasError:
             print('Model deletion error: ' + result.error)
         else:
             print('The model was deleted.')
 
     def model_update(self, folder):
@@ -2514,14 +2546,16 @@
                 'Default ownerSlug detected, please change values before uploading'
             )
         if slug == 'INSERT_SLUG_HERE':
             raise ValueError(
                 'Default slug detected, please change values before uploading')
         if is_private != None and not isinstance(is_private, bool):
             raise ValueError('model.isPrivate must be a boolean')
+        if publish_time:
+            self.validate_date(publish_time)
 
         # mask
         update_mask = {'paths': []}
         if title != None:
             update_mask['paths'].append('title')
         if subtitle != None:
             update_mask['paths'].append('subtitle')
@@ -2578,29 +2612,23 @@
             model_instance)
 
         mi = self.process_response(
             self.get_model_instance_with_http_info(owner_slug, model_slug,
                                                    framework, instance_slug))
         return mi
 
-    def model_instance_get_cli(self,
-                               model_instance,
-                               folder=None,
-                               model_instance_opt=None):
-        """ wrapper for client for model_instance_get, with additional
-            model_instance_opt to get a model instance from the API
+    def model_instance_get_cli(self, model_instance, folder=None):
+        """ wrapper for client for model_instance_get
              Parameters
             ==========
             model_instance: the string identified of the model instance
                      should be in format [owner]/[model-name]/[framework]/[instance-slug]
             folder: the folder to download the model metadata file
-            model_instance_opt: an alternative to model_instance
         """
-        m = model_instance or model_instance_opt
-        mi = self.model_instance_get(m)
+        mi = self.model_instance_get(model_instance)
         if folder is None:
             self.print_obj(mi)
         else:
             meta_file = os.path.join(folder, self.MODEL_INSTANCE_METADATA_FILE)
 
             owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
                 model_instance)
@@ -2721,15 +2749,16 @@
                                           framework=framework,
                                           overview=overview,
                                           usage=usage,
                                           license_name=license_name,
                                           fine_tunable=fine_tunable,
                                           training_data=training_data,
                                           files=[])
-        self.upload_files(request, None, folder, 'model', quiet, dir_mode)
+        self.upload_files(request, None, folder, ApiBlobType.MODEL, quiet,
+                          dir_mode)
         result = ModelNewResponse(
             self.process_response(
                 self.models_create_instance_with_http_info(
                     owner_slug, model_slug, request)))
 
         return result
 
@@ -2758,31 +2787,32 @@
                      should be in format [owner]/[model-name]/[framework]/[instance-slug]
         """
         if model_instance is None:
             raise ValueError('A model instance must be specified')
         owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
             model_instance)
 
+        if not self.confirmation():
+            print('Deletion cancelled')
+            exit(0)
+
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_instance_with_http_info(
                     owner_slug, model_slug, framework, instance_slug)))
         return res
 
-    def model_instance_delete_cli(self,
-                                  model_instance,
-                                  model_instance_opt=None):
-        """ wrapper for client for model_instance_delete, with additional
-            model_instance_opt to get a model instance from the API
+    def model_instance_delete_cli(self, model_instance):
+        """ wrapper for client for model_instance_delete
              Parameters
             ==========
-            model_instance_opt: an alternative to model instance
+            model_instance: the string identified of the model instance
+                     should be in format [owner]/[model-name]/[framework]/[instance-slug]
         """
-        mi = model_instance or model_instance_opt
-        result = self.model_instance_delete(mi)
+        result = self.model_instance_delete(model_instance)
 
         if result.hasError:
             print('Model instance deletion error: ' + result.error)
         else:
             print('The model instance was deleted.')
 
     def model_instance_update(self, folder):
@@ -2889,22 +2919,21 @@
             model_instance: the string identified of the model instance
                      should be in format [owner]/[model-name]/[framework]/[instance-slug]
             folder: the folder to get the metadata file from
             version_notes: the version notes to record for this new version
             quiet: suppress verbose output (default is False)
             dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
         """
-        if model_instance is None:
-            raise ValueError('A model instance must be specified')
         owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
             model_instance)
 
         request = ModelInstanceNewVersionRequest(version_notes=version_notes,
                                                  files=[])
-        self.upload_files(request, None, folder, 'model', quiet, dir_mode)
+        self.upload_files(request, None, folder, ApiBlobType.MODEL, quiet,
+                          dir_mode)
         result = ModelNewResponse(
             self.process_response(
                 self.models_create_instance_version_with_http_info(
                     owner_slug, model_slug, framework, instance_slug,
                     request)))
 
         return result
@@ -2977,15 +3006,15 @@
                 framework=framework,
                 instance_slug=instance_slug,
                 version_number=version_number,
                 _preload_content=False))
 
         outfile = os.path.join(effective_path, model_slug + '.tar.gz')
         if force or self.download_needed(response, outfile, quiet):
-            self.download_file(response, outfile, quiet)
+            self.download_file(response, outfile, quiet, not force)
             downloaded = True
         else:
             downloaded = False
 
         if downloaded:
             if untar:
                 try:
@@ -2999,80 +3028,105 @@
                 try:
                     os.remove(outfile)
                 except OSError as e:
                     print('Could not delete tar file, got %s' % e)
 
     def model_instance_version_download_cli(self,
                                             model_instance_version,
-                                            model_instance_version_opt=None,
                                             path=None,
                                             untar=False,
                                             force=False,
                                             quiet=False):
         """ client wrapper for model_instance_version_download.
 
             Parameters
             ==========
             model_instance_version: the string identified of the model instance version
                     should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
-            model_instance_version_opt: an alternative option to providing a model instance version
             path: the path to download the model instance version to
             force: force the download if the file already exists (default False)
             quiet: suppress verbose output (default is False)
             untar: if True, untar files upon download (default is False)
         """
-        miv = model_instance_version or model_instance_version_opt
         self.model_instance_version_download(model_instance_version,
                                              path=path,
                                              untar=untar,
                                              force=force,
                                              quiet=quiet)
 
     def model_instance_version_delete(self, model_instance_version):
         """ call to delete a model instance version from the API
              Parameters
             ==========
             model_instance_version: the string identified of the model instance version
-                     should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
+                should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
         """
         if model_instance_version is None:
             raise ValueError('A model instance version must be specified')
 
         self.validate_model_instance_version_string(model_instance_version)
         urls = model_instance_version.split('/')
         owner_slug = urls[0]
         model_slug = urls[1]
         framework = urls[2]
         instance_slug = urls[3]
         version_number = urls[4]
 
+        if not self.confirmation():
+            print('Deletion cancelled')
+            exit(0)
+
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_instance_version_with_http_info(
                     owner_slug, model_slug, framework, instance_slug,
                     version_number)))
         return res
 
-    def model_instance_version_delete_cli(self,
-                                          model_instance_version,
-                                          model_instance_version_opt=None):
-        """ wrapper for client for model_instance_version_delete, with additional
-            model_instance_version_opt to get a model instance version from the API
+    def model_instance_version_delete_cli(self, model_instance_version):
+        """ wrapper for client for model_instance_version_delete
              Parameters
             ==========
-            model_instance_version_opt: an alternative to model instance version
+            model_instance_version: the string identified of the model instance version
+                should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
         """
-        miv = model_instance_version or model_instance_version_opt
-        result = self.model_instance_version_delete(miv)
+        result = self.model_instance_version_delete(model_instance_version)
 
         if result.hasError:
             print('Model instance version deletion error: ' + result.error)
         else:
             print('The model instance version was deleted.')
 
+    def files_upload_cli(self, local_paths, inbox_path=None):
+        if len(local_paths) > self.MAX_NUM_INBOX_FILES_TO_UPLOAD:
+            print('Cannot upload more than',
+                  self.MAX_NUM_INBOX_FILES_TO_UPLOAD, 'files!')
+            return
+
+        for local_path in local_paths:
+            self.file_upload_cli(local_path, inbox_path)
+
+    def file_upload_cli(self, local_path, inbox_path=None):
+        full_path = os.path.abspath(local_path)
+        parent_path = os.path.dirname(full_path)
+        file_or_folder_name = os.path.basename(full_path)
+
+        upload_file = self._upload_file_or_folder(parent_path,
+                                                  file_or_folder_name,
+                                                  ApiBlobType.INBOX, 'zip')
+        if upload_file is None:
+            return
+
+        inbox_path = inbox_path or ''
+        create_inbox_file_request = CreateInboxFileRequest(
+            virtual_directory=inbox_path, blob_file_token=upload_file.token)
+        self.process_response(
+            self.create_inbox_file(create_inbox_file_request))
+        print('Upload complete:', file_or_folder_name)
+
     def print_obj(self, obj, indent=2):
         pretty = json.dumps(obj, indent=indent)
         print(pretty)
 
     def download_needed(self, response, outfile, quiet=True):
         """ determine if a download is needed based on timestamp. Return True
             if needed (remote is newer) or False if local is newest.
@@ -3081,16 +3135,21 @@
             response: the response from the API
             outfile: the output file to write to
             quiet: suppress verbose output (default is True)
         """
         try:
             remote_date = datetime.strptime(response.headers['Last-Modified'],
                                             '%a, %d %b %Y %X %Z')
-            if isfile(outfile):
+            file_exists = os.path.isfile(outfile)
+            if file_exists:
                 local_date = datetime.fromtimestamp(os.path.getmtime(outfile))
+                remote_size = int(response.headers['Content-Length'])
+                local_size = os.path.getsize(outfile)
+                if local_size < remote_size:
+                    return True
                 if remote_date <= local_date:
                     if not quiet:
                         print(
                             os.path.basename(outfile) +
                             ': Skipping, found more recently modified local '
                             'copy (use --force to force download)')
                     return False
@@ -3234,92 +3293,86 @@
 
         return True
 
     def upload_files(self,
                      request,
                      resources,
                      folder,
-                     entity='dataset',
+                     blob_type,
                      quiet=False,
                      dir_mode='skip'):
         """ upload files in a folder
              Parameters
             ==========
             request: the prepared request
             resources: the files to upload
             folder: the folder to upload from
-            entity: dataset or model
+            blob_type (ApiBlobType): To which entity the file/blob refers
             quiet: suppress verbose output (default is False)
         """
         for file_name in os.listdir(folder):
             if (file_name in [
                     self.DATASET_METADATA_FILE, self.OLD_DATASET_METADATA_FILE,
                     self.KERNEL_METADATA_FILE, self.MODEL_METADATA_FILE,
                     self.MODEL_INSTANCE_METADATA_FILE
             ]):
                 continue
-            full_path = os.path.join(folder, file_name)
-
-            if os.path.isfile(full_path):
-                exitcode = self._upload_file(file_name, full_path, quiet,
-                                             request, resources, entity)
-                if exitcode:
-                    return
-            elif os.path.isdir(full_path):
-                if dir_mode in ['zip', 'tar']:
-                    temp_dir = tempfile.mkdtemp()
-                    try:
-                        _, dir_name = os.path.split(full_path)
-                        archive_path = shutil.make_archive(
-                            os.path.join(temp_dir, dir_name), dir_mode,
-                            full_path)
-                        _, archive_name = os.path.split(archive_path)
-                        exitcode = self._upload_file(archive_name,
-                                                     archive_path, quiet,
-                                                     request, resources,
-                                                     entity)
-                    finally:
-                        shutil.rmtree(temp_dir)
-                    if exitcode:
-                        return
-                elif not quiet:
-                    print("Skipping folder: " + file_name +
-                          "; use '--dir-mode' to upload folders")
-            else:
-                if not quiet:
-                    print('Skipping: ' + file_name)
+            upload_file = self._upload_file_or_folder(folder, file_name,
+                                                      blob_type, dir_mode,
+                                                      quiet, resources)
+            if upload_file is not None:
+                request.files.append(upload_file)
+
+    def _upload_file_or_folder(self,
+                               parent_path,
+                               file_or_folder_name,
+                               blob_type,
+                               dir_mode,
+                               quiet=False,
+                               resources=None):
+        full_path = os.path.join(parent_path, file_or_folder_name)
+        if os.path.isfile(full_path):
+            return self._upload_file(file_or_folder_name, full_path, blob_type,
+                                     quiet, resources)
+
+        elif os.path.isdir(full_path):
+            if dir_mode in ['zip', 'tar']:
+                archive = DirectoryArchive(full_path, dir_mode)
+                with archive:
+                    return self._upload_file(archive.name, archive.path,
+                                             blob_type, quiet, resources)
+            elif not quiet:
+                print("Skipping folder: " + file_or_folder_name +
+                      "; use '--dir-mode' to upload folders")
+        else:
+            if not quiet:
+                print('Skipping: ' + file_or_folder_name)
+        return None
 
-    def _upload_file(self,
-                     file_name,
-                     full_path,
-                     quiet,
-                     request,
-                     resources,
-                     entity='dataset'):
+    def _upload_file(self, file_name, full_path, blob_type, quiet, resources):
         """ Helper function to upload a single file
             Parameters
             ==========
             file_name: name of the file to upload
             full_path: path to the file to upload
+            blob_type (ApiBlobType): To which entity the file/blob refers
             quiet: suppress verbose output
-            request: the prepared request
             resources: optional file metadata
-            entity: dataset or model
-            :return: True - upload unsuccessful; False - upload successful
+            :return: None - upload unsuccessful; instance of UploadFile - upload successful
         """
 
         if not quiet:
             print('Starting upload for file ' + file_name)
 
         content_length = os.path.getsize(full_path)
-        token = self.upload_file(full_path, quiet, entity)
+        token = self._upload_blob(full_path, quiet, blob_type)
         if token is None:
             if not quiet:
                 print('Upload unsuccessful: ' + file_name)
-            return True
+            return None
         if not quiet:
             print('Upload successful: ' + file_name + ' (' +
                   File.get_size(content_length) + ')')
         upload_file = UploadFile()
         upload_file.token = token
         if resources:
             for item in resources:
@@ -3331,16 +3384,15 @@
                         processed = []
                         count = 0
                         for field in fields:
                             processed.append(self.process_column(field))
                             processed[count].order = count
                             count += 1
                         upload_file.columns = processed
-        request.files.append(upload_file)
-        return False
+        return upload_file
 
     def process_column(self, column):
         """ process a column, check for the type, and return the processed
             column
              Parameters
             ==========
             column: a list of values in a column to be processed
@@ -3396,28 +3448,45 @@
         except Exception as error:
             print(error)
             return False
         return response.status_code == 200 or response.status_code == 201
 
     def validate_dataset_string(self, dataset):
         """ determine if a dataset string is valid, meaning it is in the format
-            of {username}/{dataset-slug}.
+            of {username}/{dataset-slug} or {username}/{dataset-slug}/{version-number}.
              Parameters
             ==========
             dataset: the dataset name to validate
         """
         if dataset:
             if '/' not in dataset:
                 raise ValueError('Dataset must be specified in the form of '
                                  '\'{username}/{dataset-slug}\'')
 
             split = dataset.split('/')
-            if not split[0] or not split[1]:
+            if not split[0] or not split[1] or len(split) > 3:
                 raise ValueError('Invalid dataset specification ' + dataset)
 
+    def split_dataset_string(self, dataset):
+        """ split a dataset string into owner_slug, dataset_slug,
+            and optional version_number
+             Parameters
+            ==========
+            dataset: the dataset name to split
+        """
+        if '/' in dataset:
+            self.validate_dataset_string(dataset)
+            urls = dataset.split('/')
+            if len(urls) == 3:
+                return urls[0], urls[1], urls[2]
+            else:
+                return urls[0], urls[1], None
+        else:
+            return self.get_config_value(self.CONFIG_NAME_USER), dataset
+
     def validate_model_string(self, model):
         """ determine if a model string is valid, meaning it is in the format
             of {owner}/{model-slug}.
              Parameters
             ==========
             model: the model name to validate
         """
@@ -3611,14 +3680,27 @@
 
     def validate_date(self, date):
         datetime.strptime(date, "%Y-%m-%d")
 
     def sanitize_markdown(self, markdown):
         return bleach.clean(markdown)
 
+    def confirmation(self):
+        question = "Are you sure?"
+        prompt = "[yes/no]"
+        options = {"yes": True, "no": False}
+        while True:
+            sys.stdout.write('{} {} '.format(question, prompt))
+            choice = input().lower()
+            if choice in options:
+                return options[choice]
+            else:
+                sys.stdout.write("Please respond with 'yes' or 'no'.\n")
+                return False
+
 
 class TqdmBufferedReader(io.BufferedReader):
 
     def __init__(self, raw, progress_bar):
         """ helper class to implement an io.BufferedReader
              Parameters
             ==========
```

### Comparing `kaggle-1.6.0a2/kaggle/api_client.py` & `kaggle-1.6.0a3/kaggle/api_client.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/cli.py` & `kaggle-1.6.0a3/kaggle/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # coding=utf-8
 from __future__ import print_function
 import argparse
+import json
 from kaggle import api
 from kaggle import KaggleApi
 from .rest import ApiException
 import six
 
 
 def main():
@@ -53,25 +54,30 @@
                                        dest='command')
     subparsers.required = True
     subparsers.choices = Help.kaggle_choices
     parse_competitions(subparsers)
     parse_datasets(subparsers)
     parse_kernels(subparsers)
     parse_models(subparsers)
+    parse_files(subparsers)
     parse_config(subparsers)
     args = parser.parse_args()
     command_args = {}
     command_args.update(vars(args))
     del command_args['func']
     del command_args['command']
     error = False
     try:
         out = args.func(**command_args)
     except ApiException as e:
-        print(str(e.status) + ' - ' + e.reason)
+        msg = '{} - {}'.format(str(e.status), e.reason)
+        body = __parse_body(e.body)
+        if body and 'message' in body:
+            msg += ' - {}'.format(body['message'])
+        print(msg)
         out = None
         error = True
     except ValueError as e:
         print(e)
         out = None
         error = True
     except KeyboardInterrupt:
@@ -81,14 +87,21 @@
         print(out, end='')
 
     # This is so that scripts that pick up on error codes can tell when there was a failure
     if error:
         exit(1)
 
 
+def __parse_body(body):
+    try:
+        return json.loads(body)
+    except Exception as e:
+        return {}
+
+
 def parse_competitions(subparsers):
     if six.PY2:
         parser_competitions = subparsers.add_parser(
             'competitions',
             formatter_class=argparse.RawTextHelpFormatter,
             help=Help.group_competitions)
     else:
@@ -420,15 +433,15 @@
     parser_datasets_files_optional = parser_datasets_files._action_groups.pop()
     parser_datasets_files_optional.add_argument('dataset',
                                                 nargs='?',
                                                 default=None,
                                                 help=Help.param_dataset)
     parser_datasets_files_optional.add_argument('-d',
                                                 '--dataset',
-                                                dest='dataset',
+                                                dest='dataset_opt',
                                                 required=False,
                                                 help=argparse.SUPPRESS)
     parser_datasets_files_optional.add_argument('-v',
                                                 '--csv',
                                                 dest='csv_display',
                                                 action='store_true',
                                                 help=Help.param_csv)
@@ -440,14 +453,15 @@
         'download',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_datasets_download)
     parser_datasets_download_optional = parser_datasets_download._action_groups.pop(
     )
     parser_datasets_download_optional.add_argument('dataset',
                                                    nargs='?',
+                                                   default=None,
                                                    help=Help.param_dataset)
     parser_datasets_download_optional.add_argument('-d',
                                                    '--dataset',
                                                    dest='dataset_opt',
                                                    required=False,
                                                    help=argparse.SUPPRESS)
     parser_datasets_download_optional.add_argument(
@@ -596,15 +610,15 @@
     )
     parser_datasets_metadata_optional.add_argument('dataset',
                                                    nargs='?',
                                                    default=None,
                                                    help=Help.param_dataset)
     parser_datasets_metadata_optional.add_argument('-d',
                                                    '--dataset',
-                                                   dest='dataset',
+                                                   dest='dataset_opt',
                                                    required=False,
                                                    help=argparse.SUPPRESS)
     parser_datasets_metadata_optional.add_argument(
         '--update',
         dest='update',
         action='store_true',
         help=Help.param_dataset_metadata_update)
@@ -623,15 +637,15 @@
     )
     parser_datasets_status_optional.add_argument('dataset',
                                                  nargs='?',
                                                  default=None,
                                                  help=Help.param_dataset)
     parser_datasets_status_optional.add_argument('-d',
                                                  '--dataset',
-                                                 dest='dataset',
+                                                 dest='dataset_opt',
                                                  required=False,
                                                  help=argparse.SUPPRESS)
     parser_datasets_status._action_groups.append(
         parser_datasets_status_optional)
     parser_datasets_status.set_defaults(func=api.dataset_status_cli)
 
 
@@ -790,15 +804,15 @@
     parser_kernels_output_optional = parser_kernels_output._action_groups.pop()
     parser_kernels_output_optional.add_argument('kernel',
                                                 nargs='?',
                                                 default=None,
                                                 help=Help.param_kernel)
     parser_kernels_output_optional.add_argument('-k',
                                                 '--kernel',
-                                                dest='kernel',
+                                                dest='kernel_opt',
                                                 required=False,
                                                 help=argparse.SUPPRESS)
     parser_kernels_output_optional.add_argument('-p',
                                                 '--path',
                                                 dest='path',
                                                 required=False,
                                                 help=Help.param_downfolder)
@@ -832,15 +846,15 @@
     parser_kernels_status_optional = parser_kernels_status._action_groups.pop()
     parser_kernels_status_optional.add_argument('kernel',
                                                 nargs='?',
                                                 default=None,
                                                 help=Help.param_kernel)
     parser_kernels_status_optional.add_argument('-k',
                                                 '--kernel',
-                                                dest='kernel',
+                                                dest='kernel_opt',
                                                 required=False,
                                                 help=argparse.SUPPRESS)
     parser_kernels_status._action_groups.append(parser_kernels_status_optional)
     parser_kernels_status.set_defaults(func=api.kernels_status_cli)
 
 
 def parse_models(subparsers):
@@ -860,23 +874,15 @@
 
     # Models get
     parser_models_get = subparsers_models.add_parser(
         'get',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_models_get)
     parser_models_get_optional = parser_models_get._action_groups.pop()
-    parser_models_get_optional.add_argument('model',
-                                            nargs='?',
-                                            default=None,
-                                            help=Help.param_model)
-    parser_models_get_optional.add_argument('-m',
-                                            '--model',
-                                            dest='model',
-                                            required=False,
-                                            help=argparse.SUPPRESS)
+    parser_models_get_optional.add_argument('model', help=Help.param_model)
     parser_models_get_optional.add_argument('-p',
                                             '--path',
                                             dest='folder',
                                             required=False,
                                             help=Help.param_model_downfile)
     parser_models_get._action_groups.append(parser_models_get_optional)
     parser_models_get.set_defaults(func=api.model_get_cli)
@@ -946,23 +952,15 @@
 
     # Models delete
     parser_models_delete = subparsers_models.add_parser(
         'delete',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_models_delete)
     parser_models_delete_optional = parser_models_delete._action_groups.pop()
-    parser_models_delete_optional.add_argument('model',
-                                               nargs='?',
-                                               default=None,
-                                               help=Help.param_model)
-    parser_models_delete_optional.add_argument('-m',
-                                               '--model',
-                                               dest='model',
-                                               required=False,
-                                               help=argparse.SUPPRESS)
+    parser_models_delete_optional.add_argument('model', help=Help.param_model)
     parser_models_delete._action_groups.append(parser_models_delete_optional)
     parser_models_delete.set_defaults(func=api.model_delete_cli)
 
     # Models update
     parser_models_update = subparsers_models.add_parser(
         'update',
         formatter_class=argparse.RawTextHelpFormatter,
@@ -980,51 +978,43 @@
 def parse_model_instances(subparsers):
     parser_model_instances = subparsers.add_parser(
         'instances',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.group_model_instances,
         aliases=['mi'])
 
-    subparsers_model_intances = parser_model_instances.add_subparsers(
+    subparsers_model_instances = parser_model_instances.add_subparsers(
         title='commands', dest='command')
-    subparsers_model_intances.required = True
-    subparsers_model_intances.choices = Help.model_instances_choices
+    subparsers_model_instances.required = True
+    subparsers_model_instances.choices = Help.model_instances_choices
 
     # Models Instances Versions.
-    parse_model_instance_versions(subparsers_model_intances)
+    parse_model_instance_versions(subparsers_model_instances)
 
     # Models Instances get
-    parser_model_instance_get = subparsers_model_intances.add_parser(
+    parser_model_instance_get = subparsers_model_instances.add_parser(
         'get',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instances_get)
     parser_model_instance_get_optional = parser_model_instance_get._action_groups.pop(
     )
     parser_model_instance_get_optional.add_argument(
-        'model_instance',
-        nargs='?',
-        default=None,
-        help=Help.param_model_instance)
-    parser_model_instance_get_optional.add_argument('-m',
-                                                    '--modelInstance',
-                                                    dest='model_instance',
-                                                    required=False,
-                                                    help=argparse.SUPPRESS)
+        'model_instance', help=Help.param_model_instance)
     parser_model_instance_get_optional.add_argument(
         '-p',
         '--path',
         dest='folder',
         required=False,
         help=Help.param_model_instance_downfile)
     parser_model_instance_get._action_groups.append(
         parser_model_instance_get_optional)
     parser_model_instance_get.set_defaults(func=api.model_instance_get_cli)
 
     # Model Instances init
-    parser_model_instances_init = subparsers_model_intances.add_parser(
+    parser_model_instances_init = subparsers_model_instances.add_parser(
         'init',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instances_init)
     parser_model_instances_init_optional = parser_model_instances_init._action_groups.pop(
     )
     parser_model_instances_init_optional.add_argument(
         '-p',
@@ -1034,15 +1024,15 @@
         help=Help.param_model_instance_upfile)
     parser_model_instances_init._action_groups.append(
         parser_model_instances_init_optional)
     parser_model_instances_init.set_defaults(
         func=api.model_instance_initialize_cli)
 
     # Model Instances create
-    parser_model_instances_create = subparsers_model_intances.add_parser(
+    parser_model_instances_create = subparsers_model_instances.add_parser(
         'create',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instances_new)
     parser_model_instances_create_optional = parser_model_instances_create._action_groups.pop(
     )
     parser_model_instances_create_optional.add_argument(
         '-p',
@@ -1064,37 +1054,29 @@
         help=Help.param_dir_mode)
     parser_model_instances_create._action_groups.append(
         parser_model_instances_create_optional)
     parser_model_instances_create.set_defaults(
         func=api.model_instance_create_cli)
 
     # Models Instances delete
-    parser_model_instances_delete = subparsers_model_intances.add_parser(
+    parser_model_instances_delete = subparsers_model_instances.add_parser(
         'delete',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instances_delete)
     parser_model_instances_delete_optional = parser_model_instances_delete._action_groups.pop(
     )
     parser_model_instances_delete_optional.add_argument(
-        'model_instance',
-        nargs='?',
-        default=None,
-        help=Help.param_model_instance)
-    parser_model_instances_delete_optional.add_argument('-mi',
-                                                        '--modelInstance',
-                                                        dest='model_instance',
-                                                        required=False,
-                                                        help=argparse.SUPPRESS)
+        'model_instance', help=Help.param_model_instance)
     parser_model_instances_delete._action_groups.append(
         parser_model_instances_delete_optional)
     parser_model_instances_delete.set_defaults(
         func=api.model_instance_delete_cli)
 
     # Models Instances update
-    parser_model_instances_update = subparsers_model_intances.add_parser(
+    parser_model_instances_update = subparsers_model_instances.add_parser(
         'update',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instances_update)
     parser_model_instances_update_optional = parser_model_instances_update._action_groups.pop(
     )
     parser_model_instances_update_optional.add_argument(
         '-p',
@@ -1124,18 +1106,15 @@
     parser_model_instance_versions_create = subparsers_model_intance_versions.add_parser(
         'create',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instance_versions_new)
     parser_model_instance_versions_create_optional = parser_model_instance_versions_create._action_groups.pop(
     )
     parser_model_instance_versions_create_optional.add_argument(
-        'model_instance',
-        nargs='?',
-        default=None,
-        help=Help.param_model_instance)
+        'model_instance', help=Help.param_model_instance)
     parser_model_instance_versions_create_optional.add_argument(
         '-p',
         '--path',
         dest='folder',
         required=False,
         help=Help.param_model_instance_version_upfile)
     parser_model_instance_versions_create_optional.add_argument(
@@ -1166,23 +1145,15 @@
     parser_model_instance_versions_download = subparsers_model_intance_versions.add_parser(
         'download',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instance_versions_download)
     parser_model_instance_versions_download_optional = parser_model_instance_versions_download._action_groups.pop(
     )
     parser_model_instance_versions_download_optional.add_argument(
-        'model_instance_version',
-        nargs='?',
-        help=Help.param_model_instance_version)
-    parser_model_instance_versions_download_optional.add_argument(
-        '-miv',
-        '--modelInstanceVersion',
-        dest='model_instance_version_opt',
-        required=False,
-        help=argparse.SUPPRESS)
+        'model_instance_version', help=Help.param_model_instance_version)
     parser_model_instance_versions_download_optional.add_argument(
         '-p',
         '--path',
         dest='path',
         required=False,
         help=Help.param_downfolder)
     parser_model_instance_versions_download_optional.add_argument(
@@ -1208,30 +1179,55 @@
     parser_model_instance_versions_delete = subparsers_model_intance_versions.add_parser(
         'delete',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instance_versions_delete)
     parser_model_instance_versions_delete_optional = parser_model_instance_versions_delete._action_groups.pop(
     )
     parser_model_instance_versions_delete_optional.add_argument(
-        'model_instance_version',
-        nargs='?',
-        default=None,
-        help=Help.param_model_instance_version)
-    parser_model_instance_versions_delete_optional.add_argument(
-        '-miv',
-        '--modelInstanceVersion',
-        dest='model_instance_version',
-        required=False,
-        help=argparse.SUPPRESS)
+        'model_instance_version', help=Help.param_model_instance_version)
     parser_model_instance_versions_delete._action_groups.append(
         parser_model_instance_versions_delete_optional)
     parser_model_instance_versions_delete.set_defaults(
         func=api.model_instance_version_delete_cli)
 
 
+def parse_files(subparsers):
+    parser_files = subparsers.add_parser(
+        'files',
+        formatter_class=argparse.RawTextHelpFormatter,
+        help=Help.group_files,
+        aliases=['f'])
+
+    subparsers_files = parser_files.add_subparsers(title='commands',
+                                                   dest='command')
+    subparsers_files.required = True
+    subparsers_files.choices = Help.files_choices
+
+    # Files upload
+    parser_files_upload = subparsers_files.add_parser(
+        'upload',
+        formatter_class=argparse.RawTextHelpFormatter,
+        help=Help.command_files_upload,
+        aliases=['u'])
+    parser_files_upload_optional = parser_files_upload._action_groups.pop()
+    parser_files_upload_optional.add_argument(
+        '-i',
+        '--inbox-path',
+        dest='inbox_path',
+        required=False,
+        help=Help.param_files_upload_inbox_path)
+    parser_files_upload_optional.add_argument(
+        'local_paths',
+        metavar='local-path',
+        nargs='+',
+        help=Help.param_files_upload_local_paths)
+    parser_files_upload._action_groups.append(parser_files_upload_optional)
+    parser_files_upload.set_defaults(func=api.files_upload_cli)
+
+
 def parse_config(subparsers):
     parser_config = subparsers.add_parser(
         'config',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.group_config)
     subparsers_config = parser_config.add_subparsers(title='commands',
                                                      dest='command')
@@ -1277,15 +1273,15 @@
                                               help=Help.param_config_name)
     parser_config_unset.set_defaults(func=api.unset_config_value)
 
 
 class Help(object):
     kaggle_choices = [
         'competitions', 'c', 'datasets', 'd', 'kernels', 'k', 'models', 'm',
-        'config'
+        'files', 'f', 'config'
     ]
     competitions_choices = [
         'list', 'files', 'download', 'submit', 'submissions', 'leaderboard'
     ]
     datasets_choices = [
         'list', 'files', 'download', 'create', 'version', 'init', 'metadata',
         'status'
@@ -1294,14 +1290,15 @@
     models_choices = [
         'instances', 'get', 'list', 'init', 'create', 'delete', 'update'
     ]
     model_instances_choices = [
         'versions', 'get', 'init', 'create', 'delete', 'update'
     ]
     model_instance_versions_choices = ['init', 'create', 'download', 'delete']
+    files_choices = ['upload']
     config_choices = ['view', 'set', 'unset']
 
     kaggle = 'Use one of:\ncompetitions {' + ', '.join(
         competitions_choices) + '}\ndatasets {' + ', '.join(
             datasets_choices) + '}\nmodels {' + ', '.join(
                 models_choices) + '}\nmodels instances {' + ', '.join(
                     model_instances_choices
@@ -1311,14 +1308,15 @@
 
     group_competitions = 'Commands related to Kaggle competitions'
     group_datasets = 'Commands related to Kaggle datasets'
     group_kernels = 'Commands related to Kaggle kernels'
     group_models = 'Commands related to Kaggle models'
     group_model_instances = 'Commands related to Kaggle model instances'
     group_model_instance_versions = 'Commands related to Kaggle model instance versions'
+    group_files = 'Commands related files'
     group_config = 'Configuration settings'
 
     # Competitions commands
     command_competitions_list = 'List available competitions'
     command_competitions_files = 'List competition files'
     command_competitions_download = 'Download competition files'
     command_competitions_submit = 'Make a new competition submission'
@@ -1349,14 +1347,17 @@
     command_models_get = 'Get a model'
     command_models_list = 'List models'
     command_models_init = 'Initialize metadata file for model creation'
     command_models_new = 'Create a new model'
     command_models_delete = 'Delete a model'
     command_models_update = 'Update a model'
 
+    # Files commands
+    command_files_upload = 'Upload files'
+
     # Config commands
     command_config_path = (
         'Set folder where competition or dataset files will be '
         'downloaded')
     command_config_proxy = 'Set proxy server'
     command_config_competition = 'Set default competition'
     command_config_view = 'View current config values'
@@ -1545,14 +1546,21 @@
         'special model-instance_version-metadata.json file '
         '(https://github.com/Kaggle/kaggle-api/wiki/ModelInstanceVersion-Metadata). '
         'Defaults to current working directory')
     command_model_instance_versions_delete = 'Delete a model instance version'
     command_model_instance_versions_download = 'Download model instance version files'
     param_model_instance_version_notes = 'Version notes to record for the new model instance version'
 
+    # Files params
+    param_files_upload_inbox_path = 'Virtual path on the server where the uploaded files will be stored'
+    param_files_upload_local_paths = (
+        'List of local filesystem paths. Each path creates a separate file on the server. '
+        'Directories are uploaded as zip archives (e.g., a directory called "data" will be uploaded as "data.zip")'
+    )
+
     # Config params
     param_config_name = ('Name of the configuration parameter\n(one of '
                          'competition, path, proxy)')
     param_config_value = (
         ('Value of the configuration parameter, valid values '
          'depending on name\n- competition: ') + param_competition_nonempty +
         '\n- path: ' + param_downfolder + '\n- proxy: ' + param_proxy)
```

### Comparing `kaggle-1.6.0a2/kaggle/configuration.py` & `kaggle-1.6.0a3/kaggle/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
         # Default Base url
-        self.host = "https://www.kaggle.com/api/v1"
+        self.host = _get_endpoint_from_env() or "https://www.kaggle.com/api/v1"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
@@ -257,7 +257,18 @@
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1\n"\
                "SDK Package Version: 1".\
                format(env=sys.platform, pyversion=sys.version)
+
+
+def _get_endpoint_from_env():
+    import os
+    endpoint = os.environ.get("KAGGLE_API_ENDPOINT")
+    if endpoint is None:
+        return None
+    endpoint = endpoint.rstrip("/")
+    if endpoint.endswith("/api/v1"):
+        return endpoint
+    return endpoint + "/api/v1"
```

### Comparing `kaggle-1.6.0a2/kaggle/models/__init__.py` & `kaggle-1.6.0a3/kaggle/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,22 +27,26 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
+from kaggle.models.api_blob_type import ApiBlobType
 from kaggle.models.collaborator import Collaborator
+from kaggle.models.create_inbox_file_request import CreateInboxFileRequest
 from kaggle.models.dataset_column import DatasetColumn
 from kaggle.models.dataset_new_request import DatasetNewRequest
 from kaggle.models.dataset_new_version_request import DatasetNewVersionRequest
 from kaggle.models.dataset_update_settings_request import DatasetUpdateSettingsRequest
 from kaggle.models.error import Error
 from kaggle.models.kernel_push_request import KernelPushRequest
 from kaggle.models.license import License
 from kaggle.models.model_instance_new_version_request import ModelInstanceNewVersionRequest
 from kaggle.models.model_instance_update_request import ModelInstanceUpdateRequest
 from kaggle.models.model_new_instance_request import ModelNewInstanceRequest
 from kaggle.models.model_new_request import ModelNewRequest
 from kaggle.models.model_update_request import ModelUpdateRequest
 from kaggle.models.result import Result
+from kaggle.models.start_blob_upload_request import StartBlobUploadRequest
+from kaggle.models.start_blob_upload_response import StartBlobUploadResponse
 from kaggle.models.upload_file import UploadFile
```

### Comparing `kaggle-1.6.0a2/kaggle/models/collaborator.py` & `kaggle-1.6.0a3/kaggle/models/collaborator.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/dataset_column.py` & `kaggle-1.6.0a3/kaggle/models/dataset_column.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/dataset_new_request.py` & `kaggle-1.6.0a3/kaggle/models/dataset_new_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         """Sets the license_name of this DatasetNewRequest.
 
         The license that should be associated with the dataset  # noqa: E501
 
         :param license_name: The license_name of this DatasetNewRequest.  # noqa: E501
         :type: str
         """
-        allowed_values = ["CC0-1.0", "CC-BY-SA-4.0", "GPL-2.0", "ODbL-1.0", "CC-BY-NC-SA-4.0", "unknown", "DbCL-1.0", "CC-BY-SA-3.0", "copyright-authors", "other", "reddit-api", "world-bank"]  # noqa: E501
+        allowed_values = ["CC0-1.0", "CC-BY-SA-4.0", "GPL-2.0", "ODbL-1.0", "CC-BY-NC-SA-4.0", "unknown", "DbCL-1.0", "CC-BY-SA-3.0", "copyright-authors", "other", "reddit-api", "world-bank", "CC-BY-4.0", "CC-BY-NC-4.0", "PDDL", "CC-BY-3.0", "CC-BY-3.0-IGO", "US-Government-Works", "CC-BY-NC-SA-3.0-IGO", "CDLA-Permissive-1.0", "CDLA-Sharing-1.0", "CC-BY-ND-4.0", "CC-BY-NC-ND-4.0", "ODC-BY-1.0", "LGPL-3.0", "AGPL-3.0", "FDL-1.3", "EU-ODP-Legal-Notice", "apache-2.0"]  # noqa: E501
         if license_name not in allowed_values:
             raise ValueError(
                 "Invalid value for `license_name` ({0}), must be one of {1}"  # noqa: E501
                 .format(license_name, allowed_values)
             )
 
         self._license_name = license_name
```

### Comparing `kaggle-1.6.0a2/kaggle/models/dataset_new_version_request.py` & `kaggle-1.6.0a3/kaggle/models/dataset_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/dataset_update_settings_request.py` & `kaggle-1.6.0a3/kaggle/models/dataset_update_settings_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/error.py` & `kaggle-1.6.0a3/kaggle/models/error.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/kaggle_models_extended.py` & `kaggle-1.6.0a3/kaggle/models/kaggle_models_extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,24 +153,14 @@
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.ref
 
 
-class FileUploadInfo(object):
-
-    def __init__(self, init_dict):
-        parsed_dict = {k: parse(v) for k, v in init_dict.items()}
-        self.__dict__.update(parsed_dict)
-
-    def __repr__(self):
-        return self.token
-
-
 class DatasetNewVersionResponse(object):
 
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
```

### Comparing `kaggle-1.6.0a2/kaggle/models/kernel_push_request.py` & `kaggle-1.6.0a3/kaggle/models/kernel_push_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         'slug': 'str',
         'new_title': 'str',
         'text': 'str',
         'language': 'str',
         'kernel_type': 'str',
         'is_private': 'bool',
         'enable_gpu': 'bool',
+        'enable_tpu': 'bool',
         'enable_internet': 'bool',
         'dataset_data_sources': 'list[str]',
         'competition_data_sources': 'list[str]',
         'kernel_data_sources': 'list[str]',
         'model_data_sources': 'list[str]',
         'category_ids': 'list[str]',
         'docker_image_pinning_type': 'str'
@@ -69,34 +70,36 @@
         'slug': 'slug',
         'new_title': 'newTitle',
         'text': 'text',
         'language': 'language',
         'kernel_type': 'kernelType',
         'is_private': 'isPrivate',
         'enable_gpu': 'enableGpu',
+        'enable_tpu': 'enableTpu',
         'enable_internet': 'enableInternet',
         'dataset_data_sources': 'datasetDataSources',
         'competition_data_sources': 'competitionDataSources',
         'kernel_data_sources': 'kernelDataSources',
         'model_data_sources': 'modelDataSources',
         'category_ids': 'categoryIds',
         'docker_image_pinning_type': 'dockerImagePinningType'
     }
 
-    def __init__(self, id=None, slug=None, new_title=None, text=None, language=None, kernel_type=None, is_private=None, enable_gpu=None, enable_internet=None, dataset_data_sources=None, competition_data_sources=None, kernel_data_sources=None, model_data_sources=None, category_ids=None, docker_image_pinning_type=None):  # noqa: E501
+    def __init__(self, id=None, slug=None, new_title=None, text=None, language=None, kernel_type=None, is_private=None, enable_gpu=None, enable_tpu=None, enable_internet=None, dataset_data_sources=None, competition_data_sources=None, kernel_data_sources=None, model_data_sources=None, category_ids=None, docker_image_pinning_type=None):  # noqa: E501
         """KernelPushRequest - a model defined in Swagger"""  # noqa: E501
 
         self._id = None
         self._slug = None
         self._new_title = None
         self._text = None
         self._language = None
         self._kernel_type = None
         self._is_private = None
         self._enable_gpu = None
+        self._enable_tpu = None
         self._enable_internet = None
         self._dataset_data_sources = None
         self._competition_data_sources = None
         self._kernel_data_sources = None
         self._model_data_sources = None
         self._category_ids = None
         self._docker_image_pinning_type = None
@@ -111,14 +114,16 @@
         self.text = text
         self.language = language
         self.kernel_type = kernel_type
         if is_private is not None:
             self.is_private = is_private
         if enable_gpu is not None:
             self.enable_gpu = enable_gpu
+        if enable_tpu is not None:
+            self.enable_tpu = enable_tpu
         if enable_internet is not None:
             self.enable_internet = enable_internet
         if dataset_data_sources is not None:
             self.dataset_data_sources = dataset_data_sources
         if competition_data_sources is not None:
             self.competition_data_sources = competition_data_sources
         if kernel_data_sources is not None:
@@ -329,14 +334,37 @@
         :param enable_gpu: The enable_gpu of this KernelPushRequest.  # noqa: E501
         :type: bool
         """
 
         self._enable_gpu = enable_gpu
 
     @property
+    def enable_tpu(self):
+        """Gets the enable_tpu of this KernelPushRequest.  # noqa: E501
+
+        Whether or not the kernel should run on a TPU  # noqa: E501
+
+        :return: The enable_tpu of this KernelPushRequest.  # noqa: E501
+        :rtype: bool
+        """
+        return self._enable_tpu
+
+    @enable_tpu.setter
+    def enable_tpu(self, enable_tpu):
+        """Sets the enable_tpu of this KernelPushRequest.
+
+        Whether or not the kernel should run on a TPU  # noqa: E501
+
+        :param enable_tpu: The enable_tpu of this KernelPushRequest.  # noqa: E501
+        :type: bool
+        """
+
+        self._enable_tpu = enable_tpu
+
+    @property
     def enable_internet(self):
         """Gets the enable_internet of this KernelPushRequest.  # noqa: E501
 
         Whether or not the kernel should be able to access the internet  # noqa: E501
 
         :return: The enable_internet of this KernelPushRequest.  # noqa: E501
         :rtype: bool
```

### Comparing `kaggle-1.6.0a2/kaggle/models/license.py` & `kaggle-1.6.0a3/kaggle/models/license.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         Name of the license  # noqa: E501
 
         :param name: The name of this License.  # noqa: E501
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        allowed_values = ["CC0-1.0", "CC-BY-SA-4.0", "GPL-2.0", "ODbL-1.0", "CC-BY-NC-SA-4.0", "unknown", "DbCL-1.0", "CC-BY-SA-3.0", "copyright-authors", "other", "reddit-api", "world-bank"]  # noqa: E501
+        allowed_values = ["CC0-1.0", "CC-BY-SA-4.0", "GPL-2.0", "ODbL-1.0", "CC-BY-NC-SA-4.0", "unknown", "DbCL-1.0", "CC-BY-SA-3.0", "copyright-authors", "other", "reddit-api", "world-bank", "CC-BY-4.0", "CC-BY-NC-4.0", "PDDL", "CC-BY-3.0", "CC-BY-3.0-IGO", "US-Government-Works", "CC-BY-NC-SA-3.0-IGO", "CDLA-Permissive-1.0", "CDLA-Sharing-1.0", "CC-BY-ND-4.0", "CC-BY-NC-ND-4.0", "ODC-BY-1.0", "LGPL-3.0", "AGPL-3.0", "FDL-1.3", "EU-ODP-Legal-Notice", "apache-2.0"]  # noqa: E501
         if name not in allowed_values:
             raise ValueError(
                 "Invalid value for `name` ({0}), must be one of {1}"  # noqa: E501
                 .format(name, allowed_values)
             )
 
         self._name = name
```

### Comparing `kaggle-1.6.0a2/kaggle/models/model_instance_new_version_request.py` & `kaggle-1.6.0a3/kaggle/models/model_instance_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/model_instance_update_request.py` & `kaggle-1.6.0a3/kaggle/models/model_instance_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/model_new_instance_request.py` & `kaggle-1.6.0a3/kaggle/models/model_new_instance_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/model_new_request.py` & `kaggle-1.6.0a3/kaggle/models/model_new_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/model_update_request.py` & `kaggle-1.6.0a3/kaggle/models/model_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/result.py` & `kaggle-1.6.0a3/kaggle/models/result.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/models/upload_file.py` & `kaggle-1.6.0a3/kaggle/models/upload_file.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/rest.py` & `kaggle-1.6.0a3/kaggle/rest.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/tests/__init__.py` & `kaggle-1.6.0a3/kaggle/test/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle/tests/test_authenticate.py` & `kaggle-1.6.0a3/kaggle/test/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a2/kaggle.egg-info/PKG-INFO` & `kaggle-1.6.0a3/kaggle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a2
+Version: 1.6.0a3
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a2/kaggle.egg-info/SOURCES.txt` & `kaggle-1.6.0a3/kaggle.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 kaggle.egg-info/entry_points.txt
 kaggle.egg-info/requires.txt
 kaggle.egg-info/top_level.txt
 kaggle/api/__init__.py
 kaggle/api/kaggle_api.py
 kaggle/api/kaggle_api_extended.py
 kaggle/models/__init__.py
+kaggle/models/api_blob_type.py
 kaggle/models/collaborator.py
+kaggle/models/create_inbox_file_request.py
 kaggle/models/dataset_column.py
 kaggle/models/dataset_new_request.py
 kaggle/models/dataset_new_version_request.py
 kaggle/models/dataset_update_settings_request.py
 kaggle/models/error.py
 kaggle/models/kaggle_models_extended.py
 kaggle/models/kernel_push_request.py
 kaggle/models/license.py
 kaggle/models/model_instance_new_version_request.py
 kaggle/models/model_instance_update_request.py
 kaggle/models/model_new_instance_request.py
 kaggle/models/model_new_request.py
 kaggle/models/model_update_request.py
 kaggle/models/result.py
+kaggle/models/start_blob_upload_request.py
+kaggle/models/start_blob_upload_response.py
 kaggle/models/upload_file.py
-kaggle/tests/__init__.py
-kaggle/tests/test_authenticate.py
+kaggle/test/__init__.py
+kaggle/test/test_authenticate.py
```

### Comparing `kaggle-1.6.0a2/setup.py` & `kaggle-1.6.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='kaggle',
-    version='1.6.0a2',
+    version='1.6.0a3',
     description='Kaggle API',
     long_description=
     ('Official API for https://www.kaggle.com, accessible using a command line '
      'tool implemented in Python. Beta release - Kaggle reserves the right to '
      'modify the API functionality currently offered.'),
     author='Kaggle',
     author_email='support@kaggle.com',
```

