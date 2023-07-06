# Comparing `tmp/cybrex-1.0.3.tar.gz` & `tmp/cybrex-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.0.3.tar", last modified: Wed Jul  5 20:45:21 2023, max compression
+gzip compressed data, was "cybrex-1.0.4.tar", last modified: Thu Jul  6 09:55:58 2023, max compression
```

## Comparing `cybrex-1.0.3.tar` & `cybrex-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 20:45:21.433070 cybrex-1.0.3/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.3/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-05 20:45:21.432873 cybrex-1.0.3/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      943 2023-07-05 20:42:40.000000 cybrex-1.0.3/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 20:45:21.431115 cybrex-1.0.3/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)     1300 2023-07-05 20:29:36.000000 cybrex-1.0.3/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     5727 2023-07-05 20:29:36.000000 cybrex-1.0.3/cybrex/cybrex_ai.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 20:45:21.432564 cybrex-1.0.3/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-05 20:45:21.000000 cybrex-1.0.3/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-05 20:45:21.000000 cybrex-1.0.3/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-05 20:45:21.000000 cybrex-1.0.3/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-05 20:45:21.000000 cybrex-1.0.3/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-05 20:45:21.000000 cybrex-1.0.3/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-05 20:45:21.000000 cybrex-1.0.3/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-05 20:44:54.000000 cybrex-1.0.3/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-05 19:35:09.000000 cybrex-1.0.3/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-05 20:45:21.433145 cybrex-1.0.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:55:58.437226 cybrex-1.0.4/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.4/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:55:58.436953 cybrex-1.0.4/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      943 2023-07-05 20:42:40.000000 cybrex-1.0.4/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:55:58.433940 cybrex-1.0.4/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)     1298 2023-07-06 09:55:22.000000 cybrex-1.0.4/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5805 2023-07-06 09:55:22.000000 cybrex-1.0.4/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:55:58.436432 cybrex-1.0.4/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-06 09:55:12.000000 cybrex-1.0.4/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-05 19:35:09.000000 cybrex-1.0.4/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 09:55:58.437347 cybrex-1.0.4/setup.cfg
```

### Comparing `cybrex-1.0.3/PKG-INFO` & `cybrex-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.3
+Version: 1.0.4
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.0.3/README.md` & `cybrex-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.0.3/cybrex/cli.py` & `cybrex-1.0.4/cybrex/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import fire
+from cybrex_ai import CybrexAI
 from termcolor import colored
 
-from .cybrex_ai import CybrexAI
-
 
 class CybrexCli:
     def __init__(self):
         self.cybrex = CybrexAI()
 
     async def chat_doc(self, doi: str, question: str):
         """
```

### Comparing `cybrex-1.0.3/cybrex/cybrex_ai.py` & `cybrex-1.0.4/cybrex/cybrex_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import io
 import os.path
 import uuid
-from typing import List, Optional
+from typing import (
+    List,
+    Optional,
+)
 
 import chromadb
 import pypdf
 import yaml
 from aiokit import AioThing
 from izihawa_configurator import Configurator
 from izihawa_utils.exceptions import BaseError
@@ -89,15 +93,15 @@
             self.starts.append(self.geck)
 
     async def resolve_document_content(self, document: dict) -> Optional[str]:
         if 'content' in document:
             return document['content']
         elif 'links' in document:
             pdf_file = await self.geck.download(document['links'][0]['cid'])
-            pdf_reader = pypdf.PdfReader(pdf_file)
+            pdf_reader = pypdf.PdfReader(io.BytesIO(pdf_file))
             return '\n'.join(page.extract_text() for page in pdf_reader.pages)
 
     async def add_documents(self, documents: List[dict]):
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=300)
 
         metadatas = []
         texts = []
@@ -128,24 +132,25 @@
     async def summarize_document(self, doi):
         documents = await self.add_document_by_doi(doi)
         chain = load_summarize_chain(llm=OpenAI(), chain_type="map_reduce")
         result = chain.run(documents)
         return result.strip()
 
     async def add_document_by_doi(self, doi) -> List[Document]:
-        if not self.collection.get(where={'doi': doi}):
+        if not self.collection.get(where={'doi': doi})['documents']:
             documents = await self.geck.get_summa_client().search_documents([{
                 'index_alias': 'nexus_science',
                 'collectors': [{'top_docs': {'limit': 1}}],
                 'query': {'term': {'field': 'doi', 'value': doi}}
             }])
             if not documents:
                 raise DocumentNotFoundError(doi=doi)
             await self.add_documents(documents)
-        return [Document(page_content=text) for text in self.collection.get(where={'doi': doi})['documents']]
+        documents = [Document(page_content=text) for text in self.collection.get(where={'doi': doi})['documents']]
+        return documents
 
     async def add_document_by_topic(self, topic):
         documents = await get_documents_on_topic(summa_client=self.geck.get_summa_client(), topic=topic, documents=20)
         return await self.add_documents(documents)
 
     def as_retriever(self, **kwargs):
         chroma = Chroma(
```

### Comparing `cybrex-1.0.3/cybrex.egg-info/PKG-INFO` & `cybrex-1.0.4/cybrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.3
+Version: 1.0.4
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.0.3/pyproject.toml` & `cybrex-1.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.0.3"
+version = "1.0.4"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

