# Comparing `tmp/biochatter-0.1.3.tar.gz` & `tmp/biochatter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biochatter-0.1.3.tar", max compression
+gzip compressed data, was "biochatter-0.1.4.tar", max compression
```

## Comparing `biochatter-0.1.3.tar` & `biochatter-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.3/LICENSE
--rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.3/biochatter/__init__.py
--rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.3/biochatter/_stats.py
--rw-r--r--   0        0        0    17960 2023-07-03 22:09:12.868928 biochatter-0.1.3/biochatter/llm_connect.py
--rw-r--r--   0        0        0     5226 2023-06-16 12:53:15.891015 biochatter-0.1.3/biochatter/vectorstore.py
--rw-r--r--   0        0        0      667 2023-07-03 15:05:25.410204 biochatter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 biochatter-0.1.3/setup.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 biochatter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.4/LICENSE
+-rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.4/biochatter/__init__.py
+-rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.4/biochatter/_stats.py
+-rw-r--r--   0        0        0    18229 2023-07-06 14:40:38.478751 biochatter-0.1.4/biochatter/llm_connect.py
+-rw-r--r--   0        0        0     5839 2023-07-06 14:40:38.478959 biochatter-0.1.4/biochatter/podcast.py
+-rw-r--r--   0        0        0     5788 2023-07-06 14:40:38.479205 biochatter-0.1.4/biochatter/vectorstore.py
+-rw-r--r--   0        0        0      740 2023-07-06 14:40:38.480642 biochatter-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 biochatter-0.1.4/setup.py
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 biochatter-0.1.4/PKG-INFO
```

### Comparing `biochatter-0.1.3/LICENSE` & `biochatter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.3/biochatter/_stats.py` & `biochatter-0.1.4/biochatter/_stats.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.3/biochatter/llm_connect.py` & `biochatter-0.1.4/biochatter/llm_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,22 @@
 
     """
 
     def __init__(
         self,
         model_name: str,
         prompts: dict,
+        correct: bool = True,
         split_correction: bool = False,
         docsum: DocumentEmbedder = None,
     ):
         super().__init__()
         self.model_name = model_name
         self.prompts = prompts
+        self.correct = correct
         self.split_correction = split_correction
         self.docsum = docsum
         self.history = []
         self.messages = []
         self.ca_messages = []
         self.current_statements = []
 
@@ -159,14 +161,17 @@
 
         msg, token_usage = self._primary_query()
 
         if not token_usage:
             # indicates error
             return (msg, token_usage, None)
 
+        if not self.correct:
+            return (msg, token_usage, "OK")
+
         cor_msg = (
             "Correcting (using single sentences) ..."
             if self.split_correction
             else "Correcting ..."
         )
 
         if st:
@@ -288,15 +293,16 @@
 
 
 class GptConversation(Conversation):
     def __init__(
         self,
         model_name: str,
         prompts: dict,
-        split_correction: bool,
+        correct: bool = True,
+        split_correction: bool = False,
         docsum: DocumentEmbedder = None,
     ):
         """
         Connect to OpenAI's GPT API and set up a conversation with the user.
         Also initialise a second conversational agent to provide corrections to
         the model output, if necessary.
 
@@ -311,14 +317,15 @@
 
             docsum (DocumentEmbedder): A document summariser to use for
                 document summarisation.
         """
         super().__init__(
             model_name=model_name,
             prompts=prompts,
+            correct=correct,
             split_correction=split_correction,
             docsum=docsum,
         )
 
         self.ca_model_name = "gpt-3.5-turbo"
         # TODO make accessible by drop-down
 
@@ -440,15 +447,16 @@
 
 class AzureGptConversation(GptConversation):
     def __init__(
         self,
         deployment_name: str,
         model_name: str,
         prompts: dict,
-        split_correction: bool,
+        correct: bool = True,
+        split_correction: bool = False,
         docsum: DocumentEmbedder = None,
         version: Optional[str] = None,
         base: Optional[str] = None,
     ):
         """
         Connect to Azure's GPT API and set up a conversation with the user.
         Extends GptConversation.
@@ -471,14 +479,15 @@
             version (str): The version of the Azure API to use.
 
             base (str): The base URL of the Azure API to use.
         """
         super().__init__(
             model_name=model_name,
             prompts=prompts,
+            correct=correct,
             split_correction=split_correction,
             docsum=docsum,
         )
 
         self.version = version
         self.base = base
         self.deployment_name = deployment_name
```

### Comparing `biochatter-0.1.3/biochatter/vectorstore.py` & `biochatter-0.1.4/biochatter/vectorstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,42 +67,16 @@
     def set_separators(self, separators: list) -> None:
         self.separators = separators
 
     def set_document(self, document: List[Document]) -> None:
         self.document = document
 
     def _load_document(self, path: str) -> None:
-        """
-        Loads a document from a path; accepts txt and pdf files. Txt files are
-        loaded as-is, pdf files are converted to text using fitz.
-
-        Args:
-            path (str): path to document
-
-        Returns:
-            List[Document]: list of documents
-        """
-        if path.endswith(".txt"):
-            loader = TextLoader(path)
-            self.document = loader.load()
-        elif path.endswith(".pdf"):
-            doc = fitz.open(path)
-            text = ""
-            for page in doc:
-                text += page.get_text()
-
-            meta = {k: v for k, v in doc.metadata.items() if v}
-            meta.update({"source": path})
-
-            self.document = [
-                Document(
-                    page_content=text,
-                    metadata=meta,
-                )
-            ]
+        reader = DocumentReader()
+        self.document = reader.load_document(path)
 
     def split_document(self) -> None:
         text_splitter = RecursiveCharacterTextSplitter(
             chunk_size=self.chunk_size,
             chunk_overlap=self.chunk_overlap,
             separators=self.separators,
         )
@@ -135,40 +109,83 @@
             return self.vector_db.similarity_search(
                 query=query, k=k or self.n_results
             )
         else:
             raise NotImplementedError(self.vector_db_vendor)
 
 
-def document_from_pdf(pdf) -> List[Document]:
-    """
-    Receive a byte representation of a pdf file and return a list of Documents
-    with metadata.
-    """
-    doc = fitz.open(stream=pdf, filetype="pdf")
-    text = ""
-    for page in doc:
-        text += page.get_text()
-
-    meta = {k: v for k, v in doc.metadata.items() if v}
-    meta.update({"source": "pdf"})
-
-    return [
-        Document(
-            page_content=text,
-            metadata=meta,
-        )
-    ]
+class DocumentReader:
+    def load_document(self, path: str) -> List[Document]:
+        """
+        Loads a document from a path; accepts txt and pdf files. Txt files are
+        loaded as-is, pdf files are converted to text using fitz.
 
+        Args:
+            path (str): path to document
 
-def document_from_txt(txt) -> List[Document]:
-    """
-    Receive a byte representation of a txt file and return a list of Documents
-    with metadata.
-    """
-    meta = {"source": "txt"}
-    return [
-        Document(
-            page_content=txt,
-            metadata=meta,
-        )
-    ]
+        Returns:
+            List[Document]: list of documents
+        """
+        if path.endswith(".txt"):
+            loader = TextLoader(path)
+            return loader.load()
+
+        elif path.endswith(".pdf"):
+            doc = fitz.open(path)
+            text = ""
+            for page in doc:
+                text += page.get_text()
+
+            meta = {k: v for k, v in doc.metadata.items() if v}
+            meta.update({"source": path})
+
+            return [
+                Document(
+                    page_content=text,
+                    metadata=meta,
+                )
+            ]
+
+    def document_from_pdf(self, pdf: bytes) -> List[Document]:
+        """
+        Receive a byte representation of a pdf file and return a list of Documents
+        with metadata.
+
+        Args:
+            pdf (bytes): byte representation of pdf file
+
+        Returns:
+            List[Document]: list of documents
+        """
+        doc = fitz.open(stream=pdf, filetype="pdf")
+        text = ""
+        for page in doc:
+            text += page.get_text()
+
+        meta = {k: v for k, v in doc.metadata.items() if v}
+        meta.update({"source": "pdf"})
+
+        return [
+            Document(
+                page_content=text,
+                metadata=meta,
+            )
+        ]
+
+    def document_from_txt(self, txt: bytes) -> List[Document]:
+        """
+        Receive a byte representation of a txt file and return a list of Documents
+        with metadata.
+
+        Args:
+            txt (bytes): byte representation of txt file
+
+        Returns:
+            List[Document]: list of documents
+        """
+        meta = {"source": "txt"}
+        return [
+            Document(
+                page_content=txt,
+                metadata=meta,
+            )
+        ]
```

### Comparing `biochatter-0.1.3/pyproject.toml` & `biochatter-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "biochatter"
-version = "0.1.3"
+version = "0.1.4"
 description = "Backend library for conversational AI in biomedicine"
 authors = ["Sebastian Lobentanzer <sebastian.lobentanzer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.12"
 langchain = "^0.0.146"
 openai = "^0.27.8"
 pymupdf = "^1.22.3"
 pymilvus = "2.2.8"
 tiktoken = "^0.4.0"
 nltk = "^3.8.1"
 redis = "^4.5.5"
 retry = "^0.9.2"
 streamlit = { version = "^1.23.1", optional = true }
+gTTS = { version = "^2.3.2", optional = true }
 
 [tool.poetry.extras]
 streamlit = ["streamlit"]
+podcast = ["gTTS"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `biochatter-0.1.3/setup.py` & `biochatter-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,28 +14,28 @@
  'pymilvus==2.2.8',
  'pymupdf>=1.22.3,<2.0.0',
  'redis>=4.5.5,<5.0.0',
  'retry>=0.9.2,<0.10.0',
  'tiktoken>=0.4.0,<0.5.0']
 
 extras_require = \
-{'streamlit': ['streamlit>=1.23.1,<2.0.0']}
+{'podcast': ['gTTS>=2.3.2,<3.0.0'], 'streamlit': ['streamlit>=1.23.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'biochatter',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Backend library for conversational AI in biomedicine',
     'long_description': '# biochatter\nThis repository contains the `biochatter` Python package, a generic backend library for the connection of biomedical applications to conversational AI. Used in [ChatGSE](https://chat.biocypher.org), which is being developed at https://github.com/biocypher/ChatGSE. More to come, so stay tuned!\n\n## Installation\nTo use the package, install it from PyPI, for instance using pip (`pip install biochatter`) or Poetry (`poetry add biochatter`).\n',
     'author': 'Sebastian Lobentanzer',
     'author_email': 'sebastian.lobentanzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.10,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `biochatter-0.1.3/PKG-INFO` & `biochatter-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: biochatter
-Version: 0.1.3
+Version: 0.1.4
 Summary: Backend library for conversational AI in biomedicine
 License: MIT
 Author: Sebastian Lobentanzer
 Author-email: sebastian.lobentanzer@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: podcast
 Provides-Extra: streamlit
+Requires-Dist: gTTS (>=2.3.2,<3.0.0); extra == "podcast"
 Requires-Dist: langchain (>=0.0.146,<0.0.147)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pymilvus (==2.2.8)
 Requires-Dist: pymupdf (>=1.22.3,<2.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
```

