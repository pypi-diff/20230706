# Comparing `tmp/python_tss_sdk-1.2.1.tar.gz` & `tmp/python_tss_sdk-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tss_sdk-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "python_tss_sdk-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `python_tss_sdk-1.2.1.tar` & `python_tss_sdk-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      332 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      582 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      489 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/ISSUE_TEMPLATE/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      742 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      536 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      612 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      895 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0     1984 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.gitignore
--rw-r--r--   0        0        0      541 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.whitesource
--rw-r--r--   0        0        0     1051 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/LICENSE
--rw-r--r--   0        0        0     6252 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/README.md
--rw-r--r--   0        0        0      818 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/conftest.py
--rw-r--r--   0        0        0       69 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/delinea/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/delinea/secrets/__init__.py
--rw-r--r--   0        0        0    15995 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/delinea/secrets/server.py
--rw-r--r--   0        0        0      965 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/example.py
--rw-r--r--   0        0        0      638 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      128 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/renovate.json
--rw-r--r--   0        0        0       53 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/requirements.txt
--rw-r--r--   0        0        0     1774 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/tests/test_server.py
--rw-r--r--   0        0        0      621 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/tox.ini
--rw-r--r--   0        0        0     6829 1970-01-01 00:00:00.000000 python_tss_sdk-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      332 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      582 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      489 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.github/ISSUE_TEMPLATE/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      742 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      536 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      612 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      895 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0     1984 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.gitignore
+-rw-r--r--   0        0        0      541 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/.whitesource
+-rw-r--r--   0        0        0     1051 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/LICENSE
+-rw-r--r--   0        0        0     6252 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/README.md
+-rw-r--r--   0        0        0      818 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/conftest.py
+-rw-r--r--   0        0        0       69 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/delinea/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/delinea/secrets/__init__.py
+-rw-r--r--   0        0        0    16548 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/delinea/secrets/server.py
+-rw-r--r--   0        0        0      965 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/example.py
+-rw-r--r--   0        0        0      638 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-07-06 14:07:04.515014 python_tss_sdk-1.2.2/renovate.json
+-rw-r--r--   0        0        0       53 2023-07-06 14:07:04.519014 python_tss_sdk-1.2.2/requirements.txt
+-rw-r--r--   0        0        0     1774 2023-07-06 14:07:04.519014 python_tss_sdk-1.2.2/tests/test_server.py
+-rw-r--r--   0        0        0      621 2023-07-06 14:07:04.519014 python_tss_sdk-1.2.2/tox.ini
+-rw-r--r--   0        0        0     6829 1970-01-01 00:00:00.000000 python_tss_sdk-1.2.2/PKG-INFO
```

### Comparing `python_tss_sdk-1.2.1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md` & `python_tss_sdk-1.2.2/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md` & `python_tss_sdk-1.2.2/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/.github/workflows/lint.yml` & `python_tss_sdk-1.2.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/.github/workflows/release.yml` & `python_tss_sdk-1.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/.github/workflows/run_tests.yml` & `python_tss_sdk-1.2.2/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/.gitignore` & `python_tss_sdk-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/.whitesource` & `python_tss_sdk-1.2.2/.whitesource`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/LICENSE` & `python_tss_sdk-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/README.md` & `python_tss_sdk-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/conftest.py` & `python_tss_sdk-1.2.2/conftest.py`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/delinea/secrets/server.py` & `python_tss_sdk-1.2.2/delinea/secrets/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,20 +336,27 @@
             secret = json.loads(response)
         except json.JSONDecodeError:
             raise SecretServerError(response)
 
         if fetch_file_attachments:
             for item in secret["items"]:
                 if item["fileAttachmentId"]:
-                    item["itemValue"] = self.process(
-                        requests.get(
-                            f"{self.api_url}/secrets/{id}/fields/{item['slug']}",
-                            headers=self.headers(),
+                    endpoint_url = f"{self.api_url}/secrets/{id}/fields/{item['slug']}"
+                    if query_params is None:
+                        item["itemValue"] = self.process(
+                            requests.get(endpoint_url, headers=self.headers())
+                        )
+                    else:
+                        item["itemValue"] = self.process(
+                            requests.get(
+                                endpoint_url,
+                                params=query_params,
+                                headers=self.headers(),
+                            )
                         )
-                    )
         return secret
 
     def get_secret_by_path(self, secret_path, fetch_file_attachments=True):
         """Gets a secret by path
 
         :param secret_path: full path of the secret
         :type secret_path: str
@@ -404,14 +411,18 @@
         :raise: :class:`SecretServerAccessError` when the caller does not have
                 permission to access the secret
         :raise: :class:`SecretServerError` when the REST API call fails for
                 any other reason
         """
 
         params = {"filter.folderId": folder_id}
+        endpoint_url = f"{self.api_url}/secrets/search-total"
+        params["take"] = self.process(
+            requests.get(endpoint_url, params=params, headers=self.headers())
+        ).text
         response = self.search_secrets(query_params=params)
 
         try:
             secrets = json.loads(response)
         except json.JSONDecodeError:
             raise SecretServerError(response)
```

### Comparing `python_tss_sdk-1.2.1/example.py` & `python_tss_sdk-1.2.2/example.py`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/pyproject.toml` & `python_tss_sdk-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/tests/test_server.py` & `python_tss_sdk-1.2.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/tox.ini` & `python_tss_sdk-1.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `python_tss_sdk-1.2.1/PKG-INFO` & `python_tss_sdk-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tss-sdk
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Delinea Secret Server Python SDK
 Author: Delinea Integrations
 Author-email: GitHub@delinea.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

