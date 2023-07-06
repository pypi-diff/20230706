# Comparing `tmp/pyxui-0.0.7.tar.gz` & `tmp/pyxui-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxui-0.0.7.tar", last modified: Fri Jun  9 11:54:20 2023, max compression
+gzip compressed data, was "pyxui-0.0.9.tar", last modified: Thu Jul  6 08:33:52 2023, max compression
```

## Comparing `pyxui-0.0.7.tar` & `pyxui-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.984479 pyxui-0.0.7/
--rw-rw-rw-   0        0        0     1070 2023-05-15 16:46:45.000000 pyxui-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5606 2023-06-09 11:54:20.983012 pyxui-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4996 2023-06-09 11:49:10.000000 pyxui-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.957797 pyxui-0.0.7/pyxui/
--rw-rw-rw-   0        0        0       26 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.973554 pyxui-0.0.7/pyxui/config_gen/
--rw-rw-rw-   0        0        0      441 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/config_gen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.973554 pyxui-0.0.7/pyxui/errors/
--rw-rw-rw-   0        0        0      884 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.982012 pyxui-0.0.7/pyxui/methods/
--rw-rw-rw-   0        0        0      235 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/methods/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-06-09 11:40:06.000000 pyxui-0.0.7/pyxui/methods/base.py
--rw-rw-rw-   0        0        0     6850 2023-06-09 11:34:11.000000 pyxui-0.0.7/pyxui/methods/clients.py
--rw-rw-rw-   0        0        0     1182 2023-06-09 11:41:26.000000 pyxui-0.0.7/pyxui/methods/inbounds.py
--rw-rw-rw-   0        0        0     1077 2023-05-15 16:46:45.000000 pyxui-0.0.7/pyxui/methods/login.py
--rw-rw-rw-   0        0        0      573 2023-06-09 11:40:26.000000 pyxui-0.0.7/pyxui/xui.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:54:20.972051 pyxui-0.0.7/pyxui.egg-info/
--rw-rw-rw-   0        0        0     5606 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 11:54:20.000000 pyxui-0.0.7/pyxui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 11:54:20.984479 pyxui-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-06-09 11:52:22.000000 pyxui-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.555309 pyxui-0.0.9/
+-rw-rw-rw-   0        0        0     1070 2023-07-06 08:30:19.000000 pyxui-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6043 2023-07-06 08:33:52.554312 pyxui-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5411 2023-07-06 08:30:19.000000 pyxui-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.487572 pyxui-0.0.9/pyxui/
+-rw-rw-rw-   0        0        0       26 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.509795 pyxui-0.0.9/pyxui/config_gen/
+-rw-rw-rw-   0        0        0      441 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/config_gen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.516535 pyxui-0.0.9/pyxui/errors/
+-rw-rw-rw-   0        0        0      884 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.553314 pyxui-0.0.9/pyxui/methods/
+-rw-rw-rw-   0        0        0      235 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/__init__.py
+-rw-rw-rw-   0        0        0     1612 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/base.py
+-rw-rw-rw-   0        0        0     7953 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/clients.py
+-rw-rw-rw-   0        0        0     1190 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/inbounds.py
+-rw-rw-rw-   0        0        0     1077 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/login.py
+-rw-rw-rw-   0        0        0      573 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/xui.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.502531 pyxui-0.0.9/pyxui.egg-info/
+-rw-rw-rw-   0        0        0     6043 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 08:33:52.555309 pyxui-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-07-06 08:32:01.000000 pyxui-0.0.9/setup.py
```

### Comparing `pyxui-0.0.7/LICENSE` & `pyxui-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.7/PKG-INFO` & `pyxui-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.7
+Version: 0.0.9
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -85,31 +85,31 @@
             "tag": "inbound-443",
             "sniffing": "{\n  \"enabled\": true,\n  \"destOverride\": [\n    \"http\",\n    \"tls\"\n  ]\n}"
         }
     ]
 }
 ```
 
-- Add client to exist inbound
+- Add client to the existing inbound
 ```python
 get = xui.add_client(
     inbound_id=1,
     email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
     limit_ip = 0,
     total_gb = 5368709120,
-    expire_time = 1684948641772,
+    expire_time = 1684948641772, # You must pass 13 digit timestamp
     telegram_id = "",
     subscription_id = ""
 )
 ```
 
-- Update exist client
+- Update the existing client
 ```python
 get = xui.update_client(
     inbound_id=1,
     email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
@@ -117,42 +117,64 @@
     total_gb = 5368709120,
     expire_time = 1684948641772,
     telegram_id = "",
     subscription_id = ""
 )
 ```
 
-- Get client information:
+- Get client's information:
 ```python
 get_client = xui.get_client(
     inbound_id=1,
     email="Me",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa" # Make note you don't have to pass both of them (emaill, uuid), just one is enough
 )
 
 # Result
 {
-    'id': 1,
-    'inboundId': 1,
-    'enable': True,
-    'email': 'Me',
-    'up': 194895832,
-    'down': 4959786483,
-    'expiryTime': 0,
-    'total': 0
+     'email': 'Me',
+     'enable': True,
+     'expiryTime': 0,
+     'flow': 'xtls-rprx-vision',
+     'id': '5d3d1bac-49cd-4b66-8be9-a728efa205fa',
+     'limitIp': 0,
+     'subId': '',
+     'tgId': '',
+     'totalGB': 0
+}
+```
+
+- Get client's statistics:
+```python
+get_client = xui.get_client_stats(
+    inbound_id=1,
+    email="Me",
+)
+
+# Result
+{
+     'id': 1,
+     'inboundId': 1,
+     'enable': True,
+     'email': 'Me',
+     'up': 111494230,
+     'down': 620533614,
+     'expiryTime': 0,
+     'total': 0
 }
 ```
 
-- Delete client from exist inbound:
+- Delete client from the existing inbound:
 ```python
 get_client = xui.delete_client(
     inbound_id=1,
     email="Me",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa" # Make note you don't have to pass both of them (email, uuid), just one is enough
 )
+```
 
 # Create vmess and vless config string
 - Import config_generator
 ```python
 from pyxui.config_gen import config_generator
 ```
```

### Comparing `pyxui-0.0.7/README.md` & `pyxui-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,31 +72,31 @@
             "tag": "inbound-443",
             "sniffing": "{\n  \"enabled\": true,\n  \"destOverride\": [\n    \"http\",\n    \"tls\"\n  ]\n}"
         }
     ]
 }
 ```
 
-- Add client to exist inbound
+- Add client to the existing inbound
 ```python
 get = xui.add_client(
     inbound_id=1,
     email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
     limit_ip = 0,
     total_gb = 5368709120,
-    expire_time = 1684948641772,
+    expire_time = 1684948641772, # You must pass 13 digit timestamp
     telegram_id = "",
     subscription_id = ""
 )
 ```
 
-- Update exist client
+- Update the existing client
 ```python
 get = xui.update_client(
     inbound_id=1,
     email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
@@ -104,42 +104,64 @@
     total_gb = 5368709120,
     expire_time = 1684948641772,
     telegram_id = "",
     subscription_id = ""
 )
 ```
 
-- Get client information:
+- Get client's information:
 ```python
 get_client = xui.get_client(
     inbound_id=1,
     email="Me",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa" # Make note you don't have to pass both of them (emaill, uuid), just one is enough
 )
 
 # Result
 {
-    'id': 1,
-    'inboundId': 1,
-    'enable': True,
-    'email': 'Me',
-    'up': 194895832,
-    'down': 4959786483,
-    'expiryTime': 0,
-    'total': 0
+     'email': 'Me',
+     'enable': True,
+     'expiryTime': 0,
+     'flow': 'xtls-rprx-vision',
+     'id': '5d3d1bac-49cd-4b66-8be9-a728efa205fa',
+     'limitIp': 0,
+     'subId': '',
+     'tgId': '',
+     'totalGB': 0
+}
+```
+
+- Get client's statistics:
+```python
+get_client = xui.get_client_stats(
+    inbound_id=1,
+    email="Me",
+)
+
+# Result
+{
+     'id': 1,
+     'inboundId': 1,
+     'enable': True,
+     'email': 'Me',
+     'up': 111494230,
+     'down': 620533614,
+     'expiryTime': 0,
+     'total': 0
 }
 ```
 
-- Delete client from exist inbound:
+- Delete client from the existing inbound:
 ```python
 get_client = xui.delete_client(
     inbound_id=1,
     email="Me",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa" # Make note you don't have to pass both of them (email, uuid), just one is enough
 )
+```
 
 # Create vmess and vless config string
 - Import config_generator
 ```python
 from pyxui.config_gen import config_generator
 ```
```

### Comparing `pyxui-0.0.7/pyxui/errors/__init__.py` & `pyxui-0.0.9/pyxui/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.7/pyxui/methods/base.py` & `pyxui-0.0.9/pyxui/methods/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 class Base:
     def request(
         self: "pyxui.XUI",
         path: str,
         method: str,
         params: dict = None
     ) -> requests.Response:
-        """Request to xui panel.
+        """Request to the xui panel.
 
         Parameters:
             path (``str``):
-                Your request path, you can see all of them in https://github.com/alireza0/x-ui#api-routes
+                The request path, you can see all of them in https://github.com/alireza0/x-ui#api-routes
                 
             method (``str``):
-                Your request method, GET or POST
+                The request method, GET or POST
                 
             params (``dict``, optional):
-                Your request parameters, None is set for default but it's necessary for some POST methods
+                The request parameters, None is set for default but it's necessary for some POST methods
 
         Returns:
             `~requests.Response`: On success, the response is returned.
         """
         
         if path == "login":
             url = f"{self.full_address}/login"
```

### Comparing `pyxui-0.0.7/pyxui/methods/clients.py` & `pyxui-0.0.9/pyxui/methods/clients.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 class Clients:
     def get_client(
         self: "pyxui.XUI",
         inbound_id: int,
         email: str = False,
         uuid: str = False
     ) -> Union[dict, errors.NotFound]:
-        """Get client from exist inbound.
+        """Get client from the existing inbound.
 
         Parameters:
             inbound_id (``int``):
                 Inbound id
                 
             email (``str``, optional):
-               Email of client
+               Email of the client
                 
             uuid (``str``, optional):
-               UUID of client
+               UUID of the client
             
         Returns:
-            `~Dict`: On success, a dict is returned else 404 error will be raised
+            `~Dict`: On success, a dict is returned or else 404 an error will be raised
         """
         
         get_inbounds = self.get_inbounds()
         
         if not email and not uuid:
             raise ValueError()
         
@@ -42,59 +42,96 @@
                 if client['email'] != email and client['id'] != uuid:
                     continue
                 
                 return client
 
         raise errors.NotFound()
 
+    def get_client_stats(
+        self: "pyxui.XUI",
+        inbound_id: int,
+        email: str,
+    ) -> Union[dict, errors.NotFound]:
+        """Get client stats from the existing inbound.
+
+        Parameters:
+            inbound_id (``int``):
+                Inbound id
+                
+            email (``str``):
+               Email of the client
+            
+        Returns:
+            `~Dict`: On success, a dict is returned or else 404 error will be raised
+        """
+        
+        get_inbounds = self.get_inbounds()
+        
+        if not email:
+            raise ValueError()
+        
+        for inbound in get_inbounds['obj']:
+            if inbound['id'] != inbound_id:
+                continue
+            
+            client_stats = inbound['clientStats']
+            
+            for client in client_stats:
+                if client['email'] != email:
+                    continue
+                
+                return client
+
+        raise errors.NotFound()
+
     def add_client(
         self: "pyxui.XUI",
         inbound_id: int,
         email: str,
         uuid: str,
         enable: bool = True,
         flow: str = "",
         limit_ip: int = 0,
         total_gb: int = 0,
         expire_time: int = 0,
         telegram_id: str = "",
         subscription_id: str = "",
     ) -> Union[dict, errors.NotFound]:
-        """Add client to exist inbound.
+        """Add client to the existing inbound.
 
         Parameters:
             inbound_id (``int``):
                 Inbound id
                 
             email (``str``):
-               Email of client
+               Email of the client
                 
             uuid (``str``):
-               UUID of client
+               UUID of the client
                 
             enable (``bool``, optional):
-               Status of client
+               Status of the client
                 
             flow (``str``, optional):
-               Flow of client
+               Flow of the client
                 
             limit_ip (``str``, optional):
-               IP Limit of client
+               IP Limit of the client
                 
             total_gb (``str``, optional):
-                Download and uploader limition of client and it's in bytes
+                Download and uploader limition of the client and it's in bytes
                 
             expire_time (``str``, optional):
                 Client expiration date and it's in timestamp (epoch)
                 
             telegram_id (``str``, optional):
-               Telegram id of client
+               Telegram id of the client
                 
             subscription_id (``str``, optional):
-               Subscription id of client
+               Subscription id of the client
             
         Returns:
             `~Dict`: On success, a dict is returned else 404 error will be raised
         """
         
         settings = {
             "clients": [
@@ -129,25 +166,25 @@
 
     def delete_client(
         self: "pyxui.XUI",
         inbound_id: int,
         email: str = False,
         uuid: str = False
     ) -> Union[dict, errors.NotFound]:
-        """Delete client from exist inbound.
+        """Delete client from the existing inbound.
 
         Parameters:
             inbound_id (``int``):
                 Inbound id
                 
             email (``str``, optional):
-               Email of client
+               Email of the client
                 
             uuid (``str``, optional):
-               UUID of client
+               UUID of the client
             
         Returns:
             `~Dict`: On success, a dict is returned else 404 error will be raised
         """
         
         find_client = self.get_client(
             inbound_id=inbound_id,
@@ -171,46 +208,46 @@
         flow: str,
         limit_ip: int,
         total_gb: int,
         expire_time: int,
         telegram_id: str,
         subscription_id: str,
     ) -> Union[dict, errors.NotFound]:
-        """Add client to exist inbound.
+        """Add client to the existing inbound.
 
         Parameters:
             inbound_id (``int``):
                 Inbound id
                 
             email (``str``):
-               Email of client
+               Email of the client
                 
             uuid (``str``):
-               UUID of client
+               UUID of the client
                 
             enable (``bool``):
-               Status of client
+               Status of the client
                 
             flow (``str``):
-               Flow of client
+               Flow of the client
                 
             limit_ip (``str``):
-               IP Limit of client
+               IP Limit of the client
                 
             total_gb (``str``):
-                Download and uploader limition of client and it's in bytes
+                Download and uploader limition of the client and it's in bytes
                 
             expire_time (``str``):
                 Client expiration date and it's in timestamp (epoch)
                 
             telegram_id (``str``):
-               Telegram id of client
+               Telegram id of the client
                 
             subscription_id (``str``):
-               Subscription id of client
+               Subscription id of the client
             
         Returns:
             `~Dict`: On success, a dict is returned else 404 error will be raised
         """
         
         find_client = self.get_client(
             inbound_id=inbound_id,
```

### Comparing `pyxui-0.0.7/pyxui/methods/inbounds.py` & `pyxui-0.0.9/pyxui/methods/inbounds.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pyxui
 from pyxui import errors
 
 class Inbounds:
     def get_inbounds(
         self: "pyxui.XUI"
     ) -> Union[dict, errors.NotFound]:
-        """Get inbounds of xui panel.
+        """Get inbounds of the xui panel.
         
         Returns:
             `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
         """
         
         
         if self.panel == "alireza":
@@ -27,15 +27,15 @@
 
         return self.verify_response(response)
         
     def get_inbound(
         self: "pyxui.XUI",
         inbound_id: int
     ) -> Union[dict, errors.NotFound]:
-        """Get inbounds of xui panel.
+        """Get inbounds of the xui panel.
 
         Parameters:
             inbound_id (``int``):
                 Inbound id
         
         Returns:
             `~Dict | errors.NotFound`: On success, a dict is returned else 404 error will be raised
```

### Comparing `pyxui-0.0.7/pyxui/methods/login.py` & `pyxui-0.0.9/pyxui/methods/login.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.7/pyxui/xui.py` & `pyxui-0.0.9/pyxui/xui.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.7/pyxui.egg-info/PKG-INFO` & `pyxui-0.0.9/pyxui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.7
+Version: 0.0.9
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -85,31 +85,31 @@
             "tag": "inbound-443",
             "sniffing": "{\n  \"enabled\": true,\n  \"destOverride\": [\n    \"http\",\n    \"tls\"\n  ]\n}"
         }
     ]
 }
 ```
 
-- Add client to exist inbound
+- Add client to the existing inbound
 ```python
 get = xui.add_client(
     inbound_id=1,
     email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
     limit_ip = 0,
     total_gb = 5368709120,
-    expire_time = 1684948641772,
+    expire_time = 1684948641772, # You must pass 13 digit timestamp
     telegram_id = "",
     subscription_id = ""
 )
 ```
 
-- Update exist client
+- Update the existing client
 ```python
 get = xui.update_client(
     inbound_id=1,
     email="example@gmal.com",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa",
     enable = True,
     flow = "",
@@ -117,42 +117,64 @@
     total_gb = 5368709120,
     expire_time = 1684948641772,
     telegram_id = "",
     subscription_id = ""
 )
 ```
 
-- Get client information:
+- Get client's information:
 ```python
 get_client = xui.get_client(
     inbound_id=1,
     email="Me",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa" # Make note you don't have to pass both of them (emaill, uuid), just one is enough
 )
 
 # Result
 {
-    'id': 1,
-    'inboundId': 1,
-    'enable': True,
-    'email': 'Me',
-    'up': 194895832,
-    'down': 4959786483,
-    'expiryTime': 0,
-    'total': 0
+     'email': 'Me',
+     'enable': True,
+     'expiryTime': 0,
+     'flow': 'xtls-rprx-vision',
+     'id': '5d3d1bac-49cd-4b66-8be9-a728efa205fa',
+     'limitIp': 0,
+     'subId': '',
+     'tgId': '',
+     'totalGB': 0
+}
+```
+
+- Get client's statistics:
+```python
+get_client = xui.get_client_stats(
+    inbound_id=1,
+    email="Me",
+)
+
+# Result
+{
+     'id': 1,
+     'inboundId': 1,
+     'enable': True,
+     'email': 'Me',
+     'up': 111494230,
+     'down': 620533614,
+     'expiryTime': 0,
+     'total': 0
 }
 ```
 
-- Delete client from exist inbound:
+- Delete client from the existing inbound:
 ```python
 get_client = xui.delete_client(
     inbound_id=1,
     email="Me",
     uuid="5d3d1bac-49cd-4b66-8be9-a728efa205fa" # Make note you don't have to pass both of them (email, uuid), just one is enough
 )
+```
 
 # Create vmess and vless config string
 - Import config_generator
 ```python
 from pyxui.config_gen import config_generator
 ```
```

### Comparing `pyxui-0.0.7/setup.py` & `pyxui-0.0.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from setuptools import setup, find_packages
-    
-VERSION = "0.0.7"
-
-with open("README.md", "r") as f:
-    readme = f.read()
-
-setup(
-    name="pyxui",
-    version=VERSION,
-    author="Staliox",
-    description="An application with python that allows you to modify your xui panel",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    url="https://github.com/staliox/pyxui",
-    keywords=[
-        "pyxui",
-        "xui",
-        "xui python",
-        "xui panel"
-    ],
-    packages=find_packages(),
-    install_requires=["requests"],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-    ],
-    license="MIT"
-)
+from setuptools import setup, find_packages
+    
+VERSION = "0.0.9"
+
+with open("README.md", "r") as f:
+    readme = f.read()
+
+setup(
+    name="pyxui",
+    version=VERSION,
+    author="Staliox",
+    description="An application with python that allows you to modify your xui panel",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    url="https://github.com/staliox/pyxui",
+    keywords=[
+        "pyxui",
+        "xui",
+        "xui python",
+        "xui panel"
+    ],
+    packages=find_packages(),
+    install_requires=["requests"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+    ],
+    license="MIT"
+)
```

