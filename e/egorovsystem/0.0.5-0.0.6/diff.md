# Comparing `tmp/egorovsystem-0.0.5.tar.gz` & `tmp/egorovsystem-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\egorovsystem-0.0.5.tar", last modified: Thu Jul  6 02:10:46 2023, max compression
+gzip compressed data, was "dist\egorovsystem-0.0.6.tar", last modified: Thu Jul  6 03:33:53 2023, max compression
```

## Comparing `egorovsystem-0.0.5.tar` & `egorovsystem-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.915886 egorovsystem-0.0.5/
--rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1562 2023-07-06 02:10:46.914885 egorovsystem-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.865873 egorovsystem-0.0.5/egolocal/
--rw-rw-rw-   0        0        0     1473 2023-07-05 20:07:45.000000 egorovsystem-0.0.5/egolocal/main.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.867874 egorovsystem-0.0.5/egorovsystem/
--rw-rw-rw-   0        0        0      475 2023-07-05 19:40:59.000000 egorovsystem-0.0.5/egorovsystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.876876 egorovsystem-0.0.5/egorovsystem.egg-info/
--rw-rw-rw-   0        0        0     1562 2023-07-06 02:10:46.000000 egorovsystem-0.0.5/egorovsystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2023-07-06 02:10:46.000000 egorovsystem-0.0.5/egorovsystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 02:10:46.000000 egorovsystem-0.0.5/egorovsystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-06 02:10:46.000000 egorovsystem-0.0.5/egorovsystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2023-07-06 02:10:46.000000 egorovsystem-0.0.5/egorovsystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-06 02:10:46.000000 egorovsystem-0.0.5/egorovsystem.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.881877 egorovsystem-0.0.5/egoserver/
--rw-rw-rw-   0        0        0        0 2023-07-06 02:03:41.000000 egorovsystem-0.0.5/egoserver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.892880 egorovsystem-0.0.5/egoserver/egoserver/
--rw-rw-rw-   0        0        0        0 2023-07-05 17:33:47.000000 egorovsystem-0.0.5/egoserver/egoserver/__init__.py
--rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.5/egoserver/egoserver/asgi.py
--rw-rw-rw-   0        0        0       83 2023-07-05 17:41:34.000000 egorovsystem-0.0.5/egoserver/egoserver/secret.py
--rw-rw-rw-   0        0        0     3369 2023-07-05 19:09:44.000000 egorovsystem-0.0.5/egoserver/egoserver/settings.py
--rw-rw-rw-   0        0        0      847 2023-07-05 17:55:04.000000 egorovsystem-0.0.5/egoserver/egoserver/urls.py
--rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.5/egoserver/egoserver/wsgi.py
--rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.5/egoserver/manage.py
--rw-rw-rw-   0        0        0      823 2023-07-06 02:10:10.000000 egorovsystem-0.0.5/egoserver/run.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.906883 egorovsystem-0.0.5/egoserver/server/
--rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.5/egoserver/server/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-05 17:41:04.000000 egorovsystem-0.0.5/egoserver/server/admin.py
--rw-rw-rw-   0        0        0      150 2023-07-05 17:35:32.000000 egorovsystem-0.0.5/egoserver/server/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.909883 egorovsystem-0.0.5/egoserver/server/migrations/
--rw-rw-rw-   0        0        0     1387 2023-07-05 18:07:03.000000 egorovsystem-0.0.5/egoserver/server/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.5/egoserver/server/migrations/__init__.py
--rw-rw-rw-   0        0        0      747 2023-07-05 18:02:46.000000 egorovsystem-0.0.5/egoserver/server/models.py
--rw-rw-rw-   0        0        0       63 2023-07-05 17:35:32.000000 egorovsystem-0.0.5/egoserver/server/tests.py
--rw-rw-rw-   0        0        0      405 2023-07-05 18:59:18.000000 egorovsystem-0.0.5/egoserver/server/urls.py
--rw-rw-rw-   0        0        0      215 2023-07-05 17:59:31.000000 egorovsystem-0.0.5/egoserver/server/utils.py
--rw-rw-rw-   0        0        0     2466 2023-07-05 20:02:50.000000 egorovsystem-0.0.5/egoserver/server/views.py
--rw-rw-rw-   0        0        0       42 2023-07-06 02:10:46.915886 egorovsystem-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-07-06 02:10:41.000000 egorovsystem-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:10:46.912884 egorovsystem-0.0.5/test/
--rw-rw-rw-   0        0        0        0 2023-07-05 19:43:29.000000 egorovsystem-0.0.5/test/__init__.py
--rw-rw-rw-   0        0        0       63 2023-07-05 19:43:40.000000 egorovsystem-0.0.5/test/a.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.410831 egorovsystem-0.0.6/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1562 2023-07-06 03:33:53.409831 egorovsystem-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.349311 egorovsystem-0.0.6/egolocal/
+-rw-rw-rw-   0        0        0     1662 2023-07-06 02:37:41.000000 egorovsystem-0.0.6/egolocal/main.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.352311 egorovsystem-0.0.6/egorovsystem/
+-rw-rw-rw-   0        0        0     1880 2023-07-06 03:33:15.000000 egorovsystem-0.0.6/egorovsystem/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-07-06 03:29:21.000000 egorovsystem-0.0.6/egorovsystem/run_command.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.361313 egorovsystem-0.0.6/egorovsystem.egg-info/
+-rw-rw-rw-   0        0        0     1562 2023-07-06 03:33:53.000000 egorovsystem-0.0.6/egorovsystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      872 2023-07-06 03:33:53.000000 egorovsystem-0.0.6/egorovsystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:33:53.000000 egorovsystem-0.0.6/egorovsystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-06 03:33:53.000000 egorovsystem-0.0.6/egorovsystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-07-06 03:33:53.000000 egorovsystem-0.0.6/egorovsystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-06 03:33:53.000000 egorovsystem-0.0.6/egorovsystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.373316 egorovsystem-0.0.6/egoserver/
+-rw-rw-rw-   0        0        0        0 2023-07-06 02:03:41.000000 egorovsystem-0.0.6/egoserver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.384826 egorovsystem-0.0.6/egoserver/egoserver/
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:33:47.000000 egorovsystem-0.0.6/egoserver/egoserver/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.6/egoserver/egoserver/asgi.py
+-rw-rw-rw-   0        0        0       83 2023-07-05 17:41:34.000000 egorovsystem-0.0.6/egoserver/egoserver/secret.py
+-rw-rw-rw-   0        0        0     3369 2023-07-05 19:09:44.000000 egorovsystem-0.0.6/egoserver/egoserver/settings.py
+-rw-rw-rw-   0        0        0      847 2023-07-05 17:55:04.000000 egorovsystem-0.0.6/egoserver/egoserver/urls.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.6/egoserver/egoserver/wsgi.py
+-rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.6/egoserver/manage.py
+-rw-rw-rw-   0        0        0      823 2023-07-06 02:10:10.000000 egorovsystem-0.0.6/egoserver/run.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.399830 egorovsystem-0.0.6/egoserver/server/
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.6/egoserver/server/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-05 17:41:04.000000 egorovsystem-0.0.6/egoserver/server/admin.py
+-rw-rw-rw-   0        0        0      150 2023-07-05 17:35:32.000000 egorovsystem-0.0.6/egoserver/server/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.403831 egorovsystem-0.0.6/egoserver/server/migrations/
+-rw-rw-rw-   0        0        0     1387 2023-07-05 18:07:03.000000 egorovsystem-0.0.6/egoserver/server/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.6/egoserver/server/migrations/__init__.py
+-rw-rw-rw-   0        0        0      747 2023-07-05 18:02:46.000000 egorovsystem-0.0.6/egoserver/server/models.py
+-rw-rw-rw-   0        0        0       63 2023-07-05 17:35:32.000000 egorovsystem-0.0.6/egoserver/server/tests.py
+-rw-rw-rw-   0        0        0      405 2023-07-06 03:33:23.000000 egorovsystem-0.0.6/egoserver/server/urls.py
+-rw-rw-rw-   0        0        0      215 2023-07-05 17:59:31.000000 egorovsystem-0.0.6/egoserver/server/utils.py
+-rw-rw-rw-   0        0        0     2466 2023-07-06 03:33:36.000000 egorovsystem-0.0.6/egoserver/server/views.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:33:53.410831 egorovsystem-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-07-06 03:33:41.000000 egorovsystem-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:33:53.407832 egorovsystem-0.0.6/test/
+-rw-rw-rw-   0        0        0        0 2023-07-05 19:43:29.000000 egorovsystem-0.0.6/test/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-06 02:57:10.000000 egorovsystem-0.0.6/test/a.py
```

### Comparing `egorovsystem-0.0.5/LICENSE` & `egorovsystem-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.5/PKG-INFO` & `egorovsystem-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.5
+Version: 0.0.6
 Author: Yongyi Yang
 Author-email: yongyi@umich.edu
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `egorovsystem-0.0.5/egolocal/main.py` & `egorovsystem-0.0.6/egolocal/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 def ask_ip(): # 这个函数向环境变量中询问远端的地址
     server_ip = os.environ.get("EGOROV_SERVER")
     if server_ip is None:
         server_ip = input("server ip = ")
     return server_ip.strip()
 
 def ask_password(): # 这个函数询问密码
+    if os.environ.get("EGOROV_PWD"): # 只在个人计算机上存密码
+        return os.environ["EGOROV_PWD"]
     return input("password = ").strip()
 
 def get_data(server_ip, password, key, type):
     return requests.post("http://{0}/get/{1}/{2}".format(server_ip, type, key), json = {"password": password}).json()
 
 def run():
     # os.chdir(os.path.dirname(__file__))
@@ -33,15 +35,17 @@
     C.add_argument("--port" , type = int , default = 11451)
     C = C.parse_args()
 
     def ask_variable(request, key):
         return get_data(server_ip, password, key, "variable")
     def ask_function(request, key):
         return get_data(server_ip, password, key, "function")
-
+    def hello(request):
+        return "hello"
     start_server(ip = "127.0.0.1" , port = C.port , responsers = {
+        "hello":  hello, 
         "ask_variable/<str:key>":  ask_variable, 
         "ask_function/<str:key>":  ask_function, 
     } , encode = "json" , cross_domain = True)
 
 if __name__ == "__main__":
     run()
```

### Comparing `egorovsystem-0.0.5/egorovsystem.egg-info/PKG-INFO` & `egorovsystem-0.0.6/egorovsystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.5
+Version: 0.0.6
 Author: Yongyi Yang
 Author-email: yongyi@umich.edu
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `egorovsystem-0.0.5/egorovsystem.egg-info/SOURCES.txt` & `egorovsystem-0.0.6/egorovsystem.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 egolocal/main.py
 egorovsystem/__init__.py
+egorovsystem/run_command.py
 egorovsystem.egg-info/PKG-INFO
 egorovsystem.egg-info/SOURCES.txt
 egorovsystem.egg-info/dependency_links.txt
 egorovsystem.egg-info/entry_points.txt
 egorovsystem.egg-info/requires.txt
 egorovsystem.egg-info/top_level.txt
 egoserver/__init__.py
```

### Comparing `egorovsystem-0.0.5/egoserver/egoserver/settings.py` & `egorovsystem-0.0.6/egoserver/egoserver/settings.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.5/egoserver/egoserver/urls.py` & `egorovsystem-0.0.6/egoserver/egoserver/urls.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.5/egoserver/manage.py` & `egorovsystem-0.0.6/egoserver/manage.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.5/egoserver/run.py` & `egorovsystem-0.0.6/egoserver/run.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.5/egoserver/server/migrations/0001_initial.py` & `egorovsystem-0.0.6/egoserver/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.5/egoserver/server/models.py` & `egorovsystem-0.0.6/egoserver/server/models.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.5/egoserver/server/views.py` & `egorovsystem-0.0.6/egoserver/server/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     var = var [0]
 
     return JsonResponse({
         "val": var.val , 
         "errorflag": False , 
     })
 
-def get_fucntion(request , key):
+def get_function(request , key):
 
     flag, info = check_password(request)
     if flag == 0:
         return info
 
     fun = Function.objects.filter(key = key)
     if len(fun) == 0: # no such function
```

### Comparing `egorovsystem-0.0.5/setup.py` & `egorovsystem-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 print (find_packages())
 pkgs = [p for p in find_packages() if p.startswith("ego")]
 print(pkgs)
 
 setup(
 	name					= "egorovsystem",
-	version					= "0.0.5",
+	version					= "0.0.6",
 	description				= "",
 	long_description		= readme,
 	long_description_content_type	= "text/markdown",
 	license					= license,
 	author					= "Yongyi Yang",
 	author_email 			= "yongyi@umich.edu",
 	python_requires			= ">=3.6",
```

