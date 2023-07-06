# Comparing `tmp/arcee-align-0.0.2.tar.gz` & `tmp/arcee-align-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcee-align-0.0.2.tar", last modified: Mon Jun 26 04:36:13 2023, max compression
+gzip compressed data, was "arcee-align-0.0.3.tar", last modified: Thu Jul  6 18:17:24 2023, max compression
```

## Comparing `arcee-align-0.0.2.tar` & `arcee-align-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.652157 arcee-align-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2152 2023-06-26 04:36:13.652157 arcee-align-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2023-06-25 17:41:45.000000 arcee-align-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.636157 arcee-align-0.0.2/arcee/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-26 04:36:09.000000 arcee-align-0.0.2/arcee/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.640157 arcee-align-0.0.2/arcee/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-06-25 23:31:22.000000 arcee-align-0.0.2/arcee/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5076 2023-06-25 23:39:47.000000 arcee-align-0.0.2/arcee/data/generate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2262 2023-06-26 03:23:40.000000 arcee-align-0.0.2/arcee/data/instruction_set.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.644157 arcee-align-0.0.2/arcee/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-06-22 05:12:31.000000 arcee-align-0.0.2/arcee/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-06-26 03:23:40.000000 arcee-align-0.0.2/arcee/models/lm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.648157 arcee-align-0.0.2/arcee_align.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2152 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 04:36:13.652157 arcee-align-0.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1136 2023-06-26 04:17:02.000000 arcee-align-0.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 18:17:24.540779 arcee-align-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2168 2023-07-06 18:17:24.540779 arcee-align-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1216 2023-06-26 14:33:57.000000 arcee-align-0.0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 18:17:24.536779 arcee-align-0.0.3/arcee/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-07-06 18:14:45.000000 arcee-align-0.0.3/arcee/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 18:17:24.540779 arcee-align-0.0.3/arcee/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-06-25 23:31:22.000000 arcee-align-0.0.3/arcee/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5076 2023-06-25 23:39:47.000000 arcee-align-0.0.3/arcee/data/generate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2250 2023-07-06 17:31:19.000000 arcee-align-0.0.3/arcee/data/instruction_set.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 18:17:24.540779 arcee-align-0.0.3/arcee/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-06-22 05:12:31.000000 arcee-align-0.0.3/arcee/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3498 2023-07-06 18:13:47.000000 arcee-align-0.0.3/arcee/models/lm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 18:17:24.540779 arcee-align-0.0.3/arcee_align.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2168 2023-07-06 18:17:24.000000 arcee-align-0.0.3/arcee_align.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-07-06 18:17:24.000000 arcee-align-0.0.3/arcee_align.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-06 18:17:24.000000 arcee-align-0.0.3/arcee_align.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-06 18:17:24.000000 arcee-align-0.0.3/arcee_align.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-07-06 18:17:24.000000 arcee-align-0.0.3/arcee_align.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-06 18:17:24.540779 arcee-align-0.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1066 2023-07-06 18:17:22.000000 arcee-align-0.0.3/setup.py
```

### Comparing `arcee-align-0.0.2/PKG-INFO` & `arcee-align-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: arcee-align
-Version: 0.0.2
+Version: 0.0.3
 Summary: The open source toolkit for finetuning and deploying LLMs
 Home-page: https://arcee.ai/
 Author: Arcee
 Author-email: jacob@arcee.ai
 License: UNKNOWN
 Description: # Arcee
         
-        The open source toolkit for finetuning and deploying LLMs
+        :tulip:	The open source toolkit for finetuning and deploying LLMs :tulip:
         
         ### Finetune LLMS
         
         ```
         from arcee.models import LM
         from arcee.data import Instuctions
```

### Comparing `arcee-align-0.0.2/README.md` & `arcee-align-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Arcee
 
-The open source toolkit for finetuning and deploying LLMs
+:tulip:	The open source toolkit for finetuning and deploying LLMs :tulip:
 
 ### Finetune LLMS
 
 ```
 from arcee.models import LM
 from arcee.data import Instuctions
```

### Comparing `arcee-align-0.0.2/arcee/data/generate.py` & `arcee-align-0.0.3/arcee/data/generate.py`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.2/arcee/data/instruction_set.py` & `arcee-align-0.0.3/arcee/data/instruction_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,28 +20,28 @@
         if not data_file.endswith(".csv"):
             raise (Exception("Datafile must be a .csv file"))
 
         self.dataset = load_dataset("csv", data_files=data_file, split="train")
         dataset_fields = list(self.dataset.features.keys())
         self.dataset_fields = dataset_fields
 
-        if "instruction" not in dataset_fields:
+        if "prompt" not in dataset_fields:
             raise (Exception("Datafile must contain a column named 'instruction'"))
 
-        if "response" not in dataset_fields:
+        if "completion" not in dataset_fields:
             raise (Exception("Datafile must contain a column named 'response'"))
 
         self.instruction_prefix = instruction_prefix
         self.response_prefix = response_prefix
 
         # TODO refactor for larger datasets when TRL formatting_func is fixed
 
         text_column = [
             self.instruction_prefix + str(a) + " " + self.response_prefix + str(b)
-            for a, b in zip(self.dataset["instruction"], self.dataset["response"])
+            for a, b in zip(self.dataset["prompt"], self.dataset["completion"])
         ]
         self.dataset = self.dataset.add_column("text", text_column)
 
         train_test_split_ratio = 0.2
         dataset_train_val = self.dataset.train_test_split(
             test_size=train_test_split_ratio
         )
@@ -53,15 +53,15 @@
         return len(self.dataset)
 
     def __getitem__(self, idx):
         """
         This function formats an entry as it will appear during finetuning
         """
 
-        return f"{self.instruction_prefix} {self.dataset[idx]['instruction']} {self.response_prefix} {self.dataset[idx]['response']}"
+        return f"{self.instruction_prefix} {self.dataset[idx]['prompt']} {self.response_prefix} {self.dataset[idx]['completion']}"
 
     def formatting_prompts_func(self, example):
         """
         This function takes a dataset example and formats it into a prompt for finetuning.
         """
 
-        return f"{self.instruction_prefix} {example['instruction']} {self.response_prefix} {example['response']}"
+        return f"{self.instruction_prefix} {example['prompt']} {self.response_prefix} {example['completion']}"
```

### Comparing `arcee-align-0.0.2/arcee/models/lm.py` & `arcee-align-0.0.3/arcee/models/lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from arcee.data import InstructionSet
 
 question_prompt = "### Question: "
 answer_prompt = "### Answer: "
 
 
 def formatting_prompts_func(example):
-    text = f"{question_prompt} {example['instruction']} {answer_prompt} {example['response']}"
+    text = (
+        f"{question_prompt} {example['prompt']} {answer_prompt} {example['completion']}"
+    )
     return text
 
 
 class LM:
     """General language model class"""
 
     def __init__(self, name):
```

### Comparing `arcee-align-0.0.2/arcee_align.egg-info/PKG-INFO` & `arcee-align-0.0.3/arcee_align.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: arcee-align
-Version: 0.0.2
+Version: 0.0.3
 Summary: The open source toolkit for finetuning and deploying LLMs
 Home-page: https://arcee.ai/
 Author: Arcee
 Author-email: jacob@arcee.ai
 License: UNKNOWN
 Description: # Arcee
         
-        The open source toolkit for finetuning and deploying LLMs
+        :tulip:	The open source toolkit for finetuning and deploying LLMs :tulip:
         
         ### Finetune LLMS
         
         ```
         from arcee.models import LM
         from arcee.data import Instuctions
```

