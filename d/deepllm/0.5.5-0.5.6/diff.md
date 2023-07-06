# Comparing `tmp/deepllm-0.5.5.tar.gz` & `tmp/deepllm-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-0.5.5.tar", last modified: Wed Jul  5 03:58:08 2023, max compression
+gzip compressed data, was "deepllm-0.5.6.tar", last modified: Thu Jul  6 02:14:32 2023, max compression
```

## Comparing `deepllm-0.5.5.tar` & `deepllm-0.5.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-05 03:58:08.304219 deepllm-0.5.5/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.5.5/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     3551 2023-07-05 03:58:08.303756 deepllm-0.5.5/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     3266 2023-07-05 03:51:22.000000 deepllm-0.5.5/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-05 03:58:08.285363 deepllm-0.5.5/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2023-07-05 03:57:34.000000 deepllm-0.5.5/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     1329 2023-07-05 03:10:27.000000 deepllm-0.5.5/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-05 03:58:08.289190 deepllm-0.5.5/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.5.5/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     1296 2023-07-05 03:38:00.000000 deepllm-0.5.5/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.5.5/deepllm/apps/app.sh
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.5/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       10 2023-07-03 02:55:55.000000 deepllm-0.5.5/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.5.5/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-05 03:58:08.293191 deepllm-0.5.5/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.5.5/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.5/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.5.5/deepllm/demos/demo.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.5/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       45 2023-07-03 02:33:17.000000 deepllm-0.5.5/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.5.5/deepllm/demos/wikifetch.py
--rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.5.5/deepllm/embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.5.5/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.5.5/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-05 03:58:08.296834 deepllm-0.5.5/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.5.5/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.5/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.5/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.5.5/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.5.5/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.5.5/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.5.5/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3008 2023-07-05 00:47:50.000000 deepllm-0.5.5/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     6111 2023-07-05 03:41:23.000000 deepllm-0.5.5/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     6933 2023-07-04 23:57:27.000000 deepllm-0.5.5/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.5.5/deepllm/refiners.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-05 03:58:08.302997 deepllm-0.5.5/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.5.5/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.5.5/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.5.5/deepllm/tests/test_all.sh
--rw-r--r--   0 tarau      (503) staff       (20)      571 2023-07-05 03:35:45.000000 deepllm-0.5.5/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.5.5/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.5.5/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.5.5/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.5.5/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.5.5/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.5.5/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2246 2023-07-05 00:10:55.000000 deepllm-0.5.5/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.5.5/deepllm/tools.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-05 03:58:08.287404 deepllm-0.5.5/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     3551 2023-07-05 03:58:08.000000 deepllm-0.5.5/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1256 2023-07-05 03:58:08.000000 deepllm-0.5.5/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-05 03:58:08.000000 deepllm-0.5.5/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-05 03:58:08.000000 deepllm-0.5.5/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-05 03:58:08.000000 deepllm-0.5.5/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-05 03:58:08.000000 deepllm-0.5.5/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-05 03:58:08.304376 deepllm-0.5.5/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.5.5/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:14:32.614230 deepllm-0.5.6/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.5.6/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4283 2023-07-06 02:14:32.613931 deepllm-0.5.6/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     3998 2023-07-06 02:07:22.000000 deepllm-0.5.6/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:14:32.597386 deepllm-0.5.6/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2023-07-06 02:12:07.000000 deepllm-0.5.6/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1329 2023-07-05 04:00:30.000000 deepllm-0.5.6/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:14:32.601568 deepllm-0.5.6/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.5.6/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     1296 2023-07-05 03:38:00.000000 deepllm-0.5.6/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.5.6/deepllm/apps/app.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.6/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       10 2023-07-03 02:55:55.000000 deepllm-0.5.6/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.5.6/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:14:32.604413 deepllm-0.5.6/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.5.6/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.6/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.5.6/deepllm/demos/demo.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.6/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       36 2023-07-05 04:04:08.000000 deepllm-0.5.6/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.5.6/deepllm/demos/wikifetch.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.5.6/deepllm/embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.5.6/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.5.6/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:14:32.607851 deepllm-0.5.6/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.5.6/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.6/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.6/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.5.6/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.5.6/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.5.6/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.5.6/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3006 2023-07-06 02:11:51.000000 deepllm-0.5.6/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6111 2023-07-05 03:41:23.000000 deepllm-0.5.6/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6933 2023-07-04 23:57:27.000000 deepllm-0.5.6/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.5.6/deepllm/refiners.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:14:32.613426 deepllm-0.5.6/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.5.6/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.5.6/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.5.6/deepllm/tests/test_all.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      571 2023-07-05 03:35:45.000000 deepllm-0.5.6/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.5.6/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.5.6/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.5.6/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.5.6/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.5.6/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.5.6/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2246 2023-07-05 00:10:55.000000 deepllm-0.5.6/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.5.6/deepllm/tools.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:14:32.599481 deepllm-0.5.6/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4283 2023-07-06 02:14:32.000000 deepllm-0.5.6/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1256 2023-07-06 02:14:32.000000 deepllm-0.5.6/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:14:32.000000 deepllm-0.5.6/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:14:32.000000 deepllm-0.5.6/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-06 02:14:32.000000 deepllm-0.5.6/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-06 02:14:32.000000 deepllm-0.5.6/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-06 02:14:32.614347 deepllm-0.5.6/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.5.6/setup.py
```

### Comparing `deepllm-0.5.5/LICENSE` & `deepllm-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/PKG-INFO` & `deepllm-0.5.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: deepllm
-Version: 0.5.5
-Summary: Deep, recursive, goal-driven LLM explorer
-Home-page: https://github.com/ptarau/recursors.git
-Author: Paul Tarau
-Author-email: paul.tarau@gmail.com
-License: GPL-3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # deepllm: Full Automation of Goal-driven LLM Dialog Threads with And-Or Recursors and Refiner Oracles
 
 
 ### Overview
 We automate deep step-by step reasoning in an LLM dialog thread by recursively exploring alternatives (OR-nodes) and expanding details (AND-nodes) up to a given depth. Starting from a single succinct task-specific initiator we steer the automated dialog thread to stay focussed on the task by synthesizing a prompt that summarizes the depth-first steps taken so far. 
 
 Our algorithm is derived from a simple recursive descent implementation
@@ -39,31 +28,55 @@
 
 ```
 git clone git@github.com:ptarau/recursors.git
 ```
 
 #### Installing
 
-You can install the package ```deepllm``` by typing in folder ```recursors```
+If you have cloned this repo, you can install the package ```deepllm``` by typing in folder ```recursors```
 
 ```
 pip3 install -e .
 ```
 
+You can also install it from [pypi](https://pypi.org/search/?q=deepllm) with
+
+```
+pip3 install deepllm
+```
+
+#### API
+
+The DeepLLM [API](https://github.com/ptarau/recursors/blob/main/deepllm/api.py) exposes its high-level functions ready to embed in your application with something as simple as (assuming the your OPENAI_KEY is exported by your environment):
+
+```
+from deepllm.api import *
+for result in run_recursor(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
+  print(result)
+
+```
+Also, you can ask more interesting questions like in:
+
+```
+from deepllm.api import *
+for result in run_rrater(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
+  print(result)
+```
+
 #### Tests and demos 
 
 * Take a look at folder [deepllm/tests](https://github.com/ptarau/recursors/tree/main/deepllm/tests) for typical uses.
 
 * There are more extensive demos in folder  [deepllm/demos](https://github.com/ptarau/recursors/tree/main/deepllm/demos) .
 
 * There will be soon ```streamlit``` apps at https://github.com/ptarau/recursors/tree/main/deepllm/apps showing typical use cases.
 
 * If you install  [fastchat](https://github.com/lm-sys/FastChat), there are examples of using Vicuna models with it in folder [deepllm/local_llms](https://github.com/ptarau/recursors/tree/main/deepllm/local_llms).
 
-#### Streamlit eeb app
+#### Streamlit web app
 
 After installing streamlit, try it with:
 
 ```
 streamlit run deepllm/apps/app.py
 ```
 
@@ -86,12 +99,12 @@
        eprint = {2306.14077},
  primaryClass = {cs.AI},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2023arXiv230614077T},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
 
-You can also find the paper (and future related work) in folder  [docs](https://github.com/ptarau/recursors/tree/main/deepllm/docs).
+You can also find the paper (and future related work) in folder  [docs](https://github.com/ptarau/recursors/tree/main/docs).
 
 Enjoy,
 
 Paul Tarau
```

### Comparing `deepllm-0.5.5/README.md` & `deepllm-0.5.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: deepllm
+Version: 0.5.6
+Summary: Deep, recursive, goal-driven LLM explorer
+Home-page: https://github.com/ptarau/recursors.git
+Author: Paul Tarau
+Author-email: paul.tarau@gmail.com
+License: GPL-3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # deepllm: Full Automation of Goal-driven LLM Dialog Threads with And-Or Recursors and Refiner Oracles
 
 
 ### Overview
 We automate deep step-by step reasoning in an LLM dialog thread by recursively exploring alternatives (OR-nodes) and expanding details (AND-nodes) up to a given depth. Starting from a single succinct task-specific initiator we steer the automated dialog thread to stay focussed on the task by synthesizing a prompt that summarizes the depth-first steps taken so far. 
 
 Our algorithm is derived from a simple recursive descent implementation
@@ -28,31 +39,55 @@
 
 ```
 git clone git@github.com:ptarau/recursors.git
 ```
 
 #### Installing
 
-You can install the package ```deepllm``` by typing in folder ```recursors```
+If you have cloned this repo, you can install the package ```deepllm``` by typing in folder ```recursors```
 
 ```
 pip3 install -e .
 ```
 
+You can also install it from [pypi](https://pypi.org/search/?q=deepllm) with
+
+```
+pip3 install deepllm
+```
+
+#### API
+
+The DeepLLM [API](https://github.com/ptarau/recursors/blob/main/deepllm/api.py) exposes its high-level functions ready to embed in your application with something as simple as (assuming the your OPENAI_KEY is exported by your environment):
+
+```
+from deepllm.api import *
+for result in run_recursor(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
+  print(result)
+
+```
+Also, you can ask more interesting questions like in:
+
+```
+from deepllm.api import *
+for result in run_rrater(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
+  print(result)
+```
+
 #### Tests and demos 
 
 * Take a look at folder [deepllm/tests](https://github.com/ptarau/recursors/tree/main/deepllm/tests) for typical uses.
 
 * There are more extensive demos in folder  [deepllm/demos](https://github.com/ptarau/recursors/tree/main/deepllm/demos) .
 
 * There will be soon ```streamlit``` apps at https://github.com/ptarau/recursors/tree/main/deepllm/apps showing typical use cases.
 
 * If you install  [fastchat](https://github.com/lm-sys/FastChat), there are examples of using Vicuna models with it in folder [deepllm/local_llms](https://github.com/ptarau/recursors/tree/main/deepllm/local_llms).
 
-#### Streamlit eeb app
+#### Streamlit web app
 
 After installing streamlit, try it with:
 
 ```
 streamlit run deepllm/apps/app.py
 ```
 
@@ -75,12 +110,12 @@
        eprint = {2306.14077},
  primaryClass = {cs.AI},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2023arXiv230614077T},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
 
-You can also find the paper (and future related work) in folder  [docs](https://github.com/ptarau/recursors/tree/main/deepllm/docs).
+You can also find the paper (and future related work) in folder  [docs](https://github.com/ptarau/recursors/tree/main/docs).
 
 Enjoy,
 
 Paul Tarau
```

### Comparing `deepllm-0.5.5/deepllm/api.py` & `deepllm-0.5.6/deepllm/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .refiners import Advisor, Rater, TruthRater, AbstractMaker
 
 def run_recursor(initiator=None, prompter=None, lim=None):
     assert None not in (prompter, initiator, lim)
     recursor = AndOrExplorer(initiator=initiator, prompter=prompter, lim=lim)
     yield from recursor.run()
 
-def run_advisor(initiator=None, prompter=None, lim=None):
+def run_adviser(initiator=None, prompter=None, lim=None):
     assert None not in (prompter, initiator, lim)
     recursor = Advisor(initiator=initiator, prompter=prompter, lim=lim)
     yield from recursor.run()
 
 def run_rater(initiator=None, prompter=None, lim=None, threshold=None):
     assert None not in (prompter, initiator, lim, threshold)
     recursor = Rater(initiator=initiator, prompter=prompter, lim=lim, threshold=threshold)
```

### Comparing `deepllm-0.5.5/deepllm/apps/app.py` & `deepllm-0.5.6/deepllm/apps/app.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/configurator.py` & `deepllm-0.5.6/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/demos/demo.py` & `deepllm-0.5.6/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/demos/wikifetch.py` & `deepllm-0.5.6/deepllm/demos/wikifetch.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/embedders.py` & `deepllm-0.5.6/deepllm/embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/horn_prover.py` & `deepllm-0.5.6/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/interactors.py` & `deepllm-0.5.6/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/local_llms/local_runs.py` & `deepllm-0.5.6/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/local_llms/test_vicuna.py` & `deepllm-0.5.6/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/params.py` & `deepllm-0.5.6/deepllm/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 IS_LOCAL_LLM = [False]
 
 GPT_PARAMS = dict(
     TRACE=0,
-    ROOT="../STATE/",
+    ROOT="./STATE/",
     CACHES="caches/",
     DATA="data/",
     OUT='out/',
     model="gpt-3.5-turbo",
     emebedding_model="text-embedding-ada-002",
     temperature=0.2,
     n=1,
     max_toks=4000,
     TOP_K=3,
     # LOCAL_LLM=IS_LOCAL_LLM[0]
 )
 
 LOCAL_PARAMS = dict(
     TRACE=0,
-    ROOT="../STATE_LOCAL/",
+    ROOT="./STATE_LOCAL/",
     CACHES="caches/",
     OUT='out/',
     DATA='data/',
     model="vicuna-7b-v1.3",
     emebedding_model="vicuna-7b-v1.3",
     temperature=0.2,
     n=1,
```

### Comparing `deepllm-0.5.5/deepllm/prompters.py` & `deepllm-0.5.6/deepllm/prompters.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/recursors.py` & `deepllm-0.5.6/deepllm/recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/refiners.py` & `deepllm-0.5.6/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/tests/test_api.py` & `deepllm-0.5.6/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/tests/test_recursors.py` & `deepllm-0.5.6/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/tests/test_refiners.py` & `deepllm-0.5.6/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm/tools.py` & `deepllm-0.5.6/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/deepllm.egg-info/PKG-INFO` & `deepllm-0.5.6/deepllm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.5.5
+Version: 0.5.6
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -39,31 +39,55 @@
 
 ```
 git clone git@github.com:ptarau/recursors.git
 ```
 
 #### Installing
 
-You can install the package ```deepllm``` by typing in folder ```recursors```
+If you have cloned this repo, you can install the package ```deepllm``` by typing in folder ```recursors```
 
 ```
 pip3 install -e .
 ```
 
+You can also install it from [pypi](https://pypi.org/search/?q=deepllm) with
+
+```
+pip3 install deepllm
+```
+
+#### API
+
+The DeepLLM [API](https://github.com/ptarau/recursors/blob/main/deepllm/api.py) exposes its high-level functions ready to embed in your application with something as simple as (assuming the your OPENAI_KEY is exported by your environment):
+
+```
+from deepllm.api import *
+for result in run_recursor(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
+  print(result)
+
+```
+Also, you can ask more interesting questions like in:
+
+```
+from deepllm.api import *
+for result in run_rrater(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
+  print(result)
+```
+
 #### Tests and demos 
 
 * Take a look at folder [deepllm/tests](https://github.com/ptarau/recursors/tree/main/deepllm/tests) for typical uses.
 
 * There are more extensive demos in folder  [deepllm/demos](https://github.com/ptarau/recursors/tree/main/deepllm/demos) .
 
 * There will be soon ```streamlit``` apps at https://github.com/ptarau/recursors/tree/main/deepllm/apps showing typical use cases.
 
 * If you install  [fastchat](https://github.com/lm-sys/FastChat), there are examples of using Vicuna models with it in folder [deepllm/local_llms](https://github.com/ptarau/recursors/tree/main/deepllm/local_llms).
 
-#### Streamlit eeb app
+#### Streamlit web app
 
 After installing streamlit, try it with:
 
 ```
 streamlit run deepllm/apps/app.py
 ```
 
@@ -86,12 +110,12 @@
        eprint = {2306.14077},
  primaryClass = {cs.AI},
        adsurl = {https://ui.adsabs.harvard.edu/abs/2023arXiv230614077T},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
 
-You can also find the paper (and future related work) in folder  [docs](https://github.com/ptarau/recursors/tree/main/deepllm/docs).
+You can also find the paper (and future related work) in folder  [docs](https://github.com/ptarau/recursors/tree/main/docs).
 
 Enjoy,
 
 Paul Tarau
```

### Comparing `deepllm-0.5.5/deepllm.egg-info/SOURCES.txt` & `deepllm-0.5.6/deepllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.5/setup.py` & `deepllm-0.5.6/setup.py`

 * *Files identical despite different names*

