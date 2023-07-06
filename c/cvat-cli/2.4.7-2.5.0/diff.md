# Comparing `tmp/cvat-cli-2.4.7.tar.gz` & `tmp/cvat-cli-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat-cli-2.4.7.tar", last modified: Wed Jun 21 13:51:10 2023, max compression
+gzip compressed data, was "cvat-cli-2.5.0.tar", last modified: Thu Jul  6 08:18:03 2023, max compression
```

## Comparing `cvat-cli-2.4.7.tar` & `cvat-cli-2.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/README.md
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-04-14 14:12:32.000000 cvat-cli-2.4.7/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/setup.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.643545 cvat-cli-2.4.7/src/
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/src/cvat_cli/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.4.7/src/cvat_cli/__init__.py
--rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2229 2023-06-17 07:46:59.000000 cvat-cli-2.4.7/src/cvat_cli/__main__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4805 2023-04-05 10:02:25.000000 cvat-cli-2.4.7/src/cvat_cli/cli.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13469 2023-06-17 07:46:59.000000 cvat-cli-2.4.7/src/cvat_cli/parser.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-21 13:40:56.000000 cvat-cli-2.4.7/src/cvat_cli/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:51:10.653545 cvat-cli-2.4.7/src/cvat_cli.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/entry_points.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-21 13:51:10.000000 cvat-cli-2.4.7/src/cvat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       47 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1981 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/README.md
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      114 2023-07-06 04:10:23.000000 cvat-cli-2.5.0/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1969 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/src/
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/src/cvat_cli/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2022-11-18 08:29:30.000000 cvat-cli-2.5.0/src/cvat_cli/__init__.py
+-rwxr-xr-x   0 andrey    (1000) andrey    (1000)     2229 2023-06-17 07:46:59.000000 cvat-cli-2.5.0/src/cvat_cli/__main__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4879 2023-07-05 11:32:32.000000 cvat-cli-2.5.0/src/cvat_cli/cli.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13469 2023-06-17 07:46:59.000000 cvat-cli-2.5.0/src/cvat_cli/parser.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-07-06 04:10:23.000000 cvat-cli-2.5.0/src/cvat_cli/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:18:03.904710 cvat-cli-2.5.0/src/cvat_cli.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2325 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      402 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       52 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       49 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-07-06 08:18:03.000000 cvat-cli-2.5.0/src/cvat_cli.egg-info/top_level.txt
```

### Comparing `cvat-cli-2.4.7/PKG-INFO` & `cvat-cli-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.4.7
+Version: 2.5.0
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cvat-cli-2.4.7/README.md` & `cvat-cli-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.7/setup.py` & `cvat-cli-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.7/src/cvat_cli/__main__.py` & `cvat-cli-2.5.0/src/cvat_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.7/src/cvat_cli/cli.py` & `cvat-cli-2.5.0/src/cvat_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 from cvat_sdk.core.proxies.tasks import ResourceType
 
 
 class CLI:
     def __init__(self, client: Client, credentials: Tuple[str, str]):
         self.client = client
 
-        # allow arbitrary kwargs in models
-        # TODO: will silently ignore invalid args, so remove this ASAP
-        self.client.api_client.configuration.discard_unknown_keys = True
-
         self.client.login(credentials)
 
         self.client.check_server_version(fail_if_unsupported=False)
 
     def tasks_list(self, *, use_json_output: bool = False, **kwargs):
         """List all tasks in either basic or JSON format."""
         results = self.client.tasks.list(return_json=use_json_output, **kwargs)
@@ -47,19 +43,29 @@
         dataset_repository_url: str = "",
         lfs: bool = False,
         **kwargs,
     ) -> None:
         """
         Create a new task with the given name and labels JSON and add the files to it.
         """
+
+        task_params = {}
+        data_params = {}
+
+        for k, v in kwargs.items():
+            if k in models.DataRequest.attribute_map or k == "frame_step":
+                data_params[k] = v
+            else:
+                task_params[k] = v
+
         task = self.client.tasks.create_from_data(
-            spec=models.TaskWriteRequest(name=name, labels=labels, **kwargs),
+            spec=models.TaskWriteRequest(name=name, labels=labels, **task_params),
             resource_type=resource_type,
             resources=resources,
-            data_params=kwargs,
+            data_params=data_params,
             annotation_path=annotation_path,
             annotation_format=annotation_format,
             status_check_period=status_check_period,
             dataset_repository_url=dataset_repository_url,
             use_lfs=lfs,
             pbar=self._make_pbar(),
         )
```

### Comparing `cvat-cli-2.4.7/src/cvat_cli/parser.py` & `cvat-cli-2.5.0/src/cvat_cli/parser.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.4.7/src/cvat_cli.egg-info/PKG-INFO` & `cvat-cli-2.5.0/src/cvat_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.4.7
+Version: 2.5.0
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

