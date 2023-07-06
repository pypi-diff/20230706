# Comparing `tmp/kanonym4text-0.2.1.tar.gz` & `tmp/kanonym4text-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanonym4text-0.2.1.tar", last modified: Thu Jul  6 10:22:52 2023, max compression
+gzip compressed data, was "kanonym4text-0.2.2.tar", last modified: Thu Jul  6 10:51:46 2023, max compression
```

## Comparing `kanonym4text-0.2.1.tar` & `kanonym4text-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     5099 2023-07-01 20:45:19.000000 kanonym4text-0.2.1/README.md
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      119 2023-07-06 09:36:30.000000 kanonym4text-0.2.1/kanonym4text/__init__.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/data/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.2.1/kanonym4text/data/5000_most_common_words_by_order.txt
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/objects/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       52 2023-07-06 09:06:10.000000 kanonym4text-0.2.1/kanonym4text/objects/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8013 2023-07-06 10:20:08.000000 kanonym4text-0.2.1/kanonym4text/objects/kanonym.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text/utils/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.2.1/kanonym4text/utils/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13290 2023-07-06 10:16:14.000000 kanonym4text-0.2.1/kanonym4text/utils/anonym_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-06 10:17:19.000000 kanonym4text-0.2.1/kanonym4text/utils/cluster_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6024 2023-07-06 10:14:17.000000 kanonym4text-0.2.1/kanonym4text/utils/llm_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.2.1/kanonym4text/utils/models.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11168 2023-07-06 08:39:12.000000 kanonym4text-0.2.1/kanonym4text/utils/nlp_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3152 2023-07-06 08:40:32.000000 kanonym4text-0.2.1/kanonym4text/utils/utilization_utils.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/kanonym4text.egg-info/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      576 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/SOURCES.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/dependency_links.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/requires.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       13 2023-07-06 10:22:52.000000 kanonym4text-0.2.1/kanonym4text.egg-info/top_level.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-06 10:22:52.730272 kanonym4text-0.2.1/setup.cfg
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1571 2023-07-06 10:22:24.000000 kanonym4text-0.2.1/setup.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     5099 2023-07-01 20:45:19.000000 kanonym4text-0.2.2/README.md
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      119 2023-07-06 09:36:30.000000 kanonym4text-0.2.2/kanonym4text/__init__.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/data/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.2.2/kanonym4text/data/5000_most_common_words_by_order.txt
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/objects/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       52 2023-07-06 09:06:10.000000 kanonym4text-0.2.2/kanonym4text/objects/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8013 2023-07-06 10:20:08.000000 kanonym4text-0.2.2/kanonym4text/objects/kanonym.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/utils/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.2.2/kanonym4text/utils/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13287 2023-07-06 10:50:11.000000 kanonym4text-0.2.2/kanonym4text/utils/anonym_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-06 10:17:19.000000 kanonym4text-0.2.2/kanonym4text/utils/cluster_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6024 2023-07-06 10:14:17.000000 kanonym4text-0.2.2/kanonym4text/utils/llm_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.2.2/kanonym4text/utils/models.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11168 2023-07-06 08:39:12.000000 kanonym4text-0.2.2/kanonym4text/utils/nlp_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3152 2023-07-06 08:40:32.000000 kanonym4text-0.2.2/kanonym4text/utils/utilization_utils.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text.egg-info/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      576 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/SOURCES.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/dependency_links.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/requires.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       13 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/top_level.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/setup.cfg
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1571 2023-07-06 10:51:34.000000 kanonym4text-0.2.2/setup.py
```

### Comparing `kanonym4text-0.2.1/PKG-INFO` & `kanonym4text-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kanonym4text
-Version: 0.2.1
+Version: 0.2.2
 Summary: k-anonymity for texts
 Home-page: https://github.com/neumanh/K-anonymity-fot-texts
 Author: Lior Trieman, Hadas Neuman
 Author-email: liortr30@gmail.com, hadas.doron@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.2.tar.gz
 Description: A package that takes a dataframe with a corpus and return an anonymized corpus
 Keywords: python,k-anonymity,privacy,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `kanonym4text-0.2.1/README.md` & `kanonym4text-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text/data/5000_most_common_words_by_order.txt` & `kanonym4text-0.2.2/kanonym4text/data/5000_most_common_words_by_order.txt`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text/objects/kanonym.py` & `kanonym4text-0.2.2/kanonym4text/objects/kanonym.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text/utils/anonym_utils.py` & `kanonym4text-0.2.2/kanonym4text/utils/anonym_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         logging.warning('Creating BoW without stopwords removal')
         cc = corpus
     try:
         count_data = vectorizer.fit_transform(cc)
         voc = vectorizer.get_feature_names_out()
 
     except Exception as e:
-        logging.warning(f'Could not create a bow: {e}')
+        logging.info(f'Could not create a bow: {e}')
         count_data, voc = None, None
     return count_data, voc
 
 
 def get_tfidf(corpus):  # stop_list, clean = True, lemmatize = True):
     """ Vectorize the corpus using CountVectorizer """
```

### Comparing `kanonym4text-0.2.1/kanonym4text/utils/cluster_utils.py` & `kanonym4text-0.2.2/kanonym4text/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text/utils/llm_utils.py` & `kanonym4text-0.2.2/kanonym4text/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text/utils/models.py` & `kanonym4text-0.2.2/kanonym4text/utils/models.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text/utils/nlp_utils.py` & `kanonym4text-0.2.2/kanonym4text/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text/utils/utilization_utils.py` & `kanonym4text-0.2.2/kanonym4text/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/kanonym4text.egg-info/PKG-INFO` & `kanonym4text-0.2.2/kanonym4text.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kanonym4text
-Version: 0.2.1
+Version: 0.2.2
 Summary: k-anonymity for texts
 Home-page: https://github.com/neumanh/K-anonymity-fot-texts
 Author: Lior Trieman, Hadas Neuman
 Author-email: liortr30@gmail.com, hadas.doron@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.2.tar.gz
 Description: A package that takes a dataframe with a corpus and return an anonymized corpus
 Keywords: python,k-anonymity,privacy,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `kanonym4text-0.2.1/kanonym4text.egg-info/SOURCES.txt` & `kanonym4text-0.2.2/kanonym4text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.1/setup.py` & `kanonym4text-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'k-anonymity for texts'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="kanonym4text",
     version=VERSION,
     author="Lior Trieman, Hadas Neuman",
     author_email="liortr30@gmail.com, hadas.doron@gmail.com",
     url='https://github.com/neumanh/K-anonymity-fot-texts',
 
-    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.1.tar.gz',
+    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.2.tar.gz',
 
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # package_dir={'kanonym4text': 'kanonym4text'},
     install_requires=[
```

