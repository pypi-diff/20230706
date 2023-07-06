# Comparing `tmp/libsodium-2.6.0.tar.gz` & `tmp/libsodium-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsodium-2.6.0.tar", last modified: Wed Jul  5 19:00:23 2023, max compression
+gzip compressed data, was "libsodium-2.6.1.tar", last modified: Thu Jul  6 21:52:54 2023, max compression
```

## Comparing `libsodium-2.6.0.tar` & `libsodium-2.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.242575 libsodium-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 18:59:57.000000 libsodium-2.6.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-05 19:00:23.242575 libsodium-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-05 18:59:57.000000 libsodium-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 18:59:57.000000 libsodium-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 19:00:23.242575 libsodium-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.238575 libsodium-2.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.238575 libsodium-2.6.0/src/libsodium/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27113 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.242575 libsodium-2.6.0/src/libsodium/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/db/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-05 18:59:57.000000 libsodium-2.6.0/src/libsodium/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:00:23.238575 libsodium-2.6.0/src/libsodium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 19:00:23.000000 libsodium-2.6.0/src/libsodium.egg-info/top_level.txt
+drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-07-06 21:52:54.615748 libsodium-2.6.1/
+-rw-r--r--   0 ahsan      (502) staff       (20)     1064 2023-06-19 17:00:12.000000 libsodium-2.6.1/LICENCE
+-rw-r--r--   0 ahsan      (502) staff       (20)      980 2023-07-06 21:52:54.615875 libsodium-2.6.1/PKG-INFO
+-rw-r--r--   0 ahsan      (502) staff       (20)      485 2023-07-06 21:17:35.000000 libsodium-2.6.1/README.md
+-rw-r--r--   0 ahsan      (502) staff       (20)      104 2023-06-19 17:00:12.000000 libsodium-2.6.1/pyproject.toml
+-rw-r--r--   0 ahsan      (502) staff       (20)      620 2023-07-06 21:52:54.616535 libsodium-2.6.1/setup.cfg
+drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-07-06 21:52:54.398018 libsodium-2.6.1/src/
+drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-07-06 21:52:54.553453 libsodium-2.6.1/src/libsodium/
+-rw-r--r--   0 ahsan      (502) staff       (20)      297 2023-07-04 21:10:32.000000 libsodium-2.6.1/src/libsodium/__init__.py
+-rw-r--r--   0 ahsan      (502) staff       (20)    27120 2023-07-06 21:17:12.000000 libsodium-2.6.1/src/libsodium/__main__.py
+-rw-r--r--   0 ahsan      (502) staff       (20)     3981 2023-07-05 16:16:16.000000 libsodium-2.6.1/src/libsodium/classes.py
+drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-07-06 21:52:54.615012 libsodium-2.6.1/src/libsodium/db/
+-rw-r--r--   0 ahsan      (502) staff       (20)      487 2023-06-19 17:00:12.000000 libsodium-2.6.1/src/libsodium/db/__init__.py
+-rw-r--r--   0 ahsan      (502) staff       (20)      302 2023-06-19 17:00:12.000000 libsodium-2.6.1/src/libsodium/db/connect.py
+-rw-r--r--   0 ahsan      (502) staff       (20)      348 2023-07-04 21:10:32.000000 libsodium-2.6.1/src/libsodium/utils.py
+-rw-r--r--   0 ahsan      (502) staff       (20)    10707 2023-07-06 21:16:45.000000 libsodium-2.6.1/src/libsodium/wsgi.py
+drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-07-06 21:52:54.571328 libsodium-2.6.1/src/libsodium.egg-info/
+-rw-r--r--   0 ahsan      (502) staff       (20)      980 2023-07-06 21:52:54.000000 libsodium-2.6.1/src/libsodium.egg-info/PKG-INFO
+-rw-r--r--   0 ahsan      (502) staff       (20)      369 2023-07-06 21:52:54.000000 libsodium-2.6.1/src/libsodium.egg-info/SOURCES.txt
+-rw-r--r--   0 ahsan      (502) staff       (20)        1 2023-07-06 21:52:54.000000 libsodium-2.6.1/src/libsodium.egg-info/dependency_links.txt
+-rw-r--r--   0 ahsan      (502) staff       (20)       10 2023-07-06 21:52:54.000000 libsodium-2.6.1/src/libsodium.egg-info/top_level.txt
```

### Comparing `libsodium-2.6.0/LICENCE` & `libsodium-2.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `libsodium-2.6.0/PKG-INFO` & `libsodium-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `libsodium-2.6.0/setup.cfg` & `libsodium-2.6.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libsodium
-version = 2.6.0
+version = 2.6.1
 author = Ahsan Ahmed
 author_email = ahsan.ahmed3246@gmail.com
 description = A simple web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://libsodium.readthedocs.io/en/latest/
 project_urls =
```

### Comparing `libsodium-2.6.0/src/libsodium/__main__.py` & `libsodium-2.6.1/src/libsodium/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             S:::::So::::o     o::::od:::::d     d:::::d  i::::i u:::::uuuu:::::u  m::::m   m::::m   m::::m
 SSSSSSS     S:::::So:::::ooooo:::::od::::::ddddd::::::ddi::::::iu:::::::::::::::uum::::m   m::::m   m::::m
 S::::::SSSSSS:::::So:::::::::::::::o d:::::::::::::::::di::::::i u:::::::::::::::um::::m   m::::m   m::::m
 S:::::::::::::::SS  oo:::::::::::oo   d:::::::::ddd::::di::::::i  uu::::::::uu:::um::::m   m::::m   m::::m
  SSSSSSSSSSSSSSS      ooooooooooo      ddddddddd   dddddiiiiiiii    uuuuuuuu  uuuummmmmm   mmmmmm   mmmmmm
 """
     print("\x1b[32m"+x+"\x1b[0m")
-    print("v2.60\nMade by ahsan")
+    print("v2.61\nMade by ahsan")
     exit()
 
 if args[0] == "init":
     print("\033[93m"+"Name for project(leave blank to use current directory):"+"\x1b[0m")
     project_name = input("\x1b[32m"+"> ")
     print("\033[93m"+"What is your interpreter(ex. python3, python, py)"+"\x1b[0m")
     interpreter = input("\x1b[32m"+"> ")
@@ -180,15 +180,15 @@
     return server
 
 if __name__ == "__main__":
     import grpc
     from concurrent import futures
     addAll(grpc.server(futures.ThreadPoolExecutor(max_workers=10)))""")
 
-    os.mkdir("src/templates")
+    os.mkdir(prefix+"src/templates")
     x = open(prefix+"src/templates/.sodium", "w")
     x.write(os.getcwd()+f"/{project_name}")
     x.close()
 
     x = open(prefix+"start.py", 'w')
     x.write('''from libsodium import Deamon
 from sonora.wsgi import grpcWSGI
@@ -252,15 +252,15 @@
 SSSSSSS     S:::::So:::::ooooo:::::od::::::ddddd::::::ddi::::::iu:::::::::::::::uum::::m   m::::m   m::::m
 S::::::SSSSSS:::::So:::::::::::::::o d:::::::::::::::::di::::::i u:::::::::::::::um::::m   m::::m   m::::m
 S:::::::::::::::SS  oo:::::::::::oo   d:::::::::ddd::::di::::::i  uu::::::::uu:::um::::m   m::::m   m::::m
  SSSSSSSSSSSSSSS      ooooooooooo      ddddddddd   dddddiiiiiiii    uuuuuuuu  uuuummmmmm   mmmmmm   mmmmmm
 
     """
     print(F_Green+x+F_End)
-    print("v2.60")
+    print("v2.61")
     print(f"{getCurrentTime()} [{F_Magenta}INFO{F_End}] Creating Deamon... ")
     MainDeamon = Deamon()
 
     print(f"{getCurrentTime()} [{F_LightCyan}SocketIO{F_End}] Loading SocketIO app...")
     from src.websockets.app import sio
     from os import listdir
     from os.path import isfile
```

### Comparing `libsodium-2.6.0/src/libsodium/classes.py` & `libsodium-2.6.1/src/libsodium/classes.py`

 * *Files identical despite different names*

### Comparing `libsodium-2.6.0/src/libsodium/wsgi.py` & `libsodium-2.6.1/src/libsodium/wsgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                     rules = []
                     for name, value in zip(names, values):
                         rules.append((name, value.typ, value.regex))
                     blueprint = Blueprint(rules)
 
                 blueprint = blueprint.blueprint
                 if not request.mimetype in targetMimetypes:
-                    rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.60</p>")
+                    rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.61</p>")
                     rsp.headers['Content-Type'] = 'text/html' 
                     return rsp(environ, start_response)
                 if request.mimetype == "application/x-www-form-urlencoded":
                     target = request.form
                 elif request.mimetype == "multipart/form":
                         target = request.form
                 elif request.mimetype == "application/json":
```

### Comparing `libsodium-2.6.0/src/libsodium.egg-info/PKG-INFO` & `libsodium-2.6.1/src/libsodium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

