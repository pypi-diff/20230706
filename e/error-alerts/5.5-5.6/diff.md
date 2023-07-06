# Comparing `tmp/error-alerts-5.5.tar.gz` & `tmp/error-alerts-5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-5.5.tar", last modified: Tue Jul  4 14:42:01 2023, max compression
+gzip compressed data, was "error-alerts-5.6.tar", last modified: Thu Jul  6 12:01:26 2023, max compression
```

## Comparing `error-alerts-5.5.tar` & `error-alerts-5.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 14:42:01.515481 error-alerts-5.5/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.5/.gitignore
--rw-rw-rw-   0        0        0     1301 2023-07-04 14:42:01.515481 error-alerts-5.5/PKG-INFO
--rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 14:42:01.510484 error-alerts-5.5/error_alerts/
--rw-rw-rw-   0        0        0     4167 2023-07-04 14:41:51.000000 error-alerts-5.5/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:42:01.514481 error-alerts-5.5/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 14:42:01.516480 error-alerts-5.5/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-04 14:41:56.000000 error-alerts-5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:01:26.104025 error-alerts-5.6/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.6/.gitignore
+-rw-rw-rw-   0        0        0     1301 2023-07-06 12:01:26.105024 error-alerts-5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:01:26.092033 error-alerts-5.6/error_alerts/
+-rw-rw-rw-   0        0        0     4169 2023-07-06 12:01:05.000000 error-alerts-5.6/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:01:26.098029 error-alerts-5.6/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-07-06 12:01:25.000000 error-alerts-5.6/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-06 12:01:25.000000 error-alerts-5.6/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:01:25.000000 error-alerts-5.6/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-06 12:01:25.000000 error-alerts-5.6/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 12:01:25.000000 error-alerts-5.6/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-06 12:01:26.106023 error-alerts-5.6/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-06 12:01:12.000000 error-alerts-5.6/setup.py
```

### Comparing `error-alerts-5.5/PKG-INFO` & `error-alerts-5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.5
+Version: 5.6
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-5.5/README.md` & `error-alerts-5.6/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-5.5/error_alerts/__init__.py` & `error-alerts-5.6/error_alerts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 DEFAULT_IGNORED_ERRORS = [
     'The service is currently unavailable', # Google sheets API down
     'Could not authenticate you', # Twitter app suspended
     ]
 
 class alerts(Bot):
-    def __init__(self, token=None, channel=None, logger=None, full_error=True, raise_error=False, resend_repeat_errors=True):
+    def __init__(self, token=None, channel=None, logger=None, full_error=False, raise_error=False, resend_repeat_errors=False):
         if token and channel:
             bot = super()
             bot.__init__(token=token)
             self.telegram_bot = bot
 
             chat = self.get_chat(channel)
             # print(chat.title)
```

### Comparing `error-alerts-5.5/error_alerts.egg-info/PKG-INFO` & `error-alerts-5.6/error_alerts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.5
+Version: 5.6
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

