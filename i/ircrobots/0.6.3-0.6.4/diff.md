# Comparing `tmp/ircrobots-0.6.3.tar.gz` & `tmp/ircrobots-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ircrobots-0.6.3.tar", last modified: Thu Jul  6 00:41:54 2023, max compression
+gzip compressed data, was "ircrobots-0.6.4.tar", last modified: Thu Jul  6 00:45:08 2023, max compression
```

## Comparing `ircrobots-0.6.3.tar` & `ircrobots-0.6.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:41:54.479158 ircrobots-0.6.3/
--rw-r--r--   0 jess      (1001) jess      (1001)     1063 2020-09-24 19:44:20.000000 ircrobots-0.6.3/LICENSE
--rw-r--r--   0 jess      (1001) jess      (1001)      969 2023-07-06 00:41:54.479158 ircrobots-0.6.3/PKG-INFO
--rw-r--r--   0 jess      (1001) jess      (1001)      401 2021-06-26 15:14:30.000000 ircrobots-0.6.3/README.md
-drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:41:54.479158 ircrobots-0.6.3/ircrobots/
--rw-r--r--   0 jess      (1001) jess      (1001)      215 2023-02-06 19:43:44.000000 ircrobots-0.6.3/ircrobots/__init__.py
--rw-r--r--   0 jess      (1001) jess      (1001)     1371 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/asyncs.py
--rw-r--r--   0 jess      (1001) jess      (1001)     2206 2022-01-07 11:46:10.000000 ircrobots-0.6.3/ircrobots/bot.py
--rw-r--r--   0 jess      (1001) jess      (1001)      126 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/contexts.py
--rw-r--r--   0 jess      (1001) jess      (1001)     1006 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/formatting.py
--rw-r--r--   0 jess      (1001) jess      (1001)     1210 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/glob.py
--rw-r--r--   0 jess      (1001) jess      (1001)     3791 2022-01-24 10:02:17.000000 ircrobots-0.6.3/ircrobots/interface.py
--rw-r--r--   0 jess      (1001) jess      (1001)     6613 2022-01-24 10:02:17.000000 ircrobots-0.6.3/ircrobots/ircv3.py
-drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:41:54.479158 ircrobots-0.6.3/ircrobots/matching/
--rw-r--r--   0 jess      (1001) jess      (1001)       51 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/matching/__init__.py
--rw-r--r--   0 jess      (1001) jess      (1001)     4294 2023-02-06 19:43:44.000000 ircrobots-0.6.3/ircrobots/matching/params.py
--rw-r--r--   0 jess      (1001) jess      (1001)     2291 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/matching/responses.py
--rw-r--r--   0 jess      (1001) jess      (1001)     2118 2023-07-06 00:36:07.000000 ircrobots-0.6.3/ircrobots/params.py
--rw-r--r--   0 jess      (1001) jess      (1001)        0 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/py.typed
--rw-r--r--   0 jess      (1001) jess      (1001)     6895 2021-09-19 21:36:50.000000 ircrobots-0.6.3/ircrobots/sasl.py
--rw-r--r--   0 jess      (1001) jess      (1001)     5055 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/scram.py
--rw-r--r--   0 jess      (1001) jess      (1001)      647 2023-07-06 00:36:07.000000 ircrobots-0.6.3/ircrobots/security.py
--rw-r--r--   0 jess      (1001) jess      (1001)    20443 2022-01-24 10:02:17.000000 ircrobots-0.6.3/ircrobots/server.py
--rw-r--r--   0 jess      (1001) jess      (1001)      575 2020-09-24 19:44:20.000000 ircrobots-0.6.3/ircrobots/struct.py
--rw-r--r--   0 jess      (1001) jess      (1001)     2581 2023-02-06 19:43:44.000000 ircrobots-0.6.3/ircrobots/transport.py
-drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:41:54.479158 ircrobots-0.6.3/ircrobots.egg-info/
--rw-r--r--   0 jess      (1001) jess      (1001)      969 2023-07-06 00:41:54.000000 ircrobots-0.6.3/ircrobots.egg-info/PKG-INFO
--rw-r--r--   0 jess      (1001) jess      (1001)      608 2023-07-06 00:41:54.000000 ircrobots-0.6.3/ircrobots.egg-info/SOURCES.txt
--rw-r--r--   0 jess      (1001) jess      (1001)        1 2023-07-06 00:41:54.000000 ircrobots-0.6.3/ircrobots.egg-info/dependency_links.txt
--rw-r--r--   0 jess      (1001) jess      (1001)      118 2023-07-06 00:41:54.000000 ircrobots-0.6.3/ircrobots.egg-info/requires.txt
--rw-r--r--   0 jess      (1001) jess      (1001)       10 2023-07-06 00:41:54.000000 ircrobots-0.6.3/ircrobots.egg-info/top_level.txt
--rw-r--r--   0 jess      (1001) jess      (1001)       38 2023-07-06 00:41:54.479158 ircrobots-0.6.3/setup.cfg
--rw-r--r--   0 jess      (1001) jess      (1001)     1130 2022-01-07 11:46:10.000000 ircrobots-0.6.3/setup.py
+drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:45:08.318300 ircrobots-0.6.4/
+-rw-r--r--   0 jess      (1001) jess      (1001)     1063 2020-09-24 19:44:20.000000 ircrobots-0.6.4/LICENSE
+-rw-r--r--   0 jess      (1001) jess      (1001)      969 2023-07-06 00:45:08.314300 ircrobots-0.6.4/PKG-INFO
+-rw-r--r--   0 jess      (1001) jess      (1001)      401 2021-06-26 15:14:30.000000 ircrobots-0.6.4/README.md
+drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:45:08.314300 ircrobots-0.6.4/ircrobots/
+-rw-r--r--   0 jess      (1001) jess      (1001)      215 2023-02-06 19:43:44.000000 ircrobots-0.6.4/ircrobots/__init__.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     1371 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/asyncs.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     2206 2022-01-07 11:46:10.000000 ircrobots-0.6.4/ircrobots/bot.py
+-rw-r--r--   0 jess      (1001) jess      (1001)      126 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/contexts.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     1006 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/formatting.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     1210 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/glob.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     3791 2022-01-24 10:02:17.000000 ircrobots-0.6.4/ircrobots/interface.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     6614 2023-07-06 00:45:05.000000 ircrobots-0.6.4/ircrobots/ircv3.py
+drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:45:08.314300 ircrobots-0.6.4/ircrobots/matching/
+-rw-r--r--   0 jess      (1001) jess      (1001)       51 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/matching/__init__.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     4294 2023-02-06 19:43:44.000000 ircrobots-0.6.4/ircrobots/matching/params.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     2291 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/matching/responses.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     2118 2023-07-06 00:36:07.000000 ircrobots-0.6.4/ircrobots/params.py
+-rw-r--r--   0 jess      (1001) jess      (1001)        0 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/py.typed
+-rw-r--r--   0 jess      (1001) jess      (1001)     6895 2021-09-19 21:36:50.000000 ircrobots-0.6.4/ircrobots/sasl.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     5055 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/scram.py
+-rw-r--r--   0 jess      (1001) jess      (1001)      647 2023-07-06 00:36:07.000000 ircrobots-0.6.4/ircrobots/security.py
+-rw-r--r--   0 jess      (1001) jess      (1001)    20443 2022-01-24 10:02:17.000000 ircrobots-0.6.4/ircrobots/server.py
+-rw-r--r--   0 jess      (1001) jess      (1001)      575 2020-09-24 19:44:20.000000 ircrobots-0.6.4/ircrobots/struct.py
+-rw-r--r--   0 jess      (1001) jess      (1001)     2581 2023-02-06 19:43:44.000000 ircrobots-0.6.4/ircrobots/transport.py
+drwxr-xr-x   0 jess      (1001) jess      (1001)        0 2023-07-06 00:45:08.314300 ircrobots-0.6.4/ircrobots.egg-info/
+-rw-r--r--   0 jess      (1001) jess      (1001)      969 2023-07-06 00:45:08.000000 ircrobots-0.6.4/ircrobots.egg-info/PKG-INFO
+-rw-r--r--   0 jess      (1001) jess      (1001)      608 2023-07-06 00:45:08.000000 ircrobots-0.6.4/ircrobots.egg-info/SOURCES.txt
+-rw-r--r--   0 jess      (1001) jess      (1001)        1 2023-07-06 00:45:08.000000 ircrobots-0.6.4/ircrobots.egg-info/dependency_links.txt
+-rw-r--r--   0 jess      (1001) jess      (1001)      118 2023-07-06 00:45:08.000000 ircrobots-0.6.4/ircrobots.egg-info/requires.txt
+-rw-r--r--   0 jess      (1001) jess      (1001)       10 2023-07-06 00:45:08.000000 ircrobots-0.6.4/ircrobots.egg-info/top_level.txt
+-rw-r--r--   0 jess      (1001) jess      (1001)       38 2023-07-06 00:45:08.318300 ircrobots-0.6.4/setup.cfg
+-rw-r--r--   0 jess      (1001) jess      (1001)     1130 2022-01-07 11:46:10.000000 ircrobots-0.6.4/setup.py
```

### Comparing `ircrobots-0.6.3/LICENSE` & `ircrobots-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/PKG-INFO` & `ircrobots-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ircrobots
-Version: 0.6.3
+Version: 0.6.4
 Summary: Asyncio IRC bot framework
 Home-page: https://github.com/jesopo/ircrobots
 Author: jesopo
 Author-email: pip@jesopo.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ircrobots-0.6.3/ircrobots/asyncs.py` & `ircrobots-0.6.4/ircrobots/asyncs.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/bot.py` & `ircrobots-0.6.4/ircrobots/bot.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/formatting.py` & `ircrobots-0.6.4/ircrobots/formatting.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/glob.py` & `ircrobots-0.6.4/ircrobots/glob.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/interface.py` & `ircrobots-0.6.4/ircrobots/interface.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/ircv3.py` & `ircrobots-0.6.4/ircrobots/ircv3.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from irctokens   import build
 from ircstates.server import ServerDisconnectedException
 
 from .contexts  import ServerContext
 from .matching  import Response, ANY
 from .interface import ICapability
 from .params    import ConnectionParams, STSPolicy, ResumePolicy
-from .security  import TLS_VERIFYCHAIN
+from .security  import TLSVerifyChain
 
 class Capability(ICapability):
     def __init__(self,
             ratified_name: Optional[str],
             draft_name:    Optional[str]=None,
             alias:         Optional[str]=None,
             depends_on:    List[str]=[]):
@@ -103,15 +103,15 @@
 
 async def sts_transmute(params: ConnectionParams):
     if not params.sts is None and params.tls is None:
         now   = time()
         since = (now-params.sts.created)
         if since <= params.sts.duration:
             params.port = params.sts.port
-            params.tls  = TLS_VERIFYCHAIN
+            params.tls  = TLSVerifyChain()
 async def resume_transmute(params: ConnectionParams):
     if params.resume is not None:
         params.host = params.resume.address
 
 class HandshakeCancel(Exception):
     pass
 
@@ -179,15 +179,15 @@
         cap_sts = CAP_STS.available(tokens)
         if not cap_sts is None:
             sts_dict = _cap_dict(tokens[cap_sts])
             params   = self.server.params
             if not params.tls:
                 if "port" in sts_dict:
                     params.port = int(sts_dict["port"])
-                    params.tls  = TLS_VERIFYCHAIN
+                    params.tls  = TLSVerifyChain()
 
                     await self.server.bot.disconnect(self.server)
                     await self.server.bot.add_server(self.server.name, params)
                     raise ServerDisconnectedException()
 
             elif "duration" in sts_dict:
                 policy = STSPolicy(
```

### Comparing `ircrobots-0.6.3/ircrobots/matching/params.py` & `ircrobots-0.6.4/ircrobots/matching/params.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/matching/responses.py` & `ircrobots-0.6.4/ircrobots/matching/responses.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/params.py` & `ircrobots-0.6.4/ircrobots/params.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/sasl.py` & `ircrobots-0.6.4/ircrobots/sasl.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/scram.py` & `ircrobots-0.6.4/ircrobots/scram.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/security.py` & `ircrobots-0.6.4/ircrobots/security.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/server.py` & `ircrobots-0.6.4/ircrobots/server.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/struct.py` & `ircrobots-0.6.4/ircrobots/struct.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots/transport.py` & `ircrobots-0.6.4/ircrobots/transport.py`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/ircrobots.egg-info/PKG-INFO` & `ircrobots-0.6.4/ircrobots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ircrobots
-Version: 0.6.3
+Version: 0.6.4
 Summary: Asyncio IRC bot framework
 Home-page: https://github.com/jesopo/ircrobots
 Author: jesopo
 Author-email: pip@jesopo.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ircrobots-0.6.3/ircrobots.egg-info/SOURCES.txt` & `ircrobots-0.6.4/ircrobots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ircrobots-0.6.3/setup.py` & `ircrobots-0.6.4/setup.py`

 * *Files identical despite different names*

