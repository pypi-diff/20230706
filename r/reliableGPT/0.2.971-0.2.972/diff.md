# Comparing `tmp/reliableGPT-0.2.971.tar.gz` & `tmp/reliableGPT-0.2.972.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.971.tar", last modified: Wed Jul  5 20:54:44 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.972.tar", last modified: Thu Jul  6 19:25:26 2023, max compression
```

## Comparing `reliableGPT-0.2.971.tar` & `reliableGPT-0.2.972.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-05 20:54:44.389678 reliableGPT-0.2.971/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.971/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-05 20:54:44.389567 reliableGPT-0.2.971/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8271 2023-07-03 21:43:04.000000 reliableGPT-0.2.971/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.971/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-05 20:54:44.387437 reliableGPT-0.2.971/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-05 20:54:44.000000 reliableGPT-0.2.971/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      514 2023-07-05 20:54:44.000000 reliableGPT-0.2.971/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-05 20:54:44.000000 reliableGPT-0.2.971/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       54 2023-07-05 20:54:44.000000 reliableGPT-0.2.971/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-05 20:54:44.000000 reliableGPT-0.2.971/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-05 20:54:44.389265 reliableGPT-0.2.971/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4210 2023-06-28 20:45:06.000000 reliableGPT-0.2.971/reliablegpt/APICallHandler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3120 2023-06-28 23:12:14.000000 reliableGPT-0.2.971/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4407 2023-06-28 20:45:06.000000 reliableGPT-0.2.971/reliablegpt/CustomQueue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    11802 2023-07-05 20:47:04.000000 reliableGPT-0.2.971/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.971/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5170 2023-07-02 02:49:46.000000 reliableGPT-0.2.971/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7119 2023-07-03 21:43:04.000000 reliableGPT-0.2.971/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      375 2023-07-05 20:54:24.000000 reliableGPT-0.2.971/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5667 2023-07-05 20:54:13.000000 reliableGPT-0.2.971/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2363 2023-07-03 21:42:46.000000 reliableGPT-0.2.971/reliablegpt/reliableQuery.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-05 20:54:44.389713 reliableGPT-0.2.971/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-07-05 20:54:00.000000 reliableGPT-0.2.971/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-06 19:25:26.693442 reliableGPT-0.2.972/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.972/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-06 19:25:26.693321 reliableGPT-0.2.972/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8271 2023-07-03 15:14:41.000000 reliableGPT-0.2.972/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.972/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-06 19:25:26.690391 reliableGPT-0.2.972/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-06 19:25:26.000000 reliableGPT-0.2.972/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-06 19:25:26.692875 reliableGPT-0.2.972/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.972/reliablegpt/APICallHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3149 2023-07-06 19:23:20.000000 reliableGPT-0.2.972/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.972/reliablegpt/CustomQueue.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    16639 2023-07-06 19:19:57.000000 reliableGPT-0.2.972/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.972/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.972/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     7483 2023-07-06 13:49:42.000000 reliableGPT-0.2.972/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      375 2023-07-06 17:39:33.000000 reliableGPT-0.2.972/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4762 2023-07-06 19:20:43.000000 reliableGPT-0.2.972/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.972/reliablegpt/reliableQuery.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-06 19:25:26.693502 reliableGPT-0.2.972/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-07-06 19:25:18.000000 reliableGPT-0.2.972/setup.py
```

### Comparing `reliableGPT-0.2.971/LICENSE` & `reliableGPT-0.2.972/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.971/README.md` & `reliableGPT-0.2.972/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.971/reliableGPT.egg-info/SOURCES.txt` & `reliableGPT-0.2.972/reliableGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.971/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.972/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.971/reliablegpt/Alerting.py` & `reliableGPT-0.2.972/reliablegpt/Alerting.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,27 +55,28 @@
     if type(user_email) == list:
       for email in user_email:
         self.user_emails.add(email)
     else:
       self.user_emails.add(user_email)
     return
 
-  def add_error(self, openai_error):
+  def add_error(self, openai_error=None, error_description=None, error_type=None):
     if openai_error != None:
       openai_error = openai_error.error  # index into the error attribute of the class
-    error_type = None  # defalt to being None
-    if openai_error != None and 'type' in openai_error:
-      error_type = openai_error['type']
+      if "type" in openai_error:
+        error_type = openai_error['type']
+    elif error_description and error_type:
+      error_type = error_type
+      openai_error = error_description
     now = datetime.datetime.now()
     curr_time = now.hour
 
     if curr_time == self.current_time_block:
       if error_type in self.unhandled_errors:
         self.unhandled_errors[error_type] += 1
-        print(f"Got unhandled error {self.unhandled_errors}")
       else:
         self.unhandled_errors[error_type] = 1
       if self.unhandled_errors[error_type] >= 5:
         self.unhandled_errors[error_type] = 0  # reset this to 0
         # cooldown for 15 minutes -> do this to prevent email spam.
         if self.set_cooldown and time.time() - self.cooldown_start_time > 900:
           self.send_alert(error_type, openai_error)
```

### Comparing `reliableGPT-0.2.971/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.972/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.971/reliablegpt/Model.py` & `reliableGPT-0.2.972/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.971/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.972/reliablegpt/RateLimitHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.971/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.972/reliablegpt/ReliableDataLoaders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-import subprocess
+# import subprocess
 
-# Libraries to install
-packages = ['langchain', 'resend', 'pypdf', 'pymupdf', 'pdfminer', 'pdfminer.six', 'unstructured']
+# # Libraries to install
+# packages = ['langchain', 'resend', 'pypdf', 'pymupdf', 'pdfminer', 'pdfminer.six', 'unstructured']
 
-# Try importing the libraries
-try:
-    import langchain
-    import resend
-    import pypdf
-    import pymupdf
-    import pdfminer
-    import pdfminer.six
-    import unstructured
-except ImportError as e:
-    print(f"Import error: {e}")
-    print("Installing required packages...")
-
-    # Install missing packages using pip
-    for package in packages:
-        try:
-            subprocess.check_call(['pip', 'install', package])
-            print(f"Successfully installed {package}")
-        except subprocess.CalledProcessError:
-            print(f"Failed to install {package}")
-
-from typing import Any
-from functools import wraps
-from langchain.document_loaders.pdf import (PyMuPDFLoader, PDFMinerLoader, PyPDFLoader, OnlinePDFLoader)
-from langchain.document_loaders.csv_loader import CSVLoader
-from langchain.document_loaders import UnstructuredURLLoader
-import resend
-from termcolor import colored
-from langchain.text_splitter import RecursiveCharacterTextSplitter
-import traceback
-import requests
-import os
-from uuid import uuid4
-from urllib.parse import urlparse
-
-pdf_modules = [
-  PyMuPDFLoader, PDFMinerLoader, PyPDFLoader, OnlinePDFLoader
-]
-
-csv_modules = [
-  CSVLoader
-]
-
-resend.api_key = "re_X1PBTBvD_5mJfFM98AuF2278fNAGfXVNV"
-
-default_text_splitter = RecursiveCharacterTextSplitter(chunk_size=3000,
-                                               chunk_overlap=200,
-                                               length_function=len)
-
-class reliableData:
-
-  def __init__(self, user_emails, priority_customers=[], metadata={}, text_splitter=None) -> None:
-    self.user_emails = user_emails
-    self.priority_customer_list = priority_customers
-    self.metadata = metadata
-    self.text_splitter = text_splitter
-    self.customer_email = None
-    pass
+# # Try importing the libraries
+# try:
+#     import langchain
+#     import resend
+#     import pypdf
+#     import pymupdf
+#     import pdfminer
+#     import pdfminer.six
+#     import unstructured
+# except ImportError as e:
+#     print(f"Import error: {e}")
+#     print("Installing required packages...")
+
+#     # Install missing packages using pip
+#     for package in packages:
+#         try:
+#             subprocess.check_call(['pip', 'install', package])
+#             print(f"Successfully installed {package}")
+#         except subprocess.CalledProcessError:
+#             print(f"Failed to install {package}")
+
+# from typing import Any
+# from functools import wraps
+# from langchain.document_loaders.pdf import (PyMuPDFLoader, PDFMinerLoader, PyPDFLoader, OnlinePDFLoader)
+# from langchain.document_loaders.csv_loader import CSVLoader
+# from langchain.document_loaders import UnstructuredURLLoader
+# import resend
+# from termcolor import colored
+# from langchain.text_splitter import RecursiveCharacterTextSplitter
+# import traceback
+# import requests
+# import os
+# from uuid import uuid4
+# from urllib.parse import urlparse
+
+# pdf_modules = [
+#   PyMuPDFLoader, PDFMinerLoader, PyPDFLoader, OnlinePDFLoader
+# ]
+
+# csv_modules = [
+#   CSVLoader
+# ]
+
+# resend.api_key = "re_X1PBTBvD_5mJfFM98AuF2278fNAGfXVNV"
+
+# default_text_splitter = RecursiveCharacterTextSplitter(chunk_size=3000,
+#                                                chunk_overlap=200,
+#                                                length_function=len)
+
+# class reliableData:
+
+#   def __init__(self, user_emails, priority_customers=[], metadata={}, text_splitter=None) -> None:
+#     self.user_emails = user_emails
+#     self.priority_customer_list = priority_customers
+#     self.metadata = metadata
+#     self.text_splitter = text_splitter
+#     self.customer_email = None
+#     pass
   
-  def set_user(self, customer_email):
-    self.customer_email = customer_email
-    return 
+#   def set_user(self, customer_email):
+#     self.customer_email = customer_email
+#     return 
   
-  def fix_malformed_url(self, url):
-    # Fix escaped characters
-    url = url.replace("\\/", "/")
-
-    # Parse URL
-    parsed_url = urlparse(url)
-
-    # If scheme is missing, add it
-    if not parsed_url.scheme:
-        url = "http://" + url
-        parsed_url = urlparse(url)
-
-    # Check if URL is valid
-    if not parsed_url.netloc:
-        return None
-    else:
-        return url
+#   def fix_malformed_url(self, url):
+#     # Fix escaped characters
+#     url = url.replace("\\/", "/")
+
+#     # Parse URL
+#     parsed_url = urlparse(url)
+
+#     # If scheme is missing, add it
+#     if not parsed_url.scheme:
+#         url = "http://" + url
+#         parsed_url = urlparse(url)
+
+#     # Check if URL is valid
+#     if not parsed_url.netloc:
+#         return None
+#     else:
+#         return url
     
-  def send_alert(self, error_type, filepath=None, web_url=None, additional_args=None):
-    print(colored("Sending alert", "magenta"))
-    # save the file
-    print(f"params: {error_type}, {filepath}, {web_url}, {additional_args}")
-    file_url = "" 
-    if filepath and isinstance(filepath, str) and os.path.exists(filepath):
-      print("INSIDE FILEPATH")
-      file_extension = os.path.splitext(filepath)[1]
-      filename = str(uuid4()) + file_extension
-      print(filename)
-      querystring = {
-        "filename": filename,
-      }
-
-      post_request = requests.post(
-          url='https://reliablegpt-logging-server-7nq8.zeet-berri.zeet.app/write_file',
-          params=querystring,
-          files={
-              'file': open(filepath, 'rb')
-          },
-      )
+#   def send_alert(self, error_type, filepath=None, web_url=None, additional_args=None):
+#     print(colored("Sending alert", "magenta"))
+#     # save the file
+#     print(f"params: {error_type}, {filepath}, {web_url}, {additional_args}")
+#     file_url = "" 
+#     if filepath and isinstance(filepath, str) and os.path.exists(filepath):
+#       print("INSIDE FILEPATH")
+#       file_extension = os.path.splitext(filepath)[1]
+#       filename = str(uuid4()) + file_extension
+#       print(filename)
+#       querystring = {
+#         "filename": filename,
+#       }
+
+#       post_request = requests.post(
+#           url='https://reliablegpt-logging-server-7nq8.zeet-berri.zeet.app/write_file',
+#           params=querystring,
+#           files={
+#               'file': open(filepath, 'rb')
+#           },
+#       )
       
-      # Get the response
-      response = post_request.json()
-      print("response: ", response)
-      file_url = response["response"]
+#       # Get the response
+#       response = post_request.json()
+#       print("response: ", response)
+#       file_url = response["response"]
     
-    print("before HTML")
-    html = """
-        <p><strong>ReliableGPT Error:</strong></p>
-        <p>A critical error occurred that ReliableGPT was unable to handle.</p>
-        <p>This error has happened for {}:</p>
-        <p><strong>{}</strong></p>
-        """.format(self.customer_email, error_type)
-
-    print(f"html: {html}")
-    if len(file_url) > 0:
-      html += """<p> Here is the <a href={}>file</a> which caused the error</p>""".format(file_url)
-
-    if web_url and len(web_url) > 0: 
-      html += """<p> Here is the url which caused the error: {}</p>""".format(web_url)
-
-    if additional_args:
-      html += """<p> Here is the additional args which got passed in: {}</p>""".format(additional_args)
-
-    # Check if the metadata exists and modify the html string
-    if self.metadata:
-      html += "<p>Here's the attached metadata: <strong>{}</strong></p>".format(self.metadata)
-
-    html += """
-    <p>Suggest a way we could cover this error with reliableGPT 💪:
-    <a href="https://github.com/BerriAI/reliableGPT/issues/new">Here</a></p>
-    <p>Join our Discord for Support:
-    <a href=" https://discord.com/invite/WXFfTeEXRh">Here</a></p>"""
-    params = {
-      "from": "krrish@berri.ai",
-      "subject": "reliableGPT 💪: {} - Unhandled Ingestion Error ".format(self.customer_email),
-      "html": html
-    }
-    print(params)
-
-    for user_email in self.user_emails:
-      params["to"] = user_email
-      print(params)
-      email = resend.Emails.send(params)
-    return
-
-  def exceptionHandler(self, error_description, filepath=None, web_url=None):
-    pages = []
-    additional_args = None
-    try: 
-      if filepath and os.path.exists(filepath):
-          if "pdf" in filepath.lower():
-              for module in pdf_modules:
-                  try:
-                      loader = module(filepath)
-                      pages = loader.load_and_split(self.text_splitter)
-                      if len(pages) > 0: # it worked!
-                          break
-                  except:
-                      pass
-          elif "csv" in filepath.lower():
-              for module in csv_modules:
-                  try:
-                      loader = module(filepath)
-                      pages = loader.load_and_split(self.text_splitter)
-                      if len(pages) > 0: # it worked!
-                          break
-                  except:
-                      pass
-      elif web_url:
-        url = self.fix_malformed_url(web_url)
-        try:
-          loader = UnstructuredURLLoader(urls=[url])
-          pages = loader.load_and_split(self.text_splitter)
-        except: 
-          pass
-      else:
-        additional_args = "Neither a valid filepath nor a web url were passed"
-    except:
-       additional_args = "Neither a valid filepath nor a web url were passed"
-       pass
+#     print("before HTML")
+#     html = """
+#         <p><strong>ReliableGPT Error:</strong></p>
+#         <p>A critical error occurred that ReliableGPT was unable to handle.</p>
+#         <p>This error has happened for {}:</p>
+#         <p><strong>{}</strong></p>
+#         """.format(self.customer_email, error_type)
+
+#     print(f"html: {html}")
+#     if len(file_url) > 0:
+#       html += """<p> Here is the <a href={}>file</a> which caused the error</p>""".format(file_url)
+
+#     if web_url and len(web_url) > 0: 
+#       html += """<p> Here is the url which caused the error: {}</p>""".format(web_url)
+
+#     if additional_args:
+#       html += """<p> Here is the additional args which got passed in: {}</p>""".format(additional_args)
+
+#     # Check if the metadata exists and modify the html string
+#     if self.metadata:
+#       html += "<p>Here's the attached metadata: <strong>{}</strong></p>".format(self.metadata)
+
+#     html += """
+#     <p>Suggest a way we could cover this error with reliableGPT 💪:
+#     <a href="https://github.com/BerriAI/reliableGPT/issues/new">Here</a></p>
+#     <p>Join our Discord for Support:
+#     <a href=" https://discord.com/invite/WXFfTeEXRh">Here</a></p>"""
+#     params = {
+#       "from": "krrish@berri.ai",
+#       "subject": "reliableGPT 💪: {} - Unhandled Ingestion Error ".format(self.customer_email),
+#       "html": html
+#     }
+#     print(params)
+
+#     for user_email in self.user_emails:
+#       params["to"] = user_email
+#       print(params)
+#       email = resend.Emails.send(params)
+#     return
+
+#   def exceptionHandler(self, error_description, filepath=None, web_url=None):
+#     pages = []
+#     additional_args = None
+#     try: 
+#       if filepath and os.path.exists(filepath):
+#           if "pdf" in filepath.lower():
+#               for module in pdf_modules:
+#                   try:
+#                       loader = module(filepath)
+#                       pages = loader.load_and_split(self.text_splitter)
+#                       if len(pages) > 0: # it worked!
+#                           break
+#                   except:
+#                       pass
+#           elif "csv" in filepath.lower():
+#               for module in csv_modules:
+#                   try:
+#                       loader = module(filepath)
+#                       pages = loader.load_and_split(self.text_splitter)
+#                       if len(pages) > 0: # it worked!
+#                           break
+#                   except:
+#                       pass
+#       elif web_url:
+#         url = self.fix_malformed_url(web_url)
+#         try:
+#           loader = UnstructuredURLLoader(urls=[url])
+#           pages = loader.load_and_split(self.text_splitter)
+#         except: 
+#           pass
+#       else:
+#         additional_args = "Neither a valid filepath nor a web url were passed"
+#     except:
+#        additional_args = "Neither a valid filepath nor a web url were passed"
+#        pass
           
-    if len(pages) == 0: # alert user
-      if filepath:
-        self.send_alert(error_type=error_description, filepath=filepath, additional_args=additional_args)
-      elif web_url:
-        self.send_alert(error_type=error_description, web_url=web_url, additional_args=additional_args)
-      else:
-        self.send_alert(error_type=error_description, additional_args=additional_args)
-    return pages
+#     if len(pages) == 0: # alert user
+#       if filepath:
+#         self.send_alert(error_type=error_description, filepath=filepath, additional_args=additional_args)
+#       elif web_url:
+#         self.send_alert(error_type=error_description, web_url=web_url, additional_args=additional_args)
+#       else:
+#         self.send_alert(error_type=error_description, additional_args=additional_args)
+#     return pages
   
-  def reliableDataLoaders(self, ingest_func, filepath, web_url):
-    try:
-       response = ingest_func
-       if response == None or (isinstance(ingest_func, list) and len(ingest_func) == 0):
-          # retry 
-          updated_response = self.exceptionHandler("error in your ingestion function", filepath=filepath, web_url=web_url)
-          if len(updated_response) == 0: # if we're not able to fix it, just return the original response
-              raise Exception()
-          return updated_response
-    except:
-       return ingest_func
-    return ingest_func
+#   def reliableDataLoaders(self, ingest_func, filepath, web_url):
+#     try:
+#        response = ingest_func
+#        if response == None or (isinstance(ingest_func, list) and len(ingest_func) == 0):
+#           # retry 
+#           updated_response = self.exceptionHandler("error in your ingestion function", filepath=filepath, web_url=web_url)
+#           if len(updated_response) == 0: # if we're not able to fix it, just return the original response
+#               raise Exception()
+#           return updated_response
+#     except:
+#        return ingest_func
+#     return ingest_func
```

### Comparing `reliableGPT-0.2.971/reliablegpt/main.py` & `reliableGPT-0.2.972/reliablegpt/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # # Prod Imports
-from reliablegpt.IndividualRequest import IndividualRequest
-from reliablegpt.RateLimitHandler import RateLimitHandler
-from reliablegpt.Model import Model
-from reliablegpt.alerting import Alerting
-from reliablegpt.reliableQuery import reliable_query
+# from reliablegpt.IndividualRequest import IndividualRequest
+# from reliablegpt.RateLimitHandler import RateLimitHandler
+# from reliablegpt.Model import Model
+# from reliablegpt.Alerting import Alerting
+# from reliablegpt.reliableQuery import reliable_query
 import requests
 
 # # Dev Imports
-# from IndividualRequest import IndividualRequest
-# from RateLimitHandler import RateLimitHandler
-# from Model import Model
-# from alerting import Alerting
+from IndividualRequest import IndividualRequest
+from Model import Model
+from Alerting import Alerting
 
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
@@ -87,17 +86,17 @@
            fallback_strategy=[
              'gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'
            ],
            graceful_string="Sorry, the OpenAI API is currently down",
            user_email="",
            user_token="",
            send_notification=True,
-           model_limits_dir={},
+           caching=False,
+           max_threads=None,
            backup_openai_key=None,
-           queue_requests=False, 
            verbose=False):
   """Determine if an instantiation is calling the rate limit handler or the individual request wrapper directly and return the correct object"""
 
   primary_email = ""  # which api key management is mapped to
   ## Add email for alerting
   if isinstance(user_email, str):
     if user_email == "":
@@ -108,35 +107,19 @@
   elif isinstance(user_email, list):
     primary_email = user_email[0]
     for email in user_email:
       alerting.add_emails(email)
 
   model = Model(openai_create_function)
   ## Route to the right object
-  if queue_requests == False:
-    return IndividualRequest(model,
-                             fallback_strategy=fallback_strategy,
-                             graceful_string=graceful_string,
-                             user_email=primary_email,
-                             user_token=user_token,
-                             logging_fn=save_request,
-                             send_notification=send_notification,
-                             backup_openai_key=backup_openai_key, 
-                             verbose=verbose)
-  elif queue_requests == True:
-    max_token_capacity = 40000
-    max_request_capacity = 200
-    ## [TODO]: Allow handling multiple model types (gpt-3.5-turbo AND gpt-4)
-    if model_limits_dir and isinstance(model_limits_dir, dict):
-      keys = list(model_limits_dir.keys())
-      max_token_capacity = model_limits_dir[keys[0]]["max_token_capacity"]
-      max_request_capacity = model_limits_dir[keys[0]]["max_request_capacity"]
-
-    return RateLimitHandler(model,
+  return IndividualRequest(model,
                             fallback_strategy=fallback_strategy,
                             graceful_string=graceful_string,
                             user_email=primary_email,
                             user_token=user_token,
+                            logging_fn=save_request,
                             send_notification=send_notification,
-                            max_request_capacity=max_request_capacity,
-                            max_token_capacity=max_token_capacity,
-                            logging_fn=save_request)
+                            backup_openai_key=backup_openai_key, 
+                            caching=caching,
+                            max_threads=max_threads,
+                            alerting=alerting,
+                            verbose=verbose)
```

### Comparing `reliableGPT-0.2.971/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.972/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*

