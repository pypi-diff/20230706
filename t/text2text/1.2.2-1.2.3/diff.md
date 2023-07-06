# Comparing `tmp/text2text-1.2.2.tar.gz` & `tmp/text2text-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.2.2.tar", last modified: Thu Jul  6 02:56:37 2023, max compression
+gzip compressed data, was "text2text-1.2.3.tar", last modified: Thu Jul  6 03:23:14 2023, max compression
```

## Comparing `text2text-1.2.2.tar` & `text2text-1.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:56:37.408189 text2text-1.2.2/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-07-06 02:37:32.000000 text2text-1.2.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    56262 2023-07-06 02:56:37.408189 text2text-1.2.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    55448 2023-07-06 02:37:32.000000 text2text-1.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 02:56:37.408189 text2text-1.2.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1266 2023-07-06 02:56:13.000000 text2text-1.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:56:37.404189 text2text-1.2.2/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      603 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:56:37.406189 text2text-1.2.2/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-07-06 02:46:41.000000 text2text-1.2.2/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:56:37.407189 text2text-1.2.2/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-06 02:37:32.000000 text2text-1.2.2/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-07-06 02:47:15.000000 text2text-1.2.2/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:56:37.406189 text2text-1.2.2/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    56262 2023-07-06 02:56:37.000000 text2text-1.2.2/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2023-07-06 02:56:37.000000 text2text-1.2.2/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 02:56:37.000000 text2text-1.2.2/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-06 02:56:37.000000 text2text-1.2.2/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-06 02:56:37.000000 text2text-1.2.2/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:23:14.163278 text2text-1.2.3/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-07-06 02:37:32.000000 text2text-1.2.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-07-06 03:23:14.163278 text2text-1.2.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    55448 2023-07-06 02:37:32.000000 text2text-1.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 03:23:14.163278 text2text-1.2.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1266 2023-07-06 03:14:25.000000 text2text-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:23:14.160278 text2text-1.2.3/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      603 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:23:14.161278 text2text-1.2.3/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-07-06 02:46:41.000000 text2text-1.2.3/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:23:14.163278 text2text-1.2.3/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-06 02:37:32.000000 text2text-1.2.3/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-06 03:21:55.000000 text2text-1.2.3/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 03:23:14.161278 text2text-1.2.3/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-07-06 03:23:13.000000 text2text-1.2.3/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-06 03:23:14.000000 text2text-1.2.3/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 03:23:13.000000 text2text-1.2.3/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-06 03:23:13.000000 text2text-1.2.3/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-06 03:23:13.000000 text2text-1.2.3/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.2.2/LICENSE.txt` & `text2text-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/PKG-INFO` & `text2text-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.2
+Version: 1.2.3
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.2.2/README.md` & `text2text-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/setup.py` & `text2text-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.2.2",
+  version="1.2.3",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.2.2/text2text/__init__.py` & `text2text-1.2.3/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/abstractor.py` & `text2text-1.2.3/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/answerer.py` & `text2text-1.2.3/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/assistant.py` & `text2text-1.2.3/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/biunilm/loader_utils.py` & `text2text-1.2.3/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/biunilm/seq2seq_loader.py` & `text2text-1.2.3/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/bm25er.py` & `text2text-1.2.3/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/counter.py` & `text2text-1.2.3/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/fitter.py` & `text2text-1.2.3/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/handler.py` & `text2text-1.2.3/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/identifier.py` & `text2text-1.2.3/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/indexer.py` & `text2text-1.2.3/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/measurer.py` & `text2text-1.2.3/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.2.3/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.2.3/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.2.3/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.2.3/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.2.3/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/questioner.py` & `text2text-1.2.3/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/server.py` & `text2text-1.2.3/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/summarizer.py` & `text2text-1.2.3/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/tfidfer.py` & `text2text-1.2.3/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/tokenizer.py` & `text2text-1.2.3/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/transformer.py` & `text2text-1.2.3/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/translator.py` & `text2text-1.2.3/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.2/text2text/vectorizer.py` & `text2text-1.2.3/text2text/vectorizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 def mean_pooling(model_output, attention_mask):
   token_embeddings = model_output[0]
   input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
   return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
 
 class Vectorizer(t2t.Transformer):
 
-  def __init__(self, pretrained_model='sentence-transformers/all-mpnet-base-v2', batch_process=True):
+  def __init__(self, pretrained_model='sentence-transformers/all-mpnet-base-v2', batch_size=0):
     self.__class__.tokenizer = AutoTokenizer.from_pretrained(pretrained_model)
     self.__class__.model = AutoModel.from_pretrained(pretrained_model)
-    self.__class__.batch_process = batch_process
+    self.__class__.batch_size = batch_size
 
   def batch_embed(self, input_lines):
     encoder_inputs = self.__class__.tokenizer(input_lines, padding=True, truncation=True, return_tensors='pt')
     with torch.no_grad():
       model_output = self.__class__.model(**encoder_inputs)
     X = mean_pooling(model_output, encoder_inputs['attention_mask'])
     return preprocessing.normalize(X, norm='l2')
 
   def transform(self, input_lines, src_lang='en', batch_process=False, **kwargs):
     input_lines = t2t.Transformer.transform(self, input_lines, src_lang=src_lang, **kwargs)
     tokenizer = self.__class__.tokenizer
     model = self.__class__.model
-    if self.__class__.batch_process:
-      return np.array(self.batch_embed(input_lines))
-    else:
+    batch_size = self.__class__.batch_size
+    if batch_size > 0:
       embeddings = None
-      for line in input_lines:
-        if embeddings is None: embeddings = self.batch_embed([line])
-        else: embeddings = np.concatenate((embeddings, self.batch_embed([line])), axis=0)
+      for i in range(0, len(input_lines), batch_size):
+        lines = input_lines[i:i+batch_size]
+        this_batch = self.batch_embed(lines)
+        if embeddings is None: embeddings = this_batch
+        else: embeddings = np.concatenate((embeddings, this_batch), axis=0)
       return np.array(embeddings)
+    else:
+      return np.array(self.batch_embed(input_lines))
```

### Comparing `text2text-1.2.2/text2text.egg-info/PKG-INFO` & `text2text-1.2.3/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.2
+Version: 1.2.3
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.2.2/text2text.egg-info/SOURCES.txt` & `text2text-1.2.3/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

