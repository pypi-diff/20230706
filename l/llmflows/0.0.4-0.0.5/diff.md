# Comparing `tmp/llmflows-0.0.4.tar.gz` & `tmp/llmflows-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflows-0.0.4.tar", last modified: Tue Jul  4 05:41:52 2023, max compression
+gzip compressed data, was "llmflows-0.0.5.tar", last modified: Thu Jul  6 06:02:36 2023, max compression
```

## Comparing `llmflows-0.0.4.tar` & `llmflows-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-04 05:41:41.000000 llmflows-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-04 05:41:52.589293 llmflows-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-04 05:41:41.000000 llmflows-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/async_base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/async_functional_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/functional_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/functional_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/vectorstore_flowstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/llmflows/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/openai_embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/llmflows/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/prompts/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/llmflows/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/vector_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-04 05:41:41.000000 llmflows-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:41:52.589293 llmflows-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-06 06:02:25.000000 llmflows-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-06 06:02:36.152041 llmflows-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-06 06:02:25.000000 llmflows-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.144041 llmflows-0.0.5/llmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.148041 llmflows-0.0.5/llmflows/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/async_base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/async_functional_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/functional_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.148041 llmflows-0.0.5/llmflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/functional_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/vectorstore_flowstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/llmflows/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/openai_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/llmflows/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/prompts/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/llmflows/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/vector_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.148041 llmflows-0.0.5/llmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-06 06:02:25.000000 llmflows-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:02:36.152041 llmflows-0.0.5/setup.cfg
```

### Comparing `llmflows-0.0.4/LICENSE` & `llmflows-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/PKG-INFO` & `llmflows-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.4
+Version: 0.0.5
 Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
 Author: Stoyan Stoyanov
 Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
 Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llmflows-0.0.4/README.md` & `llmflows-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/callbacks/async_base_callback.py` & `llmflows-0.0.5/llmflows/callbacks/async_base_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/callbacks/async_functional_callback.py` & `llmflows-0.0.5/llmflows/callbacks/async_functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/callbacks/base_callback.py` & `llmflows-0.0.5/llmflows/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/callbacks/functional_callback.py` & `llmflows-0.0.5/llmflows/callbacks/functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/async_base_flow.py` & `llmflows-0.0.5/llmflows/flows/async_base_flow.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/async_base_flowstep.py` & `llmflows-0.0.5/llmflows/flows/async_base_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/async_chat_flowstep.py` & `llmflows-0.0.5/llmflows/flows/async_chat_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/async_flow.py` & `llmflows-0.0.5/llmflows/flows/async_flow.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/async_flowstep.py` & `llmflows-0.0.5/llmflows/flows/async_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/base_flow.py` & `llmflows-0.0.5/llmflows/flows/base_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,15 @@
             user_inputs (dict): The set of input keys provided by the user.
 
         Raises:
             ValueError: If not all required input keys are covered.
         """
 
         print(self.output_keys.union(user_inputs.keys()))
+        print(self.input_keys)
         if not self.input_keys.issubset(self.output_keys.union(user_inputs.keys())):
             raise ValueError("Some flowsteps have missing inputs")
 
     def execute(self, **inputs):
         """
         Placeholder method for executing the flow.
```

### Comparing `llmflows-0.0.4/llmflows/flows/base_flowstep.py` & `llmflows-0.0.5/llmflows/flows/base_flowstep.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,18 +48,39 @@
         Args:
             *steps (BaseFlowStep): Flow steps to connect to this step.
 
         Raises:
             ValueError: If connected flow steps have the same output key.
         """
         self._check_unique_keys(*steps)
+        for step in steps:
+            if self._introduces_cycle(step):
+                raise ValueError("Adding this connection would introduce a cycle.")
         self.next_steps.extend(steps)
         for step in steps:
             step.parents.append(self)
 
+    def _introduces_cycle(self, step: "BaseFlowStep") -> bool:
+        """
+        Checks if adding a connection to the given step would introduce a cycle.
+
+        Args:
+            step (BaseFlowStep): The step to which a connection is being added.
+
+        Returns:
+            bool: True if adding the connection would introduce a cycle, False otherwise.
+        """
+        to_visit = [step]
+        while to_visit:
+            current_step = to_visit.pop()
+            if current_step == self:
+                return True
+            to_visit.extend(current_step.next_steps)
+        return False
+
     def _check_unique_keys(self, *steps: "BaseFlowStep") -> None:
         """
         Checks that all connected flow steps have unique output keys.
 
         Args:
             *steps (BaseFlowStep): Flow steps to be connected to this step.
```

### Comparing `llmflows-0.0.4/llmflows/flows/chat_flowstep.py` & `llmflows-0.0.5/llmflows/flows/chat_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/flow.py` & `llmflows-0.0.5/llmflows/flows/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
             step (FlowStep): The step to execute.
             inputs (dict): The inputs to the step.
             verbose (bool): Specifies if the flow step should print its output.
 
         Returns:
             Any: The output of the step.
         """
+
         if not step or any(parent.output_key not in inputs for parent in step.parents):
             return
 
         required_inputs = {
             key: inputs[key] for key in step.required_keys
         }
```

### Comparing `llmflows-0.0.4/llmflows/flows/flowstep.py` & `llmflows-0.0.5/llmflows/flows/flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/functional_flowstep.py` & `llmflows-0.0.5/llmflows/flows/functional_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/flows/vectorstore_flowstep.py` & `llmflows-0.0.5/llmflows/flows/vectorstore_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/llms/llm.py` & `llmflows-0.0.5/llmflows/llms/llm.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/llms/llm_utils.py` & `llmflows-0.0.5/llmflows/llms/llm_utils.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/llms/openai.py` & `llmflows-0.0.5/llmflows/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/llms/openai_chat.py` & `llmflows-0.0.5/llmflows/llms/openai_chat.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/llms/openai_embeddings.py` & `llmflows-0.0.5/llmflows/llms/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/prompts/prompt_template.py` & `llmflows-0.0.5/llmflows/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/vectorstores/pinecone.py` & `llmflows-0.0.5/llmflows/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/vectorstores/vector_doc.py` & `llmflows-0.0.5/llmflows/vectorstores/vector_doc.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows/vectorstores/vector_store.py` & `llmflows-0.0.5/llmflows/vectorstores/vector_store.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/llmflows.egg-info/PKG-INFO` & `llmflows-0.0.5/llmflows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.4
+Version: 0.0.5
 Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
 Author: Stoyan Stoyanov
 Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
 Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llmflows-0.0.4/llmflows.egg-info/SOURCES.txt` & `llmflows-0.0.5/llmflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.4/pyproject.toml` & `llmflows-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llmflows"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Stoyan Stoyanov"},
 ]
 description = "LLMFlows - Simple, Explicit and Transparent LLM Apps"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

