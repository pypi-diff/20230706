# Comparing `tmp/text2text-1.2.0.tar.gz` & `tmp/text2text-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.2.0.tar", last modified: Mon Jul  3 04:34:30 2023, max compression
+gzip compressed data, was "text2text-1.2.1.tar", last modified: Thu Jul  6 02:17:45 2023, max compression
```

## Comparing `text2text-1.2.0.tar` & `text2text-1.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:34:30.318968 text2text-1.2.0/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-07-03 03:29:27.000000 text2text-1.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    56262 2023-07-03 04:34:30.317968 text2text-1.2.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    55448 2023-07-03 03:29:27.000000 text2text-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 04:34:30.318968 text2text-1.2.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-07-03 04:33:50.000000 text2text-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:34:30.314967 text2text-1.2.0/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      603 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:34:30.316967 text2text-1.2.0/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-07-03 04:28:59.000000 text2text-1.2.0/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:34:30.317968 text2text-1.2.0/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-03 03:29:27.000000 text2text-1.2.0/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-07-03 04:32:53.000000 text2text-1.2.0/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:34:30.315967 text2text-1.2.0/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    56262 2023-07-03 04:34:30.000000 text2text-1.2.0/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2023-07-03 04:34:30.000000 text2text-1.2.0/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 04:34:30.000000 text2text-1.2.0/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-03 04:34:30.000000 text2text-1.2.0/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 04:34:30.000000 text2text-1.2.0/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:17:45.839836 text2text-1.2.1/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-07-06 01:47:22.000000 text2text-1.2.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-07-06 02:17:45.838836 text2text-1.2.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    55448 2023-07-06 01:47:22.000000 text2text-1.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 02:17:45.839836 text2text-1.2.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1266 2023-07-06 02:01:33.000000 text2text-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:17:45.834835 text2text-1.2.1/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      603 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:17:45.836835 text2text-1.2.1/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-07-06 02:05:18.000000 text2text-1.2.1/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:17:45.838836 text2text-1.2.1/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-06 01:47:22.000000 text2text-1.2.1/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-07-06 02:15:48.000000 text2text-1.2.1/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:17:45.835835 text2text-1.2.1/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-07-06 02:17:45.000000 text2text-1.2.1/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-06 02:17:45.000000 text2text-1.2.1/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 02:17:45.000000 text2text-1.2.1/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-06 02:17:45.000000 text2text-1.2.1/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-06 02:17:45.000000 text2text-1.2.1/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.2.0/LICENSE.txt` & `text2text-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/PKG-INFO` & `text2text-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.0
+Version: 1.2.1
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.2.0/README.md` & `text2text-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/setup.py` & `text2text-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.2.0",
+  version="1.2.1",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
@@ -25,14 +25,15 @@
     'bitsandbytes',
     'peft',
     'faiss-cpu',
     'flask',
     'googledrivedownloader',
     'numpy',
     'pandas',
+    'scikit-learn',
     'scipy',
     'sentencepiece',
     'torch',
     'tqdm',
     'transformers',
   ],
 )
```

### Comparing `text2text-1.2.0/text2text/__init__.py` & `text2text-1.2.1/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/abstractor.py` & `text2text-1.2.1/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/answerer.py` & `text2text-1.2.1/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/assistant.py` & `text2text-1.2.1/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/biunilm/loader_utils.py` & `text2text-1.2.1/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/biunilm/seq2seq_loader.py` & `text2text-1.2.1/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/bm25er.py` & `text2text-1.2.1/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/counter.py` & `text2text-1.2.1/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/fitter.py` & `text2text-1.2.1/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/handler.py` & `text2text-1.2.1/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/identifier.py` & `text2text-1.2.1/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/indexer.py` & `text2text-1.2.1/text2text/indexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import text2text as t2t
 import faiss
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
+import sklearn.preprocessing as preprocessing
 import warnings
 
 class Indexer(t2t.Transformer):
 
   def get_formatted_matrix(self, input_lines, src_lang='en', **kwargs):
     res = np.array([[]]*len(input_lines))
     if not self.encoders:
       self.encoders = [t2t.Tfidfer()]
     for encoder in self.encoders:
       x = encoder.transform(input_lines, src_lang=src_lang, output='matrix', batch_process=True, **kwargs)
       if not isinstance(x, np.ndarray):
         x = x.toarray()
       res = np.concatenate((res, x.reshape(len(input_lines),-1)), axis=1)
+    res = preprocessing.normalize(res, norm='l2')
     return res.astype('float32')
 
   def size(self, **kwargs):
     return self.index.ntotal
 
   def add(self, input_lines, src_lang='en', faiss_index=None, **kwargs):
     if faiss_index is not None:
```

### Comparing `text2text-1.2.0/text2text/measurer.py` & `text2text-1.2.1/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.2.1/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.2.1/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.2.1/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.2.1/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.2.1/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/questioner.py` & `text2text-1.2.1/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/server.py` & `text2text-1.2.1/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/summarizer.py` & `text2text-1.2.1/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/tfidfer.py` & `text2text-1.2.1/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/tokenizer.py` & `text2text-1.2.1/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/transformer.py` & `text2text-1.2.1/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/translator.py` & `text2text-1.2.1/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.0/text2text/vectorizer.py` & `text2text-1.2.1/text2text/vectorizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import torch
 import numpy as np
 import text2text as t2t
 from transformers import AutoTokenizer, AutoModel
+import sklearn.preprocessing as preprocessing
 
 def mean_pooling(model_output, attention_mask):
   token_embeddings = model_output[0]
   input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
   return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
 
 class Vectorizer(t2t.Transformer):
 
-  pretrained_model = 'sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2'
-
-  def __init__(self):
-    self.__class__.tokenizer = AutoTokenizer.from_pretrained(self.__class__.pretrained_model)
-    self.__class__.model = AutoModel.from_pretrained(self.__class__.pretrained_model)
+  def __init__(self, pretrained_model='sentence-transformers/all-mpnet-base-v2'):
+    self.__class__.tokenizer = AutoTokenizer.from_pretrained(pretrained_model)
+    self.__class__.model = AutoModel.from_pretrained(pretrained_model)
 
   def batch_embed(self, input_lines):
     encoder_inputs = self.__class__.tokenizer(input_lines, padding=True, truncation=True, return_tensors='pt')
     with torch.no_grad():
       model_output = self.__class__.model(**encoder_inputs)
-    return mean_pooling(model_output, encoder_inputs['attention_mask'])
+    X = mean_pooling(model_output, encoder_inputs['attention_mask'])
+    return preprocessing.normalize(X, norm='l2')
 
   def transform(self, input_lines, src_lang='en', batch_process=False, **kwargs):
     input_lines = t2t.Transformer.transform(self, input_lines, src_lang=src_lang, **kwargs)
     tokenizer = self.__class__.tokenizer
     model = self.__class__.model
     if batch_process:
       return np.array(self.batch_embed(input_lines))
```

### Comparing `text2text-1.2.0/text2text.egg-info/PKG-INFO` & `text2text-1.2.1/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.0
+Version: 1.2.1
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.2.0/text2text.egg-info/SOURCES.txt` & `text2text-1.2.1/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

