# Comparing `tmp/datatypes-0.9.4.tar.gz` & `tmp/datatypes-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatypes-0.9.4.tar", last modified: Thu Jun 15 04:30:59 2023, max compression
+gzip compressed data, was "datatypes-0.9.5.tar", last modified: Wed Jul  5 00:00:59 2023, max compression
```

## Comparing `datatypes-0.9.4.tar` & `datatypes-0.9.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.400069 datatypes-0.9.4/
--rw-r--r--   0 jaymon     (501) staff       (20)     1083 2020-07-08 22:29:16.000000 datatypes-0.9.4/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-06-15 04:30:59.399937 datatypes-0.9.4/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      408 2020-07-08 22:45:30.000000 datatypes-0.9.4/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.398208 datatypes-0.9.4/datatypes/
--rw-r--r--   0 jaymon     (501) staff       (20)     2287 2023-06-15 04:29:18.000000 datatypes-0.9.4/datatypes/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    33663 2023-02-18 01:09:36.000000 datatypes-0.9.4/datatypes/collections.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5556 2023-02-18 01:09:45.000000 datatypes-0.9.4/datatypes/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7749 2023-02-16 23:56:47.000000 datatypes-0.9.4/datatypes/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4902 2023-01-15 22:38:58.000000 datatypes-0.9.4/datatypes/copy.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11028 2021-09-01 07:52:59.000000 datatypes-0.9.4/datatypes/csv.py
--rw-r--r--   0 jaymon     (501) staff       (20)    22349 2023-03-04 08:31:34.000000 datatypes-0.9.4/datatypes/datetime.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.399647 datatypes-0.9.4/datatypes/decorators/
--rw-r--r--   0 jaymon     (501) staff       (20)      389 2023-01-20 01:17:21.000000 datatypes-0.9.4/datatypes/decorators/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    14105 2023-02-01 23:11:59.000000 datatypes-0.9.4/datatypes/decorators/base.py
--rw-r--r--   0 jaymon     (501) staff       (20)    13007 2023-01-30 19:17:34.000000 datatypes-0.9.4/datatypes/decorators/descriptor.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3551 2023-02-01 23:14:06.000000 datatypes-0.9.4/datatypes/decorators/misc.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11912 2022-12-23 00:30:10.000000 datatypes-0.9.4/datatypes/email.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5747 2020-08-06 08:36:37.000000 datatypes-0.9.4/datatypes/enum.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7575 2023-02-16 08:34:44.000000 datatypes-0.9.4/datatypes/environ.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7339 2023-01-26 00:06:46.000000 datatypes-0.9.4/datatypes/event.py
--rw-r--r--   0 jaymon     (501) staff       (20)    15804 2023-01-21 21:27:07.000000 datatypes-0.9.4/datatypes/html.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23175 2023-02-27 22:34:26.000000 datatypes-0.9.4/datatypes/http.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11306 2023-06-15 04:11:55.000000 datatypes-0.9.4/datatypes/logging.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5758 2023-06-13 23:17:08.000000 datatypes-0.9.4/datatypes/number.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3739 2023-02-27 22:36:06.000000 datatypes-0.9.4/datatypes/parse.py
--rw-r--r--   0 jaymon     (501) staff       (20)   124391 2023-06-13 20:01:59.000000 datatypes-0.9.4/datatypes/path.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6236 2023-03-18 21:36:58.000000 datatypes-0.9.4/datatypes/profile.py
--rw-r--r--   0 jaymon     (501) staff       (20)    35861 2023-03-15 19:55:58.000000 datatypes-0.9.4/datatypes/reflection.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11167 2023-02-18 01:09:49.000000 datatypes-0.9.4/datatypes/server.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6612 2023-02-16 00:02:52.000000 datatypes-0.9.4/datatypes/service.py
--rw-r--r--   0 jaymon     (501) staff       (20)    42752 2023-02-21 19:23:11.000000 datatypes-0.9.4/datatypes/string.py
--rw-r--r--   0 jaymon     (501) staff       (20)    12955 2023-01-06 07:52:19.000000 datatypes-0.9.4/datatypes/token.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23472 2023-01-24 22:20:57.000000 datatypes-0.9.4/datatypes/url.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2828 2023-02-18 01:11:42.000000 datatypes-0.9.4/datatypes/utils.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.398772 datatypes-0.9.4/datatypes.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      784 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-15 04:30:59.400108 datatypes-0.9.4/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1950 2020-07-08 22:29:00.000000 datatypes-0.9.4/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.261099 datatypes-0.9.5/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1083 2020-07-08 22:29:16.000000 datatypes-0.9.5/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-07-05 00:00:59.260957 datatypes-0.9.5/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      408 2020-07-08 22:45:30.000000 datatypes-0.9.5/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.259472 datatypes-0.9.5/datatypes/
+-rw-r--r--   0 jaymon     (501) staff       (20)     2287 2023-07-04 23:59:31.000000 datatypes-0.9.5/datatypes/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    33663 2023-02-18 01:09:36.000000 datatypes-0.9.5/datatypes/collections.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5556 2023-02-18 01:09:45.000000 datatypes-0.9.5/datatypes/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7749 2023-02-16 23:56:47.000000 datatypes-0.9.5/datatypes/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4902 2023-01-15 22:38:58.000000 datatypes-0.9.5/datatypes/copy.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11028 2021-09-01 07:52:59.000000 datatypes-0.9.5/datatypes/csv.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    22349 2023-03-04 08:31:34.000000 datatypes-0.9.5/datatypes/datetime.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.260752 datatypes-0.9.5/datatypes/decorators/
+-rw-r--r--   0 jaymon     (501) staff       (20)      389 2023-01-20 01:17:21.000000 datatypes-0.9.5/datatypes/decorators/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    14105 2023-02-01 23:11:59.000000 datatypes-0.9.5/datatypes/decorators/base.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    13007 2023-01-30 19:17:34.000000 datatypes-0.9.5/datatypes/decorators/descriptor.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3551 2023-02-01 23:14:06.000000 datatypes-0.9.5/datatypes/decorators/misc.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11912 2022-12-23 00:30:10.000000 datatypes-0.9.5/datatypes/email.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5747 2020-08-06 08:36:37.000000 datatypes-0.9.5/datatypes/enum.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7575 2023-02-16 08:34:44.000000 datatypes-0.9.5/datatypes/environ.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7339 2023-01-26 00:06:46.000000 datatypes-0.9.5/datatypes/event.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    15804 2023-01-21 21:27:07.000000 datatypes-0.9.5/datatypes/html.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    23175 2023-02-27 22:34:26.000000 datatypes-0.9.5/datatypes/http.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    12930 2023-07-04 00:02:42.000000 datatypes-0.9.5/datatypes/logging.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5758 2023-06-13 23:17:08.000000 datatypes-0.9.5/datatypes/number.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3739 2023-02-27 22:36:06.000000 datatypes-0.9.5/datatypes/parse.py
+-rw-r--r--   0 jaymon     (501) staff       (20)   124655 2023-06-29 22:48:32.000000 datatypes-0.9.5/datatypes/path.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6236 2023-03-18 21:36:58.000000 datatypes-0.9.5/datatypes/profile.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    36242 2023-07-04 22:29:52.000000 datatypes-0.9.5/datatypes/reflection.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11373 2023-06-24 18:12:15.000000 datatypes-0.9.5/datatypes/server.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6612 2023-02-16 00:02:52.000000 datatypes-0.9.5/datatypes/service.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    42752 2023-02-21 19:23:11.000000 datatypes-0.9.5/datatypes/string.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    12955 2023-01-06 07:52:19.000000 datatypes-0.9.5/datatypes/token.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    23472 2023-01-24 22:20:57.000000 datatypes-0.9.5/datatypes/url.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2828 2023-02-18 01:11:42.000000 datatypes-0.9.5/datatypes/utils.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-05 00:00:59.260189 datatypes-0.9.5/datatypes.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      784 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-07-05 00:00:59.000000 datatypes-0.9.5/datatypes.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-07-05 00:00:59.261141 datatypes-0.9.5/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1950 2020-07-08 22:29:00.000000 datatypes-0.9.5/setup.py
```

### Comparing `datatypes-0.9.4/LICENSE.txt` & `datatypes-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/PKG-INFO` & `datatypes-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatypes
-Version: 0.9.4
+Version: 0.9.5
 Summary: Utility Classes and Functions that are handy across multiple projects
 Home-page: http://github.com/Jaymon/datatypes
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `datatypes-0.9.4/datatypes/__init__.py` & `datatypes-0.9.5/datatypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,14 @@
 from .server import (
     PathServer,
     CallbackServer,
     WSGIServer,
 )
 
 
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 
 # get rid of "No handler found" warnings (cribbed from requests)
 # DEPRECATED 7-15-2022, doesn't seem to be needed in python3
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `datatypes-0.9.4/datatypes/collections.py` & `datatypes-0.9.5/datatypes/collections.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/compat.py` & `datatypes-0.9.5/datatypes/compat.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/config.py` & `datatypes-0.9.5/datatypes/config.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/copy.py` & `datatypes-0.9.5/datatypes/copy.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/csv.py` & `datatypes-0.9.5/datatypes/csv.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/datetime.py` & `datatypes-0.9.5/datatypes/datetime.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/decorators/base.py` & `datatypes-0.9.5/datatypes/decorators/base.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/decorators/descriptor.py` & `datatypes-0.9.5/datatypes/decorators/descriptor.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/decorators/misc.py` & `datatypes-0.9.5/datatypes/decorators/misc.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/email.py` & `datatypes-0.9.5/datatypes/email.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/enum.py` & `datatypes-0.9.5/datatypes/enum.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/environ.py` & `datatypes-0.9.5/datatypes/environ.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/event.py` & `datatypes-0.9.5/datatypes/event.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/html.py` & `datatypes-0.9.5/datatypes/html.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/http.py` & `datatypes-0.9.5/datatypes/http.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/logging.py` & `datatypes-0.9.5/datatypes/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # -*- coding: utf-8 -*-
 from logging import * # allow using this module as a passthrough for builtin logging
 import logging
 import logging.config
 from logging import config
 import sys
+from collections.abc import (
+    Mapping,
+    Sequence,
+)
+from string import Formatter
 
 
 def null_config(name):
     """This will configure a null logger for name, it is meant to avoid the "no handler found"
     warnings when libraries would use logging that hadn't been configured, but it
     seems like it is no longer needed in python 3
 
@@ -91,22 +96,34 @@
 
     # avoid circular dependency
     from .collections import Dict
 
     dict_config = Dict({
         'version': 1,
         'formatters': {
+            # https://docs.python.org/3/library/logging.html#logrecord-attributes
             'shortformatter': {
-                #'format': '[%(levelname).1s|%(asctime)s|%(process)d.%(thread)d|%(filename)s:%(lineno)s] %(message)s',
-                #'format': '[%(levelname).1s|%(filename)s:%(lineno)s] %(message)s',
                 'format': '[%(levelname).1s] %(message)s',
             },
             'longformatter': {
-                'format': '[%(levelname).1s|%(asctime)s|%(process)d.%(thread)d|%(filename)s:%(lineno)s] %(message)s',
-            }
+                'format': "|".join(['[%(levelname).1s',
+                    '%(asctime)s',
+                    '%(process)d.%(thread)d',
+                    '%(filename)s:%(lineno)s] %(message)s',
+                ])
+            },
+            'verboseformatter': {
+                'format': "|".join([
+                    '[%(levelname).1s',
+                    '%(asctime)s',
+                    '%(process)d.%(thread)d',
+                    '%(name)s', # logger name
+                    '%(pathname)s:%(lineno)s] %(message)s',
+                ])
+            },
         },
         'handlers': {
             'streamhandler': {
                 'level': 'DEBUG',
                 'class': 'logging.StreamHandler',
                 'formatter': 'shortformatter',
                 'filters': [],
@@ -244,47 +261,81 @@
         logmod = self.get_logging_module(**kwargs)
         level_name = logmod.getLevelName(logger.getEffectiveLevel())
 
         if level_name not in kwargs:
             level_name = level_name.lower()
 
         if level_name in kwargs:
-            arguments = kwargs[level_name]
-            log_args = arguments[0]
-            log_kwargs = {}
-            if len(arguments) > 1:
-                log_kwargs = arguments[1]
+            args = kwargs[level_name]
+            if isinstance(args, str):
+                # debug="a string value"
+                log_args = [args]
+                log_kwargs = {}
+
+            elif isinstance(args, Sequence):
+                if len(args) == 2:
+                    if isinstance(args[0], Sequence) and isinstance(args[1], Mapping):
+                        # debug=("a string value", {})
+                        # debug=(["a", "list", "value"], {})
+                        log_args = [args[0]]
+                        log_kwargs = args[1]
+
+                    else:
+                        # debug=["a list", "value"]
+                        log_args = args
+                        log_kwargs = {}
+
+                else:
+                    log_args = args
+                    log_kwargs = {}
+
+            else:
+                raise ValueError(f"Unknown value for {level_name}")
+
+            if len(log_args) == 1 and isinstance(log_args[0], list):
+                # https://docs.python.org/3/library/string.html#string.Formatter
+                parts = list(Formatter().parse(log_args[0][0]))
+                if len(parts) > 1 or parts[0][1] is not None:
+                    log_args = log_args[0] 
 
             log_kwargs["level"] = level_name
             self.log(*log_args, **log_kwargs)
 
     def log(self, format_str, *format_args, **kwargs):
         """wrapper around the module's logger
 
         :param format_str: str|list[str], the message to log, if this is a list
             then it will be joined with a space
         :param *format_args: list, if format_str is a string containing {},
             then format_str.format(*format_args) is ran
         :param **kwargs:
             level: str|int, something like logging.DEBUG or "DEBUG"
+            sentinel: callable|bool, if evaluates to False then the log will be
+                ignored
         """
+        sentinel = kwargs.pop("sentinel", None)
+        if sentinel is None:
+            sentinel = True
+
+        else:
+            if callable(sentinel):
+                sentinel = sentinel()
+
         logger = self.get_logger_instance(**kwargs)
         if isinstance(format_str, Exception):
             level = self.get_log_level(default_level="ERROR", **kwargs)
-            if self.is_logging(level):
-                #logger.exception(format_str)
-                #logger.log(level, f"{format_str}", *format_args, exc_info=format_str)
+            if self.is_logging(level) and sentinel:
                 logger.log(level, f"{format_str}", *format_args)
 
         else:
             if isinstance(format_str, list):
                 format_str = " ".join(filter(None, format_str))
 
             level = self.get_log_level(**kwargs)
-            if self.is_logging(level):
+            if self.is_logging(level) and sentinel:
                 try:
                     if format_args:
                         logger.log(level, format_str.format(*format_args))
                     else:
                         logger.log(level, format_str)
 
                 except UnicodeError as e:
```

### Comparing `datatypes-0.9.4/datatypes/number.py` & `datatypes-0.9.5/datatypes/number.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/parse.py` & `datatypes-0.9.5/datatypes/parse.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/path.py` & `datatypes-0.9.5/datatypes/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,23 @@
 import string
 import random
 import struct
 import imghdr
 from pathlib import Path as Pathlib
 import pickle
 from contextlib import contextmanager
-import fcntl
 import errno
 
+# not available on Windows
+try:
+    import fcntl
+except ImportError:
+    fcntl = None
+
+
 from .compat import *
 from . import environ
 from .string import String, ByteString
 from .collections import ListIterator
 from .copy import Deepcopy
 from .http import HTTPClient
 from .url import Url
@@ -1801,15 +1807,15 @@
         ret = True
         if self.exists():
             st = self.stat()
             ret = False if st.st_size else True
         return ret
 
     @contextmanager
-    def flock(self, mode="", operation=fcntl.LOCK_EX | fcntl.LOCK_NB, **kwargs):
+    def flock(self, mode="", operation=None, **kwargs):
         """similar to open but will also lock the file resource and will release
         the resource when the context manager is done
 
         :Example:
             filepath = Filepath("<PATH>")
             with filepath.lock("r") as fp:
                 if fp:
@@ -1822,14 +1828,21 @@
 
         :param mode: see .open()
         :param operation: defaults to exclusive lock, see fcntl module
         :param **kwargs: will be passed to .open()
         :returns: file descriptor with an active lock, it will return None if
             the lock wasn't successfully acquired
         """
+        if fcntl:
+            if operation is None:
+                operation = fcntl.LOCK_EX | fcntl.LOCK_NB
+
+        else:
+            raise ValueError("flock does not work because fcntl module is unavailable")
+
         try:
             with self.open(mode, **kwargs) as fp:
                 fcntl.flock(fp, operation)
                 try:
                     yield fp
 
                 finally:
```

### Comparing `datatypes-0.9.4/datatypes/profile.py` & `datatypes-0.9.5/datatypes/profile.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/reflection.py` & `datatypes-0.9.5/datatypes/reflection.py`

 * *Files 1% similar despite different names*

```diff
@@ -928,14 +928,23 @@
         """
         for class_name, rc in self.get_info(): 
             if isinstance(rc, self.reflect_class_class):
                 if ignore_private and rc.is_private():
                     continue
                 yield rc
 
+    def classes(self, ignore_private=True):
+        """yields classes (type instances) that are found in only this module (not submodules)
+
+        :param ignore_private: bool, if True then ignore classes considered private
+        :returns: a generator of type instances
+        """
+        for rc in self.reflect_classes(ignore_private=ignore_private):
+            yield rc.cls
+
     def reflect_class(self, name, *default_val):
         """Get a ReflectClass instance of name"""
         try:
             return self.get_info()[name]
 
         except KeyError as e:
             if default_val:
```

### Comparing `datatypes-0.9.4/datatypes/server.py` & `datatypes-0.9.5/datatypes/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         kwargs.setdefault("RequestHandlerClass", self.handler_class)
         super().__init__(server_address, **kwargs)
 
     def get_url(self, *args, **kwargs):
         """Create a url using the server's server_address information
 
         :example:
-            s = PathServer("/some/path")
+            s = BaseServer()
             print(s.get_url("foo.txt")) # http://localhost:PORT/foo.txt
 
         :param *args: passed through to Url
         :param **kwargs: passed throught to Url, scheme, hostname, and port will
             be set if not overridden
         :returns: Url instance
         """
@@ -136,14 +136,22 @@
             hostname=hostname,
             port=self.server_port
         ))
         kwargs.setdefault("scheme", "http")
 
         return Url(*args, **kwargs)
 
+    def serve_forever(self, *args, **kwargs):
+        # wrapped to call server close to avoid unclosed socket warnings
+        try:
+            super().serve_forever()
+
+        finally:
+            self.server_close()
+
 
 class PathHandler(SimpleHTTPRequestHandler):
     """Handler for PathServer
 
     the parent classes:
         https://github.com/python/cpython/blob/3.9/Lib/http/server.py
         https://github.com/python/cpython/blob/3.9/Lib/socketserver.py
@@ -173,15 +181,14 @@
 class PathServer(BaseServer):
     """A server that serves files from a path
 
     Moved from testdata.server on 1-24-2023
 
     :Example:
         basedir = "/some/path/to/directory/containing/files/to/server"
-
         s = PathServer(basedir)
 
     https://docs.python.org/3/library/http.server.html
     https://github.com/python/cpython/blob/3.9/Lib/http/server.py
     https://github.com/python/cpython/blob/3.9/Lib/socketserver.py
     """
     handler_class = PathHandler
```

### Comparing `datatypes-0.9.4/datatypes/service.py` & `datatypes-0.9.5/datatypes/service.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/string.py` & `datatypes-0.9.5/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/token.py` & `datatypes-0.9.5/datatypes/token.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/url.py` & `datatypes-0.9.5/datatypes/url.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes/utils.py` & `datatypes-0.9.5/datatypes/utils.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/datatypes.egg-info/PKG-INFO` & `datatypes-0.9.5/datatypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatypes
-Version: 0.9.4
+Version: 0.9.5
 Summary: Utility Classes and Functions that are handy across multiple projects
 Home-page: http://github.com/Jaymon/datatypes
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `datatypes-0.9.4/datatypes.egg-info/SOURCES.txt` & `datatypes-0.9.5/datatypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.4/setup.py` & `datatypes-0.9.5/setup.py`

 * *Files identical despite different names*

