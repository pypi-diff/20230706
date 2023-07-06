# Comparing `tmp/overfast-py-1.0.tar.gz` & `tmp/overfast-py-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overfast-py-1.0.tar", last modified: Wed Jul  5 12:33:42 2023, max compression
+gzip compressed data, was "overfast-py-1.1.tar", last modified: Thu Jul  6 12:14:42 2023, max compression
```

## Comparing `overfast-py-1.0.tar` & `overfast-py-1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 12:33:42.560902 overfast-py-1.0/
--rw-rw-rw-   0        0        0     1083 2023-07-05 12:29:57.000000 overfast-py-1.0/LICENSE
--rw-rw-rw-   0        0        0      425 2023-07-05 12:33:42.561399 overfast-py-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-07-05 12:18:15.000000 overfast-py-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 12:33:42.491283 overfast-py-1.0/overfast/
--rw-rw-rw-   0        0        0        0 2023-07-04 20:00:20.000000 overfast-py-1.0/overfast/__init__.py
--rw-rw-rw-   0        0        0     3697 2023-07-05 11:57:17.000000 overfast-py-1.0/overfast/overfast.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:33:42.558424 overfast-py-1.0/overfast_py.egg-info/
--rw-rw-rw-   0        0        0      425 2023-07-05 12:33:42.000000 overfast-py-1.0/overfast_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-05 12:33:42.000000 overfast-py-1.0/overfast_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 12:33:42.000000 overfast-py-1.0/overfast_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 12:33:42.000000 overfast-py-1.0/overfast_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 12:33:42.000000 overfast-py-1.0/overfast_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      433 2023-07-05 12:32:40.000000 overfast-py-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      212 2023-07-05 12:33:42.563387 overfast-py-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 12:14:42.236767 overfast-py-1.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 12:29:57.000000 overfast-py-1.1/LICENSE
+-rw-rw-rw-   0        0        0      485 2023-07-06 12:14:42.237260 overfast-py-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      119 2023-07-05 12:47:29.000000 overfast-py-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:14:42.214368 overfast-py-1.1/overfast/
+-rw-rw-rw-   0        0        0     3306 2023-07-06 12:09:10.000000 overfast-py-1.1/overfast/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:14:42.235772 overfast-py-1.1/overfast_py.egg-info/
+-rw-rw-rw-   0        0        0      485 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      433 2023-07-06 12:14:10.000000 overfast-py-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      212 2023-07-06 12:14:42.238748 overfast-py-1.1/setup.cfg
```

### Comparing `overfast-py-1.0/LICENSE` & `overfast-py-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `overfast-py-1.0/overfast/overfast.py` & `overfast-py-1.1/overfast/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,91 @@
 import requests
 
-class Overfast:
-    def get(type: str, locale: str = "en-us", key: str = None):
-        """Get any OverFast data except players.
-        Cache TTL may vary, see https://overfast-api.tekrop.fr/"""
-        url = "https://overfast-api.tekrop.fr/"
-        params = {}
-        types = ["hero", "heroes", "gamemodes", "maps"]
-        if type not in types:
-            return "Invalid type argument. Available types: " + ", ".join(types)
-        
-        if type == "hero":
-            if not key:
-                type = "heroes"
-            else:
-                type = "heroes/" + key
-        if type in ['hero', 'heroes', 'gamemodes']:
-            params["locale"] : locale
-        if type == "maps":
-            if key:
-                params["gamemode"] = key
-        
-        data = requests.get(url + type, params)
-        response = data.json()
+def get(type: str, locale: str = "en-us", key: str = None):
+    """Get any OverFast data except players.
+    Cache TTL may vary, see https://overfast-api.tekrop.fr/"""
+    url = "https://overfast-api.tekrop.fr/"
+    params = {}
+    types = ["hero", "heroes", "gamemodes", "maps"]
+    if type not in types:
+        return "Invalid type argument. Available types: " + ", ".join(types)
+    
+    if type == "hero":
+        if not key:
+            type = "heroes"
+        else:
+            type = "heroes/" + key
+    if type in ['hero', 'heroes', 'gamemodes']:
+        params["locale"] : locale
+    if type == "maps":
+        if key:
+            params["gamemode"] = key
+    
+    data = requests.get(url + type, params)
+    response = data.json()
 
-        if data.status_code != 200:
-            if data.status_code == 422:
-                return "Validation error"
-            else:
-                
-                return response["error"]
+    if data.status_code != 200:
+        if data.status_code == 422:
+            return "Validation error"
         else:
-            return response
-        
-    def player(type: str = None, name: str = None, id: str = None,
-               privacy: str = None, order_by: str = None, offset: str=None,
-               limit: str=None, gamemode: str = None, platform: str = None, hero: str = None):
-        """Get player data from the OverFast API.
-           Cache TTL may vary. Requests accept different arguments:
-             No type (search by name): name (required)
-             summary: player id (required)
-             stats_summary: player id (required), gamemode, platform
-             stats_career: player id (required), gamemode, platform, hero
-             stats: player id (required), gamemode, platform, hero
-             all: player_id (required)"""
-        types = ["summary", "stats_summary", "stats_career", "stats", "all"]
-        url = "https://overfast-api.tekrop.fr/" + "players"
-        params = {} # The dict we send as our parameters
-        args = [] # The key names of the values we'll send over
+            
+            return response["error"]
+    else:
+        return response
+    
+def player(type: str = None, name: str = None, id: str = None,
+            privacy: str = None, order_by: str = None, offset: str=None,
+            limit: str=None, gamemode: str = None, platform: str = None, hero: str = None):
+    """Get player data from the OverFast API.
+        Cache TTL may vary. Requests accept different arguments:
+            No type (search by name): name (required)
+            summary: player id (required)
+            stats_summary: player id (required), gamemode, platform
+            stats_career: player id (required), gamemode, platform, hero
+            stats: player id (required), gamemode, platform, hero
+            all: player_id (required)"""
+    types = ["summary", "stats_summary", "stats_career", "stats", "all"]
+    url = "https://overfast-api.tekrop.fr/" + "players"
+    params = {} # The dict we send as our parameters
+    args = [] # The key names of the values we'll send over
 
-        if id != None and type == None:
-            type = "summary"
-        if type and type not in types:
-            return "Invalid type argument. Available types: " + ", ".join(types)
-        if type == "all":
-            # Evil hack to fix the URL
-            type = ""
+    if id != None and type == None:
+        type = "summary"
+    if type and type not in types:
+        return "Invalid type argument. Available types: " + ", ".join(types)
+    if type == "all":
+        # Evil hack to fix the URL
+        type = ""
 
-        if type != None:
-            if not id:
-                return "A player id is required."
-            if type == "stats_summary":
-                args.extend(["gamemode", "platform"])
-            elif type in ["stats_career", "stats"]:
-                args.extend(["gamemode", "platform", "hero"])
-            id = id.replace("#", "-")
-            type = type.replace("_", "/")
-            url = url + "/" + id + "/" + type
-        else:
-            args.extend(["name", "privacy", "order_by", "offset", "limit"])
-            if not name:
-                return "A player name is required."
-        keys = {}
-        for key, val in list(locals().items()):
-            if locals()['key'] != None:
-                keys[key] = val
-        for x in keys:
-            if locals().get(x) != None:
-                if x in args:
-                    params[x] = locals().get(x)
+    if type != None:
+        if not id:
+            return "A player id is required."
+        if type == "stats_summary":
+            args.extend(["gamemode", "platform"])
+        elif type in ["stats_career", "stats"]:
+            args.extend(["gamemode", "platform", "hero"])
+        id = id.replace("#", "-")
+        type = type.replace("_", "/")
+        url = url + "/" + id + "/" + type
+    else:
+        args.extend(["name", "privacy", "order_by", "offset", "limit"])
+        if not name:
+            return "A player name is required."
+    keys = {}
+    for key, val in list(locals().items()):
+        if locals()['key'] != None:
+            keys[key] = val
+    for x in keys:
+        if locals().get(x) != None:
+            if x in args:
+                params[x] = locals().get(x)
 
-        data = requests.get(url, params)
-        response = data.json()
-        if data.status_code != 200:
-            if data.status_code == 422:
-                return "Validation error: " + str(response)
-            else:
-                return response["error"]
+    data = requests.get(url, params)
+    response = data.json()
+    if data.status_code != 200:
+        if data.status_code == 422:
+            return "Validation error: " + str(response)
         else:
-            return response
-        
-print(Overfast.player(id="xanaxkitten-2112", type="all"))
+            return response["error"]
+    else:
+        return response
+
```

