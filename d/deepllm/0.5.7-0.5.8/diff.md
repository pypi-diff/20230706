# Comparing `tmp/deepllm-0.5.7.tar.gz` & `tmp/deepllm-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-0.5.7.tar", last modified: Thu Jul  6 02:21:42 2023, max compression
+gzip compressed data, was "deepllm-0.5.8.tar", last modified: Thu Jul  6 02:52:10 2023, max compression
```

## Comparing `deepllm-0.5.7.tar` & `deepllm-0.5.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:21:42.575861 deepllm-0.5.7/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.5.7/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4261 2023-07-06 02:21:42.575533 deepllm-0.5.7/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     3976 2023-07-06 02:19:27.000000 deepllm-0.5.7/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:21:42.566292 deepllm-0.5.7/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2023-07-06 02:15:55.000000 deepllm-0.5.7/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     1329 2023-07-05 04:00:30.000000 deepllm-0.5.7/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:21:42.569026 deepllm-0.5.7/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.5.7/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     1296 2023-07-05 03:38:00.000000 deepllm-0.5.7/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.5.7/deepllm/apps/app.sh
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.7/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       10 2023-07-03 02:55:55.000000 deepllm-0.5.7/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.5.7/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:21:42.570326 deepllm-0.5.7/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.5.7/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.7/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.5.7/deepllm/demos/demo.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.7/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       36 2023-07-05 04:04:08.000000 deepllm-0.5.7/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.5.7/deepllm/demos/wikifetch.py
--rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.5.7/deepllm/embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.5.7/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.5.7/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:21:42.571905 deepllm-0.5.7/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.5.7/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.7/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.7/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.5.7/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.5.7/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.5.7/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.5.7/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3006 2023-07-06 02:11:51.000000 deepllm-0.5.7/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     6111 2023-07-05 03:41:23.000000 deepllm-0.5.7/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     6933 2023-07-04 23:57:27.000000 deepllm-0.5.7/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.5.7/deepllm/refiners.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:21:42.575007 deepllm-0.5.7/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.5.7/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.5.7/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.5.7/deepllm/tests/test_all.sh
--rw-r--r--   0 tarau      (503) staff       (20)      571 2023-07-05 03:35:45.000000 deepllm-0.5.7/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.5.7/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.5.7/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.5.7/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.5.7/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.5.7/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.5.7/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2246 2023-07-05 00:10:55.000000 deepllm-0.5.7/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.5.7/deepllm/tools.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:21:42.567758 deepllm-0.5.7/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4261 2023-07-06 02:21:42.000000 deepllm-0.5.7/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1256 2023-07-06 02:21:42.000000 deepllm-0.5.7/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:21:42.000000 deepllm-0.5.7/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:21:42.000000 deepllm-0.5.7/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-06 02:21:42.000000 deepllm-0.5.7/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-06 02:21:42.000000 deepllm-0.5.7/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-06 02:21:42.575970 deepllm-0.5.7/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.5.7/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.964865 deepllm-0.5.8/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.5.8/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4261 2023-07-06 02:52:10.964568 deepllm-0.5.8/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     3976 2023-07-06 02:19:27.000000 deepllm-0.5.8/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.952422 deepllm-0.5.8/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2023-07-06 02:52:00.000000 deepllm-0.5.8/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1329 2023-07-05 04:00:30.000000 deepllm-0.5.8/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.956106 deepllm-0.5.8/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.5.8/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     1296 2023-07-05 03:38:00.000000 deepllm-0.5.8/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.5.8/deepllm/apps/app.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.8/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       10 2023-07-03 02:55:55.000000 deepllm-0.5.8/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.5.8/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.957883 deepllm-0.5.8/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.5.8/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.8/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.5.8/deepllm/demos/demo.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.8/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       36 2023-07-05 04:04:08.000000 deepllm-0.5.8/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.5.8/deepllm/demos/wikifetch.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.5.8/deepllm/embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.5.8/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.5.8/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.960192 deepllm-0.5.8/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.5.8/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.8/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.8/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.5.8/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.5.8/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.5.8/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.5.8/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3006 2023-07-06 02:11:51.000000 deepllm-0.5.8/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6111 2023-07-05 03:41:23.000000 deepllm-0.5.8/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6880 2023-07-06 02:50:36.000000 deepllm-0.5.8/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.5.8/deepllm/refiners.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.964072 deepllm-0.5.8/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.5.8/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.5.8/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.5.8/deepllm/tests/test_all.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      571 2023-07-05 03:35:45.000000 deepllm-0.5.8/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.5.8/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.5.8/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.5.8/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.5.8/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.5.8/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.5.8/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2246 2023-07-05 00:10:55.000000 deepllm-0.5.8/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.5.8/deepllm/tools.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.954271 deepllm-0.5.8/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4261 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1256 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-06 02:52:10.964981 deepllm-0.5.8/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.5.8/setup.py
```

### Comparing `deepllm-0.5.7/LICENSE` & `deepllm-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/PKG-INFO` & `deepllm-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.5.7
+Version: 0.5.8
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-0.5.7/README.md` & `deepllm-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/api.py` & `deepllm-0.5.8/deepllm/api.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/apps/app.py` & `deepllm-0.5.8/deepllm/apps/app.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/configurator.py` & `deepllm-0.5.8/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/demos/demo.py` & `deepllm-0.5.8/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/demos/wikifetch.py` & `deepllm-0.5.8/deepllm/demos/wikifetch.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/embedders.py` & `deepllm-0.5.8/deepllm/embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/horn_prover.py` & `deepllm-0.5.8/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/interactors.py` & `deepllm-0.5.8/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/local_llms/local_runs.py` & `deepllm-0.5.8/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/local_llms/test_vicuna.py` & `deepllm-0.5.8/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/params.py` & `deepllm-0.5.8/deepllm/params.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/prompters.py` & `deepllm-0.5.8/deepllm/prompters.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/recursors.py` & `deepllm-0.5.8/deepllm/recursors.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,22 +148,20 @@
 
         css = [(h, bs) for (h, bss) in self.clauses.items() for bs in bss]
 
         # css=list(self.clauses.items())
 
         self.logic_model = qprove(css, goal=self.initiator)
 
-        if PARAMS().TRACE > 0:
-            if self.logic_model is None:
-                print('\nNO MODEL ENTAILING:', self.initiator)
-            else:
-                print('\nMODEL:', len(self.logic_model), 'facts', '\n')
-                for fact in self.logic_model: print(fact)
-                save_model(self.initiator, self.logic_model, pro_name + "_model")
-
+        if self.logic_model is None:
+            tprint('\nNO MODEL ENTAILING:', self.initiator)
+        else:
+            tprint('\nMODEL:', len(self.logic_model), 'facts', '\n')
+            for fact in self.logic_model: tprint(fact)
+            save_model(self.initiator, self.logic_model, pro_name + "_model")
 
     def run(self):
         for r in self.solve():
             yield 'TRACE', r
         yield 'CLAUSES',dict(self.clauses)
         yield 'MODEL', self.logic_model
         yield 'COSTS', self.costs()
```

### Comparing `deepllm-0.5.7/deepllm/refiners.py` & `deepllm-0.5.8/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/tests/test_api.py` & `deepllm-0.5.8/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/tests/test_recursors.py` & `deepllm-0.5.8/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/tests/test_refiners.py` & `deepllm-0.5.8/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm/tools.py` & `deepllm-0.5.8/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/deepllm.egg-info/PKG-INFO` & `deepllm-0.5.8/deepllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.5.7
+Version: 0.5.8
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-0.5.7/deepllm.egg-info/SOURCES.txt` & `deepllm-0.5.8/deepllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.7/setup.py` & `deepllm-0.5.8/setup.py`

 * *Files identical despite different names*

