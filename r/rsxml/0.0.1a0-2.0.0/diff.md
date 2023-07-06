# Comparing `tmp/rsxml-0.0.1a0.tar.gz` & `tmp/rsxml-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsxml-0.0.1a0.tar", last modified: Tue May 23 14:37:02 2023, max compression
+gzip compressed data, was "rsxml-2.0.0.tar", last modified: Wed Jul  5 23:49:26 2023, max compression
```

## Comparing `rsxml-0.0.1a0.tar` & `rsxml-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,33 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.650679 rsxml-0.0.1a0/
--rw-r--r--   0 matt       (501) staff       (20)      478 2023-05-23 14:37:02.650772 rsxml-0.0.1a0/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)       39 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/README.md
--rw-r--r--   0 matt       (501) staff       (20)      550 2023-05-23 14:30:46.000000 rsxml-0.0.1a0/pyproject.toml
--rw-r--r--   0 matt       (501) staff       (20)       79 2023-05-23 14:37:02.651038 rsxml-0.0.1a0/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     1197 2023-05-23 14:24:16.000000 rsxml-0.0.1a0/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.642647 rsxml-0.0.1a0/src/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.644759 rsxml-0.0.1a0/src/debug/
--rw-r--r--   0 matt       (501) staff       (20)      102 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     7971 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/debug_proc.py
--rw-r--r--   0 matt       (501) staff       (20)     3118 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/loop_timer.py
--rw-r--r--   0 matt       (501) staff       (20)     1904 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/timer.py
--rw-r--r--   0 matt       (501) staff       (20)     8508 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/timer_buckets.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.645199 rsxml-0.0.1a0/src/logging/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/logging/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     8209 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/logging/logger.py
--rw-r--r--   0 matt       (501) staff       (20)     3712 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/logging/progress_bar.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.647792 rsxml-0.0.1a0/src/rsxml/
--rw-r--r--   0 matt       (501) staff       (20)     2768 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Analysis.py
--rw-r--r--   0 matt       (501) staff       (20)     7517 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Dataset.py
--rw-r--r--   0 matt       (501) staff       (20)     2214 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/MetaData.py
--rw-r--r--   0 matt       (501) staff       (20)     5713 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Project.py
--rw-r--r--   0 matt       (501) staff       (20)     2611 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/ProjectBounds.py
--rw-r--r--   0 matt       (501) staff       (20)     3128 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/QAQCEvent.py
--rw-r--r--   0 matt       (501) staff       (20)     2984 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/RSObj.py
--rw-r--r--   0 matt       (501) staff       (20)     2461 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Realization.py
--rw-r--r--   0 matt       (501) staff       (20)      236 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      428 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/common.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.648821 rsxml-0.0.1a0/src/rsxml.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)      478 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      824 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 14:32:36.000000 rsxml-0.0.1a0/src/rsxml.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)       24 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)       26 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/top_level.txt
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.650431 rsxml-0.0.1a0/src/tests/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     2320 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_dotenv.py
--rw-r--r--   0 matt       (501) staff       (20)     1127 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_etags.py
--rw-r--r--   0 matt       (501) staff       (20)     1325 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_paths.py
--rw-r--r--   0 matt       (501) staff       (20)     6908 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_project_xml.py
--rw-r--r--   0 matt       (501) staff       (20)     7499 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_timers.py
--rw-r--r--   0 matt       (501) staff       (20)     3202 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_util.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-05 23:49:26.330300 rsxml-2.0.0/
+-rw-r--r--   0 matt       (501) staff       (20)     1072 2023-07-05 23:12:54.000000 rsxml-2.0.0/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-05 23:49:26.330409 rsxml-2.0.0/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     6578 2023-07-05 23:39:56.000000 rsxml-2.0.0/README.md
+-rw-r--r--   0 matt       (501) staff       (20)      864 2023-07-05 23:36:34.000000 rsxml-2.0.0/pyproject.toml
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-05 23:49:26.327186 rsxml-2.0.0/rsxml/
+-rw-r--r--   0 matt       (501) staff       (20)      385 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)       22 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/__version__.py
+-rw-r--r--   0 matt       (501) staff       (20)    13856 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/api.py
+-rw-r--r--   0 matt       (501) staff       (20)      151 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/constants.py
+-rw-r--r--   0 matt       (501) staff       (20)     2852 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/dotenv.py
+-rw-r--r--   0 matt       (501) staff       (20)     1741 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/etag.py
+-rw-r--r--   0 matt       (501) staff       (20)      766 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/rspaths.py
+-rw-r--r--   0 matt       (501) staff       (20)     7339 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/util.py
+-rw-r--r--   0 matt       (501) staff       (20)     1999 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/validation.py
+-rw-r--r--   0 matt       (501) staff       (20)      371 2023-07-05 23:12:54.000000 rsxml-2.0.0/rsxml/xml.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-05 23:49:26.328393 rsxml-2.0.0/rsxml.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-05 23:49:26.000000 rsxml-2.0.0/rsxml.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      542 2023-07-05 23:49:26.000000 rsxml-2.0.0/rsxml.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-05 23:49:26.000000 rsxml-2.0.0/rsxml.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 16:11:44.000000 rsxml-2.0.0/rsxml.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)       68 2023-07-05 23:49:26.000000 rsxml-2.0.0/rsxml.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)        6 2023-07-05 23:49:26.000000 rsxml-2.0.0/rsxml.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)       79 2023-07-05 23:49:26.330693 rsxml-2.0.0/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     1195 2023-07-05 23:49:20.000000 rsxml-2.0.0/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-05 23:49:26.329950 rsxml-2.0.0/tests/
+-rw-r--r--   0 matt       (501) staff       (20)     2302 2023-07-05 23:12:54.000000 rsxml-2.0.0/tests/test_dotenv.py
+-rw-r--r--   0 matt       (501) staff       (20)     1131 2023-07-05 23:12:54.000000 rsxml-2.0.0/tests/test_etags.py
+-rw-r--r--   0 matt       (501) staff       (20)      679 2023-07-05 23:12:54.000000 rsxml-2.0.0/tests/test_load_samples.py
+-rw-r--r--   0 matt       (501) staff       (20)     1327 2023-07-05 23:12:54.000000 rsxml-2.0.0/tests/test_paths.py
+-rw-r--r--   0 matt       (501) staff       (20)     8133 2023-07-05 23:12:54.000000 rsxml-2.0.0/tests/test_project_xml.py
+-rw-r--r--   0 matt       (501) staff       (20)     7503 2023-07-05 23:12:54.000000 rsxml-2.0.0/tests/test_timers.py
+-rw-r--r--   0 matt       (501) staff       (20)     3204 2023-07-05 23:27:33.000000 rsxml-2.0.0/tests/test_util.py
```

### Comparing `rsxml-0.0.1a0/src/debug/debug_proc.py` & `rsxml-2.0.0/rsxml/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,250 +1,260 @@
-from __future__ import annotations
-import math
-import csv
+"""_summary_
+
+Raises:
+    Exception: _description_
+    Exception: _description_
+    e: _description_
+    Exception: _description_
+    Exception: _description_
+    Exception: _description_
+    Exception: _description_
+
+Returns:
+    _type_: _description_
+
+Yields:
+    _type_: _description_
+"""
+import sys
+import gc
+import shutil
+import hashlib
 import os
-from datetime import datetime
-from concurrent.futures import ThreadPoolExecutor
-from time import sleep
-# Make sure this module doesn't crash if these aren't installed.
-try:
-    import psutil
-except ImportError:
-    psutil = None
-try:
-    import matplotlib.pyplot as plt
-except ImportError:
-    plt = None
-from src.logging.logger import Logger
+import math
+from rsxml.logging.logger import Logger
 
-# https://medium.com/survata-engineering-blog/monitoring-memory-usage-of-a-running-python-program-49f027e3d1ba
+# Set if this environment variable is set don't show any UI
+NO_UI = os.environ.get('NO_UI') is not None
 
 
-class ProcStats():
-    """_summary_
+def batch(iterable, num=1):
+    """Split a list into a list of regularly-sized lists of size n
+
+    Args:
+        iterable ([type]): [description]
+        n (int, optional): [description]. Defaults to 1.
+
+    Yields:
+        [type]: [description]
+    """
+    length = len(iterable)
+    for ndx in range(0, length, num):
+        yield iterable[ndx:min(ndx + num, length)]
+
+
+def safe_remove_file(file_path):
+    """Remove a file without throwing an error
+
+    Args:
+        file_path ([type]): [description]
+    """
+    log = Logger("safe_remove_file")
+    try:
+        if not os.path.isfile(file_path):
+            log.warning(f'File not found: {file_path}')
+        os.remove(file_path)
+        log.debug(f'File removed: {file_path}')
+    except Exception as err:
+        log.error(str(err))
+
+
+def file_compare(file_a, file_b, md5=True):
+    """Do a file comparison, starting with file size and finishing with md5
+
+    Args:
+        file_a ([type]): [description]
+        file_b ([type]): [description]
 
     Returns:
-        _type_: _description_
+        [type]: [description]
     """
-    headers = ['datetime', 'cpu_percent', 'resident_memory', 'virtual_memory', 'children', 'children_resident', 'children_virtual']
+    log = Logger("file_compare")
+    log.debug('Comparing: {} {}'.format(file_a, file_b))
+    try:
+        # If the file sizes aren't the same then there's
+        # no reason to do anything more
+        a_stats = os.stat(file_a)
+        b_stats = os.stat(file_b)
+        if a_stats.st_size != b_stats.st_size:
+            log.debug('Files are NOT the same size: {:,} vs. {:,}')
+            return False
+
+        # If we want this to be a quick-compare and not do MD5 then we just
+        # do the file size and leave it at that
+        if not md5:
+            return True
+
+        with open(file_a, 'rb') as afile:
+            hasher1 = hashlib.md5()
+            buf1 = afile.read()
+            hasher1.update(buf1)
+            md5_a = (str(hasher1.hexdigest()))
+
+        with open(file_b, 'rb') as bfile:
+            hasher2 = hashlib.md5()
+            buf1 = bfile.read()
+            hasher2.update(buf1)
+            md5_b = (str(hasher2.hexdigest()))
+
+        # Compare md5
+        if md5_a == md5_b:
+            log.debug('File MD5 hashes match')
+            return True
+        else:
+            log.debug('File MD5 hashes DO NOT match')
+            return False
+    except Exception as err:
+        log.error(f'Error comparing files: {err}')
+        return False
 
-    def __init__(self, cpu_percent, rss_raw: int, vms_raw: int, children: int, children_rss_raw: int, children_vms_raw: int):
-        """_summary_
 
-        Args:
-            cpu_percent (_type_): _description_
-            rss_raw (int): _description_
-            vms_raw (int): _description_
-            children (int): _description_
-            children_rss_raw (int): _description_
-            children_vms_raw (int): _description_
-        """
-        self.datetime = datetime.now()
-        self.cpu_percent = cpu_percent
-        self.children = children
-        self.rss = rss_raw / float(2 ** 20)
-        self.vms = vms_raw / float(2 ** 20)
-        self.children_rss = children_rss_raw / float(2 ** 20)
-        self.children_vms = children_vms_raw / float(2 ** 20)
-
-    def row(self):
-        """_summary_
-
-        Returns:
-            _type_: _description_
-        """
-        return [
-            self.datetime.strftime('%Y-%m-%d %H:%M:%S'),
-            math.ceil(self.cpu_percent),
-            f"{self.rss:.2f}",
-            f"{self.vms:.2f}",
-            f"{self.children}",
-            f"{self.rss:.2f}",
-            f"{self.vms:.2f}"
-        ]
-
-    def toString(self) -> str:
-        """_summary_
-
-        Returns:
-            _type_: _description_
-        """
-        return f"datetime: {self.datetime.strftime('%Y-%m-%d %H:%M:%S')}, cpu_percent: {math.ceil(self.cpu_percent)}, mem_resident: {self.rss:.2f}Mb, mem_virtual: {self.vms:.2f}Mb, num_children: {self.children}, mem_children_resident: {self.rss:.2f}Mb, mem_children_virtual: {self.vms:.2f}Mb"
-
-    def max(self, tick: ProcStats):
-        """_summary_
-
-        Args:
-            tick (ProcStats): _description_
-        """
-        self.cpu_percent = max(self.cpu_percent, tick.cpu_percent)
-        self.children = max(self.children, tick.children)
-        self.rss = max(self.rss, tick.rss)
-        self.vms = max(self.vms, tick.vms)
-        self.children_rss = max(self.children_rss, tick.children_rss)
-        self.children_vms = max(self.children_vms, tick.children_vms)
+def safe_remove_dir(dir_path):
+    """Remove a directory without throwing an error
 
+    Args:
+        file_path ([type]): [description]
+    """
+    log = Logger("safe_remove_dir")
+    try:
+        shutil.rmtree(dir_path, ignore_errors=True)
+        log.debug(f'Directory removed: {dir_path}')
+    except Exception as err:
+        log.error(f'Error removing tree: {err}')
+        return False
 
-class MemoryMonitor:
-    """_summary_
+
+def safe_makedirs(dir_create_path):
+    """safely, recursively make a directory
+
+    Arguments:
+        dir_create_path {[type]} -- [description]
+    """
+    log = Logger("MakeDir")
+
+    # Safety check on path lengths
+    if len(dir_create_path) < 5 or len(dir_create_path.split(os.path.sep)) <= 2:
+        raise Exception(f'Invalid path: {dir_create_path}')
+
+    if os.path.exists(dir_create_path) and os.path.isfile(dir_create_path):
+        raise Exception(f'Can\'t create directory if there is a file of the same name: {dir_create_path}')
+
+    if not os.path.exists(dir_create_path):
+        try:
+            log.info(f'Folder not found. Creating: {dir_create_path}')
+            os.makedirs(dir_create_path)
+        except Exception as err:
+            # Possible that something else made the folder while we were trying
+            if not os.path.exists(dir_create_path):
+                log.error(f'Could not create folder: {dir_create_path}')
+                raise err
+
+
+def sizeof_fmt(num, suffix='B'):
+    """Format bytesize properly
+
+    Arguments:
+        num {[type]} -- Size
+
+    Keyword Arguments:
+        suffix {str} -- [description] (default: {'B'})
+
+    Returns:
+        [type] -- [description]
     """
+    for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
+        if abs(num) <= 1000.0:
+            return f"{num:3.1f} {unit}{suffix}"
+        num /= 1000.0
+    return f"{num:.1f} Yi{suffix}"
+
 
-    def __init__(self, logfile: str, loop_delay=1):
-        if not psutil:
-            return
-        self.keep_measuring = True
-        self.filepath = logfile
-        self.loop_delay = loop_delay
-        self.process = psutil.Process(os.getpid())
-        self.headers_written = False
-        self.max_stats = ProcStats(0, 0, 0, 0, 0, 0)
-
-    def write_line(self, arr, mode='a'):
-        """_summary_
-
-        Args:
-            arr (_type_): _description_
-            mode (str, optional): _description_. Defaults to 'a'.
-        """
-        with open(self.filepath, mode, newline='', encoding='utf-8') as csvfile:
-            csvwriter = csv.writer(csvfile)
-            csvwriter.writerow(arr)
-
-    def getstats(self) -> ProcStats:
-        """_summary_
-
-        Returns:
-            ProcStats: _description_
-        """
-        cpu_percent = self.process.cpu_percent()
-        mem_info = self.process.memory_info()
-        children = 0
-        children_rss = 0
-        children_vms = 0
-
-        for child in self.process.children():
-            child_mem = child.memory_info()
-            children_rss += child_mem.rss
-            children_vms += child_mem.vms
-            children += 1
-
-        stats = ProcStats(cpu_percent, mem_info.rss, mem_info.vms, children, children_rss, children_vms)
-        self.max_stats.max(stats)
-        return stats
-
-    def measure_usage(self):
-        """_summary_
-
-        Returns:
-            _type_: _description_
-        """
-        self.write_line(ProcStats.headers, 'w')
-        while self.keep_measuring:
-            self.write_line(self.getstats().row())
-            sleep(self.loop_delay)
-        return self.max_stats
-
-    def write_plot(self, imgpath: str):
-        """_summary_
-
-        Args:
-            imgpath (str): _description_
-        """
-        log = Logger('write_plot')
-        if not plt:
-            log.error('You need Matplotlib to run write_plot')
-            return
-        x = []
-        data = {}
-        with open(self.filepath, encoding='utf8') as csvfile:
-            reader = csv.DictReader(csvfile)
-            for row in reader:
-                for key in row.keys():
-                    if key == 'datetime':
-                        x.append(row[key])
-                    else:
-                        if key in ['children', 'cpu_percent']:
-                            val = int(row[key])
-                        else:
-                            val = float(row[key])
-                        if key not in data:
-                            data[key] = [val]
-                        else:
-                            data[key].append(val)
-
-        chart_title = 'Process stats'
-        xlabel = 'time'
-        ylabel = 'Mb'
-
-        plt.clf()
-
-        fig, plt_ax = plt.subplots()
-        plt_ax.title.set_text(chart_title)
-        ax2 = plt_ax.twinx()
-        #  ['datetime', 'cpu_percent', 'resident_memory', 'virtual_memory', 'children', 'children_resident', 'children_virtual']
-        for key in ['children_resident', 'children_virtual', 'resident_memory', 'virtual_memory']:
-            if key in data:
-                plt_ax.plot(x, data[key], label=key)
-            ax2._get_lines.get_next_color()
-
-        plt_ax.set_xlabel(xlabel)
-        plt_ax.set_ylabel(ylabel)
-
-        for key in ['cpu_percent', 'children']:
-            if key in data:
-                ax2.plot(x, data[key], label=key)
-
-        plt_ax.legend(loc='lower left')
-        ax2.legend(loc='lower right')
-
-        freq = math.floor(len(x) / 10)
-        if freq == 0:
-            freq = 1
-        plt_ax.set_xticks(x[::freq])
-        plt_ax.set_xticklabels(x[::freq], rotation=45)
-        plt_ax.grid(True)
-
-        # plt.tight_layout()
-        fig.set_size_inches(8, 6)
-        fig.savefig(imgpath, format='png', dpi=300)
+def get_obj_size(obj):
+    """Generic function to get the byte-size of a variable
 
+    Arguments:
+        obj {[type]} -- [description]
+
+    Returns:
+        [type] -- [description]
+    """
+    marked = {id(obj)}
+    obj_q = [obj]
+    osize = 0
 
-def thread_run(callback, memlogfile: str, *args, **kwargs):
+    while obj_q:
+        osize += sum(map(sys.getsizeof, obj_q))
+
+        # Lookup all the object referred to by the object in obj_q.
+        # See: https://docs.python.org/3.7/library/gc.html#gc.get_referents
+        all_refr = ((id(o), o) for o in gc.get_referents(*obj_q))
+
+        # Filter object that are already marked.
+        # Using dict notation will prevent repeated objects.
+        new_refr = {o_id: o for o_id, o in all_refr if o_id not in marked and not isinstance(o, type)}
+
+        # The new obj_q will be the ones that were not marked,
+        # and we will update marked with their ids so we will
+        # not traverse them again.
+        obj_q = new_refr.values()
+        marked.update(new_refr.keys())
+
+    return osize
+
+
+def pretty_duration(time_s=False):
+    """
+    Get a datetime object or a int() Epoch timestamp and return a
+    pretty string like 'an hour ago', 'Yesterday', '3 months ago',
+    'just now', etc
+    """
+    if not time_s >= 0:
+        return '???'
+    seconds = math.floor(time_s % 60)
+    minutes = math.floor(time_s / 60) % 60
+    hours = math.floor(time_s / 3600) % 24
+    if time_s < 60:
+        return f"{seconds:.1f} seconds".format()
+    elif time_s < 3600:
+        return f"{minutes}:{seconds:02} minutes"
+    elif time_s < 86400:
+        return f"{hours}:{minutes:02} hours"
+    else:
+        days = math.floor(time_s / 86400)
+        return f"{days} days, {hours}:{minutes:02} hours"
+
+
+def parse_metadata(arg_string):
     """_summary_
 
     Args:
-        callback (function): _description_
-        memlogfile (str): _description_
+        arg_string (_type_): _description_
+
+    Raises:
+        Exception: _description_
+        Exception: _description_
+        Exception: _description_
+        Exception: _description_
 
     Returns:
         _type_: _description_
     """
-    log = Logger('Debug')
-    if not psutil:
-        log.error('You need "psutil" to run the debug tools')
-        return
-
-    memmon = MemoryMonitor(memlogfile, 1)
-    result = None
-    max_obj = None
-    try:
-        with ThreadPoolExecutor() as executor:
-            mem_thread = executor.submit(memmon.measure_usage)
-            try:
-                fn_thread = executor.submit(callback, *args, **kwargs)
-                result = fn_thread.result()
-            except Exception as err_in:
-                log.error(f"Error executing code: {err_in}")
-            finally:
-                memmon.keep_measuring = False
-                max_obj = mem_thread.result()
-                log.debug(f'MaxStats: {max_obj}')
-    except Exception as err_out:
-        # Make sure we always return so that we don't have to debug our debugger
-        log.error(err_out)
+    meta = {}
     try:
-        memmon.write_plot(os.path.splitext(memlogfile)[0] + '.png')
-    except Exception as err:
-        log.error(f'Error Writing memory plot: {err}')
+        if arg_string:
+            for kvp in arg_string.split(','):
+                key_value = kvp.split('=')
+                clean_key = key_value[0].strip()
+                clean_value = key_value[1].strip()
+                if len(clean_key) < 1:
+                    raise Exception('Empty key')
+                if len(clean_value) < 1:
+                    raise Exception('Empty value')
+                if clean_key in meta:
+                    raise Exception('Duplicate metadata key')
+
+                meta[clean_key] = clean_value
+    except Exception as ex:
+        print(ex)
+        raise Exception(f'Error parsing command line metadata: {arg_string}')
 
-    ret_val = max_obj.toString() if max_obj is not None else "process no longer exists"
-    return result, ret_val
+    return meta
```

### Comparing `rsxml-0.0.1a0/src/tests/test_dotenv.py` & `rsxml-2.0.0/tests/test_dotenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """[summary]"""
 import unittest
 import tempfile
 import argparse
 
-from src.dotenv import parse_args_env, parse_dotenv
+from rsxml.dotenv import parse_args_env, parse_dotenv
 
 
 class DotEnvTest(unittest.TestCase):
     """[summary]"""
 
     def test_parse_dotenv(self):
         """[summary]
         """
 
         # Now parse the .env file and make sure we get the right values
         with tempfile.NamedTemporaryFile(mode='w+', delete=False) as tmp:
             tmp.write('TEST_VAR=test_value\nTEST_VAR2=test_value2\n')
             tmp.close()
-            env = parse_dotenv(tmp.file.name)
+            env = parse_dotenv(tmp.name)
             self.assertEqual(env['TEST_VAR'], 'test_value')
             self.assertEqual(env['TEST_VAR2'], 'test_value2')
 
         # It should handle quotes as well
         with tempfile.NamedTemporaryFile(mode='w+', delete=False) as tmp:
             tmp.write('TEST_VARQ="test_value"\nTEST_VAR2Q=\'test_value2\'\n')
             tmp.close()
-            env = parse_dotenv(tmp.file.name)
+            env = parse_dotenv(tmp.name)
             self.assertEqual(env['TEST_VARQ'], 'test_value')
             self.assertEqual(env['TEST_VAR2Q'], 'test_value2')
 
         # it should handle spaces as well
         with tempfile.NamedTemporaryFile(mode='w+', delete=False) as tmp:
             tmp.write('TEST_VARSP= "test value "\n TEST_VAR2SP = \'   test value2\'\n')
             tmp.close()
-            env = parse_dotenv(tmp.file.name)
+            env = parse_dotenv(tmp.name)
             self.assertEqual(env['TEST_VARSP'], 'test value')
             self.assertEqual(env['TEST_VAR2SP'], 'test value2')
 
     def test_parse_args_env(self):
         """[summary]
         """
         # Now parse the .env file and make sure we get the right values
@@ -46,13 +46,13 @@
             tmp.close()
 
             args = argparse.ArgumentParser()
             args.add_argument('--test-var', type=str, default='{env:TEST_VAR}')
             args.add_argument('--test-var2', type=str, default='{env:TEST_VAR2}')
 
             # Now parse the .env file and make sure we get the right values
-            env = parse_args_env(args, tmp.file.name, [
+            env = parse_args_env(args, tmp.name, [
                 '--test-var', '{env:TEST_VAR}',
                 '--test-var2', '{env:TEST_VAR2}'
             ])
             self.assertEqual(env.test_var, 'test_value')
             self.assertEqual(env.test_var2, 'test_value2')
```

### Comparing `rsxml-0.0.1a0/src/tests/test_etags.py` & `rsxml-2.0.0/tests/test_etags.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Testing for the vector ops
 
 """
 import unittest
 import os
 
-from src.etag import calculate_etag
-from src.dotenv import parse_dotenv
+from rsxml.etag import calculate_etag
+from rsxml.dotenv import parse_dotenv
 
 
 class EtagTests(unittest.TestCase):
     """[summary]
 
     Args:
         unittest ([type]): [description]
```

### Comparing `rsxml-0.0.1a0/src/tests/test_paths.py` & `rsxml-2.0.0/tests/test_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Testing for the vector ops
 
 """
 import unittest
 import platform
 import os
 
-from src.rspaths import parse_posix_path, parse_rel_path
+from rsxml.rspaths import parse_posix_path, parse_rel_path
 
 IS_WINDOWS = platform.system() == 'Windows'
 
 
 class RSPathTests(unittest.TestCase):
     """[summary]
```

### Comparing `rsxml-0.0.1a0/src/tests/test_project_xml.py` & `rsxml-2.0.0/tests/test_project_xml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """[summary]"""
 import unittest
 import os
 from uuid import uuid4
 
-from src import rsxml
+from rsxml import project_xml
+from rsxml.project_xml import MetaData
 
 MOCK_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'mock')
 
 
 class RSObjTest(unittest.TestCase):
     """[summary]"""
 
@@ -16,53 +17,53 @@
         """
         xml_id = 'SOMEID'
         name = 'test_project'
         xml_tag = 'MyTag'
         description = 'test description'
         summary = 'test summary'
         citation = 'test citation'
-        meta = {
-            'test_key': 'test_value',
-            'test_key2': 'test_value2',
-        }
-        rsobj = rsxml.RSObj(xml_id=xml_id,
-                            xml_tag=xml_tag,
-                            name=name,
-                            summary=summary,
-                            description=description,
-                            citation=citation,
-                            meta_data=meta
-                            )
+        meta = MetaData(values=[
+            project_xml.Meta(name='test_key', value='test_value'),
+            project_xml.Meta(name='test_key2', value='test_value2')
+        ])
+
+        rsobj = project_xml.RSObj(xml_id=xml_id,
+                                  xml_tag=xml_tag,
+                                  name=name,
+                                  summary=summary,
+                                  description=description,
+                                  citation=citation,
+                                  meta_data=meta
+                                  )
         self.assertEqual(rsobj.xml_id, xml_id)
         self.assertEqual(rsobj.xml_tag, xml_tag)
         self.assertEqual(rsobj.name, name)
         self.assertEqual(rsobj.summary, summary)
         self.assertEqual(rsobj.description, description)
         self.assertEqual(rsobj.citation, citation)
-        self.assertDictEqual(rsobj.meta_data, meta)
 
         xml = rsobj.to_xml()
         self.assertEqual(xml.attrib['id'], xml_id)
         self.assertEqual(xml.find('Name').text, name)
         self.assertEqual(xml.find('Summary').text, summary)
         self.assertEqual(xml.find('Description').text, description)
         self.assertEqual(xml.find('Citation').text, citation)
-        self.assertEqual(xml.find('MetaData/Meta[@name=\'test_key\']').text, 'test_value')
+        self.assertEqual(xml.find('MetaData/Meta/[@name=\'test_key\']').text, 'test_value')
         self.assertEqual(xml.find('MetaData/Meta[@name=\'test_key2\']').text, 'test_value2')
 
 
 class ProjectClasses(unittest.TestCase):
     """[summary]"""
 
     def test_project_bounds_init(self):
         """[summary]
         """
-        bounds = rsxml.ProjectBounds(
-            bounding_box=rsxml.BoundingBox(-1.0, -2.0, -0.5, -0.5),
-            centroid=rsxml.Coords(-0.75, -1.25),
+        bounds = project_xml.ProjectBounds(
+            bounding_box=project_xml.BoundingBox(-1.0, -2.0, -0.5, -0.5),
+            centroid=project_xml.Coords(-0.75, -1.25),
             filepath='test_path/test.geojson'
         )
         self.assertEqual(bounds.bounding_box, (-1.0, -2.0, -0.5, -0.5))
         self.assertEqual(bounds.centroid, (-0.75, -1.25))
         self.assertEqual(bounds.filepath, 'test_path/test.geojson')
 
         xml = bounds.to_xml()
@@ -76,15 +77,15 @@
         self.assertEqual(xml.find('Path').text, 'test_path/test.geojson')
 
     def test_warehouse(self):
         """Test the px.Warehouse class constructor
         """
         guid = str(uuid4())
         api_url = 'https://api.something.com/api'
-        warehouse = rsxml.Warehouse(guid, api_url=api_url)
+        warehouse = project_xml.Warehouse(guid, api_url=api_url)
 
         self.assertEqual(warehouse.guid, guid)
         self.assertEqual(warehouse.api_url, api_url)
 
         xml = warehouse.to_xml()
         self.assertDictEqual(xml.attrib, {'id': guid, 'apiUrl': api_url})
 
@@ -93,67 +94,65 @@
         """
         guid = str(uuid4())
         name = 'test_project'
         description = 'test description'
         project_type = 'VBET'
         summary = 'test summary'
         citation = 'test citation'
-        bounds = rsxml.ProjectBounds(
-            bounding_box=rsxml.BoundingBox(-1.0, -2.0, -0.5, -0.5),
-            centroid=rsxml.Coords(-0.75, -1.25),
+        bounds = project_xml.ProjectBounds(
+            bounding_box=project_xml.BoundingBox(-1.0, -2.0, -0.5, -0.5),
+            centroid=project_xml.Coords(-0.75, -1.25),
             filepath='test_path/test.geojson'
         )
-        meta_data = {"test_key": "test_value"}
+        meta_data = project_xml.MetaData([project_xml.Meta(name='test_key', value='test_value')])
 
-        project = rsxml.Project(
+        project = project_xml.Project(
             name=name,
             project_type=project_type,
             description=description,
             summary=summary,
             citation=citation,
             bounds=bounds,
-            meta_data=meta_data
+            meta_data=meta_data,
         )
 
         self.assertEqual(project.name, name)
         self.assertEqual(project.description, description)
         self.assertEqual(project.project_type, project_type)
         self.assertEqual(project.summary, summary)
         self.assertEqual(project.citation, citation)
         self.assertEqual(project.bounds, bounds)
         self.assertEqual(project.meta_data, meta_data)
 
         xml = project.to_xml()
-        self.assertDictEqual(xml.attrib, {'id': guid})
         self.assertEqual(xml.find('Name').text, name)
         self.assertEqual(xml.find('Description').text, description)
         self.assertEqual(xml.find('ProjectType').text, project_type)
         self.assertEqual(xml.find('Summary').text, summary)
         self.assertEqual(xml.find('Citation').text, citation)
         self.assertEqual(xml.find('ProjectBounds/Centroid/Lng').text, '-0.75')
         self.assertEqual(xml.find('ProjectBounds/Centroid/Lat').text, '-1.25')
         self.assertEqual(xml.find('ProjectBounds/BoundingBox/MinLng').text, '-1.0')
         self.assertEqual(xml.find('ProjectBounds/BoundingBox/MinLat').text, '-2.0')
         self.assertEqual(xml.find('ProjectBounds/BoundingBox/MaxLng').text, '-0.5')
         self.assertEqual(xml.find('ProjectBounds/BoundingBox/MaxLat').text, '-0.5')
         self.assertEqual(xml.find('ProjectBounds/Path').text, 'test_path/test.geojson')
-        self.assertEqual(xml.find('MetaData/Item').attrib, {'key': 'test_key', 'value': 'test_value'})
 
     def test_dataset(self):
         """Test the px.Dataset class constructor
         """
         xml_id = 'SOMEID'
         name = 'test_dataset'
         ds_type = 'CSV'
         description = 'test description'
         ds_path = 'test_path/test.geojson'
         summary = 'test summary'
         citation = 'test citation'
 
-        dataset = rsxml.Dataset(
+        dataset = project_xml.Dataset(
             xml_id=xml_id,
             name=name,
             ds_type=ds_type,
             path=ds_path,
             description=description,
             summary=summary,
             citation=citation
@@ -170,7 +169,39 @@
         self.assertEqual(xml.tag, ds_type)
         self.assertDictEqual(xml.attrib, {'id': xml_id})
         self.assertEqual(xml.find('Name').text, name)
         self.assertEqual(xml.find('Description').text, description)
         self.assertEqual(xml.find('Summary').text, summary)
         self.assertEqual(xml.find('Path').text, ds_path)
         self.assertEqual(xml.find('Citation').text, citation)
+
+    def test_metadata(self):
+
+        # Test the metadata types
+        test_meta = MetaData(values=[
+            project_xml.Meta(name='test_key', value='test_no_type'),
+            project_xml.Meta(name='test_key2', value='test_valid_type', type='filepath')
+        ])
+
+        try:
+            test_meta2 = MetaData(values=[
+                project_xml.Meta(name='test_key2', value='test_invalid_type', type='invalid_type')
+            ])
+            # Should not be able to get here with invalid metadata
+            self.fail('Expected ValueError')
+        except ValueError:
+            pass
+
+        # Test the ext types
+        test_meta3 = MetaData(values=[
+            project_xml.Meta(name='test_key', value='test_no_type'),
+            project_xml.Meta(name='test_key2', value='test_valid_ext', ext='project')
+        ])
+
+        try:
+            test_meta4 = MetaData(values=[
+                project_xml.Meta(name='test_key2', value='test_invalid_ext', ext='invalid_ext')
+            ])
+            # Should not be able to get here with invalid metadata
+            self.fail('Expected ValueError')
+        except ValueError:
+            pass
```

### Comparing `rsxml-0.0.1a0/src/tests/test_timers.py` & `rsxml-2.0.0/tests/test_timers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 """
 import unittest
 import sqlite3
 import os
 from time import sleep
 from tempfile import NamedTemporaryFile
-from src.debug import TimerBuckets, Timer
-from src.debug.timer_buckets import TimerBucketsBorg
+from rsxml.debug import TimerBuckets, Timer
+from rsxml.debug.timer_buckets import TimerBucketsBorg
 
 
 class TimerTests(unittest.TestCase):
     """[summary]
 
     Args:
         unittest ([type]): [description]
```

### Comparing `rsxml-0.0.1a0/src/tests/test_util.py` & `rsxml-2.0.0/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Testing for the vector ops
 
 """
 import unittest
-from src import util
+from rsxml import util
 
 
 class UtilTest(unittest.TestCase):
     """[summary]
 
     Args:
         unittest ([type]): [description]
@@ -56,17 +56,17 @@
         self.assertEqual(util.sizeof_fmt(1000000000000000000000), '1000.0 EB')
         self.assertEqual(util.sizeof_fmt(10000000000000000000000), '10.0 ZB')
         self.assertEqual(util.sizeof_fmt(100000000000000000000000), '100.0 ZB')
 
     def test_get_obj_size(self):
 
         self.assertEqual(util.get_obj_size(None), 16)
-        self.assertEqual(util.get_obj_size(0), 24)
+        self.assertEqual(util.get_obj_size(0), 28)
         self.assertEqual(util.get_obj_size([1, 2, 3, 4]), 200)
-        self.assertEqual(util.get_obj_size({"key": "value"}), 286)
+        self.assertEqual(util.get_obj_size({"key": "value"}), 238)
 
     def test_parse_metadata(self):
         """[summary]
         """
         self.assertEqual(util.parse_metadata("key=value"), {"key": "value"})
         self.assertEqual(util.parse_metadata("key=value,key2=value2"),
                          {"key": "value", "key2": "value2"})
```

