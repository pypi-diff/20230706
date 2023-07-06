# Comparing `tmp/flaskz-1.6.1.tar.gz` & `tmp/flaskz-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.6.1.tar", last modified: Fri Jun 30 16:00:44 2023, max compression
+gzip compressed data, was "flaskz-1.6.2.tar", last modified: Thu Jul  6 03:11:18 2023, max compression
```

## Comparing `flaskz-1.6.1.tar` & `flaskz-1.6.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.771311 flaskz-1.6.1/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.6.1/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     7075 2023-06-30 16:00:44.771673 flaskz-1.6.1/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     6647 2023-06-30 02:28:23.000000 flaskz-1.6.1/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.6.1/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      704 2023-06-30 16:00:44.773515 flaskz-1.6.1/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.715405 flaskz-1.6.1/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.720337 flaskz-1.6.1/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-06-30 16:00:17.000000 flaskz-1.6.1/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.730228 flaskz-1.6.1/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.6.1/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.6.1/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.734334 flaskz-1.6.1/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.6.1/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.6.1/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)    13138 2023-06-26 06:34:52.000000 flaskz-1.6.1/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.735742 flaskz-1.6.1/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2390 2023-06-26 06:36:09.000000 flaskz-1.6.1/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.743379 flaskz-1.6.1/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5516 2023-06-25 03:55:22.000000 flaskz-1.6.1/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    29490 2023-06-20 08:28:35.000000 flaskz-1.6.1/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10649 2023-06-17 12:07:38.000000 flaskz-1.6.1/src/flaskz/models/_model.py
--rw-r--r--   0 taozh      (501) staff       (20)     9352 2023-06-26 02:18:53.000000 flaskz-1.6.1/src/flaskz/models/_query_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7426 2023-06-21 08:20:49.000000 flaskz-1.6.1/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.6.1/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.749027 flaskz-1.6.1/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    19434 2023-06-25 06:21:35.000000 flaskz-1.6.1/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.6.1/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.6.1/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.769925 flaskz-1.6.1/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.6.1/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.6.1/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.6.1/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.6.1/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.6.1/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.6.1/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.6.1/src/flaskz/utils/_magic.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6570 2023-06-25 10:52:01.000000 flaskz-1.6.1/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      961 2023-06-25 04:29:38.000000 flaskz-1.6.1/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.6.1/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     4522 2023-06-29 07:20:02.000000 flaskz-1.6.1/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.726687 flaskz-1.6.1/src/flaskz.egg-info/
--rwxrwxrwx   0 taozh      (501) staff       (20)     7075 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      952 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.739321 flaskz-1.6.2/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.6.2/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     7215 2023-07-06 03:11:18.739468 flaskz-1.6.2/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6769 2023-07-06 02:34:05.000000 flaskz-1.6.2/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.6.2/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      776 2023-07-06 03:11:18.740287 flaskz-1.6.2/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.711022 flaskz-1.6.2/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.716218 flaskz-1.6.2/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-07-06 02:20:13.000000 flaskz-1.6.2/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.719566 flaskz-1.6.2/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.6.2/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.6.2/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.721735 flaskz-1.6.2/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.6.2/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.6.2/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    13548 2023-07-06 03:10:54.000000 flaskz-1.6.2/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.722370 flaskz-1.6.2/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.6.2/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.726255 flaskz-1.6.2/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5524 2023-07-06 02:21:14.000000 flaskz-1.6.2/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    29523 2023-07-06 02:23:24.000000 flaskz-1.6.2/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10649 2023-06-17 12:07:38.000000 flaskz-1.6.2/src/flaskz/models/_model.py
+-rw-r--r--   0 taozh      (501) staff       (20)     9352 2023-06-26 02:18:53.000000 flaskz-1.6.2/src/flaskz/models/_query_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7426 2023-06-21 08:20:49.000000 flaskz-1.6.2/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.6.2/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.729022 flaskz-1.6.2/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    19434 2023-06-25 06:21:35.000000 flaskz-1.6.2/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.6.2/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.6.2/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.738293 flaskz-1.6.2/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.6.2/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.6.2/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.6.2/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.6.2/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.6.2/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.6.2/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.6.2/src/flaskz/utils/_magic.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6570 2023-06-25 10:52:01.000000 flaskz-1.6.2/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      973 2023-07-06 02:17:15.000000 flaskz-1.6.2/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.6.2/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     4522 2023-06-29 07:20:02.000000 flaskz-1.6.2/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-07-06 03:11:18.718433 flaskz-1.6.2/src/flaskz.egg-info/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7215 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      952 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       88 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-07-06 03:11:18.000000 flaskz-1.6.2/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.6.1/LICENSE` & `flaskz-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/PKG-INFO` & `flaskz-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.6.1
+Version: 1.6.2
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: ext
 License-File: LICENSE
 
 ## 关于
 
 *Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
@@ -24,14 +25,16 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.2** `2023/07/06`
+    - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
     - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
     - [A] `BaseModelMixin`添加`clear_db`方法, 用于清空数据
     - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
```

### Comparing `flaskz-1.6.1/README.md` & `flaskz-1.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.2** `2023/07/06`
+    - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
     - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
     - [A] `BaseModelMixin`添加`clear_db`方法, 用于清空数据
     - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
```

### Comparing `flaskz-1.6.1/setup.cfg` & `flaskz-1.6.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.6.1
+version = 1.6.2
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls = 
@@ -20,14 +20,19 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	Flask>=1.1.1
 	SQLAlchemy>=1.3.13
 	requests>=2
 
+[options.extras_require]
+ext = 
+	pycryptodome>=3.15.0
+	paramiko>=3.0.0
+
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `flaskz-1.6.1/src/flaskz/auth/_jws.py` & `flaskz-1.6.2/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/ext/cypher.py` & `flaskz-1.6.2/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/ext/ssh.py` & `flaskz-1.6.2/src/flaskz/ext/ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     # remove text before command ex) [root@localhost ~]# ls -l
     cmd_pattern = re.compile('.*([#$])( )*' + re.escape(command))  # @2023-06-07 change ([#$])? --> ([#$])
     last_match = None
     for match in cmd_pattern.finditer(txt):
         last_match = match
     if last_match:
         txt = txt[last_match.end():]
-    path_pattern = re.compile('.*[#$] ')
+    path_pattern = re.compile('.*[#$]( )?')  # @2023-07-06 change '.*[#$] ' --> '.*[#$]( )?'
     txt = path_pattern.sub('', txt)  # remove the path info
     txt = txt.replace(command + '\r\n', '')  # remove the command
     return txt.strip()
 
 
 def _remove_end_slash(path):
     """Remove ending slash """
@@ -313,19 +313,28 @@
 
 if __name__ == '__main__':
     servers = [
         {  # C9300
             'host': '10.75.37.165',
             'username': 'admin',
             'password': 'Cisco123',
-            # 'secondary_password': 'Cisco123',
+            'secondary_password': 'Cisco123',
             'recv_endswith': ['# ', '$ ', ': ', '? ', '#'],
-            'commands': ['enable', 'Cisco123', {'command': 'show run', 'wait': False}]
+            'commands': ['enable', 'show udp | in ( 514 )']
             # 'commands': ['show run']
         },
+        # {  # C9300
+        #     'host': '10.75.37.165',
+        #     'username': 'admin',
+        #     'password': 'Cisco123',
+        #     # 'secondary_password': 'Cisco123',
+        #     'recv_endswith': ['# ', '$ ', ': ', '? ', '#'],
+        #     'commands': ['enable', 'Cisco123', {'command': 'show run', 'wait': False}]
+        #     # 'commands': ['show run']
+        # },
         # {  # Centos
         #     'host': '10.124.4.21',
         #     'username': 'admin1',
         #     'password': 'Cisco@123',
         #     'commands': ['show int eth3/1']
         # },
         # {  # Centos
```

### Comparing `flaskz-1.6.1/src/flaskz/log/__init__.py` & `flaskz-1.6.2/src/flaskz/log/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
 
 
 def _log_data_converter(value):
     if isinstance(value, datetime.datetime):
         return value.__str__()
 
 
-from ..utils import get_app_config_items
+from ..utils._app import get_app_config_items
```

### Comparing `flaskz-1.6.1/src/flaskz/models/__init__.py` & `flaskz-1.6.2/src/flaskz/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 from flask import Flask
 from sqlalchemy import create_engine, event
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine import ExceptionContext
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
-from ..log import flaskz_logger
-from ..utils import Attribute
-
 DBSession = sessionmaker(autocommit=False)
 
 ModelBase = declarative_base()
 
 
 def init_model(app):
     """
@@ -126,8 +123,10 @@
 
 
 from ._base import *
 from ._model import *
 from ._util import *
 from ._query_util import *
 
-from ..utils import get_app_config_items
+from ..utils._cls import Attribute
+from ..utils._app import get_app_config_items
+from ..log import flaskz_logger
```

### Comparing `flaskz-1.6.1/src/flaskz/models/_base.py` & `flaskz-1.6.2/src/flaskz/models/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from sqlalchemy import text, Integer, Numeric
 
 from .. import res_status_codes
-from ..utils import find_list, filter_list, is_str, is_dict, is_list, ins_to_dict, get_dict_value_by_type
+from ..utils._cls import ins_to_dict
+from ..utils._common import find_list, filter_list, is_str, is_dict, is_list, get_dict_value_by_type
 
 __all__ = ['BaseModelMixin']
 
 
 class BaseModelMixin:
     # -------------------------------------------about model-------------------------------------------
     @classmethod
```

### Comparing `flaskz-1.6.1/src/flaskz/models/_model.py` & `flaskz-1.6.2/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/models/_query_util.py` & `flaskz-1.6.2/src/flaskz/models/_query_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/models/_util.py` & `flaskz-1.6.2/src/flaskz/models/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/res_status_codes.py` & `flaskz-1.6.2/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/rest/__init__.py` & `flaskz-1.6.2/src/flaskz/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/rest/_mgmt.py` & `flaskz-1.6.2/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/rest/_util.py` & `flaskz-1.6.2/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_app.py` & `flaskz-1.6.2/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_cache.py` & `flaskz-1.6.2/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_cls.py` & `flaskz-1.6.2/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_common.py` & `flaskz-1.6.2/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_func.py` & `flaskz-1.6.2/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_magic.py` & `flaskz-1.6.2/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_request_api.py` & `flaskz-1.6.2/src/flaskz/utils/_request_api.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_request_args.py` & `flaskz-1.6.2/src/flaskz/utils/_request_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,8 +39,8 @@
         pass
     if data is None:
         if len(args) > 0:
             return args[0]
     return data
 
 
-from ..models import parse_pss as get_pss
+from ..models._query_util import parse_pss as get_pss
```

### Comparing `flaskz-1.6.1/src/flaskz/utils/_response.py` & `flaskz-1.6.2/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz/utils/_timer.py` & `flaskz-1.6.2/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6.1/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.6.2/src/flaskz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.6.1
+Version: 1.6.2
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: ext
 License-File: LICENSE
 
 ## 关于
 
 *Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
@@ -24,14 +25,16 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.2** `2023/07/06`
+    - [F] 修复`flaskz.utils._request_args.py`中`import parse_pss as get_pss`的导入问题
 - **1.6.1** `2023/07/01`
     - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
     - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
     - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
     - [A] `BaseModelMixin`添加`clear_db`方法, 用于清空数据
     - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
```

### Comparing `flaskz-1.6.1/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.6.2/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

