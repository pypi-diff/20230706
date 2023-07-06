# Comparing `tmp/fajrGPT-1.3.3.tar.gz` & `tmp/fajrGPT-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.3.3.tar", last modified: Wed Jul  5 12:48:24 2023, max compression
+gzip compressed data, was "fajrGPT-1.3.4.tar", last modified: Thu Jul  6 15:24:24 2023, max compression
```

## Comparing `fajrGPT-1.3.3.tar` & `fajrGPT-1.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-05 12:48:24.444571 fajrGPT-1.3.3/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3.3/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-05 12:48:24.444426 fajrGPT-1.3.3/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3.3/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-05 12:48:24.443099 fajrGPT-1.3.3/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3.3/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3.3/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    13239 2023-07-05 12:47:24.000000 fajrGPT-1.3.3/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-05 12:48:24.444223 fajrGPT-1.3.3/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-05 12:48:24.000000 fajrGPT-1.3.3/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-05 12:48:24.000000 fajrGPT-1.3.3/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-05 12:48:24.000000 fajrGPT-1.3.3/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-05 12:48:24.000000 fajrGPT-1.3.3/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-05 12:48:24.000000 fajrGPT-1.3.3/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-05 12:48:24.000000 fajrGPT-1.3.3/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-05 12:48:24.444623 fajrGPT-1.3.3/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-05 12:47:54.000000 fajrGPT-1.3.3/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-06 15:24:24.048401 fajrGPT-1.3.4/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3.4/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-06 15:24:24.048261 fajrGPT-1.3.4/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3.4/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-06 15:24:24.047282 fajrGPT-1.3.4/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3.4/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3.4/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    13300 2023-07-06 15:23:08.000000 fajrGPT-1.3.4/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-06 15:24:24.048104 fajrGPT-1.3.4/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-06 15:24:24.048440 fajrGPT-1.3.4/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-06 15:22:39.000000 fajrGPT-1.3.4/setup.py
```

### Comparing `fajrGPT-1.3.3/LICENSE` & `fajrGPT-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.3/PKG-INFO` & `fajrGPT-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3.3/README.md` & `fajrGPT-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.3/fajrGPT/quran_metadata.py` & `fajrGPT-1.3.4/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.3/fajrGPT/wake.py` & `fajrGPT-1.3.4/fajrGPT/wake.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
         # Get the transliteration of the name of Allah
         name_of_allah_transliteration = allah_transliterations[index]
 
         # Get the explanation of the name of Allah using a GPT-3 model prompt
         prompt = f"""
 
-        For the name of Allah below, please do the following: First break down the word into its root letters. Then, using the root letters, try to guess the meaning of the name. Finally, give a brief explanation of the significane of this particular name of Allah as it relates to the Quran.
+        For the name of Allah below, please do the following: First break down the word into its root letters, giving their approximate equivalent in the english language. Then, using the root letters, try to guess the meaning of the name. Finally, give a brief explanation of the significane of this particular name of Allah as it relates to the Quran.
         
         Name of Allah: {name_of_allah_arabic}\nExplanation: 
         
         """
 
         # Get the explanation of the name of Allah
         explanation = query_gpt(prompt)
```

### Comparing `fajrGPT-1.3.3/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.3.4/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3.3/setup.py` & `fajrGPT-1.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.3.3",
+    version="1.3.4",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

