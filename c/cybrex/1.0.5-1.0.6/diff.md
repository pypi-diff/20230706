# Comparing `tmp/cybrex-1.0.5.tar.gz` & `tmp/cybrex-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.0.5.tar", last modified: Thu Jul  6 09:59:08 2023, max compression
+gzip compressed data, was "cybrex-1.0.6.tar", last modified: Thu Jul  6 11:34:35 2023, max compression
```

## Comparing `cybrex-1.0.5.tar` & `cybrex-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:59:08.525329 cybrex-1.0.5/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.5/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:59:08.525057 cybrex-1.0.5/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      943 2023-07-05 20:42:40.000000 cybrex-1.0.5/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:59:08.522411 cybrex-1.0.5/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)     1300 2023-07-06 09:58:52.000000 cybrex-1.0.5/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     5805 2023-07-06 09:55:22.000000 cybrex-1.0.5/cybrex/cybrex_ai.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:59:08.524502 cybrex-1.0.5/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-06 09:58:58.000000 cybrex-1.0.5/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-05 19:35:09.000000 cybrex-1.0.5/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 09:59:08.525436 cybrex-1.0.5/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 11:34:35.071650 cybrex-1.0.6/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.6/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 11:34:35.071407 cybrex-1.0.6/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      943 2023-07-05 20:42:40.000000 cybrex-1.0.6/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 11:34:35.068656 cybrex-1.0.6/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)     3149 2023-07-06 11:33:57.000000 cybrex-1.0.6/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6799 2023-07-06 11:32:50.000000 cybrex-1.0.6/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 11:34:35.070965 cybrex-1.0.6/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 11:34:35.000000 cybrex-1.0.6/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-06 11:34:35.000000 cybrex-1.0.6/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 11:34:35.000000 cybrex-1.0.6/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 11:34:35.000000 cybrex-1.0.6/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-06 11:34:35.000000 cybrex-1.0.6/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-06 11:34:35.000000 cybrex-1.0.6/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-06 10:24:08.000000 cybrex-1.0.6/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-06 11:34:18.000000 cybrex-1.0.6/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 11:34:35.071738 cybrex-1.0.6/setup.cfg
```

### Comparing `cybrex-1.0.5/PKG-INFO` & `cybrex-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.5
+Version: 1.0.6
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.0.5/README.md` & `cybrex-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.0.5/cybrex/cybrex_ai.py` & `cybrex-1.0.6/cybrex/cybrex_ai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import io
+import logging
 import os.path
 import uuid
 from typing import (
     List,
     Optional,
 )
 
@@ -103,57 +104,79 @@
     async def add_documents(self, documents: List[dict]):
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=300)
 
         metadatas = []
         texts = []
 
         for document in documents:
+            if self.collection.get(where={'doi': document['doi']})['documents']:
+                logging.getLogger('statbox').info({
+                    'action': 'already_stored',
+                    'doi': document['doi'],
+                })
+                continue
+            logging.getLogger('statbox').info({
+                'action': 'retrieve_content',
+                'doi': document['doi'],
+            })
             content = await self.resolve_document_content(document)
             if not content:
                 continue
+            logging.getLogger('statbox').info({
+                'action': 'chunking',
+                'doi': document['doi'],
+            })
             for chunk_id, chunk in enumerate(text_splitter.split_text(content)):
                 metadatas.append({'doi': document['doi'], 'chunk_id': chunk_id})
                 texts.append(chunk)
+        if texts:
+            return self.collection.upsert(
+                documents=texts,
+                metadatas=metadatas,
+                ids=[str(uuid.uuid1()) for _ in range(len(texts))]
+            )
 
-        return self.collection.upsert(
-            documents=texts,
-            metadatas=metadatas,
-            ids=[str(uuid.uuid1()) for _ in range(len(texts))]
-        )
-
-    async def chat_document(self, doi, question):
+    async def chat_document(self, doi, question, k):
         await self.add_document_by_doi(doi)
-        qa = RetrievalQA.from_chain_type(llm=OpenAI(), chain_type='stuff', retriever=self.as_retriever(
+        qa = RetrievalQA.from_chain_type(llm=OpenAI(), chain_type='map_reduce', retriever=self.as_retriever(
             search_type='similarity',
-            search_kwargs={'k': 3, 'filter': {'doi': doi}},
+            search_kwargs={'k': k, 'filter': {'doi': doi}},
         ))
         result = qa({"query": question})
         return result["result"].strip()
 
+    async def chat_science(self, topic, question, llm_documents, summa_documents):
+        await self.add_document_by_topic(topic, summa_documents)
+        qa = RetrievalQA.from_chain_type(llm=OpenAI(), chain_type='map_reduce', retriever=self.as_retriever(
+            search_type='similarity',
+            search_kwargs={'k': llm_documents},
+        ), return_source_documents=True)
+        result = qa({"query": question})
+        return result
+
     async def summarize_document(self, doi):
         documents = await self.add_document_by_doi(doi)
         chain = load_summarize_chain(llm=OpenAI(), chain_type="map_reduce")
         result = chain.run(documents)
         return result.strip()
 
     async def add_document_by_doi(self, doi) -> List[Document]:
-        if not self.collection.get(where={'doi': doi})['documents']:
-            documents = await self.geck.get_summa_client().search_documents([{
-                'index_alias': 'nexus_science',
-                'collectors': [{'top_docs': {'limit': 1}}],
-                'query': {'term': {'field': 'doi', 'value': doi}}
-            }])
-            if not documents:
-                raise DocumentNotFoundError(doi=doi)
-            await self.add_documents(documents)
+        documents = await self.geck.get_summa_client().search_documents([{
+            'index_alias': 'nexus_science',
+            'collectors': [{'top_docs': {'limit': 1}}],
+            'query': {'term': {'field': 'doi', 'value': doi}}
+        }])
+        if not documents:
+            raise DocumentNotFoundError(doi=doi)
+        await self.add_documents(documents)
         documents = [Document(page_content=text) for text in self.collection.get(where={'doi': doi})['documents']]
         return documents
 
-    async def add_document_by_topic(self, topic):
-        documents = await get_documents_on_topic(summa_client=self.geck.get_summa_client(), topic=topic, documents=20)
+    async def add_document_by_topic(self, topic: str, documents: int):
+        documents = await get_documents_on_topic(summa_client=self.geck.get_summa_client(), topic=topic, documents=documents)
         return await self.add_documents(documents)
 
     def as_retriever(self, **kwargs):
         chroma = Chroma(
             client=self.db,
             collection_name=self.collection_name,
             persist_directory=self.home_path,
```

### Comparing `cybrex-1.0.5/cybrex.egg-info/PKG-INFO` & `cybrex-1.0.6/cybrex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.5
+Version: 1.0.6
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.0.5/pyproject.toml` & `cybrex-1.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.0.5"
+version = "1.0.6"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

