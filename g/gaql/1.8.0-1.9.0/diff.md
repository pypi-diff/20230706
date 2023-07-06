# Comparing `tmp/gaql-1.8.0.tar.gz` & `tmp/gaql-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaql-1.8.0.tar", max compression
+gzip compressed data, was "gaql-1.9.0.tar", max compression
```

## Comparing `gaql-1.8.0.tar` & `gaql-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-01-10 12:39:04.204473 gaql-1.8.0/LICENSE
--rw-r--r--   0        0        0     2907 2023-01-10 12:39:04.204813 gaql-1.8.0/README.md
--rw-r--r--   0        0        0      244 2023-01-10 12:39:04.205018 gaql-1.8.0/gaql/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 12:39:04.205159 gaql-1.8.0/gaql/client/__init__.py
--rw-r--r--   0        0        0      864 2023-01-10 12:39:04.205324 gaql-1.8.0/gaql/client/commands.py
--rw-r--r--   0        0        0        0 2023-01-10 12:39:04.205458 gaql-1.8.0/gaql/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 12:39:04.205604 gaql-1.8.0/gaql/lib/click_decorators/__init__.py
--rw-r--r--   0        0        0     1955 2023-01-10 12:39:04.205755 gaql-1.8.0/gaql/lib/click_decorators/state.py
--rw-r--r--   0        0        0      229 2023-01-10 12:39:04.205899 gaql-1.8.0/gaql/lib/functional.py
--rw-r--r--   0        0        0        0 2023-01-10 12:39:04.206040 gaql-1.8.0/gaql/lib/google_clients/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 12:39:04.206181 gaql-1.8.0/gaql/lib/google_clients/completion/__init__.py
--rw-r--r--   0        0        0  1060111 2023-01-11 13:24:11.557830 gaql-1.8.0/gaql/lib/google_clients/completion/autocompletions.py
--rw-r--r--   0        0        0     2693 2023-01-10 12:39:04.210400 gaql-1.8.0/gaql/lib/google_clients/completion/google_completer.py
--rw-r--r--   0        0        0     1263 2023-01-10 12:39:04.210572 gaql-1.8.0/gaql/lib/google_clients/completion/trie.py
--rw-r--r--   0        0        0     2497 2023-01-11 13:24:11.558306 gaql-1.8.0/gaql/lib/google_clients/config.py
--rw-r--r--   0        0        0      650 2023-01-10 12:39:04.210917 gaql-1.8.0/gaql/lib/google_clients/queries.py
--rw-r--r--   0        0        0      816 2023-01-10 12:39:04.211070 gaql-1.8.0/gaql/lib/lexer.py
--rw-r--r--   0        0        0     2017 2023-01-10 12:39:04.211244 gaql-1.8.0/gaql/lib/output.py
--rw-r--r--   0        0        0     2221 2023-01-10 12:39:04.211438 gaql-1.8.0/gaql/lib/repl.py
--rw-r--r--   0        0        0      254 2023-01-10 12:39:04.211602 gaql-1.8.0/gaql/lib/validation.py
--rw-r--r--   0        0        0       76 2023-01-10 12:39:04.211779 gaql-1.8.0/gaql/main.py
--rw-r--r--   0        0        0     2896 2023-01-10 12:39:04.212170 gaql-1.8.0/gaql/tooling/autocomplete_generator.py
--rw-r--r--   0        0        0        0 2023-01-10 12:39:04.212403 gaql-1.8.0/gaql/tools/__init__.py
--rw-r--r--   0        0        0     1585 2023-01-10 12:39:04.212623 gaql-1.8.0/gaql/tools/commands.py
--rw-r--r--   0        0        0      571 2023-01-10 12:39:04.212862 gaql-1.8.0/gaql/tools/queries.py
--rw-r--r--   0        0        0      825 2023-01-11 13:24:11.558685 gaql-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 gaql-1.8.0/setup.py
--rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 gaql-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-06-23 08:50:49.946661 gaql-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2907 2022-10-26 14:36:46.136328 gaql-1.9.0/README.md
+-rw-r--r--   0        0        0      244 2020-06-23 08:50:49.947266 gaql-1.9.0/gaql/__init__.py
+-rw-r--r--   0        0        0        0 2020-06-23 08:50:49.947500 gaql-1.9.0/gaql/client/__init__.py
+-rw-r--r--   0        0        0      864 2020-06-23 08:50:49.947669 gaql-1.9.0/gaql/client/commands.py
+-rw-r--r--   0        0        0        0 2020-06-23 08:50:49.947806 gaql-1.9.0/gaql/lib/__init__.py
+-rw-r--r--   0        0        0        0 2020-06-23 08:50:49.947980 gaql-1.9.0/gaql/lib/click_decorators/__init__.py
+-rw-r--r--   0        0        0     1955 2020-06-23 08:50:49.948150 gaql-1.9.0/gaql/lib/click_decorators/state.py
+-rw-r--r--   0        0        0      229 2020-06-23 08:50:49.948358 gaql-1.9.0/gaql/lib/functional.py
+-rw-r--r--   0        0        0        0 2020-06-23 08:50:49.948579 gaql-1.9.0/gaql/lib/google_clients/__init__.py
+-rw-r--r--   0        0        0        0 2020-06-23 08:50:49.948849 gaql-1.9.0/gaql/lib/google_clients/completion/__init__.py
+-rw-r--r--   0        0        0  1130335 2023-07-06 11:27:21.381500 gaql-1.9.0/gaql/lib/google_clients/completion/autocompletions.py
+-rw-r--r--   0        0        0     2693 2022-10-26 14:36:46.140336 gaql-1.9.0/gaql/lib/google_clients/completion/google_completer.py
+-rw-r--r--   0        0        0     1263 2020-06-23 08:50:49.954445 gaql-1.9.0/gaql/lib/google_clients/completion/trie.py
+-rw-r--r--   0        0        0     2497 2023-07-06 10:02:23.405388 gaql-1.9.0/gaql/lib/google_clients/config.py
+-rw-r--r--   0        0        0      650 2022-10-26 14:36:46.140780 gaql-1.9.0/gaql/lib/google_clients/queries.py
+-rw-r--r--   0        0        0      816 2020-06-23 08:50:49.964917 gaql-1.9.0/gaql/lib/lexer.py
+-rw-r--r--   0        0        0     2017 2022-10-26 14:36:46.141481 gaql-1.9.0/gaql/lib/output.py
+-rw-r--r--   0        0        0     2221 2022-10-26 14:36:46.141719 gaql-1.9.0/gaql/lib/repl.py
+-rw-r--r--   0        0        0      254 2020-06-23 08:50:49.965705 gaql-1.9.0/gaql/lib/validation.py
+-rw-r--r--   0        0        0       76 2020-06-23 08:50:49.966028 gaql-1.9.0/gaql/main.py
+-rw-r--r--   0        0        0     2896 2022-10-26 14:36:46.141964 gaql-1.9.0/gaql/tooling/autocomplete_generator.py
+-rw-r--r--   0        0        0        0 2020-06-23 08:50:49.966545 gaql-1.9.0/gaql/tools/__init__.py
+-rw-r--r--   0        0        0     1585 2020-06-23 08:50:49.966715 gaql-1.9.0/gaql/tools/commands.py
+-rw-r--r--   0        0        0      571 2022-10-26 14:36:46.142196 gaql-1.9.0/gaql/tools/queries.py
+-rw-r--r--   0        0        0      824 2023-07-06 09:57:48.272156 gaql-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 gaql-1.9.0/PKG-INFO
```

### Comparing `gaql-1.8.0/LICENSE` & `gaql-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/README.md` & `gaql-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/client/commands.py` & `gaql-1.9.0/gaql/client/commands.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/lib/click_decorators/state.py` & `gaql-1.9.0/gaql/lib/click_decorators/state.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/lib/google_clients/completion/autocompletions.py` & `gaql-1.9.0/gaql/lib/google_clients/completion/autocompletions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
```

### Comparing `gaql-1.8.0/gaql/lib/google_clients/completion/google_completer.py` & `gaql-1.9.0/gaql/lib/google_clients/completion/google_completer.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/lib/google_clients/completion/trie.py` & `gaql-1.9.0/gaql/lib/google_clients/completion/trie.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/lib/google_clients/config.py` & `gaql-1.9.0/gaql/lib/google_clients/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,12 +70,12 @@
 def setup_client():
     from google.ads.googleads.client import GoogleAdsClient
 
     return GoogleAdsClient.load_from_dict(load_credentials())
 
 
 def setup_ads_service(client):
-    return client.get_service("GoogleAdsService", version="v12")
+    return client.get_service("GoogleAdsService", version="v14")
 
 
 def setup_fields_service(client):
-    return client.get_service("GoogleAdsFieldService", version="v12")
+    return client.get_service("GoogleAdsFieldService", version="v14")
```

### Comparing `gaql-1.8.0/gaql/lib/google_clients/queries.py` & `gaql-1.9.0/gaql/lib/google_clients/queries.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/lib/lexer.py` & `gaql-1.9.0/gaql/lib/lexer.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/lib/output.py` & `gaql-1.9.0/gaql/lib/output.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/lib/repl.py` & `gaql-1.9.0/gaql/lib/repl.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/tooling/autocomplete_generator.py` & `gaql-1.9.0/gaql/tooling/autocomplete_generator.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/tools/commands.py` & `gaql-1.9.0/gaql/tools/commands.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/gaql/tools/queries.py` & `gaql-1.9.0/gaql/tools/queries.py`

 * *Files identical despite different names*

### Comparing `gaql-1.8.0/pyproject.toml` & `gaql-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "gaql"
-version = "1.8.0"
+version = "1.9.0"
 description = "A command line interface to the Google Ads Query Language (GAQL). Run with `gaql` or `gaql-tools`"
 
 authors = [
   "Ben Ryves <bryves@gmail.com>"
 ]
 
 readme = 'README.md'
@@ -21,15 +21,15 @@
 gaql = 'gaql.client.commands:cli'
 gaql-tools = 'gaql.tools.commands:tools'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 toml = "^0.10.1"
 
-google-ads={ version = "19.0.0" }
+google-ads={ version = "21.2.0" }
 click={ version = "^8.0.3" }
 prompt_toolkit={ version = "^3.0.22" }
 pygments={ version = "^2.10.0" }
 
 [tool.poetry.dev-dependencies]
-black = "^22.10"
+black = "^23.3"
 flake8 = "^5.0.4"
```

### Comparing `gaql-1.8.0/PKG-INFO` & `gaql-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gaql
-Version: 1.8.0
+Version: 1.9.0
 Summary: A command line interface to the Google Ads Query Language (GAQL). Run with `gaql` or `gaql-tools`
 Home-page: https://github.com/getyourguide/gaql-cli
 Keywords: gaql,google-ads,cli
 Author: Ben Ryves
 Author-email: bryves@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: google-ads (==19.0.0)
+Requires-Dist: google-ads (==21.2.0)
 Requires-Dist: prompt_toolkit (>=3.0.22,<4.0.0)
 Requires-Dist: pygments (>=2.10.0,<3.0.0)
 Requires-Dist: toml (>=0.10.1,<0.11.0)
 Project-URL: Repository, https://github.com/getyourguide/gaql-cli
 Description-Content-Type: text/markdown
 
 # GAQL CLI
```
