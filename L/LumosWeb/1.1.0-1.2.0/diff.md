# Comparing `tmp/LumosWeb-1.1.0.tar.gz` & `tmp/LumosWeb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-1.1.0.tar", last modified: Fri Jun 23 09:18:11 2023, max compression
+gzip compressed data, was "LumosWeb-1.2.0.tar", last modified: Thu Jul  6 08:21:56 2023, max compression
```

## Comparing `LumosWeb-1.1.0.tar` & `LumosWeb-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 09:18:11.147117 LumosWeb-1.1.0/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 09:18:10.807735 LumosWeb-1.1.0/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.1.0/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5438 2023-06-03 13:53:15.000000 LumosWeb-1.1.0/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.1.0/LumosWeb/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.1.0/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6349 2023-06-07 07:36:56.000000 LumosWeb-1.1.0/LumosWeb/orm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.1.0/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 09:18:11.082922 LumosWeb-1.1.0/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6269 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-23 09:18:10.000000 LumosWeb-1.1.0/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-06-23 09:18:10.000000 LumosWeb-1.1.0/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6269 2023-06-23 09:18:11.139455 LumosWeb-1.1.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6174 2023-06-23 09:17:18.000000 LumosWeb-1.1.0/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-23 09:18:11.150378 LumosWeb-1.1.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-06-22 16:12:27.000000 LumosWeb-1.1.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:21:56.210619 LumosWeb-1.2.0/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:21:55.802714 LumosWeb-1.2.0/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.2.0/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6340 2023-07-05 15:32:54.000000 LumosWeb-1.2.0/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.2.0/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.2.0/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6349 2023-06-07 07:36:56.000000 LumosWeb-1.2.0/LumosWeb/orm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.2.0/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:21:56.125111 LumosWeb-1.2.0/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6494 2023-07-06 08:21:54.000000 LumosWeb-1.2.0/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-07-06 08:21:55.000000 LumosWeb-1.2.0/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-06 08:21:54.000000 LumosWeb-1.2.0/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-07-06 08:21:54.000000 LumosWeb-1.2.0/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      138 2023-07-06 08:21:54.000000 LumosWeb-1.2.0/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-07-06 08:21:54.000000 LumosWeb-1.2.0/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6494 2023-07-06 08:21:56.199243 LumosWeb-1.2.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6412 2023-07-06 08:20:05.000000 LumosWeb-1.2.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-06 08:21:56.215717 LumosWeb-1.2.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1891 2023-07-06 08:21:28.000000 LumosWeb-1.2.0/setup.py
```

### Comparing `LumosWeb-1.1.0/LumosWeb/api.py` & `LumosWeb-1.2.0/LumosWeb/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from wsgiadapter import WSGIAdapter as RequestsWSGIAdapter
 from wsgiref.simple_server import make_server
 import os
 from jinja2 import Environment, FileSystemLoader
 from whitenoise import WhiteNoise
 from .middleware import Middleware
 from .response import Response
+import markdown
 
 class API:
     def __init__(self, templates_dir="templates", static_dir="static"):
         self.routes = {}  # dictionary of routes and handlers, path as keys and handlers as values
 
         self.templates_env = Environment(
             loader = FileSystemLoader(os.path.abspath(templates_dir))
@@ -98,15 +99,33 @@
         session = RequestsSession()
         session.mount(prefix=base_url, adapter=RequestsWSGIAdapter(self))
         return session
     
     def template(self, template_name, context=None):
         if context is None:
             context = {}
-        return self.templates_env.get_template(template_name).render(**context)
+
+        template = self.templates_env.get_template(template_name)
+        rendered_template = template.render(**context)
+
+        # Check if the file ends with .md extension
+        if template_name.endswith('.md'):
+            # Convert the rendered template to HTML using Markdown
+            converted_html = markdown.markdown(rendered_template, extensions=['fenced_code', 'codehilite', 'tables'])
+
+            # Read the content of convert.html
+            convert_template_path = os.path.join(os.path.dirname(__file__), 'md_to_html.html')
+            with open(convert_template_path, 'r') as convert_template_file:
+                convert_template_content = convert_template_file.read()
+
+            # Replace the placeholder with the converted HTML content
+            rendered_convert_template = convert_template_content.replace('{{ markdown_content }}', converted_html)
+            return rendered_convert_template
+        
+        return rendered_template
     
     def add_exception_handler(self, exception_handler):
         self.exception_handler = exception_handler
 
     def add_middleware(self, middleware_cls):
         self.middleware.add(middleware_cls)
```

### Comparing `LumosWeb-1.1.0/LumosWeb/cli.py` & `LumosWeb-1.2.0/LumosWeb/cli.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.1.0/LumosWeb/middleware.py` & `LumosWeb-1.2.0/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.1.0/LumosWeb/orm.py` & `LumosWeb-1.2.0/LumosWeb/orm.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.1.0/LumosWeb/response.py` & `LumosWeb-1.2.0/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.1.0/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-1.2.0/LumosWeb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.1.0
+Version: 1.2.0
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
@@ -92,21 +92,25 @@
 ```
 
 ## Templates
 The default folder for templates is `templates`. You can change it when initializing the main `API()` class:
 ```python
 app = API(templates_dir="templates_dir_name")
 ```
-Then you can use HTML files in that folder like so in a handler:
+Then you can use HTML or Markdown files in that folder like so in a handler:
 
 ```python
 @app.route("/show/template")
 def handler_with_template(req, resp):
     resp.html = app.template(
         "example.html", context={"title": "Awesome Framework", "body": "welcome to the future!"})
+
+@app.route("/md-files", allowed_methods=["get"])
+def index(req, resp):
+    resp.html = app.template("index.md")
 ```
 
 ## Static Files
 
 Just like templates, the default folder for static files is `static` and you can override it:
 ```python
 app = API(static_dir="static_dir_name")
@@ -150,24 +154,29 @@
 
 app.add_middleware(SimpleCustomMiddleware)
 ```
 
  ### Database
  You can create custom middleware classes by inheriting from the `LumosWeb.orm.Database` class
  First create models file and create a class for each table in the database
- models.py
+
  ```python
+# models.py
+
 from LumosWeb.orm import Table, Column
+
 class Book(Table):
     author = Column(str)
     name = Column(str)
  ```
 Then create a storage file and import the models
-storage.py
+
 ```python
+# storage.py
+
 from models import Book
 
 class BookStorage:
     _id = 0
 
     def __init__(self):
         self._books = []
@@ -190,19 +199,23 @@
         return book
 
     def delete(self, id):
         for ind, book in enumerate(self._books):
             if book.id == id:
                 del self._books[ind]
 ```
-Then use them
-app.py
+Now you can use them
+
  ```python
+ # app.py
+
 from LumosWeb.orm import Database
+
 db = Database("./lumos.db")  # lumos.db is the name of the database file
+# which will be created in the current directory (if it doesn't exist already)
 db.create(Book)
 
 @app.route("/", allowed_methods=["get"])
 def index(req, resp):
     books = db.all(Book)
     resp.html = app.template("index.html", context={"books": books})
```

### Comparing `LumosWeb-1.1.0/PKG-INFO` & `LumosWeb-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.1.0
+Version: 1.2.0
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
@@ -92,21 +92,25 @@
 ```
 
 ## Templates
 The default folder for templates is `templates`. You can change it when initializing the main `API()` class:
 ```python
 app = API(templates_dir="templates_dir_name")
 ```
-Then you can use HTML files in that folder like so in a handler:
+Then you can use HTML or Markdown files in that folder like so in a handler:
 
 ```python
 @app.route("/show/template")
 def handler_with_template(req, resp):
     resp.html = app.template(
         "example.html", context={"title": "Awesome Framework", "body": "welcome to the future!"})
+
+@app.route("/md-files", allowed_methods=["get"])
+def index(req, resp):
+    resp.html = app.template("index.md")
 ```
 
 ## Static Files
 
 Just like templates, the default folder for static files is `static` and you can override it:
 ```python
 app = API(static_dir="static_dir_name")
@@ -150,24 +154,29 @@
 
 app.add_middleware(SimpleCustomMiddleware)
 ```
 
  ### Database
  You can create custom middleware classes by inheriting from the `LumosWeb.orm.Database` class
  First create models file and create a class for each table in the database
- models.py
+
  ```python
+# models.py
+
 from LumosWeb.orm import Table, Column
+
 class Book(Table):
     author = Column(str)
     name = Column(str)
  ```
 Then create a storage file and import the models
-storage.py
+
 ```python
+# storage.py
+
 from models import Book
 
 class BookStorage:
     _id = 0
 
     def __init__(self):
         self._books = []
@@ -190,19 +199,23 @@
         return book
 
     def delete(self, id):
         for ind, book in enumerate(self._books):
             if book.id == id:
                 del self._books[ind]
 ```
-Then use them
-app.py
+Now you can use them
+
  ```python
+ # app.py
+
 from LumosWeb.orm import Database
+
 db = Database("./lumos.db")  # lumos.db is the name of the database file
+# which will be created in the current directory (if it doesn't exist already)
 db.create(Book)
 
 @app.route("/", allowed_methods=["get"])
 def index(req, resp):
     books = db.all(Book)
     resp.html = app.template("index.html", context={"books": books})
```

### Comparing `LumosWeb-1.1.0/README.md` & `LumosWeb-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -80,21 +80,25 @@
 ```
 
 ## Templates
 The default folder for templates is `templates`. You can change it when initializing the main `API()` class:
 ```python
 app = API(templates_dir="templates_dir_name")
 ```
-Then you can use HTML files in that folder like so in a handler:
+Then you can use HTML or Markdown files in that folder like so in a handler:
 
 ```python
 @app.route("/show/template")
 def handler_with_template(req, resp):
     resp.html = app.template(
         "example.html", context={"title": "Awesome Framework", "body": "welcome to the future!"})
+
+@app.route("/md-files", allowed_methods=["get"])
+def index(req, resp):
+    resp.html = app.template("index.md")
 ```
 
 ## Static Files
 
 Just like templates, the default folder for static files is `static` and you can override it:
 ```python
 app = API(static_dir="static_dir_name")
@@ -138,24 +142,29 @@
 
 app.add_middleware(SimpleCustomMiddleware)
 ```
 
  ### Database
  You can create custom middleware classes by inheriting from the `LumosWeb.orm.Database` class
  First create models file and create a class for each table in the database
- models.py
+
  ```python
+# models.py
+
 from LumosWeb.orm import Table, Column
+
 class Book(Table):
     author = Column(str)
     name = Column(str)
  ```
 Then create a storage file and import the models
-storage.py
+
 ```python
+# storage.py
+
 from models import Book
 
 class BookStorage:
     _id = 0
 
     def __init__(self):
         self._books = []
@@ -178,19 +187,23 @@
         return book
 
     def delete(self, id):
         for ind, book in enumerate(self._books):
             if book.id == id:
                 del self._books[ind]
 ```
-Then use them
-app.py
+Now you can use them
+
  ```python
+ # app.py
+
 from LumosWeb.orm import Database
+
 db = Database("./lumos.db")  # lumos.db is the name of the database file
+# which will be created in the current directory (if it doesn't exist already)
 db.create(Book)
 
 @app.route("/", allowed_methods=["get"])
 def index(req, resp):
     books = db.all(Book)
     resp.html = app.template("index.html", context={"books": books})
```

### Comparing `LumosWeb-1.1.0/setup.py` & `LumosWeb-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.1.0"
+VERSION = "1.2.0"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
     "WebOb==1.8.7",
     "whitenoise==6.4.0",
+    "Markdown==3.4.3",
+    "Pygments==2.15.1"
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
```

