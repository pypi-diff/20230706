# Comparing `tmp/weekshot_lottery_winner_selection-0.1.1.tar.gz` & `tmp/weekshot_lottery_winner_selection-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weekshot_lottery_winner_selection-0.1.1.tar", max compression
+gzip compressed data, was "weekshot_lottery_winner_selection-0.1.2.tar", max compression
```

## Comparing `weekshot_lottery_winner_selection-0.1.1.tar` & `weekshot_lottery_winner_selection-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/LICENSE
--rw-r--r--   0        0        0       35 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/README.md
--rw-r--r--   0        0        0      564 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      856 2023-07-06 09:53:31.885767 weekshot_lottery_winner_selection-0.1.1/weekshot_lottery_winner_selection/__init__.py
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 weekshot_lottery_winner_selection-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-06 12:43:55.775285 weekshot_lottery_winner_selection-0.1.2/LICENSE
+-rw-r--r--   0        0        0       35 2023-07-06 12:43:55.775285 weekshot_lottery_winner_selection-0.1.2/README.md
+-rw-r--r--   0        0        0      564 2023-07-06 12:43:55.775285 weekshot_lottery_winner_selection-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      888 2023-07-06 12:43:55.775285 weekshot_lottery_winner_selection-0.1.2/weekshot_lottery_winner_selection/__init__.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 weekshot_lottery_winner_selection-0.1.2/PKG-INFO
```

### Comparing `weekshot_lottery_winner_selection-0.1.1/pyproject.toml` & `weekshot_lottery_winner_selection-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weekshot-lottery-winner-selection"
-version = "0.1.1"
+version = "0.1.2"
 description = "Weekshot Lottery Winner Selection"
 authors = ["Pavel Fedorovich <pa.fedorovich@heapix.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/Weekshot/Weekshot-Lottery-Winner-Selection"
 repository = "https://github.com/Weekshot/Weekshot-Lottery-Winner-Selection"
 include = [
```

### Comparing `weekshot_lottery_winner_selection-0.1.1/weekshot_lottery_winner_selection/__init__.py` & `weekshot_lottery_winner_selection-0.1.2/weekshot_lottery_winner_selection/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import httpx
 
 async def generate_random_numbers(
     api_key: str,
     max_number: int,
-    count: int
+    count: int,
+    unique: bool = True,
 ) -> list[int]:
     url = f"https://api.random.org/json-rpc/2/invoke"
     headers = {
         "Content-Type": "application/json"
     }
     payload = {
         "jsonrpc": "2.0",
         "method": "generateIntegers",
         "params": {
             "apiKey": api_key,
             "n": count,
             "min": 1,
             "max": max_number,
-            "replacement": True
+            "replacement": not unique
         },
         "id": 1
     }
     async with httpx.AsyncClient() as client:
         response = await client.post(url, headers=headers, json=payload)
     if response.status_code == 200:
         data = response.json()
```

### Comparing `weekshot_lottery_winner_selection-0.1.1/PKG-INFO` & `weekshot_lottery_winner_selection-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weekshot-lottery-winner-selection
-Version: 0.1.1
+Version: 0.1.2
 Summary: Weekshot Lottery Winner Selection
 Home-page: https://github.com/Weekshot/Weekshot-Lottery-Winner-Selection
 License: Apache-2.0
 Author: Pavel Fedorovich
 Author-email: pa.fedorovich@heapix.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

