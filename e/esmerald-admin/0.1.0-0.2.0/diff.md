# Comparing `tmp/esmerald_admin-0.1.0.tar.gz` & `tmp/esmerald_admin-0.2.0.tar.gz`

## Comparing `esmerald_admin-0.1.0.tar` & `esmerald_admin-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/esmerald_admin/__init__.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/esmerald_admin/application.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/esmerald_admin/py.typed
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/esmerald_admin/backends/__init__.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/esmerald_admin/backends/base.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/esmerald_admin/backends/email.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/esmerald_admin/backends/username.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/LICENSE
--rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/README.md
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10647 2020-02-02 00:00:00.000000 esmerald_admin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/__init__.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/application.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/py.typed
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/__init__.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/base.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/email.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/username.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/README.md
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/PKG-INFO
```

### Comparing `esmerald_admin-0.1.0/esmerald_admin/application.py` & `esmerald_admin-0.2.0/esmerald_admin/application.py`

 * *Files identical despite different names*

### Comparing `esmerald_admin-0.1.0/esmerald_admin/backends/base.py` & `esmerald_admin-0.2.0/esmerald_admin/backends/base.py`

 * *Files identical despite different names*

### Comparing `esmerald_admin-0.1.0/esmerald_admin/backends/email.py` & `esmerald_admin-0.2.0/esmerald_admin/backends/email.py`

 * *Files identical despite different names*

### Comparing `esmerald_admin-0.1.0/esmerald_admin/backends/username.py` & `esmerald_admin-0.2.0/esmerald_admin/backends/username.py`

 * *Files identical despite different names*

### Comparing `esmerald_admin-0.1.0/LICENSE` & `esmerald_admin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald_admin-0.1.0/README.md` & `esmerald_admin-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 </p>
 
 <p align="center">
     <em>The needed admin for Saffier ORM with Esmerald.</em>
 </p>
 
 <p align="center">
-<a href="https://github.com/tarsil/esmerald_admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" target="_blank">
-    <img src="https://github.com/tarsil/esmerald_admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" alt="Test Suite">
+<a href="https://github.com/tarsil/esmerald-admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" target="_blank">
+    <img src="https://github.com/tarsil/esmerald-admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" alt="Test Suite">
 </a>
 
 <a href="https://pypi.org/project/esmerald_admin" target="_blank">
     <img src="https://img.shields.io/pypi/v/esmerald_admin?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/esmerald_admin" target="_blank">
@@ -71,15 +71,15 @@
 SQLAdmin is expecting to use.
 
 This makes Saffier unique since you can use the declarative models for the admin and the core
 models for anything else.
 
 See the [declarative models][saffier_declarative] for more details on this.
 
-Let us create a some Saffier models first. This example assumes you use the [contrib user][https://esmerald.dev/databases/saffier/models/]
+Let us create a some Saffier models first. This example assumes you use the [contrib user](https://esmerald.dev/databases/saffier/models/)
 from Esmerald.
 
 !!! Warning
     Using the user provided by Esmerald is **not mandatory** and you can use your own design.
     The documentation uses the one provided by Esmerald as it is easier to explain and use.
 
 ```python
```

### Comparing `esmerald_admin-0.1.0/pyproject.toml` & `esmerald_admin-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
-    "esmerald[jwt]>=1.2.5",
-    "pydantic>=1.10.9,<2.0",
-    "saffier>=0.11.0",
+    "esmerald[jwt]>=1.3.0",
+    "saffier>=0.13.0",
     "sqladmin>=0.12.0,<1.0",
 ]
 keywords = ["esmerald_admin"]
 
 [project.urls]
 Homepage = "https://github.com/tarsil/esmerald-admin"
 Documentation = "https://esmerald-admin.tarsild.io"
```

### Comparing `esmerald_admin-0.1.0/PKG-INFO` & `esmerald_admin-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald_admin
-Version: 0.1.0
+Version: 0.2.0
 Summary: The needed admin for Saffier ORM with Esmerald
 Project-URL: Homepage, https://github.com/tarsil/esmerald-admin
 Project-URL: Documentation, https://esmerald-admin.tarsild.io
 Project-URL: Changelog, https://esmerald-admin.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/esmerald-admin
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -32,17 +32,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: esmerald[jwt]>=1.2.5
-Requires-Dist: pydantic<2.0,>=1.10.9
-Requires-Dist: saffier>=0.11.0
+Requires-Dist: esmerald[jwt]>=1.3.0
+Requires-Dist: saffier>=0.13.0
 Requires-Dist: sqladmin<1.0,>=0.12.0
 Provides-Extra: dev
 Requires-Dist: ipdb<1.0.0,>=0.13.13; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.3.1; extra == 'dev'
 Requires-Dist: types-python-jose>=3.3.4.7; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
@@ -72,16 +71,16 @@
 </p>
 
 <p align="center">
     <em>The needed admin for Saffier ORM with Esmerald.</em>
 </p>
 
 <p align="center">
-<a href="https://github.com/tarsil/esmerald_admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" target="_blank">
-    <img src="https://github.com/tarsil/esmerald_admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" alt="Test Suite">
+<a href="https://github.com/tarsil/esmerald-admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" target="_blank">
+    <img src="https://github.com/tarsil/esmerald-admin/workflows/Test%20Suite/badge.svg?event=push&branch=main" alt="Test Suite">
 </a>
 
 <a href="https://pypi.org/project/esmerald_admin" target="_blank">
     <img src="https://img.shields.io/pypi/v/esmerald_admin?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/esmerald_admin" target="_blank">
@@ -138,15 +137,15 @@
 SQLAdmin is expecting to use.
 
 This makes Saffier unique since you can use the declarative models for the admin and the core
 models for anything else.
 
 See the [declarative models][saffier_declarative] for more details on this.
 
-Let us create a some Saffier models first. This example assumes you use the [contrib user][https://esmerald.dev/databases/saffier/models/]
+Let us create a some Saffier models first. This example assumes you use the [contrib user](https://esmerald.dev/databases/saffier/models/)
 from Esmerald.
 
 !!! Warning
     Using the user provided by Esmerald is **not mandatory** and you can use your own design.
     The documentation uses the one provided by Esmerald as it is easier to explain and use.
 
 ```python
```

