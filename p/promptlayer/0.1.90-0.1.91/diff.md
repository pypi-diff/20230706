# Comparing `tmp/promptlayer-0.1.90.tar.gz` & `tmp/promptlayer-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.90.tar", last modified: Mon Jun 19 14:46:21 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.91.tar", last modified: Thu Jul  6 14:58:36 2023, max compression
```

## Comparing `promptlayer-0.1.90.tar` & `promptlayer-0.1.91.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-19 14:46:21.736165 promptlayer-0.1.90/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.90/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-19 14:46:21.735901 promptlayer-0.1.90/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.90/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-19 14:46:21.730700 promptlayer-0.1.90/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-13 14:07:07.000000 promptlayer-0.1.90/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-19 14:46:21.732675 promptlayer-0.1.90/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.90/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-19 14:46:21.733338 promptlayer-0.1.90/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.90/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.90/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.90/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-19 14:46:21.734447 promptlayer-0.1.90/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.90/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1839 2023-06-13 15:17:41.000000 promptlayer-0.1.90/promptlayer/prompts/chat.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.90/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-19 14:46:21.735404 promptlayer-0.1.90/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.90/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.90/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13481 2023-06-19 14:45:34.000000 promptlayer-0.1.90/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-19 14:46:21.732264 promptlayer-0.1.90/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-19 14:46:21.000000 promptlayer-0.1.90/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-06-19 14:46:21.000000 promptlayer-0.1.90/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-06-19 14:46:21.000000 promptlayer-0.1.90/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-06-19 14:46:21.000000 promptlayer-0.1.90/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-06-19 14:46:21.000000 promptlayer-0.1.90/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-06-19 14:46:21.736268 promptlayer-0.1.90/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-06-19 14:45:53.000000 promptlayer-0.1.90/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.996017 promptlayer-0.1.91/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.91/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-06 14:58:36.995681 promptlayer-0.1.91/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3855 2023-07-06 14:55:00.000000 promptlayer-0.1.91/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.986876 promptlayer-0.1.91/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-22 17:22:46.000000 promptlayer-0.1.91/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.989372 promptlayer-0.1.91/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.91/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.990711 promptlayer-0.1.91/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.91/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.91/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.91/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.993464 promptlayer-0.1.91/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.91/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1839 2023-06-13 15:17:41.000000 promptlayer-0.1.91/promptlayer/prompts/chat.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.91/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.994809 promptlayer-0.1.91/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.91/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.91/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    12463 2023-07-06 14:55:00.000000 promptlayer-0.1.91/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-06 14:58:36.988941 promptlayer-0.1.91/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-07-06 14:58:36.000000 promptlayer-0.1.91/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-07-06 14:58:36.996116 promptlayer-0.1.91/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-07-06 14:55:35.000000 promptlayer-0.1.91/setup.py
```

### Comparing `promptlayer-0.1.90/LICENSE` & `promptlayer-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/PKG-INFO` & `promptlayer-0.1.91/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.90
+Version: 0.1.91
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
         
         # 🍰 PromptLayer
         
         **The first platform built for <span style="background-color: rgb(219, 234, 254);">prompt engineers</span>**
         
         <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
-        <a href="https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629"><img alt="Docs" src="https://custom-icon-badges.herokuapp.com/badge/docs-PL-green.svg?logo=cake&style=for-the-badge&logoColor=white"></a>
-        <a href="https://www.loom.com/share/723cbdb43439458fb607e910faa13294"><img alt="Demo with Loom" src="https://img.shields.io/badge/Demo-loom-552586.svg?logo=loom&style=for-the-badge&labelColor=gray"></a>
+        <a href="https://docs.promptlayer.com"><img alt="Docs" src="https://custom-icon-badges.herokuapp.com/badge/docs-PL-green.svg?logo=cake&style=for-the-badge&logoColor=white"></a>
+        <a href="https://www.loom.com/share/196c42e43acd4a369d75e9a7374a0850"><img alt="Demo with Loom" src="https://img.shields.io/badge/Demo-loom-552586.svg?logo=loom&style=for-the-badge&labelColor=gray"></a>
         
         ---  
         
         <div align="left">
         
         [PromptLayer](https://promptlayer.com/) is the first platform that allows you to track, manage, and share your GPT prompt engineering. PromptLayer acts a middleware between your code and OpenAI’s python library. 
         
@@ -96,10 +96,11 @@
             "api_key": "pl_<YOUR API KEY>",
           },
         )
         ```
         
         ## Contributing
         
-        We welcome contributions to our open source project, including new features, infrastructure improvements, and better documentation. For more information or any questions, contact us at [hello@magniv.io](mailto:hello@magniv.io).
+        We welcome contributions to our open source project, including new features, infrastructure improvements, and better documentation. For more information or any questions, contact us at [hello@promptlayer.com](mailto:hello@promptlayer.com).
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.90 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.91 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
@@ -39,9 +39,10 @@
 "request_response": {"id": "cmpl-6TEeJCRVlqQSQqhD8CYKd1HdCcFxM", "object":
 "text_completion", "created": 1672425843, "model": "text-ada-001", "choices": [
 {"text": " advocacy\"\n\nMy name is advocacy.", "index": 0, "logprobs": None,
 "finish_reason": "stop"}]}, "request_start_time": 1673987077.463504,
 "request_end_time": 1673987077.463504, "api_key": "pl_", }, ) ``` ##
 Contributing We welcome contributions to our open source project, including new
 features, infrastructure improvements, and better documentation. For more
-information or any questions, contact us at [hello@magniv.io](mailto:
-hello@magniv.io). Platform: UNKNOWN Description-Content-Type: text/markdown
+information or any questions, contact us at [hello@promptlayer.com](mailto:
+hello@promptlayer.com). Platform: UNKNOWN Description-Content-Type: text/
+markdown
```

### Comparing `promptlayer-0.1.90/README.md` & `promptlayer-0.1.91/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <div align="center">
 
 # 🍰 PromptLayer
 
 **The first platform built for <span style="background-color: rgb(219, 234, 254);">prompt engineers</span>**
 
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
-<a href="https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629"><img alt="Docs" src="https://custom-icon-badges.herokuapp.com/badge/docs-PL-green.svg?logo=cake&style=for-the-badge&logoColor=white"></a>
-<a href="https://www.loom.com/share/723cbdb43439458fb607e910faa13294"><img alt="Demo with Loom" src="https://img.shields.io/badge/Demo-loom-552586.svg?logo=loom&style=for-the-badge&labelColor=gray"></a>
+<a href="https://docs.promptlayer.com"><img alt="Docs" src="https://custom-icon-badges.herokuapp.com/badge/docs-PL-green.svg?logo=cake&style=for-the-badge&logoColor=white"></a>
+<a href="https://www.loom.com/share/196c42e43acd4a369d75e9a7374a0850"><img alt="Demo with Loom" src="https://img.shields.io/badge/Demo-loom-552586.svg?logo=loom&style=for-the-badge&labelColor=gray"></a>
 
 ---  
 
 <div align="left">
 
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you to track, manage, and share your GPT prompt engineering. PromptLayer acts a middleware between your code and OpenAI’s python library. 
 
@@ -87,8 +87,8 @@
     "api_key": "pl_<YOUR API KEY>",
   },
 )
 ```
 
 ## Contributing
 
-We welcome contributions to our open source project, including new features, infrastructure improvements, and better documentation. For more information or any questions, contact us at [hello@magniv.io](mailto:hello@magniv.io).
+We welcome contributions to our open source project, including new features, infrastructure improvements, and better documentation. For more information or any questions, contact us at [hello@promptlayer.com](mailto:hello@promptlayer.com).
```

#### html2text {}

```diff
@@ -34,9 +34,9 @@
 "request_response": {"id": "cmpl-6TEeJCRVlqQSQqhD8CYKd1HdCcFxM", "object":
 "text_completion", "created": 1672425843, "model": "text-ada-001", "choices": [
 {"text": " advocacy\"\n\nMy name is advocacy.", "index": 0, "logprobs": None,
 "finish_reason": "stop"}]}, "request_start_time": 1673987077.463504,
 "request_end_time": 1673987077.463504, "api_key": "pl_", }, ) ``` ##
 Contributing We welcome contributions to our open source project, including new
 features, infrastructure improvements, and better documentation. For more
-information or any questions, contact us at [hello@magniv.io](mailto:
-hello@magniv.io).
+information or any questions, contact us at [hello@promptlayer.com](mailto:
+hello@promptlayer.com).
```

### Comparing `promptlayer-0.1.90/promptlayer/__init__.py` & `promptlayer-0.1.91/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.91/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/promptlayer/promptlayer.py` & `promptlayer-0.1.91/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/promptlayer/prompts/chat.py` & `promptlayer-0.1.91/promptlayer/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/promptlayer/prompts/prompts.py` & `promptlayer-0.1.91/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/promptlayer/track/track.py` & `promptlayer-0.1.91/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/promptlayer/utils.py` & `promptlayer-0.1.91/promptlayer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import contextvars
 import functools
 import os
 import sys
 import types
 from copy import deepcopy
+from json import JSONDecodeError
 
 import requests
 
 import promptlayer
 
 URL_API_PROMPTLAYER = os.environ.setdefault(
     "URL_API_PROMPTLAYER", "https://api.promptlayer.com"
@@ -110,14 +111,15 @@
     request_end_time,
     api_key,
     return_pl_id=False,
     metadata=None,
 ):
     if type(response) != dict and hasattr(response, "to_dict_recursive"):
         response = response.to_dict_recursive()
+    request_response = None
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/track-request",
             json={
                 "function_name": function_name,
                 "provider_type": provider_type,
                 "args": args,
@@ -127,30 +129,21 @@
                 "request_start_time": request_start_time,
                 "request_end_time": request_end_time,
                 "metadata": metadata,
                 "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
-            if hasattr(request_response, "json"):
-                print(
-                    f"WARNING: While logging your request PromptLayer had the following error: {request_response.json().get('message')}",
-                    file=sys.stderr,
-                )
-            else:
-                print(
-                    f"WARNING: While logging your request PromptLayer had the following error: {request_response}",
-                    file=sys.stderr,
-                )
+            warn_on_bad_response(request_response, "WARNING: While logging your request PromptLayer had the following error")
     except Exception as e:
         print(
             f"WARNING: While logging your request PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
-    if return_pl_id:
+    if request_response is not None and return_pl_id:
         return request_response.json().get("request_id")
 
 
 def promptlayer_api_request_async(
     function_name,
     provider_type,
     args,
@@ -185,54 +178,41 @@
     """
     try:
         request_response = requests.get(
             f"{URL_API_PROMPTLAYER}/library-get-prompt-template",
             headers={"X-API-KEY": api_key},
             params={"prompt_name": prompt_name, "version": version},
         )
-        if request_response.status_code != 200:
-            if hasattr(request_response, "json"):
-                raise Exception(
-                    f"PromptLayer had the following error while getting your prompt: {request_response.json().get('message')}"
-                )
-            else:
-                raise Exception(
-                    f"PromptLayer had the following error while getting your prompt: {request_response}"
-                )
     except Exception as e:
         raise Exception(
             f"PromptLayer had the following error while getting your prompt: {e}"
         )
+    if request_response.status_code != 200:
+        raise_on_bad_response(request_response, "PromptLayer had the following error while getting your prompt")
+
     return request_response.json()
 
 
 def promptlayer_publish_prompt(prompt_name, prompt_template, tags, api_key):
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/library-publish-prompt-template",
             json={
                 "prompt_name": prompt_name,
                 "prompt_template": prompt_template,
                 "tags": tags,
                 "api_key": api_key,
             },
         )
-        if request_response.status_code != 200:
-            if hasattr(request_response, "json"):
-                raise Exception(
-                    f"PromptLayer had the following error while publishing your prompt: {request_response.json().get('message')}"
-                )
-            else:
-                raise Exception(
-                    f"PromptLayer had the following error while publishing your prompt: {request_response}"
-                )
     except Exception as e:
         raise Exception(
             f"PromptLayer had the following error while publishing your prompt: {e}"
         )
+    if request_response.status_code != 200:
+        raise_on_bad_response(request_response, "PromptLayer had the following error while publishing your prompt")
     return True
 
 
 def promptlayer_track_prompt(
     request_id, prompt_name, input_variables, api_key, version
 ):
     try:
@@ -243,26 +223,16 @@
                 "prompt_name": prompt_name,
                 "prompt_input_variables": input_variables,
                 "api_key": api_key,
                 "version": version,
             },
         )
         if request_response.status_code != 200:
-            if hasattr(request_response, "json"):
-                print(
-                    f"WARNING: While tracking your prompt PromptLayer had the following error: {request_response.json().get('message')}",
-                    file=sys.stderr,
-                )
-                return False
-            else:
-                print(
-                    f"WARNING: While tracking your prompt PromptLayer had the following error: {request_response}",
-                    file=sys.stderr,
-                )
-                return False
+            warn_on_bad_response(request_response, "WARNING: While tracking your prompt PromptLayer had the following error")
+            return False
     except Exception as e:
         print(
             f"WARNING: While tracking your prompt PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
         return False
     return True
@@ -275,26 +245,16 @@
             json={
                 "request_id": request_id,
                 "metadata": metadata,
                 "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
-            if hasattr(request_response, "json"):
-                print(
-                    f"WARNING: While tracking your metadata PromptLayer had the following error: {request_response.json().get('message')}",
-                    file=sys.stderr,
-                )
-                return False
-            else:
-                print(
-                    f"WARNING: While tracking your metadata PromptLayer had the following error: {request_response}",
-                    file=sys.stderr,
-                )
-                return False
+            warn_on_bad_response(request_response, "WARNING: While tracking your metadata PromptLayer had the following error")
+            return False
     except Exception as e:
         print(
             f"WARNING: While tracking your metadata PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
         return False
     return True
@@ -307,26 +267,16 @@
             json={
                 "request_id": request_id,
                 "score": score,
                 "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
-            if hasattr(request_response, "json"):
-                print(
-                    f"WARNING: While tracking your score PromptLayer had the following error: {request_response.json().get('message')}",
-                    file=sys.stderr,
-                )
-                return False
-            else:
-                print(
-                    f"WARNING: While tracking your score PromptLayer had the following error: {request_response}",
-                    file=sys.stderr,
-                )
-                return False
+            warn_on_bad_response(request_response, "WARNING: While tracking your score PromptLayer had the following error")
+            return False
     except Exception as e:
         print(
             f"WARNING: While tracking your score PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
         return False
     return True
@@ -411,7 +361,43 @@
 async def run_in_thread_async(executor, func, *args, **kwargs):
     """https://github.com/python/cpython/blob/main/Lib/asyncio/threads.py"""
     loop = asyncio.get_running_loop()
     ctx = contextvars.copy_context()
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
     res = await loop.run_in_executor(executor, func_call)
     return res
+
+
+def warn_on_bad_response(request_response, main_message):
+    if hasattr(request_response, "json"):
+        try:
+            print(
+                f"{main_message}: {request_response.json().get('message')}",
+                file=sys.stderr
+            )
+        except JSONDecodeError:
+            print(
+                f"{main_message}: {request_response}",
+                file=sys.stderr,
+            )
+    else:
+        print(
+            f"{main_message}: {request_response}",
+            file=sys.stderr
+        )
+
+
+def raise_on_bad_response(request_response, main_message):
+    if hasattr(request_response, "json"):
+        try:
+            raise Exception(
+                f"{main_message}: {request_response.json().get('message')}"
+            )
+        except JSONDecodeError:
+            raise Exception(
+                f"{main_message}: {request_response}"
+            )
+    else:
+        raise Exception(
+            f"{main_message}: {request_response}"
+        )
+
```

### Comparing `promptlayer-0.1.90/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.91/promptlayer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.90
+Version: 0.1.91
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
         
         # 🍰 PromptLayer
         
         **The first platform built for <span style="background-color: rgb(219, 234, 254);">prompt engineers</span>**
         
         <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
-        <a href="https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629"><img alt="Docs" src="https://custom-icon-badges.herokuapp.com/badge/docs-PL-green.svg?logo=cake&style=for-the-badge&logoColor=white"></a>
-        <a href="https://www.loom.com/share/723cbdb43439458fb607e910faa13294"><img alt="Demo with Loom" src="https://img.shields.io/badge/Demo-loom-552586.svg?logo=loom&style=for-the-badge&labelColor=gray"></a>
+        <a href="https://docs.promptlayer.com"><img alt="Docs" src="https://custom-icon-badges.herokuapp.com/badge/docs-PL-green.svg?logo=cake&style=for-the-badge&logoColor=white"></a>
+        <a href="https://www.loom.com/share/196c42e43acd4a369d75e9a7374a0850"><img alt="Demo with Loom" src="https://img.shields.io/badge/Demo-loom-552586.svg?logo=loom&style=for-the-badge&labelColor=gray"></a>
         
         ---  
         
         <div align="left">
         
         [PromptLayer](https://promptlayer.com/) is the first platform that allows you to track, manage, and share your GPT prompt engineering. PromptLayer acts a middleware between your code and OpenAI’s python library. 
         
@@ -96,10 +96,11 @@
             "api_key": "pl_<YOUR API KEY>",
           },
         )
         ```
         
         ## Contributing
         
-        We welcome contributions to our open source project, including new features, infrastructure improvements, and better documentation. For more information or any questions, contact us at [hello@magniv.io](mailto:hello@magniv.io).
+        We welcome contributions to our open source project, including new features, infrastructure improvements, and better documentation. For more information or any questions, contact us at [hello@promptlayer.com](mailto:hello@promptlayer.com).
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.90 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.91 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
@@ -39,9 +39,10 @@
 "request_response": {"id": "cmpl-6TEeJCRVlqQSQqhD8CYKd1HdCcFxM", "object":
 "text_completion", "created": 1672425843, "model": "text-ada-001", "choices": [
 {"text": " advocacy\"\n\nMy name is advocacy.", "index": 0, "logprobs": None,
 "finish_reason": "stop"}]}, "request_start_time": 1673987077.463504,
 "request_end_time": 1673987077.463504, "api_key": "pl_", }, ) ``` ##
 Contributing We welcome contributions to our open source project, including new
 features, infrastructure improvements, and better documentation. For more
-information or any questions, contact us at [hello@magniv.io](mailto:
-hello@magniv.io). Platform: UNKNOWN Description-Content-Type: text/markdown
+information or any questions, contact us at [hello@promptlayer.com](mailto:
+hello@promptlayer.com). Platform: UNKNOWN Description-Content-Type: text/
+markdown
```

### Comparing `promptlayer-0.1.90/promptlayer.egg-info/SOURCES.txt` & `promptlayer-0.1.91/promptlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.90/setup.py` & `promptlayer-0.1.91/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={
         "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
     },
-    version="0.1.90",
+    version="0.1.91",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "langchain"],
 )
```

