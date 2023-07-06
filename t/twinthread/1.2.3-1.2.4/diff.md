# Comparing `tmp/twinthread-1.2.3.tar.gz` & `tmp/twinthread-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinthread-1.2.3.tar", max compression
+gzip compressed data, was "twinthread-1.2.4.tar", max compression
```

## Comparing `twinthread-1.2.3.tar` & `twinthread-1.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      457 2023-06-23 20:58:04.570400 twinthread-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    12520 2023-06-23 20:58:04.570855 twinthread-1.2.3/twinthread/__init__.py
--rw-r--r--   0        0        0      660 2023-06-20 21:09:20.015296 twinthread-1.2.3/twinthread/exec_task.py
--rw-r--r--   0        0        0     3247 2023-06-20 21:09:20.015428 twinthread-1.2.3/twinthread/jupyter.py
--rw-r--r--   0        0        0      725 2023-06-20 21:09:20.015543 twinthread-1.2.3/twinthread/string.py
--rw-r--r--   0        0        0      296 2023-06-22 15:31:37.239496 twinthread-1.2.3/twinthread/testing.py
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 twinthread-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      476 2023-07-06 14:42:59.490835 twinthread-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    12529 2023-07-06 14:42:59.491041 twinthread-1.2.4/twinthread/__init__.py
+-rw-r--r--   0        0        0      660 2023-06-20 21:09:20.015296 twinthread-1.2.4/twinthread/exec_task.py
+-rw-r--r--   0        0        0     3256 2023-07-06 14:42:59.491212 twinthread-1.2.4/twinthread/jupyter.py
+-rw-r--r--   0        0        0      725 2023-07-06 14:42:59.491287 twinthread-1.2.4/twinthread/string_handling.py
+-rw-r--r--   0        0        0      296 2023-07-06 14:40:48.700732 twinthread-1.2.4/twinthread/testing.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 twinthread-1.2.4/PKG-INFO
```

### Comparing `twinthread-1.2.3/twinthread/__init__.py` & `twinthread-1.2.4/twinthread/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 """Top-level package for twinthread."""
 import io
 
 from _plotly_utils.utils import PlotlyJSONEncoder
 
 from .jupyter import register_jupyter
-from .string import task_string_to_context
+from .string_handling import task_string_to_context
 
 __author__ = """Brad Johnson"""
 __email__ = "brad.johnson@twinthread.com"
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 
 import re
 import json
 import simplejson
 import requests
 import pandas as pd
 from io import StringIO
```

### Comparing `twinthread-1.2.3/twinthread/exec_task.py` & `twinthread-1.2.4/twinthread/exec_task.py`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.3/twinthread/jupyter.py` & `twinthread-1.2.4/twinthread/jupyter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from IPython import get_ipython
-from .string import task_string_to_context, pretty_result
+from .string_handling import task_string_to_context, pretty_result
 from .exec_task import exec_code
 import sys
 
 
 def confirm(text, default_yes=True):
     choice = input(text + "(Y/n)" if default_yes else "(y/N)")
     choice = choice.lower()
```

### Comparing `twinthread-1.2.3/twinthread/string.py` & `twinthread-1.2.4/twinthread/string_handling.py`

 * *Files identical despite different names*

