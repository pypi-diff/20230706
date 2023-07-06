# Comparing `tmp/goxlr-1.1.0.tar.gz` & `tmp/goxlr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.1.0.tar", last modified: Wed Jul  5 12:38:56 2023, max compression
+gzip compressed data, was "goxlr-1.2.0.tar", last modified: Thu Jul  6 18:58:09 2023, max compression
```

## Comparing `goxlr-1.1.0.tar` & `goxlr-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.832906 goxlr-1.1.0/
--rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.1.0/LICENSE-3RD-PARTY.txt
--rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2503 2023-07-05 12:38:56.832906 goxlr-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2147 2023-07-05 12:32:01.000000 goxlr-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.824905 goxlr-1.1.0/goxlr/
--rw-rw-rw-   0        0        0       62 2023-07-05 11:07:26.000000 goxlr-1.1.0/goxlr/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-05 11:19:02.000000 goxlr-1.1.0/goxlr/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.831906 goxlr-1.1.0/goxlr/commands/
--rw-rw-rw-   0        0        0      108 2023-07-05 11:52:15.000000 goxlr-1.1.0/goxlr/commands/__init__.py
--rw-rw-rw-   0        0        0     1376 2023-07-05 12:17:31.000000 goxlr-1.1.0/goxlr/commands/daemon.py
--rw-rw-rw-   0        0        0      237 2023-07-05 11:08:41.000000 goxlr-1.1.0/goxlr/commands/general.py
--rw-rw-rw-   0        0        0    26136 2023-07-05 12:17:07.000000 goxlr-1.1.0/goxlr/commands/goxlr.py
--rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.1.0/goxlr/error.py
--rw-rw-rw-   0        0        0     2482 2023-07-05 12:32:25.000000 goxlr-1.1.0/goxlr/socket.py
--rw-rw-rw-   0        0        0    11533 2023-07-05 12:17:58.000000 goxlr-1.1.0/goxlr/types.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:38:56.828906 goxlr-1.1.0/goxlr.egg-info/
--rw-rw-rw-   0        0        0     2503 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 12:38:56.000000 goxlr-1.1.0/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-05 12:38:56.833408 goxlr-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-07-04 23:15:06.000000 goxlr-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.090412 goxlr-1.2.0/
+-rw-rw-rw-   0        0        0     1134 2023-07-04 22:58:41.000000 goxlr-1.2.0/LICENSE-3RD-PARTY.txt
+-rw-rw-rw-   0        0        0     1089 2023-07-04 22:53:25.000000 goxlr-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2503 2023-07-06 18:58:09.090914 goxlr-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2147 2023-07-05 12:48:27.000000 goxlr-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.079412 goxlr-1.2.0/goxlr/
+-rw-rw-rw-   0        0        0       62 2023-07-05 11:07:26.000000 goxlr-1.2.0/goxlr/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-06 18:57:22.000000 goxlr-1.2.0/goxlr/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.089412 goxlr-1.2.0/goxlr/commands/
+-rw-rw-rw-   0        0        0      108 2023-07-05 11:52:15.000000 goxlr-1.2.0/goxlr/commands/__init__.py
+-rw-rw-rw-   0        0        0     1376 2023-07-05 12:17:31.000000 goxlr-1.2.0/goxlr/commands/daemon.py
+-rw-rw-rw-   0        0        0      237 2023-07-05 11:08:41.000000 goxlr-1.2.0/goxlr/commands/general.py
+-rw-rw-rw-   0        0        0    26136 2023-07-05 12:17:07.000000 goxlr-1.2.0/goxlr/commands/goxlr.py
+-rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.2.0/goxlr/error.py
+-rw-rw-rw-   0        0        0     5101 2023-07-06 18:56:24.000000 goxlr-1.2.0/goxlr/socket.py
+-rw-rw-rw-   0        0        0    11533 2023-07-05 12:17:58.000000 goxlr-1.2.0/goxlr/types.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:58:09.084913 goxlr-1.2.0/goxlr.egg-info/
+-rw-rw-rw-   0        0        0     2503 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 18:58:09.000000 goxlr-1.2.0/goxlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-07-04 15:57:33.000000 goxlr-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-06 18:58:09.091911 goxlr-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-04 23:15:06.000000 goxlr-1.2.0/setup.py
```

### Comparing `goxlr-1.1.0/LICENSE-3RD-PARTY.txt` & `goxlr-1.2.0/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.1.0/LICENSE.txt` & `goxlr-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.1.0/PKG-INFO` & `goxlr-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -35,15 +35,15 @@
 
 from goxlr import GoXLR
 from goxlr.types import Fader, Channel
 
 async def main():
     async with GoXLR() as xlr:
         await xlr.set_fader(Fader.A, Channel.Headphones)
-        await xlr.set_volume(Channel.Headphones, 0.5)
+        await xlr.set_volume(Channel.Headphones, 127)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
 ```py
```

### Comparing `goxlr-1.1.0/README.md` & `goxlr-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from goxlr import GoXLR
 from goxlr.types import Fader, Channel
 
 async def main():
     async with GoXLR() as xlr:
         await xlr.set_fader(Fader.A, Channel.Headphones)
-        await xlr.set_volume(Channel.Headphones, 0.5)
+        await xlr.set_volume(Channel.Headphones, 127)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
 ```py
```

### Comparing `goxlr-1.1.0/goxlr/commands/daemon.py` & `goxlr-1.2.0/goxlr/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.1.0/goxlr/commands/goxlr.py` & `goxlr-1.2.0/goxlr/commands/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.1.0/goxlr/types.py` & `goxlr-1.2.0/goxlr/types.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.1.0/goxlr.egg-info/PKG-INFO` & `goxlr-1.2.0/goxlr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -35,15 +35,15 @@
 
 from goxlr import GoXLR
 from goxlr.types import Fader, Channel
 
 async def main():
     async with GoXLR() as xlr:
         await xlr.set_fader(Fader.A, Channel.Headphones)
-        await xlr.set_volume(Channel.Headphones, 0.5)
+        await xlr.set_volume(Channel.Headphones, 127)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 You may have noticed that we use `with` to manage the connection to the GoXLR. You may also wish to use the more traditional open and close methods which is acceptable too.
 ```py
```

### Comparing `goxlr-1.1.0/setup.py` & `goxlr-1.2.0/setup.py`

 * *Files identical despite different names*

