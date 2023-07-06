# Comparing `tmp/llm_bot-0.1.2.tar.gz` & `tmp/llm_bot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.1.2.tar", max compression
+gzip compressed data, was "llm_bot-0.1.3.tar", max compression
```

## Comparing `llm_bot-0.1.2.tar` & `llm_bot-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.1.2/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.1.2/llm_bot/__init__.py
--rw-r--r--   0        0        0    23603 2023-07-06 12:48:12.984031 llm_bot-0.1.2/llm_bot/core.py
--rw-r--r--   0        0        0     1009 2023-07-06 12:48:52.263713 llm_bot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 llm_bot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.1.3/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.1.3/llm_bot/__init__.py
+-rw-r--r--   0        0        0    23603 2023-07-06 12:48:12.984031 llm_bot-0.1.3/llm_bot/core.py
+-rw-r--r--   0        0        0     1027 2023-07-06 12:50:09.976442 llm_bot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 llm_bot-0.1.3/PKG-INFO
```

### Comparing `llm_bot-0.1.2/LICENSE` & `llm_bot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.1.2/llm_bot/core.py` & `llm_bot-0.1.3/llm_bot/core.py`

 * *Files identical despite different names*

### Comparing `llm_bot-0.1.2/pyproject.toml` & `llm_bot-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
@@ -12,14 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 faiss-cpu = "^1.7.4"
 langchain = "^0.0.224"
 openai = "^0.27.4"
 tiktoken = "^0.3.3"
 requests = "^2.29.0"
+loguru = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 pre-commit = "^2.18.1"
 pytest-cov = "^3.0.0"
 flake8 = "^4.0.1"
 pdoc3 = "^0.10.0"
```

### Comparing `llm_bot-0.1.2/PKG-INFO` & `llm_bot-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: langchain (>=0.0.224,<0.0.225)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Project-URL: Repository, https://github.com/prefeitura-rio/chatbot-lab
 Description-Content-Type: text/markdown
 
 # Python Project Template
```

