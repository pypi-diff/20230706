# Comparing `tmp/zhei-0.0.4.tar.gz` & `tmp/zhei-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhei-0.0.4.tar", last modified: Mon Jun 26 12:01:31 2023, max compression
+gzip compressed data, was "zhei-0.0.6.tar", last modified: Thu Jul  6 02:14:53 2023, max compression
```

## Comparing `zhei-0.0.4.tar` & `zhei-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 12:01:31.713126 zhei-0.0.4/
--rw-r--r--   0 dengyifan   (501) staff       (20)      282 2023-06-26 12:01:31.712917 zhei-0.0.4/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-06-26 11:10:29.000000 zhei-0.0.4/README.md
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-06-26 12:01:31.713199 zhei-0.0.4/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      631 2023-06-26 12:00:32.000000 zhei-0.0.4/setup.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 12:01:31.708699 zhei-0.0.4/zhei/
--rw-r--r--   0 dengyifan   (501) staff       (20)       13 2023-06-26 10:04:51.000000 zhei-0.0.4/zhei/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)       37 2023-06-26 11:25:24.000000 zhei-0.0.4/zhei/hello.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 12:01:31.709721 zhei-0.0.4/zhei/models/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-06-26 09:58:31.000000 zhei-0.0.4/zhei/models/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-06-26 09:42:47.000000 zhei-0.0.4/zhei/models/lightning_model.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 12:01:31.712523 zhei-0.0.4/zhei/utils/
--rw-r--r--   0 dengyifan   (501) staff       (20)     4112 2023-06-26 05:12:15.000000 zhei-0.0.4/zhei/utils/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)      674 2023-06-26 07:36:31.000000 zhei-0.0.4/zhei/utils/catch_error.py
--rw-r--r--   0 dengyifan   (501) staff       (20)    21472 2023-06-26 11:59:28.000000 zhei-0.0.4/zhei/utils/eval_methods.py
--rw-r--r--   0 dengyifan   (501) staff       (20)    18328 2023-06-26 11:59:10.000000 zhei-0.0.4/zhei/utils/gpu.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3428 2023-06-26 11:59:35.000000 zhei-0.0.4/zhei/utils/io.py
--rw-r--r--   0 dengyifan   (501) staff       (20)      762 2023-06-26 07:31:23.000000 zhei-0.0.4/zhei/utils/log.py
--rw-r--r--   0 dengyifan   (501) staff       (20)      418 2023-06-26 09:20:53.000000 zhei-0.0.4/zhei/utils/notice.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4262 2023-06-26 07:25:55.000000 zhei-0.0.4/zhei/utils/result.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 12:01:31.709428 zhei-0.0.4/zhei.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      282 2023-06-26 12:01:31.000000 zhei-0.0.4/zhei.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      387 2023-06-26 12:01:31.000000 zhei-0.0.4/zhei.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-06-26 12:01:31.000000 zhei-0.0.4/zhei.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-06-26 12:01:31.000000 zhei-0.0.4/zhei.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.601797 zhei-0.0.6/
+-rw-rw-rw-   0        0        0      294 2023-07-06 02:14:53.601797 zhei-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-06-27 02:45:05.000000 zhei-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 02:14:53.602798 zhei-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-07-06 02:14:49.000000 zhei-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.571696 zhei-0.0.6/zhei/
+-rw-rw-rw-   0        0        0       74 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/__init__.py
+-rw-rw-rw-   0        0        0      782 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/intro.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.599798 zhei-0.0.6/zhei/utils/
+-rw-rw-rw-   0        0        0      259 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/__init__.py
+-rw-rw-rw-   0        0        0      674 2023-07-04 01:44:04.000000 zhei-0.0.6/zhei/utils/catch_error.py
+-rw-rw-rw-   0        0        0      169 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/dataset.py
+-rw-rw-rw-   0        0        0    21465 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/eval_methods.py
+-rw-rw-rw-   0        0        0     8721 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/init.py
+-rw-rw-rw-   0        0        0     3421 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/io.py
+-rw-rw-rw-   0        0        0     5091 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/log.py
+-rw-rw-rw-   0        0        0     1002 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/notice.py
+-rw-rw-rw-   0        0        0     7103 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/processing_unit.py
+-rw-rw-rw-   0        0        0     7054 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/redis.py
+-rw-rw-rw-   0        0        0     4262 2023-07-04 01:44:04.000000 zhei-0.0.6/zhei/utils/result.py
+-rw-rw-rw-   0        0        0      667 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/tokenize.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.584694 zhei-0.0.6/zhei.egg-info/
+-rw-rw-rw-   0        0        0      294 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       59 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/top_level.txt
```

### Comparing `zhei-0.0.4/zhei/utils/catch_error.py` & `zhei-0.0.6/zhei/utils/catch_error.py`

 * *Files identical despite different names*

### Comparing `zhei-0.0.4/zhei/utils/eval_methods.py` & `zhei-0.0.6/zhei/utils/eval_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from zhei.utils.result import Result
-from zhei.utils.log import get_logger
+from zhei.utils.log import Logger
 from zhei.utils.catch_error import print_error_info
 from datasets import Dataset
 import pandas as pd
 from evaluate import load
 from statistics import mean
 import re
 import string
@@ -17,15 +17,15 @@
 from sacrebleu.metrics import BLEU, CHRF
 import sacrebleu
 import spacy
 from rich.console import Console
 from rich.table import Table
 from typing import Union
 
-log = get_logger(__name__)
+log = Logger(__name__) 
 
 def distinct_ngram(candidates, n=2):
     """Return basic ngram statistics, as well as a dict of all ngrams and their freqsuencies."""
     ngram_freqs = {}  # ngrams with frequencies
     ngram_len = 0  # total number of ngrams
     for candidate in candidates:
         for ngram in ngrams(word_tokenize(candidate), n):
```

### Comparing `zhei-0.0.4/zhei/utils/io.py` & `zhei-0.0.6/zhei/utils/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from zhei.utils.log import get_logger
+from zhei.utils.log import Logger
 import os
 import pickle
 import json
 import jsonlines
 import torch
 import pandas as pd
 
-log = get_logger(__name__)
+log = Logger(__name__) 
 
 
 def load_in(path, data_name=""):
     """读取文件，根据文件后缀名自动选择读取方法
         目前支持保存类型有：‘pkl’、‘txt’、‘pt’、‘json’, 'jsonl'、'csv'
 
     Args:
```

### Comparing `zhei-0.0.4/zhei/utils/result.py` & `zhei-0.0.6/zhei/utils/result.py`

 * *Files identical despite different names*

