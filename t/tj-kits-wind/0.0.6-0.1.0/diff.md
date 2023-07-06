# Comparing `tmp/tj_kits_wind-0.0.6.tar.gz` & `tmp/tj_kits_wind-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tj_kits_wind-0.0.6.tar", last modified: Wed May  3 13:23:31 2023, max compression
+gzip compressed data, was "tj_kits_wind-0.1.0.tar", last modified: Thu Jul  6 04:17:24 2023, max compression
```

## Comparing `tj_kits_wind-0.0.6.tar` & `tj_kits_wind-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.615703 tj_kits_wind-0.0.6/
--rw-rw-rw-   0        0        0      261 2023-05-03 13:23:31.615703 tj_kits_wind-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-05-01 09:45:03.000000 tj_kits_wind-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 13:23:31.615703 tj_kits_wind-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      545 2023-05-03 13:23:15.000000 tj_kits_wind-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.612713 tj_kits_wind-0.0.6/tj_kits_wind/
--rw-rw-rw-   0        0        0        0 2023-05-01 09:05:59.000000 tj_kits_wind-0.0.6/tj_kits_wind/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.614706 tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/
--rw-rw-rw-   0        0        0     4048 2023-05-03 13:23:02.000000 tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/LoggerFactory.py
--rw-rw-rw-   0        0        0        0 2023-05-01 07:40:58.000000 tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.614706 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/
--rw-rw-rw-   0        0        0      261 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 04:17:24.813717 tj_kits_wind-0.1.0/
+-rw-rw-rw-   0        0        0      482 2023-07-06 04:17:24.803502 tj_kits_wind-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1412 2023-06-08 07:51:20.000000 tj_kits_wind-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 04:17:24.813717 tj_kits_wind-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      940 2023-07-06 04:17:03.000000 tj_kits_wind-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:17:24.797502 tj_kits_wind-0.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 07:51:20.000000 tj_kits_wind-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1031 2023-07-06 04:02:23.000000 tj_kits_wind-0.1.0/tests/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:17:24.797502 tj_kits_wind-0.1.0/tj_kits_wind/
+-rw-rw-rw-   0        0        0      442 2023-07-06 03:56:09.000000 tj_kits_wind-0.1.0/tj_kits_wind/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:17:24.800502 tj_kits_wind-0.1.0/tj_kits_wind/tj_logger/
+-rw-rw-rw-   0        0        0     4583 2023-07-06 03:56:44.000000 tj_kits_wind-0.1.0/tj_kits_wind/tj_logger/LoggerFactory.py
+-rw-rw-rw-   0        0        0      474 2023-07-06 03:56:34.000000 tj_kits_wind-0.1.0/tj_kits_wind/tj_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:17:24.801502 tj_kits_wind-0.1.0/tj_kits_wind/tj_path/
+-rw-rw-rw-   0        0        0      461 2023-07-03 18:24:55.000000 tj_kits_wind-0.1.0/tj_kits_wind/tj_path/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-07-03 18:24:55.000000 tj_kits_wind-0.1.0/tj_kits_wind/tj_path/project_root.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:17:24.802502 tj_kits_wind-0.1.0/tj_kits_wind/tj_time/
+-rw-rw-rw-   0        0        0      462 2023-07-03 18:24:55.000000 tj_kits_wind-0.1.0/tj_kits_wind/tj_time/__init__.py
+-rw-rw-rw-   0        0        0     9597 2023-07-03 18:24:55.000000 tj_kits_wind-0.1.0/tj_kits_wind/tj_time/tj_time_tools.py
+-rw-rw-rw-   0        0        0      164 2023-07-03 18:24:55.000000 tj_kits_wind-0.1.0/tj_kits_wind/tj_time/tt.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:17:24.799502 tj_kits_wind-0.1.0/tj_kits_wind.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-07-06 04:17:24.000000 tj_kits_wind-0.1.0/tj_kits_wind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-06 04:17:24.000000 tj_kits_wind-0.1.0/tj_kits_wind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 04:17:24.000000 tj_kits_wind-0.1.0/tj_kits_wind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-06 04:17:24.000000 tj_kits_wind-0.1.0/tj_kits_wind.egg-info/top_level.txt
```

### Comparing `tj_kits_wind-0.0.6/README.md` & `tj_kits_wind-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/LoggerFactory.py` & `tj_kits_wind-0.1.0/tj_kits_wind/tj_logger/LoggerFactory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,135 @@
-import logging
-import logging.config
-import os
-import sys
-from typing import AnyStr, Dict, Optional, Literal, Union
-
-__all__ = ["logger_console", "logger_auto"]
-
-LOGGER_FORMAT = Literal["very_short", "short", "normal", "wordy"]
-LOGGER_LEVEL = Literal['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']
-
-
-def get_logger_conf_dict() -> Dict:
-    LOGGER_CONF = {
-        'version': 1,
-        'disable_existing_loggers': False,
-        'formatters': {
-            "main": {
-                "datefmt": '%m-%d %H:%M:%S',
-                # "format": "[%(asctime)s | %(levelname)s | pid:%(process)d | %(filename)s:%(lineno)d] %(message)s"
-
-            },
-        },
-
-        #
-        "handlers": {
-            'tj_c': {
-                'level': 'DEBUG',
-                'class': 'logging.StreamHandler',
-                'stream': sys.stdout,
-                'formatter': 'main'
-            },
-        },
-
-        #
-        "loggers": {
-            # 配置文件 中 只要定义了 root logger 就一定会 先传递至 root
-            #  其他 logger 均相当其 子类, 无论配置是否扩散
-            # "root": {
-            #     'handlers': ["tj_c"],
-            #     'level': "DEBUG",
-            #     "propagate": 1,
-            # },
-            "tj_c": {
-                'handlers': ["tj_c"],
-                'level': "DEBUG",
-            },
-        }
-    }
-
-    return LOGGER_CONF
-
-
-def logger_console(logger_format: LOGGER_FORMAT = "short"):
-    return create_logger("tj_c", logger_format=logger_format)
-
-
-def logger_auto(name: AnyStr, log_path: AnyStr, logger_format: LOGGER_FORMAT = "normal",
-                max_mb: int = 100, back_up_count: int = 10):
-    add_handler = {
-        'encoding': 'utf8',
-        'level': 'DEBUG',
-        'class': 'logging.handlers.RotatingFileHandler',
-        'maxBytes': 1024 * 1024 * max_mb,  # 100MB
-        'backupCount': back_up_count,  # 100MB * 10 = 1G
-        'formatter': 'main',
-        'filename': ""
-    }
-
-    add_logger = {
-        'handlers': [name],
-        'level': "DEBUG",
-    }
-
-    return create_logger(name, file_name="{}.log".format(name), log_path=log_path, add_handler=add_handler,
-                         add_logger=add_logger, logger_format=logger_format)
-
-
-def create_logger(name: AnyStr,
-                  file_name: AnyStr = "tj.log",
-                  log_path: AnyStr = "/tmp/tj_log",
-                  add_handler: Optional[Dict] = None,
-                  add_logger: Optional[Dict] = None,
-                  logger_format: LOGGER_FORMAT = "normal",
-                  level: LOGGER_LEVEL = "INFO"):
-    LOGGER_CONF = get_logger_conf_dict()
-
-    # 1. add handler and logger
-    if add_handler:
-        LOGGER_CONF["handlers"][name] = add_handler
-    if add_logger:
-        LOGGER_CONF["loggers"][name] = add_logger
-
-    # 2. set format and level
-    if logger_format == "very_short":
-        LOGGER_CONF["formatters"]["main"]["format"] = "[%(levelname)s] %(message)s"
-    if logger_format == "short":
-        LOGGER_CONF["formatters"]["main"]["format"] = "[%(asctime)s | %(levelname)s] %(message)s"
-    if logger_format == "normal":
-        LOGGER_CONF["formatters"]["main"]["format"] = \
-            "[%(asctime)s | %(levelname)s | pid:%(process)d | %(filename)s:%(lineno)d] %(message)s"
-    if logger_format == "wordy":
-        LOGGER_CONF["formatters"]["main"]["format"] = \
-            "[%(asctime)s | %(levelname)s | pid:%(process)d | tid:%(thread)d | %(module)s | %(funcName)s | %(filename)s:%(lineno)d] %(message)s"
-
-    # 设置 level & mkdir file_path
-    LOGGER_CONF["handlers"][name]["level"] = level
-    if "filename" in LOGGER_CONF["handlers"][name].keys():
-        if not os.path.isdir(log_path):
-            os.makedirs(log_path)
-
-        LOGGER_CONF["handlers"][name]["filename"] = "{}/{}".format(log_path, file_name)
-
-    # 确定 logger name
-    logger_name = LOGGER_CONF["loggers"].keys()
-    if not name:
-        name = "tj_c"
-
-    # 返回 logger
-    logging.config.dictConfig(LOGGER_CONF)
-    logger = logging.getLogger(name)
-
-    return logger
+import logging
+import logging.config
+import os
+import sys
+from typing import AnyStr, Dict, Optional, Literal, Union
+
+__all__ = ['FORMAT_VERY_SHORT', 'FORMAT_SHORT', 'FORMAT_NORMAL', 'FORMAT_WORDY',
+           'LOG_DEBUG', 'LOG_INFO', 'LOG_WARNING', 'LOG_ERROR', 'LOG_CRITICAL',
+           'logger_console', 'logger_auto']
+
+FORMAT_VERY_SHORT = "very_short"
+FORMAT_SHORT = "short"
+FORMAT_NORMAL = "normal"
+FORMAT_WORDY = "wordy"
+LOGGER_FORMAT = Union[FORMAT_VERY_SHORT, FORMAT_SHORT, FORMAT_NORMAL, FORMAT_WORDY]
+
+LOG_DEBUG = "DEBUG"
+LOG_INFO = "INFO"
+LOG_WARNING = "WARNING"
+LOG_ERROR = "ERROR"
+LOG_CRITICAL = "CRITICAL"
+LOGGER_LEVEL = Union[LOG_DEBUG, LOG_INFO, LOG_WARNING, LOG_ERROR, LOG_CRITICAL]
+
+
+def get_logger_conf_dict() -> Dict:
+    LOGGER_CONF = {
+        'version': 1,
+        'disable_existing_loggers': False,
+        'formatters': {
+            "main": {
+                "datefmt": '%m-%d %H:%M:%S',
+                # "format": "[%(asctime)s | %(levelname)s | pid:%(process)d | %(filename)s:%(lineno)d] %(message)s"
+
+            },
+        },
+
+        #
+        "handlers": {
+            'tj_c': {
+                'level': 'DEBUG',
+                'class': 'logging.StreamHandler',
+                'stream': sys.stdout,
+                'formatter': 'main'
+            },
+        },
+
+        #
+        "loggers": {
+            # 配置文件 中 只要定义了 root logger 就一定会 先传递至 root
+            #  其他 logger 均相当其 子类, 无论配置是否扩散
+            # "root": {
+            #     'handlers': ["tj_c"],
+            #     'level': "DEBUG",
+            #     "propagate": 1,
+            # },
+            "tj_c": {
+                'handlers': ["tj_c"],
+                'level': "DEBUG",
+            },
+        }
+    }
+
+    return LOGGER_CONF
+
+
+def logger_console(logger_format: LOGGER_FORMAT = "short"):
+    return create_logger("tj_c", logger_format=logger_format)
+
+
+def logger_auto(name: AnyStr, log_path: AnyStr, logger_format: LOGGER_FORMAT = "normal",
+                max_mb: int = 100, back_up_count: int = 10):
+    add_handler = {
+        'encoding': 'utf8',
+        'level': 'DEBUG',
+        'class': 'logging.handlers.RotatingFileHandler',
+        'maxBytes': 1024 * 1024 * max_mb,  # 100MB
+        'backupCount': back_up_count,  # 100MB * 10 = 1G
+        'formatter': 'main',
+        'filename': ""
+    }
+
+    add_logger = {
+        'handlers': [name],
+        'level': "DEBUG",
+    }
+
+    return create_logger(name, file_name="{}.log".format(name), log_path=log_path, add_handler=add_handler,
+                         add_logger=add_logger, logger_format=logger_format)
+
+
+def create_logger(name: AnyStr,
+                  file_name: AnyStr = "tj.log",
+                  log_path: AnyStr = "/tmp/tj_log",
+                  add_handler: Optional[Dict] = None,
+                  add_logger: Optional[Dict] = None,
+                  logger_format: LOGGER_FORMAT = "normal",
+                  level: LOGGER_LEVEL = "INFO"):
+    LOGGER_CONF = get_logger_conf_dict()
+
+    # 1. add handler and logger
+    if add_handler:
+        LOGGER_CONF["handlers"][name] = add_handler
+    if add_logger:
+        LOGGER_CONF["loggers"][name] = add_logger
+
+    # 2. set format and level
+    if logger_format == "very_short":
+        LOGGER_CONF["formatters"]["main"]["format"] = "[%(levelname)s] %(message)s"
+    if logger_format == "short":
+        LOGGER_CONF["formatters"]["main"]["format"] = "[%(asctime)s | %(levelname)s] %(message)s"
+    if logger_format == "normal":
+        LOGGER_CONF["formatters"]["main"]["format"] = \
+            "[%(asctime)s | %(levelname)s | pid:%(process)d | %(filename)s:%(lineno)d] %(message)s"
+    if logger_format == "wordy":
+        LOGGER_CONF["formatters"]["main"]["format"] = \
+            "[%(asctime)s | %(levelname)s | pid:%(process)d | tid:%(thread)d | %(module)s | %(funcName)s | %(filename)s:%(lineno)d] %(message)s"
+
+    # 设置 level & mkdir file_path
+    LOGGER_CONF["handlers"][name]["level"] = level
+    if "filename" in LOGGER_CONF["handlers"][name].keys():
+        if not os.path.isdir(log_path):
+            os.makedirs(log_path)
+
+        LOGGER_CONF["handlers"][name]["filename"] = "{}/{}".format(log_path, file_name)
+
+    # 确定 logger name
+    logger_name = LOGGER_CONF["loggers"].keys()
+    if not name:
+        name = "tj_c"
+
+    # 返回 logger
+    logging.config.dictConfig(LOGGER_CONF)
+    logger = logging.getLogger(name)
+
+    return logger
```

