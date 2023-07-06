# Comparing `tmp/smsit-1.0.2.tar.gz` & `tmp/smsit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smsit-1.0.2.tar", last modified: Wed Jan 26 09:26:38 2022, max compression
+gzip compressed data, was "smsit-1.0.3.tar", last modified: Thu Jul  6 14:01:02 2023, max compression
```

## Comparing `smsit-1.0.2.tar` & `smsit-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxr-x   0 dobby     (1000) dobby     (1000)        0 2022-01-26 09:26:38.546715 smsit-1.0.2/
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     2606 2022-01-26 09:26:38.546715 smsit-1.0.2/PKG-INFO
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     1199 2020-10-24 17:06:30.000000 smsit-1.0.2/README.rst
--rw-rw-r--   0 dobby     (1000) dobby     (1000)       38 2022-01-26 09:26:38.546715 smsit-1.0.2/setup.cfg
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     1383 2022-01-25 16:34:02.000000 smsit-1.0.2/setup.py
-drwxrwxr-x   0 dobby     (1000) dobby     (1000)        0 2022-01-26 09:26:38.542716 smsit-1.0.2/smsit/
--rw-rw-r--   0 dobby     (1000) dobby     (1000)      223 2022-01-26 09:26:23.000000 smsit-1.0.2/smsit/__init__.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)       81 2022-01-25 12:25:41.000000 smsit-1.0.2/smsit/exceptions.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)      442 2022-01-25 15:30:38.000000 smsit-1.0.2/smsit/gateway.py
-drwxrwxr-x   0 dobby     (1000) dobby     (1000)        0 2022-01-26 09:26:38.546715 smsit-1.0.2/smsit/gateways/
--rw-rw-r--   0 dobby     (1000) dobby     (1000)      157 2022-01-25 16:38:26.000000 smsit-1.0.2/smsit/gateways/__init__.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)      283 2022-01-25 15:02:32.000000 smsit-1.0.2/smsit/gateways/dummy.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     2668 2022-01-26 09:25:56.000000 smsit-1.0.2/smsit/gateways/ghasedak.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     2239 2022-01-26 09:10:58.000000 smsit-1.0.2/smsit/gateways/niksms.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     1382 2022-01-26 09:07:07.000000 smsit-1.0.2/smsit/gateways/smsmagic.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)      744 2022-01-25 15:02:40.000000 smsit-1.0.2/smsit/manager.py
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     1241 2022-01-25 14:55:20.000000 smsit-1.0.2/smsit/message.py
-drwxrwxr-x   0 dobby     (1000) dobby     (1000)        0 2022-01-26 09:26:38.546715 smsit-1.0.2/smsit.egg-info/
--rw-rw-r--   0 dobby     (1000) dobby     (1000)     2606 2022-01-26 09:26:38.000000 smsit-1.0.2/smsit.egg-info/PKG-INFO
--rw-rw-r--   0 dobby     (1000) dobby     (1000)      382 2022-01-26 09:26:38.000000 smsit-1.0.2/smsit.egg-info/SOURCES.txt
--rw-rw-r--   0 dobby     (1000) dobby     (1000)        1 2022-01-26 09:26:38.000000 smsit-1.0.2/smsit.egg-info/dependency_links.txt
--rw-rw-r--   0 dobby     (1000) dobby     (1000)        9 2022-01-26 09:26:38.000000 smsit-1.0.2/smsit.egg-info/requires.txt
--rw-rw-r--   0 dobby     (1000) dobby     (1000)        6 2022-01-26 09:26:38.000000 smsit-1.0.2/smsit.egg-info/top_level.txt
+drwxr-xr-x   0 dobby     (1000) dobby     (1000)        0 2023-07-06 14:01:02.990184 smsit-1.0.3/
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     1062 2020-10-24 17:06:30.000000 smsit-1.0.3/LICENSE
+-rw-r--r--   0 dobby     (1000) dobby     (1000)     1996 2023-07-06 14:01:02.990184 smsit-1.0.3/PKG-INFO
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     1199 2020-10-24 17:06:30.000000 smsit-1.0.3/README.rst
+-rw-r--r--   0 dobby     (1000) dobby     (1000)       38 2023-07-06 14:01:02.990184 smsit-1.0.3/setup.cfg
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     1383 2022-01-25 16:34:02.000000 smsit-1.0.3/setup.py
+drwxr-xr-x   0 dobby     (1000) dobby     (1000)        0 2023-07-06 14:01:02.986184 smsit-1.0.3/smsit/
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)      223 2023-07-06 13:57:46.000000 smsit-1.0.3/smsit/__init__.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)       81 2022-01-25 12:25:41.000000 smsit-1.0.3/smsit/exceptions.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)      442 2022-01-25 15:30:38.000000 smsit-1.0.3/smsit/gateway.py
+drwxr-xr-x   0 dobby     (1000) dobby     (1000)        0 2023-07-06 14:01:02.986184 smsit-1.0.3/smsit/gateways/
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)      157 2022-01-25 16:38:26.000000 smsit-1.0.3/smsit/gateways/__init__.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)      283 2022-01-25 15:02:32.000000 smsit-1.0.3/smsit/gateways/dummy.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     2672 2023-07-06 13:56:58.000000 smsit-1.0.3/smsit/gateways/ghasedak.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     2239 2022-01-26 09:10:58.000000 smsit-1.0.3/smsit/gateways/niksms.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     1382 2022-01-26 09:07:07.000000 smsit-1.0.3/smsit/gateways/smsmagic.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)      744 2022-01-25 15:02:40.000000 smsit-1.0.3/smsit/manager.py
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     1241 2022-01-25 14:55:20.000000 smsit-1.0.3/smsit/message.py
+drwxr-xr-x   0 dobby     (1000) dobby     (1000)        0 2023-07-06 14:01:02.986184 smsit-1.0.3/smsit.egg-info/
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)     1996 2023-07-06 14:01:02.000000 smsit-1.0.3/smsit.egg-info/PKG-INFO
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)      412 2023-07-06 14:01:02.000000 smsit-1.0.3/smsit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)        1 2023-07-06 14:01:02.000000 smsit-1.0.3/smsit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)        9 2023-07-06 14:01:02.000000 smsit-1.0.3/smsit.egg-info/requires.txt
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)        6 2023-07-06 14:01:02.000000 smsit-1.0.3/smsit.egg-info/top_level.txt
+drwxr-xr-x   0 dobby     (1000) dobby     (1000)        0 2023-07-06 14:01:02.986184 smsit-1.0.3/tests/
+-rw-rw-r--   0 dobby     (1000) dobby     (1000)      501 2022-01-25 12:30:31.000000 smsit-1.0.3/tests/test_manager.py
```

### Comparing `smsit-1.0.2/README.rst` & `smsit-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `smsit-1.0.2/setup.py` & `smsit-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `smsit-1.0.2/smsit/gateways/ghasedak.py` & `smsit-1.0.3/smsit/gateways/ghasedak.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         if message.type == "sms":
             params["message"] = message.text
             sender = message.sender or self.config.get("sender")
             if sender:
                 params["linenumber"] = sender
 
-            return [self._call("/send/pair", headers, params)]
+            return [self._call("/sms/send/pair", headers, params)]
 
         if message.type == "templatedMessage":
             params["template"] = message.template
             for k, v in enumerate(message.params):
                 params["param%s" % (k + 1)] = v
 
             return [self._call("/verification/send/simple", headers, params)]
```

### Comparing `smsit-1.0.2/smsit/gateways/niksms.py` & `smsit-1.0.3/smsit/gateways/niksms.py`

 * *Files identical despite different names*

### Comparing `smsit-1.0.2/smsit/gateways/smsmagic.py` & `smsit-1.0.3/smsit/gateways/smsmagic.py`

 * *Files identical despite different names*

### Comparing `smsit-1.0.2/smsit/manager.py` & `smsit-1.0.3/smsit/manager.py`

 * *Files identical despite different names*

### Comparing `smsit-1.0.2/smsit/message.py` & `smsit-1.0.3/smsit/message.py`

 * *Files identical despite different names*

