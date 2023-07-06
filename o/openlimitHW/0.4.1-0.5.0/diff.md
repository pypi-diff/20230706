# Comparing `tmp/openlimitHW-0.4.1.tar.gz` & `tmp/openlimitHW-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimitHW-0.4.1.tar", last modified: Thu Jul  6 03:21:03 2023, max compression
+gzip compressed data, was "openlimitHW-0.5.0.tar", last modified: Thu Jul  6 03:23:46 2023, max compression
```

## Comparing `openlimitHW-0.4.1.tar` & `openlimitHW-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 03:21:03.393036 openlimitHW-0.4.1/
--rw-rw-rw-   0        0        0    35823 2023-05-15 06:56:00.000000 openlimitHW-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1835 2023-07-06 03:21:03.392510 openlimitHW-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-07-06 02:39:10.000000 openlimitHW-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 03:21:03.356872 openlimitHW-0.4.1/openlimit/
--rw-rw-rw-   0        0        0      172 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:21:03.371210 openlimitHW-0.4.1/openlimit/buckets/
--rw-rw-rw-   0        0        0      113 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/buckets/__init__.py
--rw-rw-rw-   0        0        0     3590 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/buckets/bucket.py
--rw-rw-rw-   0        0        0     1929 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/buckets/redis_bucket.py
--rw-rw-rw-   0        0        0     3571 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/rate_limiters.py
--rw-rw-rw-   0        0        0     2622 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/redis_rate_limiters.py
--rw-rw-rw-   0        0        0        0 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/test.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:21:03.376259 openlimitHW-0.4.1/openlimit/utilities/
--rw-rw-rw-   0        0        0      267 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/utilities/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/utilities/context_decorators.py
--rw-rw-rw-   0        0        0     1247 2023-07-06 03:01:24.000000 openlimitHW-0.4.1/openlimit/utilities/token_counters.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:21:03.365276 openlimitHW-0.4.1/openlimitHW.egg-info/
--rw-rw-rw-   0        0        0     1835 2023-07-06 03:21:03.000000 openlimitHW-0.4.1/openlimitHW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2023-07-06 03:21:03.000000 openlimitHW-0.4.1/openlimitHW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 03:21:03.000000 openlimitHW-0.4.1/openlimitHW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-06 03:21:03.000000 openlimitHW-0.4.1/openlimitHW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 03:21:03.000000 openlimitHW-0.4.1/openlimitHW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      474 2023-07-06 03:20:33.000000 openlimitHW-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 03:21:03.393036 openlimitHW-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-07-06 03:20:52.000000 openlimitHW-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:23:46.964419 openlimitHW-0.5.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-15 06:56:00.000000 openlimitHW-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1835 2023-07-06 03:23:46.956416 openlimitHW-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-07-06 02:39:10.000000 openlimitHW-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 03:23:46.828904 openlimitHW-0.5.0/openlimit/
+-rw-rw-rw-   0        0        0      172 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:23:46.843904 openlimitHW-0.5.0/openlimit/buckets/
+-rw-rw-rw-   0        0        0      113 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/buckets/__init__.py
+-rw-rw-rw-   0        0        0     3590 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/buckets/bucket.py
+-rw-rw-rw-   0        0        0     1929 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/buckets/redis_bucket.py
+-rw-rw-rw-   0        0        0     3571 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/rate_limiters.py
+-rw-rw-rw-   0        0        0     2622 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/redis_rate_limiters.py
+-rw-rw-rw-   0        0        0        0 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/test.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:23:46.954416 openlimitHW-0.5.0/openlimit/utilities/
+-rw-rw-rw-   0        0        0      267 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/utilities/context_decorators.py
+-rw-rw-rw-   0        0        0     1247 2023-07-06 03:01:24.000000 openlimitHW-0.5.0/openlimit/utilities/token_counters.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:23:46.838903 openlimitHW-0.5.0/openlimitHW.egg-info/
+-rw-rw-rw-   0        0        0     1835 2023-07-06 03:23:46.000000 openlimitHW-0.5.0/openlimitHW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-07-06 03:23:46.000000 openlimitHW-0.5.0/openlimitHW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:23:46.000000 openlimitHW-0.5.0/openlimitHW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 03:23:46.000000 openlimitHW-0.5.0/openlimitHW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 03:23:46.000000 openlimitHW-0.5.0/openlimitHW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      474 2023-07-06 03:23:35.000000 openlimitHW-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:23:46.965419 openlimitHW-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-07-06 03:20:52.000000 openlimitHW-0.5.0/setup.py
```

### Comparing `openlimitHW-0.4.1/LICENSE` & `openlimitHW-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/PKG-INFO` & `openlimitHW-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlimitHW
-Version: 0.4.1
+Version: 0.5.0
 Summary: Rate limiter for the OpenAI API (modified by HW)
 Home-page: https://github.com/williamxhero/openlimitHW
 Author: williamxhero
 Author-email: williamxhero <williamxhero@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/williamxhero/openlimitHW
 Keywords: openai,rate-limit,limit,api,request,token,leaky-bucket,gcra,redis,asyncio
```

### Comparing `openlimitHW-0.4.1/README.md` & `openlimitHW-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/openlimit/buckets/bucket.py` & `openlimitHW-0.5.0/openlimit/buckets/bucket.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/openlimit/buckets/redis_bucket.py` & `openlimitHW-0.5.0/openlimit/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/openlimit/rate_limiters.py` & `openlimitHW-0.5.0/openlimit/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/openlimit/redis_rate_limiters.py` & `openlimitHW-0.5.0/openlimit/redis_rate_limiters.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/openlimit/utilities/context_decorators.py` & `openlimitHW-0.5.0/openlimit/utilities/context_decorators.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/openlimit/utilities/token_counters.py` & `openlimitHW-0.5.0/openlimit/utilities/token_counters.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/openlimitHW.egg-info/PKG-INFO` & `openlimitHW-0.5.0/openlimitHW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlimitHW
-Version: 0.4.1
+Version: 0.5.0
 Summary: Rate limiter for the OpenAI API (modified by HW)
 Home-page: https://github.com/williamxhero/openlimitHW
 Author: williamxhero
 Author-email: williamxhero <williamxhero@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/williamxhero/openlimitHW
 Keywords: openai,rate-limit,limit,api,request,token,leaky-bucket,gcra,redis,asyncio
```

### Comparing `openlimitHW-0.4.1/openlimitHW.egg-info/SOURCES.txt` & `openlimitHW-0.5.0/openlimitHW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.4.1/setup.py` & `openlimitHW-0.5.0/setup.py`

 * *Files identical despite different names*

