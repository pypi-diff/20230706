# Comparing `tmp/llm_inference-0.0.4.tar.gz` & `tmp/llm_inference-0.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_inference-0.0.4.tar", last modified: Tue Jul  4 22:45:07 2023, max compression
+gzip compressed data, was "llm_inference-0.0.5.dev0.tar", last modified: Thu Jul  6 00:56:35 2023, max compression
```

## Comparing `llm_inference-0.0.4.tar` & `llm_inference-0.0.5.dev0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-04 22:44:56.000000 llm_inference-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-04 22:44:56.000000 llm_inference-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 22:44:56.000000 llm_inference-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-04 22:44:56.000000 llm_inference-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-04 22:45:07.874839 llm_inference-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-04 22:44:56.000000 llm_inference-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.870839 llm_inference-0.0.4/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   399922 2023-07-04 22:44:56.000000 llm_inference-0.0.4/assets/llama-inference-api-min.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-04 22:44:56.000000 llm_inference-0.0.4/requirements/chatbot.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 22:44:56.000000 llm_inference-0.0.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-04 22:45:07.878839 llm_inference-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-04 22:44:56.000000 llm_inference-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.870839 llm_inference-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/chatbot/ui/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/ui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/chatbot/ui/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/llm_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/llm_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/llm_inference/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-04 22:44:56.000000 llm_inference-0.0.4/src/llm_inference/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:45:07.874839 llm_inference-0.0.4/src/llm_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 22:45:07.000000 llm_inference-0.0.4/src/llm_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   399922 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/assets/llama-inference-api-min.png
+-rw-r--r--   0 runner    (1001) docker     (123)   395880 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/assets/llm-inference-min.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/llm_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 00:56:35.000000 llm_inference-0.0.5.dev0/llm_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.921806 llm_inference-0.0.5.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/src/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/src/chatbot/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/chatbot/ui/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:56:35.925806 llm_inference-0.0.5.dev0/src/llm_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 00:56:27.000000 llm_inference-0.0.5.dev0/src/llm_inference/serve.py
```

### Comparing `llm_inference-0.0.4/CODE_OF_CONDUCT.md` & `llm_inference-0.0.5.dev0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.4/CONTRIBUTING.md` & `llm_inference-0.0.5.dev0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.4/LICENSE` & `llm_inference-0.0.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.4/MANIFEST.in` & `llm_inference-0.0.5.dev0/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 # Exclude the documentation files
 recursive-exclude docs *
 exclude docs
 
 # Include the Requirements
 include requirements/requirements.txt
-include requirements/chatbot.txt
-recursive-include requirements/requirements *.txt
+recursive-include requirements/ *.txt
 
 # Exclude Makefile
 exclude Makefile
 
 prune .git
 prune .github
 prune scripts
```

### Comparing `llm_inference-0.0.4/PKG-INFO` & `llm_inference-0.0.5.dev0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 Metadata-Version: 2.1
 Name: llm_inference
-Version: 0.0.4
+Version: 0.0.5.dev0
 Summary: Large Language Models Inference API and Applications
 Home-page: https://github.com/aniketmaurya/llm-inference
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT,Falcon
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: chatbot
+Provides-Extra: dev
 License-File: LICENSE
 
 # Large Language Model (LLM) Inference API and Chatbot 🦙
 
-![project banner](https://github.com/aniketmaurya/LLaMA-Inference-API/raw/main/assets/llama-inference-api-min.png)
+![project banner](https://github.com/aniketmaurya/llm-inference/raw/main/assets/llm-inference-min.png)
 
-Inference API for LLaMA
+Inference API for LLMs like LLaMA and Falcon powered by Lit-GPT from [Lightning AI](https://lightning.ai)
 
 ```
 pip install llm-inference
-
-# to use chatbot
-pip install llm-inference[chatbot]
 ```
 
 ### Install from main branch
 ```bash
 pip install git+https://github.com/aniketmaurya/llm-inference.git@main
 ```
 
 > **Note**: You need to manually install [Lit-GPT](https://github.com/Lightning-AI/lit-gpt) and setup the model weights to use this project.
 
 ```
-pip install lit-gpt@git+https://github.com/Lightning-AI/lit-gpt.git@main
+pip install lit_gpt@git+https://github.com/aniketmaurya/install-lit-gpt.git@install
 ```
 
-
 ## For Inference
 
 ```python
-from llm_inference import LLMInference
-import os
-
-WEIGHTS_PATH = os.environ["WEIGHTS"]
-
-checkpoint_dir = f"checkpoints/tiiuae/falcon-7b"
+from llm_inference import LLMInference, prepare_weights
+from rich import print
 
-model = LLMInference(checkpoint_dir=checkpoint_dir, precision="bf16-true")
+path = prepare_weights("EleutherAI/pythia-70m")
+model = LLMInference(checkpoint_dir=path)
 
 print(model("New York is located in"))
 ```
 
 
 ## For deploying as a REST API
 
@@ -70,16 +63,16 @@
 ```bash
 lightning run app app.py
 ```
 
 ## How to use the Chatbot
 
 ```python
-from chatbot import LLaMAChatBot
+from chatbot import LitGPTChatBot
 
 checkpoint_dir = "weights"
 
-bot = LLaMAChatBot(
+bot = LitGPTChatBot(
     checkpoint_dir=checkpoint_dir)
 
 print(bot.send("hi, what is the capital of France?"))
 ```
```

### Comparing `llm_inference-0.0.4/README.md` & `llm_inference-0.0.5.dev0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 # Large Language Model (LLM) Inference API and Chatbot 🦙
 
-![project banner](https://github.com/aniketmaurya/LLaMA-Inference-API/raw/main/assets/llama-inference-api-min.png)
+![project banner](https://github.com/aniketmaurya/llm-inference/raw/main/assets/llm-inference-min.png)
 
-Inference API for LLaMA
+Inference API for LLMs like LLaMA and Falcon powered by Lit-GPT from [Lightning AI](https://lightning.ai)
 
 ```
 pip install llm-inference
-
-# to use chatbot
-pip install llm-inference[chatbot]
 ```
 
 ### Install from main branch
 ```bash
 pip install git+https://github.com/aniketmaurya/llm-inference.git@main
 ```
 
 > **Note**: You need to manually install [Lit-GPT](https://github.com/Lightning-AI/lit-gpt) and setup the model weights to use this project.
 
 ```
-pip install lit-gpt@git+https://github.com/Lightning-AI/lit-gpt.git@main
+pip install lit_gpt@git+https://github.com/aniketmaurya/install-lit-gpt.git@install
 ```
 
-
 ## For Inference
 
 ```python
-from llm_inference import LLMInference
-import os
-
-WEIGHTS_PATH = os.environ["WEIGHTS"]
-
-checkpoint_dir = f"checkpoints/tiiuae/falcon-7b"
+from llm_inference import LLMInference, prepare_weights
+from rich import print
 
-model = LLMInference(checkpoint_dir=checkpoint_dir, precision="bf16-true")
+path = prepare_weights("EleutherAI/pythia-70m")
+model = LLMInference(checkpoint_dir=path)
 
 print(model("New York is located in"))
 ```
 
 
 ## For deploying as a REST API
 
@@ -56,16 +49,16 @@
 ```bash
 lightning run app app.py
 ```
 
 ## How to use the Chatbot
 
 ```python
-from chatbot import LLaMAChatBot
+from chatbot import LitGPTChatBot
 
 checkpoint_dir = "weights"
 
-bot = LLaMAChatBot(
+bot = LitGPTChatBot(
     checkpoint_dir=checkpoint_dir)
 
 print(bot.send("hi, what is the capital of France?"))
 ```
```

### Comparing `llm_inference-0.0.4/assets/llama-inference-api-min.png` & `llm_inference-0.0.5.dev0/assets/llama-inference-api-min.png`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.4/src/chatbot/base.py` & `llm_inference-0.0.5.dev0/src/chatbot/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "Dummy LLM"
 
 
-class LLaMALLM(LLM, BaseModel):
+class LitGPTLLM(LLM, BaseModel):
     checkpoint_dir: str = ""
     model: Any = None
 
     def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
         if not self.model:
             self.model = LLMInference(
                 checkpoint_dir=self.checkpoint_dir,
@@ -37,28 +37,32 @@
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "Lit-GPT LLM"
 
 
 class ServerLLM(LLM, BaseModel):
     url: str = ""
+    TIMEOUT: float = 60.0
 
     def _call(self, prompt: str, stop: Optional[list[str]] = None) -> str:
         """Run the LLM on the given prompt and input."""
         if self.url == "":
             raise Exception("Server URL not set!")
 
         headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
         }
         assert isinstance(prompt, str)
         json_data = {"prompt": prompt}
         response = requests.post(
-            url=self.url + "/predict", headers=headers, json=json_data
+            url=self.url + "/predict",
+            headers=headers,
+            json=json_data,
+            timeout=self.TIMEOUT,
         )
         logger.error(response.raise_for_status())
         return response.json()["result"]
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
```

### Comparing `llm_inference-0.0.4/src/chatbot/chain.py` & `llm_inference-0.0.5.dev0/src/chatbot/chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Wrapper around Lightning App."""
 import logging
 from collections import deque
 
 from langchain.chains import ConversationChain
 from langchain.chains.conversation.memory import ConversationSummaryBufferMemory
 
-from .base import DummyLLM, LLaMALLM, ServerLLM
+from .base import DummyLLM, LitGPTLLM, ServerLLM
 
 logger = logging.getLogger(__name__)
 
 
 def build_server_chain(
     url: str, input_key: str = "input", output_key: str = "response"
 ) -> ConversationChain:
@@ -67,11 +67,11 @@
     def __init__(
         self, url: str, input_key="input", output_key="response", verbose=False
     ) -> None:
         llm = ServerLLM(url=url)
         super().__init__(llm, input_key, output_key, verbose)
 
 
-class LLaMAChatBot(BaseChatBot):
+class LitGPTChatBot(BaseChatBot):
     def __init__(self, checkpoint_dir: str, verbose=False) -> None:
-        llm = LLaMALLM(checkpoint_dir=checkpoint_dir)
+        llm = LitGPTLLM(checkpoint_dir=checkpoint_dir)
         super().__init__(llm=llm, verbose=verbose)
```

### Comparing `llm_inference-0.0.4/src/chatbot/ui/main.py` & `llm_inference-0.0.5.dev0/src/chatbot/ui/main.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.4/src/chatbot/ui/templates.py` & `llm_inference-0.0.5.dev0/src/chatbot/ui/templates.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.4/src/llm_inference/model.py` & `llm_inference-0.0.5.dev0/src/llm_inference/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,14 @@
         if idx_next == eos_id:
             return idx[:input_pos]  # include the EOS token
 
     return idx
 
 
 class LLMInference:
-    INSTRUCTION_TUNED: bool = False
-
     def __init__(
         self,
         checkpoint_dir: Path = Path(f"checkpoints/tiiuae/falcon-7b"),
         quantize: Literal["llm.int8", "gptq.int4"] = None,
         accelerator: str = "auto",
         strategy: str = "auto",
         devices: int = 1,
@@ -161,15 +159,15 @@
                 checkpoint_path=checkpoint_path, adapter_path=adapter_path
             )
 
         else:
             model = self.load_model(checkpoint_path=checkpoint_path)
 
         model.eval()
-        self.model = model = fabric.setup_module(model)
+        self.model = fabric.setup_module(model)
         self.tokenizer = Tokenizer(checkpoint_dir)
 
     def __call__(
         self,
         prompt: str,
         max_new_tokens: int = 100,
         top_k: int = 200,
```

### Comparing `llm_inference-0.0.4/src/llm_inference/serve.py` & `llm_inference-0.0.5.dev0/src/llm_inference/serve.py`

 * *Files identical despite different names*

### Comparing `llm_inference-0.0.4/src/llm_inference.egg-info/PKG-INFO` & `llm_inference-0.0.5.dev0/llm_inference.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 Metadata-Version: 2.1
 Name: llm-inference
-Version: 0.0.4
+Version: 0.0.5.dev0
 Summary: Large Language Models Inference API and Applications
 Home-page: https://github.com/aniketmaurya/llm-inference
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT,Falcon
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: chatbot
+Provides-Extra: dev
 License-File: LICENSE
 
 # Large Language Model (LLM) Inference API and Chatbot 🦙
 
-![project banner](https://github.com/aniketmaurya/LLaMA-Inference-API/raw/main/assets/llama-inference-api-min.png)
+![project banner](https://github.com/aniketmaurya/llm-inference/raw/main/assets/llm-inference-min.png)
 
-Inference API for LLaMA
+Inference API for LLMs like LLaMA and Falcon powered by Lit-GPT from [Lightning AI](https://lightning.ai)
 
 ```
 pip install llm-inference
-
-# to use chatbot
-pip install llm-inference[chatbot]
 ```
 
 ### Install from main branch
 ```bash
 pip install git+https://github.com/aniketmaurya/llm-inference.git@main
 ```
 
 > **Note**: You need to manually install [Lit-GPT](https://github.com/Lightning-AI/lit-gpt) and setup the model weights to use this project.
 
 ```
-pip install lit-gpt@git+https://github.com/Lightning-AI/lit-gpt.git@main
+pip install lit_gpt@git+https://github.com/aniketmaurya/install-lit-gpt.git@install
 ```
 
-
 ## For Inference
 
 ```python
-from llm_inference import LLMInference
-import os
-
-WEIGHTS_PATH = os.environ["WEIGHTS"]
-
-checkpoint_dir = f"checkpoints/tiiuae/falcon-7b"
+from llm_inference import LLMInference, prepare_weights
+from rich import print
 
-model = LLMInference(checkpoint_dir=checkpoint_dir, precision="bf16-true")
+path = prepare_weights("EleutherAI/pythia-70m")
+model = LLMInference(checkpoint_dir=path)
 
 print(model("New York is located in"))
 ```
 
 
 ## For deploying as a REST API
 
@@ -70,16 +63,16 @@
 ```bash
 lightning run app app.py
 ```
 
 ## How to use the Chatbot
 
 ```python
-from chatbot import LLaMAChatBot
+from chatbot import LitGPTChatBot
 
 checkpoint_dir = "weights"
 
-bot = LLaMAChatBot(
+bot = LitGPTChatBot(
     checkpoint_dir=checkpoint_dir)
 
 print(bot.send("hi, what is the capital of France?"))
 ```
```

### Comparing `llm_inference-0.0.4/src/llm_inference.egg-info/SOURCES.txt` & `llm_inference-0.0.5.dev0/llm_inference.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 assets/llama-inference-api-min.png
-requirements/chatbot.txt
+assets/llm-inference-min.png
+llm_inference.egg-info/PKG-INFO
+llm_inference.egg-info/SOURCES.txt
+llm_inference.egg-info/dependency_links.txt
+llm_inference.egg-info/requires.txt
+llm_inference.egg-info/top_level.txt
+requirements/dev.txt
 requirements/requirements.txt
 src/chatbot/__init__.py
 src/chatbot/base.py
 src/chatbot/chain.py
 src/chatbot/ui/__init__.py
 src/chatbot/ui/main.py
 src/chatbot/ui/templates.py
 src/llm_inference/__init__.py
+src/llm_inference/download.py
 src/llm_inference/model.py
-src/llm_inference/serve.py
-src/llm_inference.egg-info/PKG-INFO
-src/llm_inference.egg-info/SOURCES.txt
-src/llm_inference.egg-info/dependency_links.txt
-src/llm_inference.egg-info/requires.txt
-src/llm_inference.egg-info/top_level.txt
+src/llm_inference/serve.py
```

