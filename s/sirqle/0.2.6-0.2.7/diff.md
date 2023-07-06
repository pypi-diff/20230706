# Comparing `tmp/sirqle-0.2.6.tar.gz` & `tmp/sirqle-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirqle-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sirqle-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sirqle-0.2.6.tar` & `sirqle-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.2.6/.github/workflows/bump.yml
--rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.2.6/.gitignore
--rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      946 2023-06-09 17:07:33.977131 sirqle-0.2.6/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-05-16 15:49:30.858005 sirqle-0.2.6/LICENSE
--rw-r--r--   0        0        0     1089 2023-06-06 09:14:00.389308 sirqle-0.2.6/Makefile
--rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.2.6/README.md
--rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.2.6/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.2.6/docs/index.md
--rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.2.6/docs/reference.md
--rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.2.6/mkdocs.yml
--rw-r--r--   0        0        0     1336 2023-07-05 14:34:52.817793 sirqle-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.2.6/requirements.txt
--rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.2.6/requirements_dev.txt
--rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.2.6/setup.py
--rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.2.6/src/sirqle/__init__.py
--rw-r--r--   0        0        0    10952 2023-06-30 13:09:06.442570 sirqle-0.2.6/src/sirqle/query.py
--rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.2.6/tests/test_create.py
--rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.2.6/tests/test_insert.py
--rw-r--r--   0        0        0     4317 1970-01-01 00:00:00.000000 sirqle-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.2.7/.github/workflows/bump.yml
+-rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      946 2023-06-09 17:07:33.977131 sirqle-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-16 15:49:30.858005 sirqle-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1089 2023-06-06 09:14:00.389308 sirqle-0.2.7/Makefile
+-rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.2.7/README.md
+-rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.2.7/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.2.7/docs/index.md
+-rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.2.7/docs/reference.md
+-rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.2.7/mkdocs.yml
+-rw-r--r--   0        0        0     1336 2023-07-06 09:28:04.124333 sirqle-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.2.7/requirements.txt
+-rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.2.7/requirements_dev.txt
+-rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.2.7/setup.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.2.7/src/sirqle/__init__.py
+-rw-r--r--   0        0        0    10952 2023-07-06 09:08:42.384791 sirqle-0.2.7/src/sirqle/query.py
+-rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.2.7/tests/test_create.py
+-rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.2.7/tests/test_insert.py
+-rw-r--r--   0        0        0     4317 1970-01-01 00:00:00.000000 sirqle-0.2.7/PKG-INFO
```

### Comparing `sirqle-0.2.6/.github/workflows/bump.yml` & `sirqle-0.2.7/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/.gitignore` & `sirqle-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/.pre-commit-config.yaml` & `sirqle-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/CHANGELOG.md` & `sirqle-0.2.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/LICENSE` & `sirqle-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/Makefile` & `sirqle-0.2.7/Makefile`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/README.md` & `sirqle-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/docs/gen_ref_pages.py` & `sirqle-0.2.7/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/docs/index.md` & `sirqle-0.2.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/pyproject.toml` & `sirqle-0.2.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sirqle"
-version = "0.2.6"
+version = "0.2.7"
 authors = [{ name = "Pythia Dev Team", email = "dev@pythia.social" }]
 description = "SurrealDB Query Interface"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["python-dotenv", "surrealdb>=0.3.0"]
 license = { file = "LICENSE" }
 [project.urls]
@@ -49,15 +49,15 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.6"
+version = "0.2.7"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 bump_message = "bump: $current_version → $new_version [skip ci]"
 
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
```

### Comparing `sirqle-0.2.6/requirements_dev.txt` & `sirqle-0.2.7/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/src/sirqle/query.py` & `sirqle-0.2.7/src/sirqle/query.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,26 +63,14 @@
                 password=password,
             )
         elif url:
             scheme = str(urlparse(url).scheme)
             if scheme in ["wss", "ws"]:
                 self.client = CLIENT[scheme](url=url)
 
-    async def signup(self, user: str, password: str) -> str:
-        if isinstance(self.client, Surreal):
-            if self.client.client_state != ConnectionState.CONNECTED:
-                await self.client.connect()
-        return await self.client.signup({"user": user, "pass": password})
-
-    async def signin(self, user: str, password: str) -> str:
-        if isinstance(self.client, Surreal):
-            if self.client.client_state != ConnectionState.CONNECTED:
-                await self.client.connect()
-        return await self.client.signin({"user": user, "pass": password})
-
 
 class Query:
     def __init__(self, config: Config | None = None):
         """Create a `Query` class
 
         The Query module aims to replace the standard SurrealQL and make it more Python
             friendly. Internally it constructs a SurrealQL string from method chaining
@@ -353,14 +341,26 @@
                 url=self.client._url,
                 namespace=ns,
                 database=db,
                 username=self.client._username,
                 password=self.client._password,
             )
 
+    async def signup(self, user: str, password: str) -> str:
+        if isinstance(self.client, Surreal):
+            if self.client.client_state != ConnectionState.CONNECTED:
+                await self.client.connect()
+        return await self.client.signup({"user": user, "pass": password})
+
+    async def signin(self, user: str, password: str) -> str:
+        if isinstance(self.client, Surreal):
+            if self.client.client_state != ConnectionState.CONNECTED:
+                await self.client.connect()
+        return await self.client.signin({"user": user, "pass": password})
+
     # HACK:
     def __repr__(self):
         self._end()
         return self.query
 
     def __getitem__(self, key):
         return self.query[key]
```

### Comparing `sirqle-0.2.6/tests/test_create.py` & `sirqle-0.2.7/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/tests/test_insert.py` & `sirqle-0.2.7/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.6/PKG-INFO` & `sirqle-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirqle
-Version: 0.2.6
+Version: 0.2.7
 Summary: SurrealDB Query Interface
 Author-email: Pythia Dev Team <dev@pythia.social>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: surrealdb>=0.3.0
 Requires-Dist: pre-commit ; extra == "dev"
```

