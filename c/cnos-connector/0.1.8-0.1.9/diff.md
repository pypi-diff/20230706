# Comparing `tmp/cnos_connector-0.1.8.tar.gz` & `tmp/cnos_connector-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnos_connector-0.1.8.tar", max compression
+gzip compressed data, was "cnos_connector-0.1.9.tar", max compression
```

## Comparing `cnos_connector-0.1.8.tar` & `cnos_connector-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1063 2022-12-30 03:29:41.556088 cnos_connector-0.1.8/LICENSE
--rw-r--r--   0        0        0     2795 2023-01-09 02:06:38.505031 cnos_connector-0.1.8/README.md
--rw-r--r--   0        0        0      950 2023-01-09 02:06:38.505577 cnos_connector-0.1.8/cnosdb_connector/__init__.py
--rw-r--r--   0        0        0     2490 2023-01-12 08:58:50.363191 cnos_connector-0.1.8/cnosdb_connector/client.py
--rw-r--r--   0        0        0     7465 2023-03-02 08:51:12.055797 cnos_connector-0.1.8/cnosdb_connector/conn.py
--rw-r--r--   0        0        0     2148 2023-01-09 02:06:38.506748 cnos_connector-0.1.8/cnosdb_connector/cursor.py
--rw-r--r--   0        0        0     1160 2023-01-09 02:06:38.507121 cnos_connector-0.1.8/cnosdb_connector/error.py
--rw-r--r--   0        0        0      348 2023-03-02 08:55:26.505548 cnos_connector-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 cnos_connector-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-12-30 03:29:41.556088 cnos_connector-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2795 2023-07-04 07:41:19.793649 cnos_connector-0.1.9/README.md
+-rw-r--r--   0        0        0     1396 2023-07-06 02:50:44.917624 cnos_connector-0.1.9/cnosdb_connector/__init__.py
+-rw-r--r--   0        0        0     2582 2023-07-05 08:11:36.141789 cnos_connector-0.1.9/cnosdb_connector/client.py
+-rw-r--r--   0        0        0     7624 2023-07-05 07:01:41.992775 cnos_connector-0.1.9/cnosdb_connector/conn.py
+-rw-r--r--   0        0        0     5211 2023-07-06 10:21:53.010057 cnos_connector-0.1.9/cnosdb_connector/cursor.py
+-rw-r--r--   0        0        0     1209 2023-07-06 06:07:55.431087 cnos_connector-0.1.9/cnosdb_connector/error.py
+-rw-r--r--   0        0        0       37 2023-07-06 11:31:37.263655 cnos_connector-0.1.9/cnosdb_connector/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7598 2023-07-06 11:08:46.402525 cnos_connector-0.1.9/cnosdb_connector/sqlalchemy/dialects/__init__.py
+-rw-r--r--   0        0        0      360 2023-07-06 03:26:01.327832 cnos_connector-0.1.9/cnosdb_connector/sqlalchemy/dialects/base.py
+-rw-r--r--   0        0        0      796 2023-07-06 11:30:34.605502 cnos_connector-0.1.9/cnosdb_connector/sqlalchemy/dialects/compiler.py
+-rw-r--r--   0        0        0      448 2023-07-04 08:00:13.964932 cnos_connector-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 cnos_connector-0.1.9/PKG-INFO
```

### Comparing `cnos_connector-0.1.8/LICENSE` & `cnos_connector-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cnos_connector-0.1.8/README.md` & `cnos_connector-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cnos_connector-0.1.8/cnosdb_connector/__init__.py` & `cnos_connector-0.1.9/cnosdb_connector/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 from .conn import CnosDBConnection
+from .error import Error
+
+apilevel = "2.0"
+threadsafety = 1  # Threads may share the module, but not connections.
+paramstyle = "pyformat"  # Python extended format codes, e.g. ...WHERE name=%(name)s
 
 
 def connect(**kwargs) -> CnosDBConnection:
     """
     Keyword Arguments
     ========================================================================
     url: str
@@ -25,7 +30,12 @@
     example:
         import cnos_connector
 
         conn = cnos_connector.connect(url="http://192.168.0.11/", database="public", user="root", password="123456")
     ```
     """
     return CnosDBConnection(**kwargs)
+
+
+def make_cnosdb_langchain_uri(url="127.0.0.1:8902", user="root", password="", tenant="cnosdb",
+                              database="public"):
+    return f"cnosdb://{user}:{password}@{url}/api/v1/sql?tenant={tenant}&db={database}&pretty=true"
```

### Comparing `cnos_connector-0.1.8/cnosdb_connector/client.py` & `cnos_connector-0.1.9/cnosdb_connector/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     404: "api not found",
     500: "internal error",
     503: "system resources is not sufficient. It is may be caused by a huge query."
 }
 
 
 class Client:
-    def __init__(self, url: str = "http://localhost:31007/",
+    def __init__(self, url: str = "http://localhost:8902/",
+                 tenant: str = "cnosdb",
                  database: str = "public",
                  user: str = "root",
                  password: str = ""):
         self._url = url
+        self._tenant = tenant
         self._database = database
         self._user = user
         self._password = password
 
     def sql(self, q: str) -> dict:
-        _url = self._url + f"api/v1/sql?db={self._database}&pretty=true"
+        _url = self._url + f"api/v1/sql?db={self._database}&tenant={self._tenant}&pretty=true"
         request = self.build_request(url=_url, data=q)
         try:
             response = urlopen(request)
         except UrlLibHTTPError as e:
             logging.error(f"Invalid syntax or Object not exists, get ERROR from database : {e}")
             return {}
         else:
```

### Comparing `cnos_connector-0.1.8/cnosdb_connector/conn.py` & `cnos_connector-0.1.9/cnosdb_connector/conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,33 @@
 from .error import NotSupportedError
 from .client import Client
 from .cursor import Cursor
 
 
 class CnosDBConnection:
     def __init__(self, **kwargs):
-        url = kwargs.get("url", "http://127.0.0.1:31007/")
+        url = kwargs.get("url", "http://127.0.0.1:8902/")
         user = kwargs.get("user", "root")
         password = kwargs.get("password", "")
+        tenant = kwargs.get("tenant", "cnosdb")
         database = kwargs.get("database", "public")
         self._client = Client(
             url,
+            tenant,
             database,
             user,
             password,
         )
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self):
+        self.close()
+
     # close, commit, rollback, cursor are PEP249 method
     def close(self):
         pass
 
     def commit(self):
         pass
```

### Comparing `cnos_connector-0.1.8/cnosdb_connector/error.py` & `cnos_connector-0.1.9/cnosdb_connector/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,7 +58,10 @@
 
 class DataError(DatabaseError):
     pass
 
 
 class NotSupportedError(DatabaseError):
     pass
+
+class ProgrammingError(DatabaseError):
+    pass
```

### Comparing `cnos_connector-0.1.8/PKG-INFO` & `cnos_connector-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnos-connector
-Version: 0.1.8
+Version: 0.1.9
 Summary: CnosDB Python Client
 License: MIT
 Author: Subsegment
 Author-email: 304741833@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

