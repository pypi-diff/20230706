# Comparing `tmp/llmreflect-0.0.1.tar.gz` & `tmp/llmreflect-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.0.1.tar", max compression
+gzip compressed data, was "llmreflect-0.0.2.tar", max compression
```

## Comparing `llmreflect-0.0.1.tar` & `llmreflect-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     4043 2023-07-05 15:41:46.914964 llmreflect-0.0.1/README.md
--rw-r--r--   0        0        0     1235 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     2522 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Agents/ModerateAgent.py
--rw-r--r--   0        0        0     5183 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Agents/PostgressqlAgent.py
--rw-r--r--   0        0        0     2409 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0      762 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Chains/BasicChain.py
--rw-r--r--   0        0        0     8085 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Chains/DatabaseChain.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Chains/__init__.py
--rw-r--r--   0        0        0     8019 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     2807 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Prompt/promptbase/gradingpostgresql.json
--rw-r--r--   0        0        0     1916 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Prompt/promptbase/moderatepostgresql.json
--rw-r--r--   0        0        0     4951 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Prompt/promptbase/postgresql.json
--rw-r--r--   0        0        0     2011 2023-07-05 15:41:46.914964 llmreflect-0.0.1/llmreflect/Prompt/promptbase/questionpostgresql.json
--rw-r--r--   0        0        0      743 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     4219 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Tests/__init__.py
--rw-r--r--   0        0        0     2421 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Tests/test_chains.py
--rw-r--r--   0        0        0      442 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      690 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Utils/database.py
--rw-r--r--   0        0        0      305 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/Utils/message.py
--rw-r--r--   0        0        0        0 2023-07-05 15:41:46.918964 llmreflect-0.0.1/llmreflect/__init__.py
--rw-r--r--   0        0        0      478 2023-07-05 15:41:46.918964 llmreflect-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 llmreflect-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4061 2023-07-06 21:18:12.387481 llmreflect-0.0.2/README.md
+-rw-r--r--   0        0        0     1235 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     2522 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3204 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Agents/ModerateAgent.py
+-rw-r--r--   0        0        0     9728 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Agents/PostgresqlAgent.py
+-rw-r--r--   0        0        0     2429 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     1873 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Chains/BasicChain.py
+-rw-r--r--   0        0        0    15317 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Chains/DatabaseChain.py
+-rw-r--r--   0        0        0     1656 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Chains/ModerateChain.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Chains/__init__.py
+-rw-r--r--   0        0        0     8419 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     2807 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Prompt/promptbase/gradingpostgresql.json
+-rw-r--r--   0        0        0     2094 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Prompt/promptbase/moderatepostgresql.json
+-rw-r--r--   0        0        0     4951 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Prompt/promptbase/postgresql.json
+-rw-r--r--   0        0        0     1119 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Prompt/promptbase/postgresqlfix.json
+-rw-r--r--   0        0        0     2011 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Prompt/promptbase/questionpostgresql.json
+-rw-r--r--   0        0        0     1933 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     4219 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0     6221 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Tests/test_chains.py
+-rw-r--r--   0        0        0      442 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      690 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0      305 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/Utils/message.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:18:12.387481 llmreflect-0.0.2/llmreflect/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-06 21:18:12.387481 llmreflect-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.2/PKG-INFO
```

### Comparing `llmreflect-0.0.1/README.md` & `llmreflect-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # llmReflect
-[![PyPI version](https://badge.fury.io/py/llmreflect.svg)](https://badge.fury.io/py/llmreflect) ![Python Versions](https://img.shields.io/pypi/pyversions/llmreflect) 
-[![Python package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml)
-[![Upload Python Package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml)
-
+[![PyPI version](https://badge.fury.io/py/llmreflect.svg)](https://badge.fury.io/py/llmreflect)
+[![Python](https://img.shields.io/badge/python-3.11-blue.svg)](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Python package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml/badge.svg)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml)
 llmReflect is a python package designed for large language model (**LLM**) applications. We have seen numerous emergent abilities so far. Given by a right prompt, a LLM is capable of various tasks. Also the art of writing a prompt usually determines the performance of the LLM at that task. So is there a chance that we can use LLM to evaluate / improve itself's prompt?
 
 **Warning!** This project is at the very early stage!
 
 ## Installation
 * 1.  llmReflect is on PYPI. \
 `pip install llmreflect`
```

### Comparing `llmreflect-0.0.1/llmreflect/Agents/BasicAgent.py` & `llmreflect-0.0.2/llmreflect/Agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.1/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.0.2/llmreflect/Agents/EvaluationAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.1/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.0.2/llmreflect/Agents/QuestionAgent.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
                  prompt_name: str = 'questionpostgresql',
                  max_output_tokens: int = 512,
                  temperature: float = 0.7):
         """
-        Agent class for querying database.
+        Agent for creating questions based on a given database
         Args:
             open_ai_key (str): API key to connect to chatgpt service.
             prompt_name (str, optional): name for the prompt json file.
                 Defaults to 'questionpostgresql'.
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
```

### Comparing `llmreflect-0.0.1/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.0.2/llmreflect/Prompt/BasicPrompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 import os
 from llmreflect.Utils.message import message
 import json
 import re
 
 PROMPT_BASE_DIR = os.path.join(os.getcwd(),
                                'llmreflect', 'Prompt', 'promptbase')
-INPUT_KEY_TYPE_CHOICE = ['INPUT', 'OUTPUT']
+INPUT_KEY_TYPE_CHOICE = ['INPUT', 'OUTPUT', 'CONTEXT']
 
 
 class BasicPrompt:
     """
     Mighty mother of all prompts (In this repo I mean)
     """
     def __init__(self, prompt_dict: Dict[str, Any], promptname: str,
                  customized_input_list: list = []) -> None:
         """
         If you want to start working on a prompt from scratch,
         a dictionary containing the prompts and name of this prompt
         are required.
         Args:
             prompt_dict (Dict[str, Any]): In this design,
-            a prompt can be divided into 3 parts,
-            hard rules, soft rule and in-context learning.
+            a prompt can be divided into 4 parts,
+            hard rules, soft rule and in-context learning and format.
             Hard rules indicate the general context for the LLM and
             we usually do not change the hard rules.
             Soft rules are the rules that focus on the refine the
             behavior for the model, used for formatting or tuning.
             In-context learning is just a cool word to say examples.
             We all need examples right?
             promptname (str): nickname by you for the prompt.
@@ -44,26 +44,25 @@
 
             Overall this design is to enable the model to tune itself.
             So there are rules the model can touch and others cant.
             Also I hate people keeping prompts in the coding logic place.
 
         """
         self.promptname = promptname
-        self.__valid_prompt_dict(prompt_dict)
         self.prompt_dict = prompt_dict
         self._hard_rules = prompt_dict["HARD"]
         self._soft_rules = prompt_dict["SOFT"]
         self._in_context_learning_list = prompt_dict["INCONTEXT"]
         self._format_dict = prompt_dict["FORMAT"]
-
         self.__assemble__()
         if len(customized_input_list) > 0:
             self.input_list = customized_input_list
         else:
             self.input_list = self.__get_inputs__()
+        self.__valid_prompt_dict(prompt_dict)
         self.prompt_template = PromptTemplate(input_variables=self.input_list,
                                               template=self.string_temp)
 
     def __valid_prompt_dict(self, prompt_dict):
         """
         method for validating prompt dictionary
         Args:
@@ -100,17 +99,20 @@
         """
         assemble into one string
         """
         self.string_temp = ""
         self.string_temp += self.hard_rules
         self.string_temp += "\n\n"
         self.string_temp += self.soft_rules
-        self.string_temp += "\n\n"
-        self.string_temp += "For examples:\n\n"
-        self.string_temp += self.in_context_learning
+
+        if len(self.in_context_learning) > 0:
+            self.string_temp += "\n\n"
+            self.string_temp += "For examples:\n\n"
+            self.string_temp += self.in_context_learning
+
         self.string_temp += "\n\n"
         self.string_temp += "You must use the following format:\n\n"
         self.string_temp += self.input_format
         self.string_temp += "\n\n"
         self.string_temp += self.completion_head_up
 
     def get_langchain_prompt_template(self):
@@ -128,14 +130,29 @@
     def _load_json_file(cls, promptname: str):
         prompt_dir = os.path.join(PROMPT_BASE_DIR, promptname + '.json')
 
         with open(prompt_dir, 'r') as openfile:
             js = json.load(openfile)
         return js
 
+    @classmethod
+    def get_prompt_dict_template(cls):
+        dict_tmp = {
+            "HARD": '''\
+''',
+            "SOFT": '''\
+''',
+            "INCONTEXT": [
+
+            ],
+            "FORMAT": {
+
+            }}
+        return dict_tmp
+
     def save_prompt(self):
         """
         save prompt into json file.
         """
         try:
             self.__valid_prompt_dict(self.prompt_dict)
         except Exception:
@@ -157,26 +174,26 @@
     def hard_rules(self):
         return self._hard_rules
 
     @hard_rules.setter
     def hard_rules(self, rule: str):
         self._hard_rules = rule
         self.prompt_dict['HARD'] = self._hard_rules
-        self.__valid_prompt_dict()
+        self.__valid_prompt_dict(self.prompt_dict)
         self.__assemble__()
 
     @property
     def soft_rules(self):
         return self._soft_rules
 
     @soft_rules.setter
     def soft_rules(self, rule: str):
         self._soft_rules = rule
         self.prompt_dict['SOFT'] = self._soft_rules
-        self.__valid_prompt_dict()
+        self.__valid_prompt_dict(self.prompt_dict)
         self.__assemble__()
 
     @property
     def in_context_learning(self):
         txt = ""
 
         for each_dict in self._in_context_learning_list:
@@ -188,32 +205,32 @@
             txt += "\n"
         return txt
 
     @in_context_learning.setter
     def in_context_learning(self, rule: list):
         self._in_context_learning = rule
         self.prompt_dict['INCONTEXT'] = self._in_context_learning
-        self.__valid_prompt_dict()
+        self.__valid_prompt_dict(self.prompt_dict)
         self.__assemble__()
 
     @property
     def input_format(self):
         txt = ""
         for key in self._format_dict.keys():
             txt += "\n"
             txt += self.wrap_key_name(key)
             txt += " "
             txt += self._format_dict[key]['explanation']
         return txt
 
     @input_format.setter
-    def input_format(self, input_format: dict):
-        self._format_dict = input_format
+    def input_format(self, input_format_dict: dict):
+        self._format_dict = input_format_dict
         self.prompt_dict["FORMAT"] = self._format_dict
-        self.__valid_prompt_dict()
+        self.__valid_prompt_dict(self.prompt_dict)
         self.__assemble__()
 
     @property
     def completion_head_up(self):
         txt = ""
         for key in self._format_dict.keys():
             if self._format_dict[key]['type'] == "INPUT":
```

### Comparing `llmreflect-0.0.1/llmreflect/Prompt/promptbase/gradingpostgresql.json` & `llmreflect-0.0.2/llmreflect/Prompt/promptbase/gradingpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.1/llmreflect/Prompt/promptbase/moderatepostgresql.json` & `llmreflect-0.0.2/llmreflect/Prompt/promptbase/moderatepostgresql.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'FORMAT'": "{'topic': OrderedDict([('type', 'CONTEXT'), ('explanation', 'the expected theme for "*

 * *             "the requests')]), 'included_tables': OrderedDict([('type', 'CONTEXT'), "*

 * *             "('explanation', 'the expected theme for the requests')])}"}*

```diff
@@ -1,16 +1,24 @@
 {
     "FORMAT": {
+        "included_tables": {
+            "explanation": "the expected theme for the requests",
+            "type": "CONTEXT"
+        },
         "request": {
             "explanation": "user's request",
             "type": "INPUT"
         },
         "response": {
             "explanation": "your decision, [APPROVE] or [REJECT] plus the reason",
             "type": "OUTPUT"
+        },
+        "topic": {
+            "explanation": "the expected theme for the requests",
+            "type": "CONTEXT"
         }
     },
     "HARD": "You are a guard for a large language modeling system.Your job is to protect the system from cyber attacks, toxic content and ultra vires.\nYou will receive requests from users. And you must reject all requests involving toxic content, attempts to alter a database,\nattempts to access unauthorized tables,and content irrelavant to {topic}.Any access to any tables other than {included_tables} should be rejected.\nYou must specify the reject reasons.Otherwise, the request should be approved.\n",
     "INCONTEXT": [
         {
             "request": "show 124 patients",
             "response": "[APPROVE]"
```

### Comparing `llmreflect-0.0.1/llmreflect/Prompt/promptbase/postgresql.json` & `llmreflect-0.0.2/llmreflect/Prompt/promptbase/postgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.1/llmreflect/Prompt/promptbase/questionpostgresql.json` & `llmreflect-0.0.2/llmreflect/Prompt/promptbase/questionpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.1/llmreflect/Retriever/DatabaseRetriever.py` & `llmreflect-0.0.2/llmreflect/Retriever/DatabaseRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.1/llmreflect/Utils/database.py` & `llmreflect-0.0.2/llmreflect/Utils/database.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.1/PKG-INFO` & `llmreflect-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.0.1
+Version: 0.0.2
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,18 +15,18 @@
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Description-Content-Type: text/markdown
 
 # llmReflect
-[![PyPI version](https://badge.fury.io/py/llmreflect.svg)](https://badge.fury.io/py/llmreflect) ![Python Versions](https://img.shields.io/pypi/pyversions/llmreflect) 
-[![Python package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml)
-[![Upload Python Package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml)
-
+[![PyPI version](https://badge.fury.io/py/llmreflect.svg)](https://badge.fury.io/py/llmreflect)
+[![Python](https://img.shields.io/badge/python-3.11-blue.svg)](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Python package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml/badge.svg)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml)
 llmReflect is a python package designed for large language model (**LLM**) applications. We have seen numerous emergent abilities so far. Given by a right prompt, a LLM is capable of various tasks. Also the art of writing a prompt usually determines the performance of the LLM at that task. So is there a chance that we can use LLM to evaluate / improve itself's prompt?
 
 **Warning!** This project is at the very early stage!
 
 ## Installation
 * 1.  llmReflect is on PYPI. \
 `pip install llmreflect`
```

