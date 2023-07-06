# Comparing `tmp/ogsapi-0.6.1.tar.gz` & `tmp/ogsapi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.6.1.tar", last modified: Fri Jun 30 03:25:05 2023, max compression
+gzip compressed data, was "ogsapi-0.7.0.tar", last modified: Thu Jul  6 17:10:12 2023, max compression
```

## Comparing `ogsapi-0.6.1.tar` & `ogsapi-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:25:05.804193 ogsapi-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-06-30 03:24:53.000000 ogsapi-0.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5557 2023-06-30 03:25:05.803193 ogsapi-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5123 2023-06-30 03:24:53.000000 ogsapi-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-30 03:24:53.000000 ogsapi-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 03:25:05.804193 ogsapi-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:25:05.801193 ogsapi-0.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:25:05.802193 ogsapi-0.6.1/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-30 03:24:54.000000 ogsapi-0.6.1/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22257 2023-06-30 03:24:53.000000 ogsapi-0.6.1/src/ogsapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)    14926 2023-06-30 03:24:53.000000 ogsapi-0.6.1/src/ogsapi/ogsgame.py
--rw-rw-rw-   0 root         (0) root         (0)     6720 2023-06-30 03:24:53.000000 ogsapi-0.6.1/src/ogsapi/ogssocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:25:05.803193 ogsapi-0.6.1/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5557 2023-06-30 03:25:05.000000 ogsapi-0.6.1/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      291 2023-06-30 03:25:05.000000 ogsapi-0.6.1/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:25:05.000000 ogsapi-0.6.1/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-30 03:25:05.000000 ogsapi-0.6.1/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 03:25:05.000000 ogsapi-0.6.1/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:10:12.535318 ogsapi-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-07-06 17:09:59.000000 ogsapi-0.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 17:10:12.535318 ogsapi-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-07-06 17:09:59.000000 ogsapi-0.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-06 17:09:59.000000 ogsapi-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 17:10:12.535318 ogsapi-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:10:12.531318 ogsapi-0.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:10:12.533318 ogsapi-0.7.0/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 17:09:59.000000 ogsapi-0.7.0/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22207 2023-07-06 17:09:59.000000 ogsapi-0.7.0/src/ogsapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-06 17:09:59.000000 ogsapi-0.7.0/src/ogsapi/ogs_api_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)    14931 2023-07-06 17:09:59.000000 ogsapi-0.7.0/src/ogsapi/ogsgame.py
+-rw-rw-rw-   0 root         (0) root         (0)     6726 2023-07-06 17:09:59.000000 ogsapi-0.7.0/src/ogsapi/ogssocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:10:12.534318 ogsapi-0.7.0/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 17:10:12.000000 ogsapi-0.7.0/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-06 17:10:12.000000 ogsapi-0.7.0/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 17:10:12.000000 ogsapi-0.7.0/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 17:10:12.000000 ogsapi-0.7.0/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 17:10:12.000000 ogsapi-0.7.0/src/ogsapi.egg-info/top_level.txt
```

### Comparing `ogsapi-0.6.1/LICENSE` & `ogsapi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.6.1/PKG-INFO` & `ogsapi-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.6.1
+Version: 0.7.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.6.1/README.md` & `ogsapi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ogsapi-0.6.1/pyproject.toml` & `ogsapi-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.6.1"
+version = "0.7.0"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.6.1/src/ogsapi/client.py` & `ogsapi-0.7.0/src/ogsapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import requests
-from ogssocket import OGSSocket
+from .ogssocket import OGSSocket
+from .ogs_api_exception import OGSApiException
 
 
 # TODO: This will eventually need to be moved to `termination-api` instead of `/api/v1/`
 # TODO: Should probably implement a user class that contains all user info and functions
 # TODO: Break REST API functions into their own class, leaving the OGSClient class to be the interface for the user client
 
-class OGSApiException(Exception):
-    """Exception raised for errors in the OGS API."""
-    pass
-
 class OGSClient:
     """Connect to and interact with the OGS REST API and SocketIO API.
 
     Examples:
         >>> from ogsapi.client import OGSClient
         >>> ogs = OGSClient(
             client_id=client_id,
```

### Comparing `ogsapi-0.6.1/src/ogsapi/ogsgame.py` & `ogsapi-0.7.0/src/ogsapi/ogsgame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ogsapi.client import OGSApiException
+from .ogs_api_exception import OGSApiException
 from typing import Callable
 
 class OGSGame:
     """OGSGame class for handling games connected via the OGSSocket.
     
     Args:
         game_socket (OGSSocket): OGSSocket object to connect to the game.
```

### Comparing `ogsapi-0.6.1/src/ogsapi/ogssocket.py` & `ogsapi-0.7.0/src/ogsapi/ogssocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import socketio
 import requests
 from typing import Callable
-from ogsapi.client import OGSApiException
+from .ogs_api_exception import OGSApiException
 from time import sleep, time
-from ogsgame import OGSGame
+from .ogsgame import OGSGame
 
 class OGSSocket:
     """OGS Socket Class for handling SocketIO connections to OGS
     
     Args:
         bearer_token (str): The bearer token to use for authentication
         debug (bool, optional): Enable debug logging. Defaults to False.
```

### Comparing `ogsapi-0.6.1/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.7.0/src/ogsapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.6.1
+Version: 0.7.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

