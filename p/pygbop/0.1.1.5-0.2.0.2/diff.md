# Comparing `tmp/pygbop-0.1.1.5.tar.gz` & `tmp/pygbop-0.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygbop-0.1.1.5.tar", last modified: Tue Apr 25 09:46:41 2023, max compression
+gzip compressed data, was "dist\pygbop-0.2.0.2.tar", last modified: Wed Jul  5 08:06:40 2023, max compression
```

## Comparing `pygbop-0.1.1.5.tar` & `pygbop-0.2.0.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/
--rw-rw-rw-   0        0        0       40 2023-02-15 06:22:38.000000 pygbop-0.1.1.5/.gitignore
--rw-rw-rw-   0        0        0        2 2022-07-08 11:04:28.000000 pygbop-0.1.1.5/a.txt
--rw-rw-rw-   0        0        0      544 2022-07-08 06:25:59.000000 pygbop-0.1.1.5/main.py
--rw-rw-rw-   0        0        0      166 2022-07-08 07:20:39.000000 pygbop-0.1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1108 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/pygbop/
--rw-rw-rw-   0        0        0     3814 2023-04-25 09:46:16.000000 pygbop-0.1.1.5/pygbop/gbop.py
--rw-rw-rw-   0        0        0      359 2022-07-08 10:32:24.000000 pygbop-0.1.1.5/pygbop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/pygbop.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1108 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/requires.txt
--rw-rw-rw-   0        0        0      277 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-02-15 06:20:25.000000 pygbop-0.1.1.5/README.rst
--rw-rw-rw-   0        0        0      801 2022-10-17 05:43:54.000000 pygbop-0.1.1.5/README.txt
--rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.1.1.5/requirements.txt
--rw-rw-rw-   0        0        0       64 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-04-25 09:43:09.000000 pygbop-0.1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/
+-rw-rw-rw-   0        0        0      207 2023-07-05 07:13:48.000000 pygbop-0.2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3122 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/pygbop/
+-rw-rw-rw-   0        0        0      467 2023-06-14 03:13:50.000000 pygbop-0.2.0.2/pygbop/common.py
+-rw-rw-rw-   0        0        0     2753 2023-07-05 07:08:15.000000 pygbop-0.2.0.2/pygbop/event_push.py
+-rw-rw-rw-   0        0        0     4199 2023-07-05 06:47:47.000000 pygbop-0.2.0.2/pygbop/gbop.py
+-rw-rw-rw-   0        0        0      601 2023-07-05 07:08:15.000000 pygbop-0.2.0.2/pygbop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/pygbop.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/pygbop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3122 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/pygbop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/pygbop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      278 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/pygbop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/pygbop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2164 2023-07-05 08:06:06.000000 pygbop-0.2.0.2/readme.md
+-rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.2.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       64 2023-07-05 08:06:40.000000 pygbop-0.2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2023-07-05 08:06:18.000000 pygbop-0.2.0.2/setup.py
```

### Comparing `pygbop-0.1.1.5/pygbop/gbop.py` & `pygbop-0.2.0.2/pygbop/gbop.py`

 * *Files 15% similar despite different names*

```diff
@@ -88,15 +88,27 @@
 
     def _get_url_str(self, path, params):
         query_str = self._get_query_str(params)
         format_string = f"{self.base_url}{path}?{query_str}" if query_str else f"{self.base_url}{path}"
         url = self.protocol + format_string
         return url
 
-    def execute(self, method=Method.GET, path='', params={}, data={}, is_beta_api=False, is_have_status=False):
+    def execute(self, method=Method.GET, path='', params={}, data={}, is_beta_api=False, is_has_status=False,
+                timeout=30):
+        """
+        接口调用
+        :param method: 调用方法
+        :param path: 调用路径
+        :param params: GET参数
+        :param data: POST参数
+        :param is_beta_api: 是否测试API
+        :param is_has_status: 是否返回http code
+        :param timeout: 超时时间
+        :return:
+        """
         url = self._get_url_str(path, params)
         headers = self._get_header(path, method.value, params, is_beta_api)
-        res = requests.request(method.value, url, headers=headers, data=data)
-        if is_have_status:
+        res = requests.request(method.value, url, headers=headers, data=data, timeout=timeout)
+        if is_has_status:
             return res.status_code, res.content
         else:
             return res.content
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygbop-0.1.1.5/setup.py` & `pygbop-0.2.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 from __future__ import print_function
 from setuptools import setup, find_packages
-# from setuptools import find_package_data
-import sys
 
 setup(
     name="pygbop",
-    version="0.1.1.5",
+    version="0.2.0.2",
     author="huang.xiaogang",
     author_email="huang.xiaogang@geely.com",
     description="Geely GBOP Client",
-    long_description=open("README.rst", encoding='utf-8').read(),
+    long_description=open("readme.md", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
     license="MIT",
     url="https://pypi.python.org/pypi/GbopApiClient",
     packages=find_packages(exclude=["*.*"]),
     include_package_data=True,
     py_modules=[],
     install_requires=[
         "requests",
```

