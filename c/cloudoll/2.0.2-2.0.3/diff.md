# Comparing `tmp/cloudoll-2.0.2.tar.gz` & `tmp/cloudoll-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-2.0.2.tar", last modified: Mon Jul  3 04:39:51 2023, max compression
+gzip compressed data, was "cloudoll-2.0.3.tar", last modified: Thu Jul  6 03:43:43 2023, max compression
```

## Comparing `cloudoll-2.0.2.tar` & `cloudoll-2.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.949346 cloudoll-2.0.2/
--rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.2/LICENSE
--rw-r--r--   0 xiaobei    (501) staff       (20)     7081 2023-07-03 04:39:51.948700 cloudoll-2.0.2/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)     6448 2023-07-03 04:37:53.000000 cloudoll-2.0.2/README.md
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.933204 cloudoll-2.0.2/cloudoll/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.937559 cloudoll-2.0.2/cloudoll/error/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/error/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/error/errors.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.938274 cloudoll-2.0.2/cloudoll/logging/
--rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.2/cloudoll/logging/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.939679 cloudoll-2.0.2/cloudoll/mail/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/mail/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.2/cloudoll/mail/smtp.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.941254 cloudoll-2.0.2/cloudoll/orm/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/orm/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.2/cloudoll/orm/mysql.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.943564 cloudoll-2.0.2/cloudoll/robot/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/robot/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.2/cloudoll/robot/dingtalk.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.2/cloudoll/robot/feishu.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.947568 cloudoll-2.0.2/cloudoll/web/
--rw-r--r--   0 xiaobei    (501) staff       (20)    13907 2023-07-03 03:45:50.000000 cloudoll-2.0.2/cloudoll/web/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.2/cloudoll/web/html.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.2/cloudoll/web/http.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.2/cloudoll/web/jwt.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.2/cloudoll/web/settings.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-03 04:39:51.936372 cloudoll-2.0.2/cloudoll.egg-info/
--rw-r--r--   0 xiaobei    (501) staff       (20)     7081 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)      104 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/requires.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-03 04:39:51.000000 cloudoll-2.0.2/cloudoll.egg-info/top_level.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-03 04:39:51.949521 cloudoll-2.0.2/setup.cfg
--rw-r--r--   0 xiaobei    (501) staff       (20)     4153 2023-07-03 03:40:13.000000 cloudoll-2.0.2/setup.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.473207 cloudoll-2.0.3/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.3/LICENSE
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7131 2023-07-06 03:43:43.472624 cloudoll-2.0.3/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6497 2023-07-06 01:49:11.000000 cloudoll-2.0.3/README.md
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.459141 cloudoll-2.0.3/cloudoll/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.463281 cloudoll-2.0.3/cloudoll/error/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/error/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/error/errors.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.463921 cloudoll-2.0.3/cloudoll/logging/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.3/cloudoll/logging/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.465102 cloudoll-2.0.3/cloudoll/mail/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/mail/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.3/cloudoll/mail/smtp.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.465963 cloudoll-2.0.3/cloudoll/orm/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/orm/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.3/cloudoll/orm/mysql.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.468034 cloudoll-2.0.3/cloudoll/robot/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/robot/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.3/cloudoll/robot/dingtalk.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.3/cloudoll/robot/feishu.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.471761 cloudoll-2.0.3/cloudoll/web/
+-rw-r--r--   0 xiaobei    (501) staff       (20)    13965 2023-07-06 01:49:11.000000 cloudoll-2.0.3/cloudoll/web/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/web/html.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.3/cloudoll/web/http.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.3/cloudoll/web/jwt.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.3/cloudoll/web/settings.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.462197 cloudoll-2.0.3/cloudoll.egg-info/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7131 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)      121 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/requires.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/top_level.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-06 03:43:43.473381 cloudoll-2.0.3/setup.cfg
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4177 2023-07-06 01:49:11.000000 cloudoll-2.0.3/setup.py
```

### Comparing `cloudoll-2.0.2/LICENSE` & `cloudoll-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/PKG-INFO` & `cloudoll-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.2
+Version: 2.0.3
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -324,7 +324,14 @@
   user: root
   password: abcd
   db: blog
   charset: utf8mb4
 ```
 
 默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
+
+
+# 开发模式
+
+```sh
+adev runserver app.py
+```
```

### Comparing `cloudoll-2.0.2/README.md` & `cloudoll-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -305,7 +305,14 @@
   user: root
   password: abcd
   db: blog
   charset: utf8mb4
 ```
 
 默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
+
+
+# 开发模式
+
+```sh
+adev runserver app.py
+```
```

### Comparing `cloudoll-2.0.2/cloudoll/error/errors.py` & `cloudoll-2.0.3/cloudoll/error/errors.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/logging/__init__.py` & `cloudoll-2.0.3/cloudoll/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/mail/smtp.py` & `cloudoll-2.0.3/cloudoll/mail/smtp.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/orm/mysql.py` & `cloudoll-2.0.3/cloudoll/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/robot/dingtalk.py` & `cloudoll-2.0.3/cloudoll/robot/dingtalk.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/robot/feishu.py` & `cloudoll-2.0.3/cloudoll/robot/feishu.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/web/__init__.py` & `cloudoll-2.0.3/cloudoll/web/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,17 +148,17 @@
         loop = asyncio.get_event_loop()
         if loop is None:
             loop = asyncio.new_event_loop()
         self._loop = loop
 
         parser = argparse.ArgumentParser(description="cloudoll app.")
         parser.add_argument("--env", default="local")
-        parser.add_argument("--host")
-        parser.add_argument("--port")
-        parser.add_argument("--path")
+        parser.add_argument("--host", default=None)
+        parser.add_argument("--port", default=None)
+        parser.add_argument("--path", default=None)
         args, extra_argv = parser.parse_known_args()
         config = get_config(args.env)
 
         self._args = args
         self.config = config
 
         # middlewares
@@ -295,30 +295,30 @@
             # print(module, router)
             importlib.import_module(module, fd)
 
         self.app.add_routes(self._route_table)
         # for route in self._routes:
         #     self.app.router.add_route(**route)
 
-    def run(self, **kw):
+    def run(self, *args, **kw):
         """
         run app
         :params prot default  9001
         :params host default 127.0.0.1
         """
         conf = self.config.get("server", {})
-        if conf.get('reload',False) is True:
-            import aioreloader
-            aioreloader.start()
-        conf.update(kw)
-        conf.update(vars(self._args))
-        conf = argparse.Namespace(**conf)
-        host = conf.host if conf.host else "localhost"
-        port = conf.port if conf.port else 9001
-        path = conf.path
+        # if conf.get('reload',False) is True:
+        # import aioreloader
+        # aioreloader.start()
+        conf.update(args)
+        args = {k: v for k, v in vars(self._args).items() if v is not None}
+        conf.update(args)
+        host = conf.get("host", "127.0.0.1")
+        port = conf.get("port", 9001)
+        path = conf.get("path")
         _check_address(host, port)
         # logging.info(f"Server run at http://{host}:{port}")
         web.run_app(
             self.app,
             loop=self._loop,
             host=host,
             port=port,
```

### Comparing `cloudoll-2.0.2/cloudoll/web/html.py` & `cloudoll-2.0.3/cloudoll/web/html.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/web/http.py` & `cloudoll-2.0.3/cloudoll/web/http.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll/web/jwt.py` & `cloudoll-2.0.3/cloudoll/web/jwt.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/cloudoll.egg-info/PKG-INFO` & `cloudoll-2.0.3/cloudoll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.2
+Version: 2.0.3
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -324,7 +324,14 @@
   user: root
   password: abcd
   db: blog
   charset: utf8mb4
 ```
 
 默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
+
+
+# 开发模式
+
+```sh
+adev runserver app.py
+```
```

### Comparing `cloudoll-2.0.2/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.0.3/cloudoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.2/setup.py` & `cloudoll-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 # Package meta-data.
 NAME = "cloudoll"
 DESCRIPTION = "辅助快速创建可分布的微服务。"
 URL = "https://gitee.com/chuchur/cloudoll-py"
 EMAIL = "chuchur@qq.com"
 AUTHOR = "chuchur"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.0.2"
+VERSION = "2.0.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "colorlog",
     "aiomysql",
     "aiopg",
     "aiohttp",
     "aioredis",
     "aiomcache",
+    "aiohttp-devtools",
     "jinja2",
     "pyjwt",
     "aiohttp_session[secure]",
     "PyYAML",
 ]
 
 # What packages are optional?
```

