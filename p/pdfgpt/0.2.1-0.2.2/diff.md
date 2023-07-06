# Comparing `tmp/pdfgpt-0.2.1.tar.gz` & `tmp/pdfgpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfgpt-0.2.1.tar", last modified: Tue May 30 21:49:33 2023, max compression
+gzip compressed data, was "pdfgpt-0.2.2.tar", last modified: Thu Jul  6 13:18:12 2023, max compression
```

## Comparing `pdfgpt-0.2.1.tar` & `pdfgpt-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.267344 pdfgpt-0.2.1/
--rw-rw-rw-   0        0        0     3643 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1099 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3643 2023-05-30 21:49:33.267810 pdfgpt-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2730 2023-05-30 21:46:51.000000 pdfgpt-0.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.211587 pdfgpt-0.2.1/docs/
--rw-rw-rw-   0        0        0      627 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/authors.rst
--rw-rw-rw-   0        0        0     4945 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/history.rst
--rw-rw-rw-   0        0        0      323 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/index.rst
--rw-rw-rw-   0        0        0     1161 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/installation.rst
--rwxrwxrwx   0        0        0      804 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/readme.rst
--rw-rw-rw-   0        0        0       74 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.221265 pdfgpt-0.2.1/pdfgpt/
--rw-rw-rw-   0        0        0      167 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/pdfgpt/__init__.py
--rw-rw-rw-   0        0        0      412 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/pdfgpt/cli.py
--rw-rw-rw-   0        0        0     7855 2023-05-30 21:46:31.000000 pdfgpt-0.2.1/pdfgpt/pdfgpt.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.245602 pdfgpt-0.2.1/pdfgpt.egg-info/
--rw-rw-rw-   0        0        0     3643 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-30 21:49:33.000000 pdfgpt-0.2.1/pdfgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 21:48:24.000000 pdfgpt-0.2.1/pdfgpt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      401 2023-05-30 21:49:33.271453 pdfgpt-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1571 2023-05-30 21:06:39.000000 pdfgpt-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.265335 pdfgpt-0.2.1/tests/
--rw-rw-rw-   0        0        0       37 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0  3340858 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/tests/epanet_matlab_toolkit.pdf
--rw-rw-rw-   0        0        0      697 2023-05-30 20:47:17.000000 pdfgpt-0.2.1/tests/test_example.py
--rw-rw-rw-   0        0        0      878 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/tests/test_pdfgpt.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:18:12.671316 pdfgpt-0.2.2/
+-rw-rw-rw-   0        0        0     3643 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3782 2023-07-06 13:18:12.671316 pdfgpt-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2743 2023-07-06 13:02:20.000000 pdfgpt-0.2.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 13:18:12.640066 pdfgpt-0.2.2/docs/
+-rw-rw-rw-   0        0        0      627 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     4945 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/history.rst
+-rw-rw-rw-   0        0        0      323 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1161 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      804 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       74 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 13:18:12.640066 pdfgpt-0.2.2/pdfgpt/
+-rw-rw-rw-   0        0        0      160 2023-07-06 12:50:41.000000 pdfgpt-0.2.2/pdfgpt/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/pdfgpt/cli.py
+-rw-rw-rw-   0        0        0     7268 2023-07-06 13:04:47.000000 pdfgpt-0.2.2/pdfgpt/pdfgpt.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:18:12.655691 pdfgpt-0.2.2/pdfgpt.egg-info/
+-rw-rw-rw-   0        0        0     3782 2023-07-06 13:18:11.000000 pdfgpt-0.2.2/pdfgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-07-06 13:18:12.000000 pdfgpt-0.2.2/pdfgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:18:11.000000 pdfgpt-0.2.2/pdfgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-06 13:18:11.000000 pdfgpt-0.2.2/pdfgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 13:18:11.000000 pdfgpt-0.2.2/pdfgpt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       86 2023-07-06 13:18:11.000000 pdfgpt-0.2.2/pdfgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 13:18:12.000000 pdfgpt-0.2.2/pdfgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      401 2023-07-06 13:18:12.671316 pdfgpt-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2023-07-06 12:50:15.000000 pdfgpt-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:18:12.671316 pdfgpt-0.2.2/tests/
+-rw-rw-rw-   0        0        0       37 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/tests/__init__.py
+-rw-rw-rw-   0        0        0  3340858 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/tests/epanet_matlab_toolkit.pdf
+-rw-rw-rw-   0        0        0      677 2023-07-06 13:17:44.000000 pdfgpt-0.2.2/tests/test_example.py
+-rw-rw-rw-   0        0        0      878 2023-05-15 15:58:02.000000 pdfgpt-0.2.2/tests/test_pdfgpt.py
```

### Comparing `pdfgpt-0.2.1/CONTRIBUTING.rst` & `pdfgpt-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/LICENSE` & `pdfgpt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/PKG-INFO` & `pdfgpt-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pdfgpt
-Version: 0.2.1
+Version: 0.2.2
 Summary: pdfgpt is a Python package that provides users with the ability to engage in natural language conversations with their PDF documents.
 Home-page: https://github.com/Mariosmsk/pdfgpt
 Author: Marios S. Kyriakou
 Author-email: kiriakou.marios@ucy.ac.cy
 License: MIT license
 Keywords: pdfgpt
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 License-File: LICENSE
 
 ======
 pdfgpt
 ======
 
@@ -30,16 +33,16 @@
         :target: https://pdfgpt.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 .. image:: https://pepy.tech/badge/pdfgpt
         :target: https://pepy.tech/badge/pdfgpt
         :alt: Downloads
 
-.. image:: https://pepy.tech/badge/pdfgpt/month
-        :target: https://pepy.tech/badge/pdfgpt
+.. image:: https://static.pepy.tech/badge/pdfgpt/month
+        :target: https://pepy.tech/badge/pdfgpt/month
         :alt: Downloads
 
 pdfgpt is a Python package that provides users with the ability to engage in natural language conversations with their PDF documents.
 
 
 * Free software: MIT license
 * Documentation: https://pdfgpt.readthedocs.io.
@@ -110,7 +113,9 @@
 History
 =======
 
 0.1.0 (2023-05-11)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `pdfgpt-0.2.1/README.rst` & `pdfgpt-0.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         :target: https://pdfgpt.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 .. image:: https://pepy.tech/badge/pdfgpt
         :target: https://pepy.tech/badge/pdfgpt
         :alt: Downloads
 
-.. image:: https://pepy.tech/badge/pdfgpt/month
-        :target: https://pepy.tech/badge/pdfgpt
+.. image:: https://static.pepy.tech/badge/pdfgpt/month
+        :target: https://pepy.tech/badge/pdfgpt/month
         :alt: Downloads
 
 pdfgpt is a Python package that provides users with the ability to engage in natural language conversations with their PDF documents.
 
 
 * Free software: MIT license
 * Documentation: https://pdfgpt.readthedocs.io.
```

### Comparing `pdfgpt-0.2.1/docs/Makefile` & `pdfgpt-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/docs/conf.py` & `pdfgpt-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/docs/installation.rst` & `pdfgpt-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/docs/make.bat` & `pdfgpt-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/pdfgpt/pdfgpt.py` & `pdfgpt-0.2.2/pdfgpt/pdfgpt.py`

 * *Files 14% similar despite different names*

```diff
@@ -127,46 +127,40 @@
                 res1 = result.iloc[0][0][:7000]
             else:
                 res1 = result.iloc[0][0][:4000]
 
         except:
             res1 = result.iloc[0][0][:min_len]
 
-        if len(result) == 1:
-            prompt = f"""Given the question: {message} and the following embeddings as data:
-                               1. {res1}
-                           Give an answer based only on the data where I provide or return \"Not specified\".
-                           """
-        elif len(result) == 2:
+        try:
             try:
                 if min_len < 2000:
                     res2 = result.iloc[1][0][:4000 - min_len]
                 else:
                     res2 = result.iloc[1][0][:3500]
             except:
                 res2 = result.iloc[1][0][:min_len]
-            prompt = f"""Given the question: {message} and the following embeddings as data:
-                               1. {res1}
-                               2. {res2}
-                           Give an answer based only on the data where I provide or return \"Not specified\".
-                           """
-        else:
+        except:
+            res2 = ''
+        try:
             try:
                 if min_len < 1000:
                     res3 = result.iloc[2][0][:1000 - min_len]
                 else:
                     res3 = result.iloc[2][0][:500]
             except:
                 res3 = result.iloc[2][0][:min_len]
-            prompt = f"""Given the question: {message} and the following embeddings as data:
-                               1. {res1}
-                               2. {res2}
-                               3. {res3}
-                           Give an answer based only on the data where I provide or return \"Not specified\".
-                           """
+        except:
+            res3 = ''
+        prompt = f"""Given the question: {message} and the following embeddings as data:
+                           1. {res1}
+                           2. {res2}
+                           3. {res3}
+                       Give an answer based only on the data where I provide or return \"Not specified\".
+                       """
         return prompt
 
     # Sends a prompt to the OpenAI API and return the response
     def sendPrompt(self, prompt, model="gpt-3.5-turbo", temperature=0.9, max_tokens=1500):
 
         # response = openai.Completion.create(
         #     model=model, prompt=prompt, temperature=temperature, max_tokens=max_tokens,
```

### Comparing `pdfgpt-0.2.1/pdfgpt.egg-info/PKG-INFO` & `pdfgpt-0.2.2/pdfgpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pdfgpt
-Version: 0.2.1
+Version: 0.2.2
 Summary: pdfgpt is a Python package that provides users with the ability to engage in natural language conversations with their PDF documents.
 Home-page: https://github.com/Mariosmsk/pdfgpt
 Author: Marios S. Kyriakou
 Author-email: kiriakou.marios@ucy.ac.cy
 License: MIT license
 Keywords: pdfgpt
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 License-File: LICENSE
 
 ======
 pdfgpt
 ======
 
@@ -30,16 +33,16 @@
         :target: https://pdfgpt.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 .. image:: https://pepy.tech/badge/pdfgpt
         :target: https://pepy.tech/badge/pdfgpt
         :alt: Downloads
 
-.. image:: https://pepy.tech/badge/pdfgpt/month
-        :target: https://pepy.tech/badge/pdfgpt
+.. image:: https://static.pepy.tech/badge/pdfgpt/month
+        :target: https://pepy.tech/badge/pdfgpt/month
         :alt: Downloads
 
 pdfgpt is a Python package that provides users with the ability to engage in natural language conversations with their PDF documents.
 
 
 * Free software: MIT license
 * Documentation: https://pdfgpt.readthedocs.io.
@@ -110,7 +113,9 @@
 History
 =======
 
 0.1.0 (2023-05-11)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `pdfgpt-0.2.1/pdfgpt.egg-info/SOURCES.txt` & `pdfgpt-0.2.2/pdfgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/setup.py` & `pdfgpt-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['Click>=7.0', 'openai', 'pandas', 'pypdf', 'matplotlib', 'plotly', 'scipy', 'scikit-learn', 'tiktoken']
+requirements = ['Click>=7.0', 'openai', 'pandas', 'pypdf', 'matplotlib', 'plotly', 'scipy', 'scikit-learn',
+                'tiktoken', 'tenacity']
 
 test_requirements = []
 
 setup(
     author="Marios S. Kyriakou",
     author_email='kiriakou.marios@ucy.ac.cy',
     python_requires='>=3.6',
@@ -23,14 +24,16 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     description="pdfgpt is a Python package that provides users with the ability to engage in natural language "
                 "conversations with their PDF documents.",
     entry_points={
         'console_scripts': [
             'pdfgpt=pdfgpt.cli:main',
         ],
@@ -41,10 +44,10 @@
     include_package_data=True,
     keywords='pdfgpt',
     name='pdfgpt',
     packages=find_packages(include=['pdfgpt', 'pdfgpt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Mariosmsk/pdfgpt',
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
```

### Comparing `pdfgpt-0.2.1/tests/epanet_matlab_toolkit.pdf` & `pdfgpt-0.2.2/tests/epanet_matlab_toolkit.pdf`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.1/tests/test_example.py` & `pdfgpt-0.2.2/tests/test_example.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Unit test package for pdfgpt."""
-from pdfgpt import *
-
-d = PDFBot(openai_key='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')
-
-print('Example')
-extracted_text, num_pages = d.generateText(file_path='epanet_matlab_toolkit.pdf')
-df = d.generateEmbeddings(extracted_text)
-
-print('USER: What is EPANET?')
-prompt = d.generatePrompt(df, num_pages, 'What is EPANET?')
-response = d.sendPrompt(prompt, model="gpt-3.5-turbo")
-print('AI')
-print(response, '\n')
-
-print('USER: Give me the command to load a network?')
-prompt = d.generatePrompt(df, num_pages, 'Give me the command to load a network?')
-response = d.sendPrompt(prompt, model="gpt-3.5-turbo", temperature=0.9)
-print('AI')
-print(response)
-
+"""Unit test package for pdfgpt."""
+from pdfgpt import *
+
+d = PDFBot(openai_key='OPENAI_KEY')
+
+print('Example')
+extracted_text, num_pages = d.generateText(file_path='epanet_matlab_toolkit.pdf')
+df = d.generateEmbeddings(extracted_text)
+
+print('USER: What is EPANET?')
+prompt = d.generatePrompt(df, num_pages, 'What is EPANET?')
+response = d.sendPrompt(prompt, model="gpt-3.5-turbo")
+print('AI')
+print(response, '\n')
+
+print('USER: Give me the command to load a network?')
+prompt = d.generatePrompt(df, num_pages, 'Give me the command to load a network?')
+response = d.sendPrompt(prompt, model="gpt-3.5-turbo", temperature=0.9)
+print('AI')
+print(response)
+
```

### Comparing `pdfgpt-0.2.1/tests/test_pdfgpt.py` & `pdfgpt-0.2.2/tests/test_pdfgpt.py`

 * *Files identical despite different names*

