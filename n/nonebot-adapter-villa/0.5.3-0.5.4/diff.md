# Comparing `tmp/nonebot_adapter_villa-0.5.3.tar.gz` & `tmp/nonebot_adapter_villa-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.5.3.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.5.4.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.5.3.tar` & `nonebot_adapter_villa-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/LICENSE
--rw-r--r--   0        0        0     6796 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/README.md
--rw-r--r--   0        0        0      235 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    10977 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9536 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    13338 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      649 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11646 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0    10115 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-07-05 01:31:33.663990 nonebot_adapter_villa-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/LICENSE
+-rw-r--r--   0        0        0     6796 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/README.md
+-rw-r--r--   0        0        0      235 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    10977 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9536 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    13338 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      649 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11651 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0    10115 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1435 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-07-06 07:29:51.685559 nonebot_adapter_villa-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.4/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.5.3/LICENSE` & `nonebot_adapter_villa-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/README.md` & `nonebot_adapter_villa-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
     if (event_type := EventType._value2member_map_.get(payload["type"])) is None:
         raise ValueError(
             f"Unknown event type: {payload['type']} data={escape_tag(str(payload))}"
         )
     event_name = event_type.name
     if event_name not in payload["extend_data"]["EventData"]:
         raise ValueError("Cannot find event data for event type: {event_name}")
-    payload |= payload["extend_data"]["EventData"][event_name]
+    payload.update(payload["extend_data"]["EventData"][event_name])
     payload.pop("extend_data")
     return payload
 
 
 __all__ = [
     "Event",
     "NoticeEvent",
```

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.3/pyproject.toml` & `nonebot_adapter_villa-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.5.3"
+version = "0.5.4"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.5.3/PKG-INFO` & `nonebot_adapter_villa-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.5.3
+Version: 0.5.4
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.4 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

