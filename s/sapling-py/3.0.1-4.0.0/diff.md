# Comparing `tmp/sapling-py-3.0.1.tar.gz` & `tmp/sapling-py-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapling-py-3.0.1.tar", last modified: Tue Jun 13 20:35:18 2023, max compression
+gzip compressed data, was "sapling-py-4.0.0.tar", last modified: Wed Jul  5 23:20:01 2023, max compression
```

## Comparing `sapling-py-3.0.1.tar` & `sapling-py-4.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.542436 sapling-py-3.0.1/
--rw-r--r--   0 rishabhmarya   (501) staff       (20)    11357 2023-06-12 19:35:12.000000 sapling-py-3.0.1/LICENSE
--rw-r--r--   0 rishabhmarya   (501) staff       (20)     3341 2023-06-13 20:35:18.542329 sapling-py-3.0.1/PKG-INFO
--rw-r--r--   0 rishabhmarya   (501) staff       (20)     2964 2023-06-12 19:35:12.000000 sapling-py-3.0.1/README.md
-drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.541604 sapling-py-3.0.1/sapling/
--rw-r--r--   0 rishabhmarya   (501) staff       (20)      130 2023-06-12 19:35:12.000000 sapling-py-3.0.1/sapling/__init__.py
--rw-r--r--   0 rishabhmarya   (501) staff       (20)    17959 2023-06-12 20:07:52.000000 sapling-py-3.0.1/sapling/client.py
--rw-r--r--   0 rishabhmarya   (501) staff       (20)       22 2023-06-13 20:28:46.000000 sapling-py-3.0.1/sapling/version.py
-drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.542086 sapling-py-3.0.1/sapling_py.egg-info/
--rw-r--r--   0 rishabhmarya   (501) staff       (20)     3341 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/PKG-INFO
--rw-r--r--   0 rishabhmarya   (501) staff       (20)      269 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhmarya   (501) staff       (20)        1 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhmarya   (501) staff       (20)        9 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/requires.txt
--rw-r--r--   0 rishabhmarya   (501) staff       (20)       13 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/top_level.txt
--rw-r--r--   0 rishabhmarya   (501) staff       (20)       38 2023-06-13 20:35:18.542470 sapling-py-3.0.1/setup.cfg
--rw-r--r--   0 rishabhmarya   (501) staff       (20)      948 2023-06-12 19:35:12.000000 sapling-py-3.0.1/setup.py
-drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.542191 sapling-py-3.0.1/test/
--rw-r--r--   0 rishabhmarya   (501) staff       (20)        0 2023-06-12 19:35:12.000000 sapling-py-3.0.1/test/__init__.py
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-07-05 23:20:01.807936 sapling-py-4.0.0/
+-rw-r--r--   0 james      (502) staff       (20)    11357 2022-11-10 06:53:31.000000 sapling-py-4.0.0/LICENSE
+-rw-r--r--   0 james      (502) staff       (20)     3321 2023-07-05 23:20:01.807324 sapling-py-4.0.0/PKG-INFO
+-rw-r--r--   0 james      (502) staff       (20)     2964 2022-11-10 06:53:31.000000 sapling-py-4.0.0/README.md
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-07-05 23:20:01.806431 sapling-py-4.0.0/sapling/
+-rw-r--r--   0 james      (502) staff       (20)      130 2023-03-30 07:18:05.000000 sapling-py-4.0.0/sapling/__init__.py
+-rw-r--r--   0 james      (502) staff       (20)    18857 2023-06-23 00:20:15.000000 sapling-py-4.0.0/sapling/client.py
+-rw-r--r--   0 james      (502) staff       (20)       22 2023-06-14 00:26:34.000000 sapling-py-4.0.0/sapling/version.py
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-07-05 23:20:01.807066 sapling-py-4.0.0/sapling_py.egg-info/
+-rw-r--r--   0 james      (502) staff       (20)     3321 2023-07-05 23:20:01.000000 sapling-py-4.0.0/sapling_py.egg-info/PKG-INFO
+-rw-r--r--   0 james      (502) staff       (20)      269 2023-07-05 23:20:01.000000 sapling-py-4.0.0/sapling_py.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (502) staff       (20)        1 2023-07-05 23:20:01.000000 sapling-py-4.0.0/sapling_py.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (502) staff       (20)        9 2023-07-05 23:20:01.000000 sapling-py-4.0.0/sapling_py.egg-info/requires.txt
+-rw-r--r--   0 james      (502) staff       (20)       13 2023-07-05 23:20:01.000000 sapling-py-4.0.0/sapling_py.egg-info/top_level.txt
+-rw-r--r--   0 james      (502) staff       (20)       38 2023-07-05 23:20:01.808003 sapling-py-4.0.0/setup.cfg
+-rw-r--r--   0 james      (502) staff       (20)      948 2023-03-30 07:17:57.000000 sapling-py-4.0.0/setup.py
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-07-05 23:20:01.807180 sapling-py-4.0.0/test/
+-rw-r--r--   0 james      (502) staff       (20)        0 2022-11-10 06:53:31.000000 sapling-py-4.0.0/test/__init__.py
```

### Comparing `sapling-py-3.0.1/LICENSE` & `sapling-py-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sapling-py-3.0.1/PKG-INFO` & `sapling-py-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sapling-py
-Version: 3.0.1
+Version: 4.0.0
 Summary: Sapling Python Client
 Home-page: https://sapling.ai
 Author: Sapling Intelligence
 Author-email: info@sapling.ai
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sapling Python Client
 
@@ -88,9 +87,7 @@
 
 License
 -------
 
 Copyright 2022 Sapling Intelligence, Inc.
 
 Licensed under the Apache License, Version 2.0.
-
-
```

### Comparing `sapling-py-3.0.1/README.md` & `sapling-py-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sapling-py-3.0.1/sapling/client.py` & `sapling-py-4.0.0/sapling/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self,
         text,
         session_id=None,
         lang=None,
         variety=None,
         medical=None,
         auto_apply=False,
+        advanced_edits=None,
     ):
         '''
         Fetches edits (including for grammar and spelling) for provided text.
 
         :param text: Text to process for edits.
         :type text: str
         :param session_id: Unique name or UUID of document or portion of text that is being checked
@@ -49,23 +50,47 @@
         :type session_id: str
         :param variety: Specifies regional English variety preference. Defaults to the configuration in the user Sapling dashboard.
         :type variety: str
         :param medical: If true, the backend will apply Sapling's medical dictionary.
         :type medical: bool
         :param auto_apply: Whether to return a field with edits applied to the text
         :type auto_apply: bool
-        :rtype: list[dict]
+        :param advanced_edits: Additional edit configurations
+        :type advanced_edits: dict
+            Options:
+                - advanced_edits
+                - adverbs
+                - simplifications
+                - hard_to_read
+                - qualifiers
+                - voice
+                - dei
+                - gender
+                - gender_pronoun
+                - gender_noun
+                - gender_id
+                - sensitivity
+                - disability
+                - age
+                - race
+                - social_class
+                - violence
+\
+
+        :rtype: dict
         :return:
-            - sentence: Unedited sentence
-            - sentence_start: Offset of sentence from start of text
-            - start: Offset of edit start relative to sentence
-            - end: Offset of edit end relative to sentence
-            - replacement: Suggested replacement
-            - error_type: Error type
-            - general_error_type: General Error type
+            - edits: List of Edits:
+                - sentence: Unedited sentence
+                - sentence_start: Offset of sentence from start of text
+                - start: Offset of edit start relative to sentence
+                - end: Offset of edit end relative to sentence
+                - replacement: Suggested replacement
+                - error_type: Error type
+                - general_error_type: General Error type
+            - applied_text: Transformed text if auto_apply is set.
 
         Supported languages:
             - `de`:  German (Deutsch)
             - `el`:  Greek (Ελληνικά)
             - `en`:  English (US/UK/CA/AU)
             - `es`:  Spanish (Español)
             - `fr`:  French  (Français) (`fr-fr` and `fr-ca` coming soon)
@@ -99,23 +124,24 @@
             data['lang'] = lang
         if variety is not None:
             data['variety'] = variety
         if medical is not None:
             data['medical'] = medical
         if auto_apply is not None:
             data['auto_apply'] = auto_apply
+        if advanced_edits is not None:
+            data['advanced_edits'] = advanced_edits
 
         resp = requests.post(
             url,
             json=data,
             timeout=self.timeout,
         )
         if 200 <= resp.status_code < 300:
-            resp_json = resp.json()
-            return resp_json.get('edits')
+            return resp.json()
         raise Exception(f'HTTP {resp.status_code}: {resp.text}')
 
     def accept_edit(
         self,
         edit_uuid,
         session_id=None,
     ):
@@ -200,14 +226,16 @@
         :type min_length: int
         :param multiple_edits: Default is false. If true, will return `candidates` field containing list of other potential corrections for each error.
         :type multiple_edits: bool
         :param lang: Default is English. Specify a language to spellcheck the text against.
         :type lang: str
         :param auto_apply: Whether to return a field with edits applied to the text. Cannot be set with multiple_edits option.
         :type auto_apply: bool
+        :param advanced_edits: additional edit checking options
+        :type advanced_edits: dict
         :param variety: Specifies regional English variety preference. Defaults to the configuration in the user Sapling dashboard.
         :type variety: str
 
         :rtype: list[dict]
 
         Supported languages:
             - `en`: English
@@ -483,24 +511,26 @@
         operations,
     ):
         '''
         Performs a variety of operations that are useful for working with the outputs of an NLP (whether human or AI) system. These include:
             - Fixing or restoring punctuation
             - Fixing capitalization
             - Fixing or restoring whitespace
+
         Example use cases include repairing transcriptions or captions.
 
         :param text: Text to postprocess
         :type text: str
         :param session_id: Unique name or UUID of document or portion of text that is being chunked
         :type text: str
         :param operations: Operations to apply. The currently accepted operations are:
             - capitalize
             - punctuate
             - fixspaces
+
         :type operations: list[str]
         :rtype: list[dict]
         :return:
             Same as the edits endpoint:
             - sentence: Unedited sentence
             - sentence_start: Offset of sentence from start of text
             - start: Offset of edit start relative to sentence
@@ -519,8 +549,8 @@
         resp = requests.post(
             url,
             json=data,
             timeout=self.timeout,
         )
         if 200 <= resp.status_code < 300:
             return resp.json()
-        raise Exception(f'HTTP {resp.status_code}: {resp.text}')
+        raise Exception(f'HTTP {resp.status_code}: {resp.text}')
```

### Comparing `sapling-py-3.0.1/sapling_py.egg-info/PKG-INFO` & `sapling-py-4.0.0/sapling_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sapling-py
-Version: 3.0.1
+Version: 4.0.0
 Summary: Sapling Python Client
 Home-page: https://sapling.ai
 Author: Sapling Intelligence
 Author-email: info@sapling.ai
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sapling Python Client
 
@@ -88,9 +87,7 @@
 
 License
 -------
 
 Copyright 2022 Sapling Intelligence, Inc.
 
 Licensed under the Apache License, Version 2.0.
-
-
```

### Comparing `sapling-py-3.0.1/setup.py` & `sapling-py-4.0.0/setup.py`

 * *Files identical despite different names*

