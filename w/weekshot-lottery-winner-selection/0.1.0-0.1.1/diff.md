# Comparing `tmp/weekshot_lottery_winner_selection-0.1.0.tar.gz` & `tmp/weekshot_lottery_winner_selection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weekshot_lottery_winner_selection-0.1.0.tar", max compression
+gzip compressed data, was "weekshot_lottery_winner_selection-0.1.1.tar", max compression
```

## Comparing `weekshot_lottery_winner_selection-0.1.0.tar` & `weekshot_lottery_winner_selection-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2023-07-05 15:33:09.479107 weekshot_lottery_winner_selection-0.1.0/LICENSE
--rw-r--r--   0        0        0       35 2023-07-05 15:33:09.479107 weekshot_lottery_winner_selection-0.1.0/README.md
--rw-r--r--   0        0        0      567 2023-07-05 15:33:09.479107 weekshot_lottery_winner_selection-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      816 2023-07-05 15:33:09.479107 weekshot_lottery_winner_selection-0.1.0/weekshot_lottery_winner_selection/__init__.py
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 weekshot_lottery_winner_selection-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/LICENSE
+-rw-r--r--   0        0        0       35 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/README.md
+-rw-r--r--   0        0        0      564 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      856 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/weekshot_lottery_winner_selection/__init__.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 weekshot_lottery_winner_selection-0.1.1/PKG-INFO
```

### Comparing `weekshot_lottery_winner_selection-0.1.0/LICENSE` & `weekshot_lottery_winner_selection-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weekshot_lottery_winner_selection-0.1.0/pyproject.toml` & `weekshot_lottery_winner_selection-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "weekshot-lottery-winner-selection"
-version = "0.1.0"
+version = "0.1.1"
 description = "Weekshot Lottery Winner Selection"
 authors = ["Pavel Fedorovich <pa.fedorovich@heapix.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/Weekshot/Weekshot-Lottery-Winner-Selection"
 repository = "https://github.com/Weekshot/Weekshot-Lottery-Winner-Selection"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-requests = "^2.31.0"
+httpx = "^0.24.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `weekshot_lottery_winner_selection-0.1.0/weekshot_lottery_winner_selection/__init__.py` & `weekshot_lottery_winner_selection-0.1.1/weekshot_lottery_winner_selection/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import requests
+import httpx
 
-def generate_random_numbers(
-        api_key: str,
-        max_number: int,
-        count: int
+async def generate_random_numbers(
+    api_key: str,
+    max_number: int,
+    count: int
 ) -> list[int]:
     url = f"https://api.random.org/json-rpc/2/invoke"
     headers = {
         "Content-Type": "application/json"
     }
     payload = {
         "jsonrpc": "2.0",
@@ -17,15 +17,15 @@
             "n": count,
             "min": 1,
             "max": max_number,
             "replacement": True
         },
         "id": 1
     }
-    
-    response = requests.post(url, headers=headers, json=payload)
+    async with httpx.AsyncClient() as client:
+        response = await client.post(url, headers=headers, json=payload)
     if response.status_code == 200:
         data = response.json()
         random_numbers = data["result"]["random"]["data"]
         return random_numbers
     else:
         raise Exception("Failed to generate random numbers")
```

### Comparing `weekshot_lottery_winner_selection-0.1.0/PKG-INFO` & `weekshot_lottery_winner_selection-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: weekshot-lottery-winner-selection
-Version: 0.1.0
+Version: 0.1.1
 Summary: Weekshot Lottery Winner Selection
 Home-page: https://github.com/Weekshot/Weekshot-Lottery-Winner-Selection
 License: Apache-2.0
 Author: Pavel Fedorovich
 Author-email: pa.fedorovich@heapix.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Project-URL: Repository, https://github.com/Weekshot/Weekshot-Lottery-Winner-Selection
 Description-Content-Type: text/markdown
 
 # Weekshot-Lottery-Winner-Selection
```

