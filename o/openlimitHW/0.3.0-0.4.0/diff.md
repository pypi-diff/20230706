# Comparing `tmp/openlimitHW-0.3.0.tar.gz` & `tmp/openlimitHW-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimitHW-0.3.0.tar", last modified: Mon May 15 08:00:38 2023, max compression
+gzip compressed data, was "openlimitHW-0.4.0.tar", last modified: Thu Jul  6 02:42:58 2023, max compression
```

## Comparing `openlimitHW-0.3.0.tar` & `openlimitHW-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 08:00:38.218881 openlimitHW-0.3.0/
--rw-rw-rw-   0        0        0    35823 2023-05-15 06:56:00.000000 openlimitHW-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     3711 2023-05-15 08:00:38.217881 openlimitHW-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3057 2023-05-15 07:51:47.000000 openlimitHW-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 08:00:37.909624 openlimitHW-0.3.0/openlimit/
--rw-rw-rw-   0        0        0      227 2023-05-15 07:37:11.000000 openlimitHW-0.3.0/openlimit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:00:37.921629 openlimitHW-0.3.0/openlimit/buckets/
--rw-rw-rw-   0        0        0       99 2023-05-15 06:56:00.000000 openlimitHW-0.3.0/openlimit/buckets/__init__.py
--rw-rw-rw-   0        0        0      812 2023-05-15 07:24:56.000000 openlimitHW-0.3.0/openlimit/buckets/bucket.py
--rw-rw-rw-   0        0        0     1929 2023-05-15 07:37:06.000000 openlimitHW-0.3.0/openlimit/buckets/redis_bucket.py
--rw-rw-rw-   0        0        0     2211 2023-05-15 07:24:45.000000 openlimitHW-0.3.0/openlimit/rate_limiters.py
--rw-rw-rw-   0        0        0     3030 2023-05-15 07:37:18.000000 openlimitHW-0.3.0/openlimit/redis_rate_limiters.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:00:37.926163 openlimitHW-0.3.0/openlimit/utilities/
--rw-rw-rw-   0        0        0      253 2023-05-15 06:56:00.000000 openlimitHW-0.3.0/openlimit/utilities/__init__.py
--rw-rw-rw-   0        0        0     1575 2023-05-15 06:59:51.000000 openlimitHW-0.3.0/openlimit/utilities/context_decorators.py
--rw-rw-rw-   0        0        0     1689 2023-05-15 07:37:26.000000 openlimitHW-0.3.0/openlimit/utilities/token_counters.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:00:37.916658 openlimitHW-0.3.0/openlimitHW.egg-info/
--rw-rw-rw-   0        0        0     3711 2023-05-15 08:00:37.000000 openlimitHW-0.3.0/openlimitHW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-05-15 08:00:37.000000 openlimitHW-0.3.0/openlimitHW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 08:00:37.000000 openlimitHW-0.3.0/openlimitHW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-15 08:00:37.000000 openlimitHW-0.3.0/openlimitHW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 08:00:37.000000 openlimitHW-0.3.0/openlimitHW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      474 2023-05-15 08:00:06.000000 openlimitHW-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 08:00:38.218881 openlimitHW-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-05-15 07:58:22.000000 openlimitHW-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:42:58.048082 openlimitHW-0.4.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-15 06:56:00.000000 openlimitHW-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1835 2023-07-06 02:42:58.047082 openlimitHW-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-07-06 02:39:10.000000 openlimitHW-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 02:42:58.007407 openlimitHW-0.4.0/openlimit/
+-rw-rw-rw-   0        0        0      227 2023-05-15 07:37:11.000000 openlimitHW-0.4.0/openlimit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:42:58.039082 openlimitHW-0.4.0/openlimit/buckets/
+-rw-rw-rw-   0        0        0       99 2023-05-15 06:56:00.000000 openlimitHW-0.4.0/openlimit/buckets/__init__.py
+-rw-rw-rw-   0        0        0      898 2023-05-16 03:42:58.000000 openlimitHW-0.4.0/openlimit/buckets/bucket.py
+-rw-rw-rw-   0        0        0     1929 2023-05-15 07:37:06.000000 openlimitHW-0.4.0/openlimit/buckets/redis_bucket.py
+-rw-rw-rw-   0        0        0     2256 2023-05-16 03:41:34.000000 openlimitHW-0.4.0/openlimit/rate_limiters.py
+-rw-rw-rw-   0        0        0     3030 2023-05-15 07:37:18.000000 openlimitHW-0.4.0/openlimit/redis_rate_limiters.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:42:58.044081 openlimitHW-0.4.0/openlimit/utilities/
+-rw-rw-rw-   0        0        0      253 2023-05-15 06:56:00.000000 openlimitHW-0.4.0/openlimit/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1575 2023-05-15 06:59:51.000000 openlimitHW-0.4.0/openlimit/utilities/context_decorators.py
+-rw-rw-rw-   0        0        0     1689 2023-05-15 07:37:26.000000 openlimitHW-0.4.0/openlimit/utilities/token_counters.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:42:58.033084 openlimitHW-0.4.0/openlimitHW.egg-info/
+-rw-rw-rw-   0        0        0     1835 2023-07-06 02:42:57.000000 openlimitHW-0.4.0/openlimitHW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-07-06 02:42:57.000000 openlimitHW-0.4.0/openlimitHW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 02:42:57.000000 openlimitHW-0.4.0/openlimitHW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 02:42:57.000000 openlimitHW-0.4.0/openlimitHW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 02:42:57.000000 openlimitHW-0.4.0/openlimitHW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      474 2023-07-06 02:41:08.000000 openlimitHW-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 02:42:58.048082 openlimitHW-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-05-15 08:19:05.000000 openlimitHW-0.4.0/setup.py
```

### Comparing `openlimitHW-0.3.0/LICENSE` & `openlimitHW-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.3.0/openlimit/buckets/bucket.py` & `openlimitHW-0.4.0/openlimit/buckets/bucket.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,10 +23,13 @@
         if time_passed > (self._sec_per_tick * self._last_amount):
             self._last_checked = current_time
             self._last_amount = amount
             return True
         
         return False
     
+    def update_last_amount(self, amount):
+        self._last_amount = amount
+        
     async def wait_for_capacity(self, amount):
         while not self._has_capacity(amount):
             await asyncio.sleep(1 / self._sec_per_tick)
```

### Comparing `openlimitHW-0.3.0/openlimit/buckets/redis_bucket.py` & `openlimitHW-0.4.0/openlimit/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.3.0/openlimit/rate_limiters.py` & `openlimitHW-0.4.0/openlimit/rate_limiters.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     def limit(self, **kwargs):
         num_tokens = self.token_counter(**kwargs)
         return utils.ContextManager(num_tokens, self)
     
     def is_limited(self):
         return utils.FunctionDecorator(self)
 
+    def update(self, response):
+        pass
 
 ######
 # MAIN
 ######
 
 
 class ChatRateLimiter(RateLimiter):
```

### Comparing `openlimitHW-0.3.0/openlimit/redis_rate_limiters.py` & `openlimitHW-0.4.0/openlimit/redis_rate_limiters.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.3.0/openlimit/utilities/context_decorators.py` & `openlimitHW-0.4.0/openlimit/utilities/context_decorators.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.3.0/openlimit/utilities/token_counters.py` & `openlimitHW-0.4.0/openlimit/utilities/token_counters.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.3.0/setup.py` & `openlimitHW-0.4.0/setup.py`

 * *Files identical despite different names*

