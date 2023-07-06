# Comparing `tmp/freeplay-0.1.5.post1.tar.gz` & `tmp/freeplay-0.1.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.5.post1.tar", max compression
+gzip compressed data, was "freeplay-0.1.5.post2.tar", max compression
```

## Comparing `freeplay-0.1.5.post1.tar` & `freeplay-0.1.5.post2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-15 03:23:13.376261 freeplay-0.1.5.post1/README.md
--rw-r--r--   0        0        0       61 2023-06-28 22:11:30.981007 freeplay-0.1.5.post1/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-08 17:54:13.585930 freeplay-0.1.5.post1/freeplay/api_support.py
--rw-r--r--   0        0        0      553 2023-06-29 23:02:37.695249 freeplay-0.1.5.post1/freeplay/completions.py
--rw-r--r--   0        0        0      188 2023-06-15 15:26:56.089064 freeplay-0.1.5.post1/freeplay/errors.py
--rw-r--r--   0        0        0     8414 2023-06-29 23:02:37.695694 freeplay-0.1.5.post1/freeplay/flavors.py
--rw-r--r--   0        0        0    17759 2023-06-29 23:02:37.696236 freeplay-0.1.5.post1/freeplay/freeplay.py
--rw-r--r--   0        0        0      828 2023-06-27 23:41:00.518463 freeplay-0.1.5.post1/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      393 2023-06-29 23:06:34.925049 freeplay-0.1.5.post1/pyproject.toml
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 freeplay-0.1.5.post1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.5.post2/README.md
+-rw-r--r--   0        0        0       61 2023-06-29 11:36:19.640171 freeplay-0.1.5.post2/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.5.post2/freeplay/api_support.py
+-rw-r--r--   0        0        0      802 2023-07-05 20:48:51.495916 freeplay-0.1.5.post2/freeplay/completions.py
+-rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.5.post2/freeplay/errors.py
+-rw-r--r--   0        0        0     8414 2023-07-06 15:31:15.280860 freeplay-0.1.5.post2/freeplay/flavors.py
+-rw-r--r--   0        0        0    17926 2023-07-05 20:48:51.496816 freeplay-0.1.5.post2/freeplay/freeplay.py
+-rw-r--r--   0        0        0      828 2023-06-27 18:52:46.171090 freeplay-0.1.5.post2/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      393 2023-07-06 15:59:00.419388 freeplay-0.1.5.post2/pyproject.toml
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 freeplay-0.1.5.post2/PKG-INFO
```

### Comparing `freeplay-0.1.5.post1/freeplay/api_support.py` & `freeplay-0.1.5.post2/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.5.post1/freeplay/flavors.py` & `freeplay-0.1.5.post2/freeplay/flavors.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.5.post1/freeplay/freeplay.py` & `freeplay-0.1.5.post2/freeplay/freeplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,18 @@
     ) -> CompletionResponse:
         target_template = self.find_template_by_name(prompts, template_name)
         formatted_prompt = flavor.format(target_template, variables)
 
         # make call
         start = int(time.time())
         try:
-            params = self.client_params.merge_and_override(completion_parameters)
+            params = target_template.get_params() \
+                .merge_and_override(self.client_params) \
+                .merge_and_override(completion_parameters)
+
             completion_response = flavor.call_service(
                 formatted_prompt=formatted_prompt, llm_parameters=params)
         except Exception as e:
             raise FreeplayError("Error calling service") from e
         end = int(time.time())
 
         # record data
@@ -149,15 +152,17 @@
             completion_parameters: Optional[LLMParameters] = None
     ) -> Generator[CompletionChunk, None, None]:
         target_template = self.find_template_by_name(prompts, template_name)
         formatted_prompt = flavor.format(target_template, variables)
 
         # make call
         start = int(time.time())
-        params = self.client_params.merge_and_override(completion_parameters)
+        params = target_template.get_params() \
+            .merge_and_override(self.client_params) \
+            .merge_and_override(completion_parameters)
         completion_response = flavor.call_service_stream(formatted_prompt=formatted_prompt, llm_parameters=params)
         text_chunks = []
         last_is_complete = False
         for chunk in completion_response:
             text_chunks.append(chunk.text)
             last_is_complete = chunk.is_complete
             yield chunk
```

### Comparing `freeplay-0.1.5.post1/freeplay/llm_parameters.py` & `freeplay-0.1.5.post2/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.5.post1/PKG-INFO` & `freeplay-0.1.5.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.5.post1
+Version: 0.1.5.post2
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

