# Comparing `tmp/KucoinPy-0.0.2.tar.gz` & `tmp/KucoinPy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KucoinPy-0.0.2.tar", last modified: Wed Jun 14 18:24:35 2023, max compression
+gzip compressed data, was "KucoinPy-0.0.3.tar", last modified: Thu Jul  6 13:50:41 2023, max compression
```

## Comparing `KucoinPy-0.0.2.tar` & `KucoinPy-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 18:24:35.887347 KucoinPy-0.0.2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 18:24:35.885065 KucoinPy-0.0.2/KucoinPy/
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-06-11 17:55:30.000000 KucoinPy-0.0.2/KucoinPy/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      860 2023-06-04 20:07:32.000000 KucoinPy-0.0.2/KucoinPy/classes.py
--rwxrwxrwx   0 root         (0) root         (0)     3314 2023-06-11 10:07:52.000000 KucoinPy-0.0.2/KucoinPy/http.py
--rwxrwxrwx   0 root         (0) root         (0)    19127 2023-06-14 18:22:20.000000 KucoinPy-0.0.2/KucoinPy/wrapper.py
--rwxrwxrwx   0 root         (0) root         (0)     1937 2023-05-28 08:51:12.000000 KucoinPy-0.0.2/KucoinPy/ws.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 18:24:35.886661 KucoinPy-0.0.2/KucoinPy.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4875 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-14 18:24:35.000000 KucoinPy-0.0.2/KucoinPy.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)    18092 2023-06-08 16:53:44.000000 KucoinPy-0.0.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     4875 2023-06-14 18:24:35.887087 KucoinPy-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4291 2023-06-11 17:56:10.000000 KucoinPy-0.0.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-14 18:24:35.887424 KucoinPy-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      789 2023-06-14 18:24:06.000000 KucoinPy-0.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 13:50:41.338022 KucoinPy-0.0.3/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 13:50:41.335659 KucoinPy-0.0.3/KucoinPy/
+-rwxrwxrwx   0 root         (0) root         (0)      117 2023-06-11 17:55:30.000000 KucoinPy-0.0.3/KucoinPy/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      860 2023-06-04 20:07:32.000000 KucoinPy-0.0.3/KucoinPy/classes.py
+-rwxrwxrwx   0 root         (0) root         (0)     3366 2023-06-30 13:13:04.000000 KucoinPy-0.0.3/KucoinPy/http.py
+-rwxrwxrwx   0 root         (0) root         (0)    19201 2023-06-29 16:29:21.000000 KucoinPy-0.0.3/KucoinPy/wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1937 2023-05-28 08:51:12.000000 KucoinPy-0.0.3/KucoinPy/ws.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-06 13:50:41.337346 KucoinPy-0.0.3/KucoinPy.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4875 2023-07-06 13:50:41.000000 KucoinPy-0.0.3/KucoinPy.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-07-06 13:50:41.000000 KucoinPy-0.0.3/KucoinPy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-06 13:50:41.000000 KucoinPy-0.0.3/KucoinPy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-07-06 13:50:41.000000 KucoinPy-0.0.3/KucoinPy.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-07-06 13:50:41.000000 KucoinPy-0.0.3/KucoinPy.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)    18092 2023-06-08 16:53:44.000000 KucoinPy-0.0.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     4875 2023-07-06 13:50:41.337801 KucoinPy-0.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4291 2023-06-11 17:56:10.000000 KucoinPy-0.0.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-06 13:50:41.338095 KucoinPy-0.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      789 2023-07-06 13:49:18.000000 KucoinPy-0.0.3/setup.py
```

### Comparing `KucoinPy-0.0.2/KucoinPy/classes.py` & `KucoinPy-0.0.3/KucoinPy/classes.py`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.2/KucoinPy/http.py` & `KucoinPy-0.0.3/KucoinPy/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 hashlib.sha256,
             ).digest()
         ).decode(),
         "KC-API-TIMESTAMP": now,
         "KC-API-KEY": kc_api_key,
         "KC-API-PASSPHRASE": PASSPHRASE,
         "KC-API-KEY-VERSION": "2",
-    }
+    }, payload
 
 
 def make_PASSPHRASE(secret, passphrase):
     return base64.b64encode(hmac.new(secret.encode(), passphrase.encode(), hashlib.sha256).digest()).decode()
 
 
 class Response:
@@ -79,14 +79,15 @@
                 if data:
                     return Response(data)
                 raise TimeoutError("Connection timed out")
             data += response
 
     def send(self, method: str, location: str, payload: dict = {}, heads_only=False) -> None:
         headers, payload = get_headers(self.kc_api_secret, self.kc_api_key, self.PASSPHRASE, method, location, payload)
+        headers["Host"] = "api.kucoin.com"
         if heads_only:
             return headers
 
         d = "\r\n"
         if payload:
             req = f"{method.upper()} {location} HTTP/1.1\r\n{d.join([f'{a}: {b}' for a, b in headers.items()])}\r\nContent-Type: application/json\r\nContent-Length: {len(payload)}\r\n\r\n"
             req = req.encode() + payload
```

### Comparing `KucoinPy-0.0.2/KucoinPy/wrapper.py` & `KucoinPy-0.0.3/KucoinPy/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,27 +521,27 @@
                 "/api/v1/accounts",
             )
         except Exception as e:
             self.logger.log(
                 "WARNING",
                 "Balance maintainence",
                 msg="Failed to get balance",
-                extras={"error": e},
+                extras={"error": e, "traceback": traceback.format_exc()},
             )
             return self.get_balance(retries - 1)
 
         try:
             resp = sock.recv()
             data = resp.json()["data"]
         except Exception as e:
             self.logger.log(
                 "WARNING",
                 "Balance maintainence",
                 msg="Failed to get balance",
-                extras={"error": e},
+                extras={"error": e, "traceback": traceback.format_exc()},
             )
             return self.get_balance(retries - 1)
 
         for entry in data:
             if entry["type"] != "trade_hf":
                 continue
             self.balance[entry["currency"]] = {"available": 0, "hold": 0}
```

### Comparing `KucoinPy-0.0.2/KucoinPy/ws.py` & `KucoinPy-0.0.3/KucoinPy/ws.py`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.2/KucoinPy.egg-info/PKG-INFO` & `KucoinPy-0.0.3/KucoinPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KucoinPy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Probably the fastest kucoin API wrapper in python
 Home-page: https://www.github.com/PrivatePandaCO/KucoinPy
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: GNU GENERAL PUBLIC LICENSE Version 2
 Project-URL: Documentation, https://github.com/PrivatePandaCO/KucoinPy/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/KucoinPy
```

### Comparing `KucoinPy-0.0.2/LICENSE` & `KucoinPy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.2/PKG-INFO` & `KucoinPy-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KucoinPy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Probably the fastest kucoin API wrapper in python
 Home-page: https://www.github.com/PrivatePandaCO/KucoinPy
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: GNU GENERAL PUBLIC LICENSE Version 2
 Project-URL: Documentation, https://github.com/PrivatePandaCO/KucoinPy/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/KucoinPy
```

### Comparing `KucoinPy-0.0.2/README.md` & `KucoinPy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `KucoinPy-0.0.2/setup.py` & `KucoinPy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name="KucoinPy",
-    version="0.0.2",
+    version="0.0.3",
     description="Probably the fastest kucoin API wrapper in python",
     author="Parth Mittal",
     author_email="parth@privatepanda.co",
     url="https://www.github.com/PrivatePandaCO/KucoinPy",
     license="GNU GENERAL PUBLIC LICENSE Version 2",
     packages=["KucoinPy"],
     install_requires=["orjson", "requests", "pyloggor"],
```

