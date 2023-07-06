# Comparing `tmp/vncdotool-1.1.0.tar.gz` & `tmp/vncdotool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vncdotool-1.1.0.tar", last modified: Sat Apr  1 18:19:25 2023, max compression
+gzip compressed data, was "vncdotool-1.2.0.tar", last modified: Thu Jul  6 17:52:12 2023, max compression
```

## Comparing `vncdotool-1.1.0.tar` & `vncdotool-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-04-01 18:19:25.678867 vncdotool-1.1.0/
--rw-r--r--   0 marcs      (501) staff       (20)     1362 2023-02-24 02:07:54.000000 vncdotool-1.1.0/LICENSE.txt
--rw-r--r--   0 marcs      (501) staff       (20)      110 2019-06-12 01:45:42.000000 vncdotool-1.1.0/MANIFEST.in
--rw-r--r--   0 marcs      (501) staff       (20)     8735 2023-04-01 18:19:25.679181 vncdotool-1.1.0/PKG-INFO
--rw-r--r--   0 marcs      (501) staff       (20)     2383 2023-01-26 13:31:57.000000 vncdotool-1.1.0/README.rst
--rw-r--r--   0 marcs      (501) staff       (20)      939 2023-01-26 13:31:57.000000 vncdotool-1.1.0/TODO.txt
--rw-r--r--   0 marcs      (501) staff       (20)       57 2023-01-26 13:31:57.000000 vncdotool-1.1.0/requirements-dev.txt
--rw-r--r--   0 marcs      (501) staff       (20)       75 2023-02-24 02:07:54.000000 vncdotool-1.1.0/requirements.txt
--rw-r--r--   0 marcs      (501) staff       (20)     1300 2023-04-01 18:19:25.681291 vncdotool-1.1.0/setup.cfg
--rw-r--r--   0 marcs      (501) staff       (20)       60 2023-01-26 13:32:52.000000 vncdotool-1.1.0/setup.py
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-04-01 18:19:25.644235 vncdotool-1.1.0/tests/
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-04-01 18:19:25.658290 vncdotool-1.1.0/tests/functional/
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-04-01 18:19:25.661514 vncdotool-1.1.0/tests/functional/data/
--rw-r--r--   0 marcs      (501) staff       (20)    15830 2019-06-12 01:45:42.000000 vncdotool-1.1.0/tests/functional/data/example.png
--rw-r--r--   0 marcs      (501) staff       (20)    14682 2019-06-12 01:45:42.000000 vncdotool-1.1.0/tests/functional/data/example_nocursor.png
--rw-r--r--   0 marcs      (501) staff       (20)      452 2019-06-12 01:45:42.000000 vncdotool-1.1.0/tests/functional/data/simple.png
--rw-r--r--   0 marcs      (501) staff       (20)     2091 2023-01-26 13:31:57.000000 vncdotool-1.1.0/tests/functional/test_proxy.py
--rw-r--r--   0 marcs      (501) staff       (20)     3333 2023-02-24 03:04:57.000000 vncdotool-1.1.0/tests/functional/test_screen.py
--rw-r--r--   0 marcs      (501) staff       (20)     2648 2023-04-01 17:36:28.000000 vncdotool-1.1.0/tests/functional/test_send_events.py
--rw-r--r--   0 marcs      (501) staff       (20)     1032 2023-01-26 13:31:57.000000 vncdotool-1.1.0/tests/functional/test_xvnc.py
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-04-01 18:19:25.664680 vncdotool-1.1.0/tests/unit/
--rw-r--r--   0 marcs      (501) staff       (20)     8045 2023-02-24 02:07:54.000000 vncdotool-1.1.0/tests/unit/test_client.py
--rw-r--r--   0 marcs      (501) staff       (20)     8635 2023-01-26 13:31:57.000000 vncdotool-1.1.0/tests/unit/test_command.py
--rw-r--r--   0 marcs      (501) staff       (20)     2541 2023-02-24 02:07:54.000000 vncdotool-1.1.0/tests/unit/test_rfb.py
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-04-01 18:19:25.671769 vncdotool-1.1.0/vncdotool/
--rw-r--r--   0 marcs      (501) staff       (20)       22 2023-01-26 13:31:57.000000 vncdotool-1.1.0/vncdotool/__init__.py
--rw-r--r--   0 marcs      (501) staff       (20)     5551 2023-02-24 02:07:54.000000 vncdotool-1.1.0/vncdotool/api.py
--rw-r--r--   0 marcs      (501) staff       (20)    17398 2023-02-24 02:07:54.000000 vncdotool-1.1.0/vncdotool/client.py
--rw-r--r--   0 marcs      (501) staff       (20)    16301 2023-02-24 03:07:52.000000 vncdotool-1.1.0/vncdotool/command.py
--rw-r--r--   0 marcs      (501) staff       (20)    11428 2023-02-24 02:07:54.000000 vncdotool-1.1.0/vncdotool/loggingproxy.py
--rw-r--r--   0 marcs      (501) staff       (20)    45978 2023-02-24 02:07:54.000000 vncdotool-1.1.0/vncdotool/rfb.py
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-04-01 18:19:25.678176 vncdotool-1.1.0/vncdotool.egg-info/
--rw-r--r--   0 marcs      (501) staff       (20)     8735 2023-04-01 18:19:25.000000 vncdotool-1.1.0/vncdotool.egg-info/PKG-INFO
--rw-r--r--   0 marcs      (501) staff       (20)      767 2023-04-01 18:19:25.000000 vncdotool-1.1.0/vncdotool.egg-info/SOURCES.txt
--rw-r--r--   0 marcs      (501) staff       (20)        1 2023-04-01 18:19:25.000000 vncdotool-1.1.0/vncdotool.egg-info/dependency_links.txt
--rw-r--r--   0 marcs      (501) staff       (20)      120 2023-04-01 18:19:25.000000 vncdotool-1.1.0/vncdotool.egg-info/entry_points.txt
--rw-r--r--   0 marcs      (501) staff       (20)       29 2023-04-01 18:19:25.000000 vncdotool-1.1.0/vncdotool.egg-info/requires.txt
--rw-r--r--   0 marcs      (501) staff       (20)       10 2023-04-01 18:19:25.000000 vncdotool-1.1.0/vncdotool.egg-info/top_level.txt
--rw-r--r--   0 marcs      (501) staff       (20)        1 2023-04-01 18:19:25.000000 vncdotool-1.1.0/vncdotool.egg-info/zip-safe
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-07-06 17:52:12.001676 vncdotool-1.2.0/
+-rw-r--r--   0 marcs      (501) staff       (20)     1362 2023-02-24 02:07:54.000000 vncdotool-1.2.0/LICENSE.txt
+-rw-r--r--   0 marcs      (501) staff       (20)      110 2019-06-12 01:45:42.000000 vncdotool-1.2.0/MANIFEST.in
+-rw-r--r--   0 marcs      (501) staff       (20)     9648 2023-07-06 17:52:12.002302 vncdotool-1.2.0/PKG-INFO
+-rw-r--r--   0 marcs      (501) staff       (20)     3188 2023-07-06 17:48:56.000000 vncdotool-1.2.0/README.rst
+-rw-r--r--   0 marcs      (501) staff       (20)      939 2023-01-26 13:31:57.000000 vncdotool-1.2.0/TODO.txt
+-rw-r--r--   0 marcs      (501) staff       (20)       63 2023-04-22 11:00:45.000000 vncdotool-1.2.0/requirements-dev.txt
+-rw-r--r--   0 marcs      (501) staff       (20)       75 2023-02-24 02:07:54.000000 vncdotool-1.2.0/requirements.txt
+-rw-r--r--   0 marcs      (501) staff       (20)     1300 2023-07-06 17:52:12.003599 vncdotool-1.2.0/setup.cfg
+-rw-r--r--   0 marcs      (501) staff       (20)       60 2023-01-26 13:32:52.000000 vncdotool-1.2.0/setup.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-07-06 17:52:11.948244 vncdotool-1.2.0/tests/
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-07-06 17:52:11.967098 vncdotool-1.2.0/tests/functional/
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-07-06 17:52:11.969782 vncdotool-1.2.0/tests/functional/data/
+-rw-r--r--   0 marcs      (501) staff       (20)    15830 2019-06-12 01:45:42.000000 vncdotool-1.2.0/tests/functional/data/example.png
+-rw-r--r--   0 marcs      (501) staff       (20)    14682 2019-06-12 01:45:42.000000 vncdotool-1.2.0/tests/functional/data/example_nocursor.png
+-rw-r--r--   0 marcs      (501) staff       (20)      452 2019-06-12 01:45:42.000000 vncdotool-1.2.0/tests/functional/data/simple.png
+-rw-r--r--   0 marcs      (501) staff       (20)     2091 2023-01-26 13:31:57.000000 vncdotool-1.2.0/tests/functional/test_proxy.py
+-rw-r--r--   0 marcs      (501) staff       (20)     3333 2023-02-24 03:04:57.000000 vncdotool-1.2.0/tests/functional/test_screen.py
+-rw-r--r--   0 marcs      (501) staff       (20)     2648 2023-04-01 17:36:28.000000 vncdotool-1.2.0/tests/functional/test_send_events.py
+-rw-r--r--   0 marcs      (501) staff       (20)     1032 2023-01-26 13:31:57.000000 vncdotool-1.2.0/tests/functional/test_xvnc.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-07-06 17:52:11.972533 vncdotool-1.2.0/tests/unit/
+-rw-r--r--   0 marcs      (501) staff       (20)     8045 2023-02-24 02:07:54.000000 vncdotool-1.2.0/tests/unit/test_client.py
+-rw-r--r--   0 marcs      (501) staff       (20)     8635 2023-01-26 13:31:57.000000 vncdotool-1.2.0/tests/unit/test_command.py
+-rw-r--r--   0 marcs      (501) staff       (20)     2541 2023-02-24 02:07:54.000000 vncdotool-1.2.0/tests/unit/test_rfb.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-07-06 17:52:11.992319 vncdotool-1.2.0/vncdotool/
+-rw-r--r--   0 marcs      (501) staff       (20)       22 2023-07-06 17:44:41.000000 vncdotool-1.2.0/vncdotool/__init__.py
+-rw-r--r--   0 marcs      (501) staff       (20)     6238 2023-04-28 23:25:06.000000 vncdotool-1.2.0/vncdotool/api.py
+-rw-r--r--   0 marcs      (501) staff       (20)    17592 2023-04-28 23:25:06.000000 vncdotool-1.2.0/vncdotool/client.py
+-rw-r--r--   0 marcs      (501) staff       (20)    16392 2023-04-28 23:25:06.000000 vncdotool-1.2.0/vncdotool/command.py
+-rw-r--r--   0 marcs      (501) staff       (20)    11443 2023-04-28 23:25:06.000000 vncdotool-1.2.0/vncdotool/loggingproxy.py
+-rw-r--r--   0 marcs      (501) staff       (20)    47335 2023-04-28 23:25:06.000000 vncdotool-1.2.0/vncdotool/rfb.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-07-06 17:52:12.000968 vncdotool-1.2.0/vncdotool.egg-info/
+-rw-r--r--   0 marcs      (501) staff       (20)     9648 2023-07-06 17:52:11.000000 vncdotool-1.2.0/vncdotool.egg-info/PKG-INFO
+-rw-r--r--   0 marcs      (501) staff       (20)      767 2023-07-06 17:52:11.000000 vncdotool-1.2.0/vncdotool.egg-info/SOURCES.txt
+-rw-r--r--   0 marcs      (501) staff       (20)        1 2023-07-06 17:52:11.000000 vncdotool-1.2.0/vncdotool.egg-info/dependency_links.txt
+-rw-r--r--   0 marcs      (501) staff       (20)      120 2023-07-06 17:52:11.000000 vncdotool-1.2.0/vncdotool.egg-info/entry_points.txt
+-rw-r--r--   0 marcs      (501) staff       (20)       29 2023-07-06 17:52:11.000000 vncdotool-1.2.0/vncdotool.egg-info/requires.txt
+-rw-r--r--   0 marcs      (501) staff       (20)       10 2023-07-06 17:52:11.000000 vncdotool-1.2.0/vncdotool.egg-info/top_level.txt
+-rw-r--r--   0 marcs      (501) staff       (20)        1 2023-04-01 18:19:25.000000 vncdotool-1.2.0/vncdotool.egg-info/zip-safe
```

### Comparing `vncdotool-1.1.0/LICENSE.txt` & `vncdotool-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/PKG-INFO` & `vncdotool-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vncdotool
-Version: 1.1.0
+Version: 1.2.0
 Summary: Command line VNC client
 Home-page: http://github.com/sibson/vncdotool
 Author: Marc Sibson
 Author-email: sibson+vncdotool@gmail.com
 License: MIT License
 Keywords: VNC,RFB
 Classifier: Development Status :: 4 - Beta
@@ -22,15 +22,39 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE.txt
 
-.. image:: https://img.shields.io/pypi/v/vncdotool   :alt: PyPI
+.. image:: https://img.shields.io/pypi/pyversions/vncdotool.svg
+   :target: https://pypi.python.org/pypi/vncdotool
+   :alt: Python Versions
+
+.. image:: https://img.shields.io/pypi/v/vncdotool
+    :target: https://pypi.org/project/vncdotool/
+    :alt: PyPi Package
+
+.. image:: https://img.shields.io/pypi/pyversions/vncdotool.svg
+   :target: https://pypi.python.org/pypi/vncdotool
+   :alt: Python Versions
+
+.. image:: https://github.com/sibson/vncdotool/workflows/VNCDo%20CI/badge.svg
+   :target: https://github.com/sibson/vndotool/actions
+   :alt: Actions Status
+
+.. image:: https://readthedocs.org/projects/vncdotool/badge/?version=latest&style=flat
+   :target: https://vncdotool.readthedocs.io/en/latest/
+   :alt: ReadTheDocs
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+
+
 
 vncdotool
 ===========
 vncdotool is a command line VNC client.
 It can be useful to automating interactions with virtual machines or
 hardware devices that are otherwise difficult to control.
 
@@ -90,15 +114,19 @@
 
 .. _Read The Docs: http://vncdotool.readthedocs.org
 .. _GitHub: http://github.com/sibson/vncdotool
 .. _TigerVNC: http://sourceforge.net/apps/mediawiki/tigervnc/index.php?title=Main_Page
 .. _python-vnc-viewer: http://code.google.com/p/python-vnc-viewer
 .. _Stackoverflow: https://stackoverflow.com/questions/ask?tags=vncdotool
 
-1.1.0 (unreleased)
+1.2.0 (2023-06-06)
+----------------------
+  - fixes for api.shutdown and disconnect raise exceptions, #256
+
+1.1.0 (2023-04-01)
 ----------------------
 Huge thanks to @pmhahn for single handedly driving conversion to modern Python3, as well
 as cleaning up a ton of outstanding issues.
 
   - [BREAKING] drop python 2.x support, thanks @pmhahn
   - Use built-in Unittest and mock for testing
   - PEP-484 type hinting, thanks @pmhahn
```

### Comparing `vncdotool-1.1.0/README.rst` & `vncdotool-1.2.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,32 @@
-.. image:: https://img.shields.io/pypi/v/vncdotool   :alt: PyPI
+.. image:: https://img.shields.io/pypi/pyversions/vncdotool.svg
+   :target: https://pypi.python.org/pypi/vncdotool
+   :alt: Python Versions
+
+.. image:: https://img.shields.io/pypi/v/vncdotool
+    :target: https://pypi.org/project/vncdotool/
+    :alt: PyPi Package
+
+.. image:: https://img.shields.io/pypi/pyversions/vncdotool.svg
+   :target: https://pypi.python.org/pypi/vncdotool
+   :alt: Python Versions
+
+.. image:: https://github.com/sibson/vncdotool/workflows/VNCDo%20CI/badge.svg
+   :target: https://github.com/sibson/vndotool/actions
+   :alt: Actions Status
+
+.. image:: https://readthedocs.org/projects/vncdotool/badge/?version=latest&style=flat
+   :target: https://vncdotool.readthedocs.io/en/latest/
+   :alt: ReadTheDocs
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+
+
 
 vncdotool
 ===========
 vncdotool is a command line VNC client.
 It can be useful to automating interactions with virtual machines or
 hardware devices that are otherwise difficult to control.
```

### Comparing `vncdotool-1.1.0/TODO.txt` & `vncdotool-1.2.0/TODO.txt`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/setup.cfg` & `vncdotool-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/functional/data/example.png` & `vncdotool-1.2.0/tests/functional/data/example.png`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/functional/data/example_nocursor.png` & `vncdotool-1.2.0/tests/functional/data/example_nocursor.png`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/functional/test_proxy.py` & `vncdotool-1.2.0/tests/functional/test_proxy.py`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/functional/test_screen.py` & `vncdotool-1.2.0/tests/functional/test_screen.py`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/functional/test_send_events.py` & `vncdotool-1.2.0/tests/functional/test_send_events.py`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/functional/test_xvnc.py` & `vncdotool-1.2.0/tests/functional/test_xvnc.py`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/unit/test_client.py` & `vncdotool-1.2.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/unit/test_command.py` & `vncdotool-1.2.0/tests/unit/test_command.py`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/tests/unit/test_rfb.py` & `vncdotool-1.2.0/tests/unit/test_rfb.py`

 * *Files identical despite different names*

### Comparing `vncdotool-1.1.0/vncdotool/client.py` & `vncdotool-1.2.0/vncdotool/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,94 +25,90 @@
 TClient = TypeVar("TClient", bound="VNCDoToolClient")
 TFile = Union[str, Path, IO[bytes]]
 
 log = logging.getLogger(__name__)
 
 
 KEYMAP = {
-    'bsp': rfb.KEY_BackSpace,
-    'tab': rfb.KEY_Tab,
-    'return': rfb.KEY_Return,
-    'enter': rfb.KEY_Return,
-    'esc': rfb.KEY_Escape,
-    'ins': rfb.KEY_Insert,
-    'delete': rfb.KEY_Delete,
-    'del': rfb.KEY_Delete,
-    'home': rfb.KEY_Home,
-    'end': rfb.KEY_End,
-    'pgup': rfb.KEY_PageUp,
-    'pgdn': rfb.KEY_PageDown,
-    'left': rfb.KEY_Left,
-    'up': rfb.KEY_Up,
-    'right': rfb.KEY_Right,
-    'down': rfb.KEY_Down,
-
-    'slash': rfb.KEY_BackSlash,
-    'bslash': rfb.KEY_BackSlash,
-    'fslash': rfb.KEY_ForwardSlash,
-    'spacebar': rfb.KEY_SpaceBar,
-    'space': rfb.KEY_SpaceBar,
-    'sb': rfb.KEY_SpaceBar,
-
-    'f1': rfb.KEY_F1,
-    'f2': rfb.KEY_F2,
-    'f3': rfb.KEY_F3,
-    'f4': rfb.KEY_F4,
-    'f5': rfb.KEY_F5,
-    'f6': rfb.KEY_F6,
-    'f7': rfb.KEY_F7,
-    'f8': rfb.KEY_F8,
-    'f9': rfb.KEY_F9,
-    'f10': rfb.KEY_F10,
-    'f11': rfb.KEY_F11,
-    'f12': rfb.KEY_F12,
-    'f13': rfb.KEY_F13,
-    'f14': rfb.KEY_F14,
-    'f15': rfb.KEY_F15,
-    'f16': rfb.KEY_F16,
-    'f17': rfb.KEY_F17,
-    'f18': rfb.KEY_F18,
-    'f19': rfb.KEY_F19,
-    'f20': rfb.KEY_F20,
-
-    'lshift': rfb.KEY_ShiftLeft,
-    'shift': rfb.KEY_ShiftLeft,
-    'rshift': rfb.KEY_ShiftRight,
-    'lctrl': rfb.KEY_ControlLeft,
-    'ctrl': rfb.KEY_ControlLeft,
-    'rctrl': rfb.KEY_ControlRight,
-    'lmeta': rfb.KEY_MetaLeft,
-    'meta': rfb.KEY_MetaLeft,
-    'rmeta': rfb.KEY_MetaRight,
-    'lalt': rfb.KEY_AltLeft,
-    'alt': rfb.KEY_AltLeft,
-    'ralt': rfb.KEY_AltRight,
-    'scrlk': rfb.KEY_Scroll_Lock,
-    'sysrq': rfb.KEY_Sys_Req,
-    'numlk': rfb.KEY_Num_Lock,
-    'caplk': rfb.KEY_Caps_Lock,
-    'pause': rfb.KEY_Pause,
-    'lsuper': rfb.KEY_Super_L,
-    'super': rfb.KEY_Super_L,
-    'rsuper': rfb.KEY_Super_R,
-    'lhyper': rfb.KEY_Hyper_L,
-    'hyper': rfb.KEY_Hyper_L,
-    'rhyper': rfb.KEY_Hyper_R,
-
-    'kp0': rfb.KEY_KP_0,
-    'kp1': rfb.KEY_KP_1,
-    'kp2': rfb.KEY_KP_2,
-    'kp3': rfb.KEY_KP_3,
-    'kp4': rfb.KEY_KP_4,
-    'kp5': rfb.KEY_KP_5,
-    'kp6': rfb.KEY_KP_6,
-    'kp7': rfb.KEY_KP_7,
-    'kp8': rfb.KEY_KP_8,
-    'kp9': rfb.KEY_KP_9,
-    'kpenter': rfb.KEY_KP_Enter,
+    "bsp": rfb.KEY_BackSpace,
+    "tab": rfb.KEY_Tab,
+    "return": rfb.KEY_Return,
+    "enter": rfb.KEY_Return,
+    "esc": rfb.KEY_Escape,
+    "ins": rfb.KEY_Insert,
+    "delete": rfb.KEY_Delete,
+    "del": rfb.KEY_Delete,
+    "home": rfb.KEY_Home,
+    "end": rfb.KEY_End,
+    "pgup": rfb.KEY_PageUp,
+    "pgdn": rfb.KEY_PageDown,
+    "left": rfb.KEY_Left,
+    "up": rfb.KEY_Up,
+    "right": rfb.KEY_Right,
+    "down": rfb.KEY_Down,
+    "slash": rfb.KEY_BackSlash,
+    "bslash": rfb.KEY_BackSlash,
+    "fslash": rfb.KEY_ForwardSlash,
+    "spacebar": rfb.KEY_SpaceBar,
+    "space": rfb.KEY_SpaceBar,
+    "sb": rfb.KEY_SpaceBar,
+    "f1": rfb.KEY_F1,
+    "f2": rfb.KEY_F2,
+    "f3": rfb.KEY_F3,
+    "f4": rfb.KEY_F4,
+    "f5": rfb.KEY_F5,
+    "f6": rfb.KEY_F6,
+    "f7": rfb.KEY_F7,
+    "f8": rfb.KEY_F8,
+    "f9": rfb.KEY_F9,
+    "f10": rfb.KEY_F10,
+    "f11": rfb.KEY_F11,
+    "f12": rfb.KEY_F12,
+    "f13": rfb.KEY_F13,
+    "f14": rfb.KEY_F14,
+    "f15": rfb.KEY_F15,
+    "f16": rfb.KEY_F16,
+    "f17": rfb.KEY_F17,
+    "f18": rfb.KEY_F18,
+    "f19": rfb.KEY_F19,
+    "f20": rfb.KEY_F20,
+    "lshift": rfb.KEY_ShiftLeft,
+    "shift": rfb.KEY_ShiftLeft,
+    "rshift": rfb.KEY_ShiftRight,
+    "lctrl": rfb.KEY_ControlLeft,
+    "ctrl": rfb.KEY_ControlLeft,
+    "rctrl": rfb.KEY_ControlRight,
+    "lmeta": rfb.KEY_MetaLeft,
+    "meta": rfb.KEY_MetaLeft,
+    "rmeta": rfb.KEY_MetaRight,
+    "lalt": rfb.KEY_AltLeft,
+    "alt": rfb.KEY_AltLeft,
+    "ralt": rfb.KEY_AltRight,
+    "scrlk": rfb.KEY_Scroll_Lock,
+    "sysrq": rfb.KEY_Sys_Req,
+    "numlk": rfb.KEY_Num_Lock,
+    "caplk": rfb.KEY_Caps_Lock,
+    "pause": rfb.KEY_Pause,
+    "lsuper": rfb.KEY_Super_L,
+    "super": rfb.KEY_Super_L,
+    "rsuper": rfb.KEY_Super_R,
+    "lhyper": rfb.KEY_Hyper_L,
+    "hyper": rfb.KEY_Hyper_L,
+    "rhyper": rfb.KEY_Hyper_R,
+    "kp0": rfb.KEY_KP_0,
+    "kp1": rfb.KEY_KP_1,
+    "kp2": rfb.KEY_KP_2,
+    "kp3": rfb.KEY_KP_3,
+    "kp4": rfb.KEY_KP_4,
+    "kp5": rfb.KEY_KP_5,
+    "kp6": rfb.KEY_KP_6,
+    "kp7": rfb.KEY_KP_7,
+    "kp8": rfb.KEY_KP_8,
+    "kp9": rfb.KEY_KP_9,
+    "kpenter": rfb.KEY_KP_Enter,
 }
 
 # Enable using vncdotool without PIL. Of course capture and expect
 # won't work but at least we can still offer key, type, press and
 # move.
 try:
     from PIL import Image
@@ -128,16 +124,20 @@
         def __getattr__(self, _: str) -> Any:
             raise ImportError("PIL")
 
     Image = _RuntimeImportError()  # type: ignore[assignment]
     PIL = _RuntimeImportError()
 
 
-class AuthenticationError(Exception):
-    """ VNC Server requires Authentication """
+class VNCDoException(Exception):
+    pass
+
+
+class AuthenticationError(VNCDoException):
+    """VNC Server requires Authentication"""
 
 
 RGB32 = rfb.PixelFormat(32, 24, False, True, 255, 255, 255, 0, 8, 16)
 RGB24 = rfb.PixelFormat(24, 24, False, True, 255, 255, 255, 0, 8, 16)
 BGR16 = rfb.PixelFormat(16, 16, False, True, 31, 63, 31, 11, 5, 0)
 PF2IM = {
     RGB24: "RGB",
@@ -156,15 +156,15 @@
     screen: Optional[Image.Image] = None
     image_mode = PF2IM[rfb.PixelFormat()]
     deferred: Optional[Deferred] = None
 
     cursor: Optional[Image.Image] = None
     cmask: Optional[Image.Image] = None
 
-    SPECIAL_KEYS_US = "~!@#$%^&*()_+{}|:\"<>?"
+    SPECIAL_KEYS_US = '~!@#$%^&*()_+{}|:"<>?'
     MAX_DESKTOP_SIZE = 0x10000
 
     def connectionMade(self) -> None:
         super().connectionMade()
 
         if isinstance(self.transport, ITCPTransport):
             self.transport.setTcpNoDelay(True)
@@ -172,144 +172,148 @@
     def connectionLost(self, reason: Failure) -> None:
         super().connectionLost(reason)
         self.factory.clientConnectionLost(self, reason)
 
     def _decodeKey(self, key: str) -> List[int]:
         if self.factory.force_caps:
             if key.isupper() or key in self.SPECIAL_KEYS_US:
-                key = 'shift-%c' % key
+                key = "shift-%c" % key
 
         if len(key) == 1:
             keys = [key]
         else:
-            keys = key.split('-')
+            keys = key.split("-")
 
         return [KEYMAP.get(k) or ord(k) for k in keys]
 
     def pause(self, duration: float) -> Deferred:
         d = Deferred()
         reactor.callLater(duration, d.callback, self)
         return d
 
     def keyPress(self: TClient, key: str) -> TClient:
-        """ Send a key press to the server
+        """Send a key press to the server
 
-            key: string: either [a-z] or a from KEYMAP
+        key: string: either [a-z] or a from KEYMAP
         """
-        log.debug('keyPress %s', key)
+        log.debug("keyPress %s", key)
         self.keyDown(key)
         self.keyUp(key)
 
         return self
 
     def keyDown(self: TClient, key: str) -> TClient:
-        log.debug('keyDown %s', key)
+        log.debug("keyDown %s", key)
         keys = self._decodeKey(key)
         for k in keys:
             self.keyEvent(k, down=True)
 
         return self
 
     def keyUp(self: TClient, key: str) -> TClient:
-        log.debug('keyUp %s', key)
+        log.debug("keyUp %s", key)
         keys = self._decodeKey(key)
         for k in keys:
             self.keyEvent(k, down=False)
 
         return self
 
     def mousePress(self: TClient, button: int) -> TClient:
-        """ Send a mouse click at the last set position
+        """Send a mouse click at the last set position
 
-            button: int: [1-n]
+        button: int: [1-n]
 
         """
-        log.debug('mousePress %s', button)
+        log.debug("mousePress %s", button)
         self.mouseDown(button)
         self.mouseUp(button)
 
         return self
 
     def mouseDown(self: TClient, button: int) -> TClient:
-        """ Send a mouse button down at the last set position
+        """Send a mouse button down at the last set position
 
-            button: int: [1-n]
+        button: int: [1-n]
 
         """
-        log.debug('mouseDown %s', button)
+        log.debug("mouseDown %s", button)
         self.buttons |= 1 << (button - 1)
         self.pointerEvent(self.x, self.y, buttonmask=self.buttons)
 
         return self
 
     def mouseUp(self: TClient, button: int) -> TClient:
-        """ Send mouse button released at the last set position
+        """Send mouse button released at the last set position
 
-            button: int: [1-n]
+        button: int: [1-n]
 
         """
-        log.debug('mouseUp %s', button)
+        log.debug("mouseUp %s", button)
         self.buttons &= ~(1 << (button - 1))
         self.pointerEvent(self.x, self.y, buttonmask=self.buttons)
 
         return self
 
     def captureScreen(self, fp: TFile, incremental: bool = False) -> Deferred:
-        """ Save the current display to filename
-        """
-        log.debug('captureScreen %s', fp)
+        """Save the current display to filename"""
+        log.debug("captureScreen %s", fp)
         return self._capture(fp, incremental)
 
-    def captureRegion(self, fp: TFile, x: int, y: int, w: int, h: int, incremental: bool = False) -> Deferred:
-        """ Save a region of the current display to filename
-        """
-        log.debug('captureRegion %s', fp)
+    def captureRegion(
+        self, fp: TFile, x: int, y: int, w: int, h: int, incremental: bool = False
+    ) -> Deferred:
+        """Save a region of the current display to filename"""
+        log.debug("captureRegion %s", fp)
         return self._capture(fp, incremental, x, y, x + w, y + h)
 
     def refreshScreen(self, incremental: bool = False) -> Deferred:
         d = self.deferred = Deferred()
         self.framebufferUpdateRequest(incremental=incremental)
         return d
 
     def _capture(self, fp: TFile, incremental: bool, *args: int) -> Deferred:
         d = self.refreshScreen(incremental)
         d.addCallback(self._captureSave, fp, *args)
         return d
 
     def _captureSave(self: TClient, data: object, fp: TFile, *args: int) -> TClient:
-        log.debug('captureSave %s', fp)
+        log.debug("captureSave %s", fp)
         assert self.screen is not None
         if args:
             capture = self.screen.crop(args)  # type: ignore[arg-type]
         else:
             capture = self.screen
         capture.save(fp)
 
         return self
 
     def expectScreen(self, filename: str, maxrms: float = 0) -> Deferred:
-        """ Wait until the display matches a target image
+        """Wait until the display matches a target image
 
-            filename: an image file to read and compare against
-            maxrms: the maximum root mean square between histograms of the
-                    screen and target image
+        filename: an image file to read and compare against
+        maxrms: the maximum root mean square between histograms of the
+                screen and target image
         """
-        log.debug('expectScreen %s', filename)
+        log.debug("expectScreen %s", filename)
         return self._expectFramebuffer(filename, 0, 0, maxrms)
 
-    def expectRegion(self, filename: str, x: int, y: int, maxrms: float = 0) -> Deferred:
-        """ Wait until a portion of the screen matches the target image
+    def expectRegion(
+        self, filename: str, x: int, y: int, maxrms: float = 0
+    ) -> Deferred:
+        """Wait until a portion of the screen matches the target image
 
-            The region compared is defined by the box
-            (x, y), (x + image.width, y + image.height)
+        The region compared is defined by the box
+        (x, y), (x + image.width, y + image.height)
         """
-        log.debug('expectRegion %s (%s, %s)', filename, x, y)
+        log.debug("expectRegion %s (%s, %s)", filename, x, y)
         return self._expectFramebuffer(filename, x, y, maxrms)
 
-    def _expectFramebuffer(self, filename: str, x: int, y: int, maxrms: float) -> Deferred:
+    def _expectFramebuffer(
+        self, filename: str, x: int, y: int, maxrms: float
+    ) -> Deferred:
         image = Image.open(filename)
         w, h = image.size
         self.expected = image.histogram()
 
         return self._expectCompare(None, (x, y, x + w, y + h), maxrms)
 
     def _expectCompare(self, data: object, box: rfb.Rect, maxrms: float) -> Deferred:
@@ -319,63 +323,62 @@
             image = self.screen.crop(box)
 
             hist = image.histogram()
             if len(hist) == len(self.expected):
                 sum_ = sum((h - e) ** 2 for h, e in zip(hist, self.expected))
                 rms = math.sqrt(sum_ / len(hist))
 
-                log.debug('rms:%f maxrms:%f', rms, maxrms)
+                log.debug("rms:%f maxrms:%f", rms, maxrms)
                 if rms <= maxrms:
                     return self
 
         self.deferred = Deferred()
         self.deferred.addCallback(self._expectCompare, box, maxrms)
-        self.framebufferUpdateRequest(incremental=incremental)  # use box ~(x, y, w - x, h - y)?
+        self.framebufferUpdateRequest(
+            incremental=incremental
+        )  # use box ~(x, y, w - x, h - y)?
 
         return self.deferred
 
     def mouseMove(self: TClient, x: int, y: int) -> TClient:
-        """ Move the mouse pointer to position (x, y)
-        """
-        log.debug('mouseMove %d,%d', x, y)
+        """Move the mouse pointer to position (x, y)"""
+        log.debug("mouseMove %d,%d", x, y)
         self.x, self.y = x, y
         self.pointerEvent(x, y, self.buttons)
         return self
 
     def mouseDrag(self: TClient, x: int, y: int, step: int = 1) -> TClient:
-        """ Move the mouse point to position (x, y) in increments of step
-        """
-        log.debug('mouseDrag %d,%d', x, y)
+        """Move the mouse point to position (x, y) in increments of step"""
+        log.debug("mouseDrag %d,%d", x, y)
         if x < self.x:
             xsteps = range(self.x - step, x, -step)
         else:
             xsteps = range(self.x + step, x, step)
 
         if y < self.y:
             ysteps = range(self.y - step, y, -step)
         else:
             ysteps = range(self.y + step, y, step)
 
         for ypos in ysteps:
             self.mouseMove(self.x, ypos)
             reactor.doPoll(timeout=5)
-            time.sleep(.2)
+            time.sleep(0.2)
 
         for xpos in xsteps:
             self.mouseMove(xpos, self.y)
             reactor.doPoll(timeout=5)
-            time.sleep(.2)
+            time.sleep(0.2)
 
         self.mouseMove(x, y)
 
         return self
 
     def setImageMode(self) -> None:
-        """ Check support for PixelFormats announced by server or select client supported alternative.
-        """
+        """Check support for PixelFormats announced by server or select client supported alternative."""
         try:
             self.image_mode = PF2IM[self.pixel_format]
         except LookupError:
             if self._version_server == (3, 889):  # Apple Remote Desktop
                 pixel_format = BGR16
             else:
                 pixel_format = RGB32
@@ -385,15 +388,17 @@
 
     #
     # base customizations
     #
     def vncRequestPassword(self) -> None:
         if self.factory.password is None:
             self.transport.loseConnection()
-            self.factory.clientConnectionFailed(self, AuthenticationError('password required, but none provided'))
+            self.factory.clientConnectionFailed(
+                self, AuthenticationError("password required, but none provided")
+            )
             return
         self.sendPassword(self.factory.password)
 
     def vncConnectionMade(self) -> None:
         self.setImageMode()
         encodings = [self.encoding]
         if self.factory.pseudocursor or self.factory.nocursor:
@@ -404,37 +409,42 @@
             encodings.append(rfb.Encoding.PSEUDO_LAST_RECT)
         if self.factory.qemu_extended_key:
             encodings.append(rfb.Encoding.PSEUDO_QEMU_EXTENDED_KEY_EVENT)
         self.setEncodings(encodings)
         self.factory.clientConnectionMade(self)
 
     def bell(self) -> None:
-        log.info('ding')
+        log.info("ding")
 
     def copy_text(self, text: str) -> None:
-        log.info(f'clipboard copy {text!r}')
+        log.info(f"clipboard copy {text!r}")
 
     def paste(self: TClient, message: str) -> TClient:
         self.clientCutText(message)
         return self
 
-    def updateRectangle(self, x: int, y: int, width: int, height: int, data: bytes) -> None:
+    def updateRectangle(
+        self, x: int, y: int, width: int, height: int, data: bytes
+    ) -> None:
         # ignore empty updates
         if not data:
             return
 
         size = (width, height)
-        update = Image.frombytes('RGB', size, data, 'raw', self.image_mode)
+        update = Image.frombytes("RGB", size, data, "raw", self.image_mode)
         if not self.screen:
             self.screen = update
         # track upward screen resizes, often occurs during os boot of VMs
         # When the screen is sent in chunks (as observed on VMWare ESXi), the canvas
         # needs to be resized to fit all existing contents and the update.
         elif self.screen.size[0] < (x + width) or self.screen.size[1] < (y + height):
-            new_size = (max(x + width, self.screen.size[0]), max(y + height, self.screen.size[1]))
+            new_size = (
+                max(x + width, self.screen.size[0]),
+                max(y + height, self.screen.size[1]),
+            )
             new_screen = Image.new("RGB", new_size, "black")
             new_screen.paste(self.screen, (0, 0))
             new_screen.paste(update, (x, y))
             self.screen = new_screen
         else:
             self.screen.paste(update, (x, y))
 
@@ -442,23 +452,27 @@
 
     def commitUpdate(self, rectangles: Optional[List[rfb.Rect]] = None) -> None:
         if self.deferred:
             d = self.deferred
             self.deferred = None
             d.callback(self)
 
-    def updateCursor(self, x: int, y: int, width: int, height: int, image: bytes, mask: bytes) -> None:
+    def updateCursor(
+        self, x: int, y: int, width: int, height: int, image: bytes, mask: bytes
+    ) -> None:
         if self.factory.nocursor:
             return
 
         if not width or not height:
             self.cursor = None
 
-        self.cursor = Image.frombytes('RGB', (width, height), image, "raw", self.image_mode)
-        self.cmask = Image.frombytes('1', (width, height), mask)
+        self.cursor = Image.frombytes(
+            "RGB", (width, height), image, "raw", self.image_mode
+        )
+        self.cmask = Image.frombytes("1", (width, height), mask)
         self.cfocus = x, y
         self.drawCursor()
 
     def drawCursor(self) -> None:
         if not self.cursor:
             return
 
@@ -466,15 +480,17 @@
             return
 
         x = self.x - self.cfocus[0]
         y = self.y - self.cfocus[1]
         self.screen.paste(self.cursor, (x, y), self.cmask)
 
     def updateDesktopSize(self, width: int, height: int) -> None:
-        if not (0 <= width < self.MAX_DESKTOP_SIZE and 0 <= height < self.MAX_DESKTOP_SIZE):
+        if not (
+            0 <= width < self.MAX_DESKTOP_SIZE and 0 <= height < self.MAX_DESKTOP_SIZE
+        ):
             raise ValueError((width, height))
         new_screen = Image.new("RGB", (width, height), "black")
         if self.screen:
             new_screen.paste(self.screen, (0, 0))
         self.screen = new_screen
 
 
@@ -492,15 +508,19 @@
         # pixel-data
     )
 
     def dataReceived(self, data: bytes) -> None:
         # BUG: TCP is a *stream* orianted protocol with no *framing*.
         # Therefore there is no guarantee that these 20 bytes will arrive in one single chunk.
         # This might also match inside any other sequence if fragmentation by chance puts it at be start of a new packet.
-        if len(data) == 20 and data[0] == self.SINGLE_PIXEL_UPDATE[0] and data[2:16] == self.SINGLE_PIXEL_UPDATE[2:16]:
+        if (
+            len(data) == 20
+            and data[0] == self.SINGLE_PIXEL_UPDATE[0]
+            and data[2:16] == self.SINGLE_PIXEL_UPDATE[2:16]
+        ):
             self.framebufferUpdateRequest()
             self._handler()
         else:
             super().dataReceived(data)
 
 
 class VNCDoToolFactory(rfb.RFBFactory):
@@ -517,28 +537,30 @@
     last_rect = True
     force_caps = False
 
     def __init__(self) -> None:
         self.deferred = Deferred()
 
     def clientConnectionLost(self, connector: IConnector, reason: Failure) -> None:
-        self.deferred.errback(reason)
+        pass
 
     def clientConnectionFailed(self, connector: IConnector, reason: Failure) -> None:
         self.deferred.errback(reason)
 
     def clientConnectionMade(self, protocol: VNCDoToolClient) -> None:
         self.deferred.callback(protocol)
 
 
 class VMWareFactory(VNCDoToolFactory):
     protocol = VMWareClient
 
 
-def factory_connect(factory: VNCDoToolFactory, host: str, port: int, family: socket.AddressFamily) -> None:
+def factory_connect(
+    factory: VNCDoToolFactory, host: str, port: int, family: socket.AddressFamily
+) -> None:
     if family in {socket.AF_UNSPEC, socket.AF_INET, socket.AF_INET6}:
         ep = HostnameEndpoint(reactor, host, port)
     elif hasattr(socket, "AF_UNIX") and family == socket.AF_UNIX:
         ep = UNIXClientEndpoint(reactor, host)
     else:
         raise ValueError(family)
```

### Comparing `vncdotool-1.1.0/vncdotool/command.py` & `vncdotool-1.2.0/vncdotool/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,34 +26,36 @@
 from twisted.python.log import PythonLoggingObserver
 
 from .client import TClient, VNCDoToolClient, VNCDoToolFactory, factory_connect
 from .loggingproxy import VNCLoggingServerFactory
 
 log = logging.getLogger()
 
-SUPPORTED_FORMATS = ('png', 'jpg', 'jpeg', 'gif', 'bmp')
+SUPPORTED_FORMATS = ("png", "jpg", "jpeg", "gif", "bmp")
 
 
 class TimeoutError(RuntimeError):
     pass
 
 
-def log_exceptions(type_: Type[BaseException], value: BaseException, tb: Optional[TracebackType]) -> None:
-    log.critical('Unhandled exception:', exc_info=(type_, value, tb))
+def log_exceptions(
+    type_: Type[BaseException], value: BaseException, tb: Optional[TracebackType]
+) -> None:
+    log.critical("Unhandled exception:", exc_info=(type_, value, tb))
 
 
 def log_connected(pcol: TClient) -> TClient:
-    log.info('connected to %s', pcol.name)
+    log.info("connected to %s", pcol.name)
     return pcol
 
 
 class VNCDoCLIClient(VNCDoToolClient):
     def vncRequestPassword(self) -> None:
         if self.factory.password is None:
-            self.factory.password = getpass.getpass('VNC password:')
+            self.factory.password = getpass.getpass("VNC password:")
 
         self.sendPassword(self.factory.password)
 
 
 class VNCDoCLIFactory(VNCDoToolFactory):
     protocol = VNCDoCLIClient
 
@@ -72,48 +74,47 @@
 
     def done(self, exit_code: int) -> None:
         reactor.exit_status = exit_code
         reactor.callLater(0.1, reactor.stop)
 
 
 class ExitingProcess(protocol.ProcessProtocol):  # type: ignore[misc]
-
     def processExited(self, reason: Failure) -> None:
         reactor.callLater(0.1, reactor.stop)
 
     def errReceived(self, data: bytes) -> None:
         print(data)
 
 
 class VNCDoToolOptionParser(optparse.OptionParser):
     def format_help(self, formatter: Optional[optparse.HelpFormatter] = None) -> str:
         result = super().format_help(formatter)
         result += (
-            '\n'
-            'Common Commands (CMD):\n'
-            '  key KEY\t\tsend KEY to server, alphanumeric or keysym: ctrl-c, del\n'
-            '  type TEXT\t\tsend alphanumeric string of TEXT\n'
-            '  typefile FILENAME\t\ttype out the contents of FILENAME\n'
-            '  move X Y\t\tmove the mouse cursor to position X,Y\n'
-            '  click BUTTON\t\tsend a mouse BUTTON click\n'
-            '  capture FILE\t\tsave current screen as FILE\n'
-            '  expect FILE FUZZ\twait until screen matches FILE\n'
-            '  pause SECONDS\t\twait SECONDS before sending next command\n'
-            '\n'
-            'Other Commands (CMD):\n'
-            '  keyup KEY\t\tsend KEY released\n'
-            '  keydown KEY\t\tsend KEY pressed\n'
-            '  mousedown BUTTON\tsend BUTTON down\n'
-            '  mousemove X Y\t\talias for move\n'
-            '  mouseup BUTTON\tsend BUTTON up\n'
-            '  drag X Y\t\tmove the mouse to X,Y in small steps\n'
-            '  rcapture FILE X Y W H\tcapture a region of the screen\n'
-            '  rexpect FILE X Y FUZZ\texpect that matches a region of the screen\n'
-            '\n'
-            'If a filename is given commands will be read from it, or stdin `-`\n'
+            "\n"
+            "Common Commands (CMD):\n"
+            "  key KEY\t\tsend KEY to server, alphanumeric or keysym: ctrl-c, del\n"
+            "  type TEXT\t\tsend alphanumeric string of TEXT\n"
+            "  typefile FILENAME\t\ttype out the contents of FILENAME\n"
+            "  move X Y\t\tmove the mouse cursor to position X,Y\n"
+            "  click BUTTON\t\tsend a mouse BUTTON click\n"
+            "  capture FILE\t\tsave current screen as FILE\n"
+            "  expect FILE FUZZ\twait until screen matches FILE\n"
+            "  pause SECONDS\t\twait SECONDS before sending next command\n"
+            "\n"
+            "Other Commands (CMD):\n"
+            "  keyup KEY\t\tsend KEY released\n"
+            "  keydown KEY\t\tsend KEY pressed\n"
+            "  mousedown BUTTON\tsend BUTTON down\n"
+            "  mousemove X Y\t\talias for move\n"
+            "  mouseup BUTTON\tsend BUTTON up\n"
+            "  drag X Y\t\tmove the mouse to X,Y in small steps\n"
+            "  rcapture FILE X Y W H\tcapture a region of the screen\n"
+            "  rexpect FILE X Y FUZZ\texpect that matches a region of the screen\n"
+            "\n"
+            "If a filename is given commands will be read from it, or stdin `-`\n"
         )
         return result
 
 
 class CommandParseError(RuntimeError):
     pass
 
@@ -128,87 +129,93 @@
     client = VNCDoCLIClient
 
     if delay:
         delay = float(delay) / 1000.0
 
     while args:
         cmd = args.pop(0)
-        if cmd == 'key':
+        if cmd == "key":
             key = args.pop(0)
             factory.deferred.addCallback(client.keyPress, key)
-        elif cmd in ('kdown', 'keydown'):
+        elif cmd in ("kdown", "keydown"):
             key = args.pop(0)
             factory.deferred.addCallback(client.keyDown, key)
-        elif cmd in ('kup', 'keyup'):
+        elif cmd in ("kup", "keyup"):
             key = args.pop(0)
             factory.deferred.addCallback(client.keyUp, key)
-        elif cmd in ('move', 'mousemove'):
+        elif cmd in ("move", "mousemove"):
             x, y = int(args.pop(0)), int(args.pop(0))
             factory.deferred.addCallback(client.mouseMove, x, y)
-        elif cmd == 'click':
+        elif cmd == "click":
             button = int(args.pop(0))
             factory.deferred.addCallback(client.mousePress, button)
-        elif cmd in ('mdown', 'mousedown'):
+        elif cmd in ("mdown", "mousedown"):
             button = int(args.pop(0))
             factory.deferred.addCallback(client.mouseDown, button)
-        elif cmd in ('mup', 'mouseup'):
+        elif cmd in ("mup", "mouseup"):
             button = int(args.pop(0))
             factory.deferred.addCallback(client.mouseUp, button)
-        elif cmd == 'type':
+        elif cmd == "type":
             for key in args.pop(0):
                 factory.deferred.addCallback(client.keyPress, key)
                 if delay:
                     factory.deferred.addCallback(client.pause, delay)
-        elif cmd == 'typefile':
+        elif cmd == "typefile":
             with open(args.pop(0)) as f:
                 content = f.read()
                 for key in content:
-                    if key == '\r':
+                    if key == "\r":
                         continue
-                    if key == '\n':
-                        key = 'enter'
-                    if key == '\t':
-                        key = 'tab'
+                    if key == "\n":
+                        key = "enter"
+                    if key == "\t":
+                        key = "tab"
                     factory.deferred.addCallback(client.keyPress, key)
                     if delay:
                         factory.deferred.addCallback(client.pause, delay)
-        elif cmd == 'pastefile':
+        elif cmd == "pastefile":
             with open(args.pop(0)) as f:
-                content = f.read().replace('\r\n', '\n')
+                content = f.read().replace("\r\n", "\n")
                 factory.deferred.addCallback(client.paste, content)
-        elif cmd == 'capture':
+        elif cmd == "capture":
             filename = args.pop(0)
             imgformat = os.path.splitext(filename)[1][1:]
             if imgformat not in SUPPORTED_FORMATS:
-                raise CommandParseError(f'unsupported image format "{imgformat}", choose one of {SUPPORTED_FORMATS}')
-            factory.deferred.addCallback(client.captureScreen, filename, int(incremental_refreshes))
-        elif cmd == 'expect':
+                raise CommandParseError(
+                    f'unsupported image format "{imgformat}", choose one of {SUPPORTED_FORMATS}'
+                )
+            factory.deferred.addCallback(
+                client.captureScreen, filename, int(incremental_refreshes)
+            )
+        elif cmd == "expect":
             filename = args.pop(0)
             rms = float(args.pop(0))
             factory.deferred.addCallback(client.expectScreen, filename, rms)
-        elif cmd == 'rcapture':
+        elif cmd == "rcapture":
             filename = args.pop(0)
             x = int(args.pop(0))
             y = int(args.pop(0))
             w = int(args.pop(0))
             h = int(args.pop(0))
             imgformat = os.path.splitext(filename)[1][1:]
             if imgformat not in SUPPORTED_FORMATS:
-                raise CommandParseError(f'unsupported image format "{imgformat}", choose one of {SUPPORTED_FORMATS}')
+                raise CommandParseError(
+                    f'unsupported image format "{imgformat}", choose one of {SUPPORTED_FORMATS}'
+                )
             factory.deferred.addCallback(client.captureRegion, filename, x, y, w, h)
-        elif cmd == 'rexpect':
+        elif cmd == "rexpect":
             filename = args.pop(0)
             x = int(args.pop(0))
             y = int(args.pop(0))
             rms = float(args.pop(0))
             factory.deferred.addCallback(client.expectRegion, filename, x, y, rms)
-        elif cmd in ('pause', 'sleep'):
+        elif cmd in ("pause", "sleep"):
             duration = float(args.pop(0)) / warp
             factory.deferred.addCallback(client.pause, duration)
-        elif cmd in 'drag':
+        elif cmd in "drag":
             x, y = int(args.pop(0)), int(args.pop(0))
             factory.deferred.addCallback(client.mouseDrag, x, y)
         elif os.path.isfile(cmd):
             lex = shlex.shlex(open(cmd), posix=True)
             lex.whitespace_split = True
             args = list(lex) + args
         else:
@@ -220,21 +227,23 @@
 
 def build_tool(options: optparse.Values, args: List[str]) -> VNCDoCLIFactory:
     factory = VNCDoCLIFactory()
 
     if options.verbose:
         factory.deferred.addCallbacks(log_connected)
 
-    if args == ['-']:
+    if args == ["-"]:
         lex = shlex.shlex(posix=True)
         lex.whitespace_split = True
         args = list(lex)
 
     try:
-        build_command_list(factory, args, options.delay, options.warp, options.incremental_refreshes)
+        build_command_list(
+            factory, args, options.delay, options.warp, options.incremental_refreshes
+        )
     except CommandParseError as exc:
         sys.exit(exc)
 
     factory_connect(factory, options.host, options.port, options.address_family)
     reactor.exit_status = 1
 
     # close the connection when we're done
@@ -253,51 +262,49 @@
     return factory
 
 
 def add_standard_options(parser: optparse.OptionParser) -> optparse.OptionParser:
     parser.disable_interspersed_args()
 
     parser.add_option(
-        '-p',
-        '--password',
-        help='use password to access server',
+        "-p",
+        "--password",
+        help="use password to access server",
     )
     parser.add_option(
-        '-u',
-        '--username',
-        help='use username to access server',
+        "-u",
+        "--username",
+        help="use username to access server",
     )
     parser.add_option(
-        '-s',
-        '--server',
-        default='127.0.0.1',
-        help='connect to VNC server at ADDRESS[:DISPLAY|::PORT] [%default]',
+        "-s",
+        "--server",
+        default="127.0.0.1",
+        help="connect to VNC server at ADDRESS[:DISPLAY|::PORT] [%default]",
     )
     parser.add_option(
-        '--logfile',
-        metavar='FILE',
-        help='output logging information to FILE',
+        "--logfile",
+        metavar="FILE",
+        help="output logging information to FILE",
     )
     parser.add_option(
-        '-v',
-        '--verbose',
-        action='count',
+        "-v",
+        "--verbose",
+        action="count",
         default=0,
-        help='increase verbosity, use multiple times',
+        help="increase verbosity, use multiple times",
     )
     return parser
 
 
 def setup_logging(options: optparse.Values) -> None:
     # route Twisted log messages via stdlib logging
     if options.logfile:
         handler = logging.handlers.RotatingFileHandler(
-            options.logfile,
-            maxBytes=5 << 20,
-            backupCount=5
+            options.logfile, maxBytes=5 << 20, backupCount=5
         )
         logging.getLogger().addHandler(handler)
         sys.excepthook = log_exceptions
 
     logging.basicConfig()
     if options.verbose > 1:
         logging.getLogger().setLevel(logging.DEBUG)
@@ -309,20 +316,20 @@
 
 def parse_server(server: str) -> Tuple[socket.AddressFamily, str, int]:
     if server.startswith("["):
         host, sep, server = server[1:].partition("]")
         if not sep:
             raise ValueError(server)
         ipaddress.IPv6Address(host)
-        split = server.split(':')
+        split = server.split(":")
         address_family = socket.AF_INET6
     else:
-        split = server.split(':')
+        split = server.split(":")
         if not split[0]:
-            host = '127.0.0.1'
+            host = "127.0.0.1"
         else:
             host = split[0]
 
         if hasattr(socket, "AF_UNIX") and os.path.exists(host):
             address_family = socket.AF_UNIX
         else:
             try:
@@ -343,152 +350,150 @@
 
     return address_family, host, port
 
 
 def vnclog() -> None:
     from vncdotool import __version__
 
-    usage = '%prog [options] OUTPUT'
-    description = 'Capture user interactions with a VNC Server'
+    usage = "%prog [options] OUTPUT"
+    description = "Capture user interactions with a VNC Server"
     version = "%prog " + __version__
 
     op = optparse.OptionParser(usage=usage, description=description, version=version)
     add_standard_options(op)
     op.add_option(
-        '--listen',
-        metavar='PORT',
+        "--listen",
+        metavar="PORT",
         default=5902,
-        type='int',
-        help='listen for client connections on PORT [%default]',
+        type="int",
+        help="listen for client connections on PORT [%default]",
     )
     op.add_option(
-        '--forever',
-        action='store_true',
-        help='continually accept new connections',
+        "--forever",
+        action="store_true",
+        help="continually accept new connections",
     )
     op.add_option(
-        '--viewer',
-        metavar='CMD',
-        help='launch an interactive client using CMD [%default]',
+        "--viewer",
+        metavar="CMD",
+        help="launch an interactive client using CMD [%default]",
     )
     # ideally we wouldn't need this, VNCLoggingClient should sniff and set this properly
     op.add_option(
-        '--password-required',
-        action='store_true',
+        "--password-required",
+        action="store_true",
         default=False,
-        help='a VNC password is required to connect to the server',
+        help="a VNC password is required to connect to the server",
     )
     options, args = op.parse_args()
 
     setup_logging(options)
 
-    options.address_family, options.host, options.port = parse_server(
-        options.server)
+    options.address_family, options.host, options.port = parse_server(options.server)
 
     if len(args) != 1:
-        op.error('incorrect number of arguments')
+        op.error("incorrect number of arguments")
     output = args[0]
 
     factory = build_proxy(options)
 
     if options.forever and os.path.isdir(output):
         factory.output = output
     elif options.forever:
-        op.error('--forever requires OUTPUT to be a directory')
-    elif output == '-':
+        op.error("--forever requires OUTPUT to be a directory")
+    elif output == "-":
         factory.output = sys.stdout
     else:
-        factory.output = open(output, 'w')
+        factory.output = open(output, "w")
 
     if options.listen == 0:
-        log.info('accepting connections on ::%d', factory.listen_port)
+        log.info("accepting connections on ::%d", factory.listen_port)
 
     factory.password = options.password
 
     if options.viewer:
-        cmdline = f'{options.viewer} localhost::{factory.listen_port}'
+        cmdline = f"{options.viewer} localhost::{factory.listen_port}"
         reactor.spawnProcess(
             ExitingProcess(),
             options.viewer,
             cmdline.split(),
             env=os.environ,
         )
     reactor.run()
     sys.exit(reactor.exit_status)
 
 
 def vncdo() -> None:
     from vncdotool import __version__
 
-    usage = '%prog [options] CMD CMDARGS|-|filename'
-    description = 'Command line control of a VNC server'
+    usage = "%prog [options] CMD CMDARGS|-|filename"
+    description = "Command line control of a VNC server"
     version = "%prog " + __version__
 
     op = VNCDoToolOptionParser(usage=usage, description=description, version=version)
     add_standard_options(op)
 
     op.add_option(
-        '--delay',
-        metavar='MILLISECONDS',
-        default=os.environ.get('VNCDOTOOL_DELAY', 10),
-        type='int',
-        help='delay MILLISECONDS between actions [%defaultms]',
+        "--delay",
+        metavar="MILLISECONDS",
+        default=os.environ.get("VNCDOTOOL_DELAY", 10),
+        type="int",
+        help="delay MILLISECONDS between actions [%defaultms]",
     )
     op.add_option(
-        '--force-caps',
-        action='store_true',
-        help='for non-compliant servers, send shift-LETTER, ensures capitalization works',
+        "--force-caps",
+        action="store_true",
+        help="for non-compliant servers, send shift-LETTER, ensures capitalization works",
     )
     op.add_option(
-        '--localcursor',
-        action='store_true',
-        help='mouse pointer drawn client-side, useful when server does not include cursor',
+        "--localcursor",
+        action="store_true",
+        help="mouse pointer drawn client-side, useful when server does not include cursor",
     )
     op.add_option(
-        '--nocursor',
-        action='store_true',
-        help='no mouse pointer in screen captures',
+        "--nocursor",
+        action="store_true",
+        help="no mouse pointer in screen captures",
     )
     op.add_option(
-        '--disable-desktop-resizing',
-        action='store_true',
-        help='disable desktop resizing, this was default behaviour < 0.11',
+        "--disable-desktop-resizing",
+        action="store_true",
+        help="disable desktop resizing, this was default behaviour < 0.11",
     )
     op.add_option(
-        '-t',
-        '--timeout',
-        type='float',
-        metavar='SECONDS',
-        help='abort if unable to complete all actions within TIMEOUT seconds',
+        "-t",
+        "--timeout",
+        type="float",
+        metavar="SECONDS",
+        help="abort if unable to complete all actions within TIMEOUT seconds",
     )
     op.add_option(
-        '-w',
-        '--warp',
-        type='float',
-        metavar='FACTOR',
+        "-w",
+        "--warp",
+        type="float",
+        metavar="FACTOR",
         default=1.0,
-        help='pause time is accelerated by FACTOR [x%default]',
+        help="pause time is accelerated by FACTOR [x%default]",
     )
     op.add_option(
-        '-i',
-        '--incremental-refreshes',
-        action='store_true',
+        "-i",
+        "--incremental-refreshes",
+        action="store_true",
         default=False,
         help='set the "incremental" flag',
     )
 
     options, args = op.parse_args()
     if not len(args):
-        op.error('no command provided')
+        op.error("no command provided")
 
     setup_logging(options)
-    options.address_family, options.host, options.port = parse_server(
-        options.server)
+    options.address_family, options.host, options.port = parse_server(options.server)
 
-    log.info('connecting to %s:%s', options.host, options.port)
+    log.info("connecting to %s:%s", options.host, options.port)
 
     factory = build_tool(options, args)
     factory.username = options.username
     factory.password = options.password
 
     if options.localcursor:
         factory.pseudocursor = True
@@ -499,18 +504,18 @@
     if options.nocursor:
         factory.nocursor = True
 
     if options.force_caps:
         factory.force_caps = True
 
     if options.timeout:
-        message = 'TIMEOUT Exceeded (%ss)' % options.timeout
+        message = "TIMEOUT Exceeded (%ss)" % options.timeout
         failure = Failure(TimeoutError(message))
         reactor.callLater(options.timeout, factory.error, failure)
 
     reactor.run()
 
     sys.exit(reactor.exit_status)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     vncdo()
```

### Comparing `vncdotool-1.1.0/vncdotool/loggingproxy.py` & `vncdotool-1.2.0/vncdotool/loggingproxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 from .client import KEYMAP, VNCDoToolClient
 from .rfb import AuthTypes, Encoding, IntEnumLookup, PixelFormat, Rect
 
 log = logging.getLogger(__name__)
 
 
 class ProtocolError(Exception):
-    """ VNC Protocol error """
+    """VNC Protocol error"""
 
 
 class MsgC2S(IntEnumLookup):
     """RFC 6143 §7.5. Client-to-Server Messages."""
+
     SET_PIXEL_FORMAT = 0
     SET_ENCODING = 2
     FRAMEBUFFER_UPDATE_REQUEST = 3
     KEY_EVENT = 4
     POINTER_EVENT = 5
     CLIENT_CUT_TEXT = 6
     FILE_TRANSFER = 7
@@ -55,14 +56,15 @@
     GII_CLIENT_MESSAGE = 253  # General Input Interface
     VMWARE_254 = 254
     QEMU_CLIENT_MESSAGE = 255
 
 
 class QemuClientMessage(IntEnumLookup):
     """https://github.com/rfbproto/rfbproto/blob/master/rfbproto.rst#qemu-client-message"""
+
     EXTENDED_KEY_EVENT = 0
     AUDIO = 1
 
 
 TYPE_LEN = {
     MsgC2S.SET_PIXEL_FORMAT: 20,
     MsgC2S.SET_ENCODING: 4,
@@ -90,24 +92,24 @@
         self.buffer += data
         while len(self.buffer) >= self._handler[1]:
             self._handler[0]()
 
     def _handle_version(self) -> None:
         msg = self.buffer[:12]
         del self.buffer[:12]
-        if not msg.startswith(b'RFB 003.') and msg.endswith(b'\n'):
+        if not msg.startswith(b"RFB 003.") and msg.endswith(b"\n"):
             self.transport.loseConnection()
 
         version = msg[8:11]
-        if version in (b'003', b'005'):
+        if version in (b"003", b"005"):
             if self.factory.password_required:
                 self._handler = self._handle_VNCAuthResponse, 16
             else:
                 self._handler = self._handle_clientInit, 1
-        elif version in (b'007', b'008'):
+        elif version in (b"007", b"008"):
             # XXX send security v3.7+
             self._handler = self._handle_security, 1
 
     def _handle_security(self) -> None:
         sectype = self.buffer[0]
         log.debug("Client selected %r", AuthTypes.lookup(sectype))
         del self.buffer[:1]
@@ -122,47 +124,47 @@
         log.debug("Client shares: %s", shared)
         del self.buffer[:1]
         # XXX react to shared
         # XXX send serverInit
         self._handler = self._handle_protocol, 1
 
     def _handle_protocol(self) -> None:
-        ptype, = unpack_from('!B', self.buffer)
+        (ptype,) = unpack_from("!B", self.buffer)
         nbytes = TYPE_LEN.get(ptype, 0)
         if len(self.buffer) < nbytes:
             self._handler = self._handle_protocol, nbytes + 1
             return
 
         block = bytes(self.buffer[1:nbytes])
         del self.buffer[:nbytes]
         if ptype == MsgC2S.SET_PIXEL_FORMAT:
-            (args,) = unpack('!xxx16s', block)
+            (args,) = unpack("!xxx16s", block)
             pixel_fomat = PixelFormat.from_bytes(args)
             self.handle_setPixelFormat(pixel_fomat)
         elif ptype == MsgC2S.SET_ENCODING:
-            nencodings, = unpack('!xH', block)
+            (nencodings,) = unpack("!xH", block)
             nbytes = 4 * nencodings
-            encodings = unpack_from('!' + 'I' * nencodings, self.buffer)
+            encodings = unpack_from("!" + "I" * nencodings, self.buffer)
             del self.buffer[:nbytes]
             for encoding in encodings:
                 log.debug(f"Client announces {Encoding.lookup(encoding)!r}")
             self.handle_setEncodings(encodings)
         elif ptype == MsgC2S.FRAMEBUFFER_UPDATE_REQUEST:
-            inc, x, y, w, h = unpack('!BHHHH', block)
+            inc, x, y, w, h = unpack("!BHHHH", block)
             self.handle_framebufferUpdate(x, y, w, h, inc)
         elif ptype == MsgC2S.KEY_EVENT:
-            down, key = unpack('!BxxI', block)
+            down, key = unpack("!BxxI", block)
             self.handle_keyEvent(key, down)
         elif ptype == MsgC2S.POINTER_EVENT:
-            buttonmask, x, y = unpack('!BHH', block)
+            buttonmask, x, y = unpack("!BHH", block)
             self.handle_pointerEvent(x, y, buttonmask)
         elif ptype == MsgC2S.CLIENT_CUT_TEXT:
             self.handle_clientCutText(block)
         elif ptype == MsgC2S.QEMU_CLIENT_MESSAGE:
-            subtype, = unpack('!B', block)
+            (subtype,) = unpack("!B", block)
             if subtype == QemuClientMessage.EXTENDED_KEY_EVENT:
                 self._handler = self._handle_qemuExtendedKeyEvent, 10
             else:
                 log.debug("Unhandled subtype %r", QemuClientMessage.lookup(subtype))
                 raise ProtocolError(subtype)
         else:
             log.debug("Unhandled response %r", MsgC2S.lookup(ptype))
@@ -176,15 +178,17 @@
 
     def handle_setPixelFormat(self, pixel_format: PixelFormat) -> None:
         pass
 
     def handle_setEncodings(self, encodings: Sequence[int]) -> None:
         pass
 
-    def handle_framebufferUpdate(self, x: int, y: int, w: int, h: int, incremental: bool) -> None:
+    def handle_framebufferUpdate(
+        self, x: int, y: int, w: int, h: int, incremental: bool
+    ) -> None:
         pass
 
     def handle_keyEvent(self, key: int, down: bool) -> None:
         pass
 
     def handle_pointerEvent(self, x: int, y: int, buttonmask: int) -> None:
         pass
@@ -209,32 +213,33 @@
         return
 
     def loseConnection(self) -> None:
         return
 
 
 class VNCLoggingClient(VNCDoToolClient):
-    """ Specialization of a VNCDoToolClient that will save screen captures
-    """
+    """Specialization of a VNCDoToolClient that will save screen captures"""
+
     capture_file: Optional[str] = None
 
     def commitUpdate(self, rectangles: Optional[List[Rect]] = None) -> None:
         if self.capture_file:
             assert self.screen is not None
             self.screen.save(self.capture_file)
-            self.recorder('expect %s\n' % self.capture_file)
+            self.recorder("expect %s\n" % self.capture_file)
             self.capture_file = None
 
 
 class VNCLoggingClientProxy(portforward.ProxyClient):  # type: ignore[misc]
-    """ Accept data from a server and forward to logger and downstream client
+    """Accept data from a server and forward to logger and downstream client
 
     VNC server -> VNCLoggingClientProxy -> VNC client
                                         -> VNCLoggingClient
     """
+
     vnclog: Optional[VNCLoggingClient] = None
     ncaptures = 0
 
     def startLogging(self, peer: "VNCLoggingServerProxy") -> None:
         self.vnclog = VNCLoggingClient()
         self.vnclog.transport = NullTransport()
         self.vnclog.factory = self.peer.factory
@@ -251,27 +256,28 @@
 
 
 class VNCLoggingClientFactory(portforward.ProxyClientFactory):  # type: ignore[misc]
     protocol = VNCLoggingClientProxy
 
 
 class VNCLoggingServerProxy(portforward.ProxyServer, RFBServer):  # type: ignore[misc]
-    """ Proxy in the middle, decodes and logs RFB messages before sending them upstream
+    """Proxy in the middle, decodes and logs RFB messages before sending them upstream
 
     VNC client -> VNCLoggingServerProxy -> VNC server
                                         -> RFBServer
     """
+
     clientProtocolFactory = VNCLoggingClientFactory
 
     server: Optional[str] = None
     buttons = 0
     recorder: Optional[Callable[[str], int]] = None
 
     def connectionMade(self) -> None:
-        log.info('new connection from %s', self.transport.getPeer().host)
+        log.info("new connection from %s", self.transport.getPeer().host)
         super().connectionMade()
         RFBServer.connectionMade(self)
         self.mouse: Tuple[Optional[int], Optional[int]] = (None, None)
         self.last_event = time.time()
         self.recorder = self.factory.getRecorder()
 
     def connectionLost(self, reason: Failure) -> None:
@@ -287,39 +293,39 @@
         self.peer.startLogging(self)
 
     def handle_keyEvent(self, key: int, down: bool) -> None:
         now = time.time()
 
         rev = REVERSE_MAP.get(key, chr(key))
 
-        cmds = ['pause', '%.4f' % (now - self.last_event)]
+        cmds = ["pause", "%.4f" % (now - self.last_event)]
         self.last_event = now
         if down:
-            cmds += 'keydown', rev
+            cmds += "keydown", rev
         else:
-            cmds += 'keyup', rev
-        cmds.append('\n')
+            cmds += "keyup", rev
+        cmds.append("\n")
         assert self.recorder is not None
-        self.recorder(' '.join(cmds))
+        self.recorder(" ".join(cmds))
 
     def handle_pointerEvent(self, x: int, y: int, buttonmask: int) -> None:
         now = time.time()
 
-        cmds = ['pause', '%.4f' % (now - self.last_event)]
+        cmds = ["pause", "%.4f" % (now - self.last_event)]
         self.last_event = now
         if self.mouse != (x, y):
-            cmds.append('move %d %d' % (x, y))
+            cmds.append("move %d %d" % (x, y))
             self.mouse = x, y
 
         for button in range(1, 9):
             if buttonmask & (1 << (button - 1)):
-                cmds.append('click %d' % button)
-        cmds.append('\n')
+                cmds.append("click %d" % button)
+        cmds.append("\n")
         assert self.recorder is not None
-        self.recorder(' '.join(cmds))
+        self.recorder(" ".join(cmds))
 
 
 class VNCLoggingServerFactory(portforward.ProxyFactory):  # type: ignore[misc]
     protocol = VNCLoggingServerProxy
     shared = True
 
     pseudocursor = False
@@ -332,17 +338,17 @@
     password_required = False
 
     output: Union[IO[str], str] = sys.stdout
     _out: Optional[IO[str]] = None
 
     def getRecorder(self) -> Callable[[str], int]:
         if isinstance(self.output, str):
-            now = time.strftime('%y%m%d-%H%M%S')
-            outfile = os.path.join(self.output, '%s.vdo' % now)
-            self._out = open(outfile, 'w')
+            now = time.strftime("%y%m%d-%H%M%S")
+            outfile = os.path.join(self.output, "%s.vdo" % now)
+            self._out = open(outfile, "w")
             return self._out.write
         else:
             return self.output.write
 
     def clientConnectionMade(self, client: VNCLoggingServerProxy) -> None:
         pass
```

### Comparing `vncdotool-1.1.0/vncdotool/rfb.py` & `vncdotool-1.2.0/vncdotool/rfb.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,41 @@
 import getpass
 import os
 import sys
 import zlib
 from dataclasses import astuple, dataclass
 from enum import IntEnum, IntFlag
 from struct import Struct, pack, unpack, unpack_from
-from typing import Any, Callable, ClassVar, Collection, Dict, Iterator, List, Optional, Tuple, cast
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Collection,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    cast,
+)
 
 from Cryptodome.Cipher import AES, DES
 from Cryptodome.Hash import MD5
 from Cryptodome.Util.number import bytes_to_long, long_to_bytes
 from twisted.application import internet, service
 from twisted.internet import protocol
 from twisted.internet.interfaces import IConnector
 from twisted.internet.protocol import Protocol
 from twisted.python import log, usage
 from twisted.python.failure import Failure
 
 Rect = Tuple[int, int, int, int]
 Ver = Tuple[int, int]
 
-#~ from twisted.internet import reactor
+# ~ from twisted.internet import reactor
 
 
 class IntEnumLookup(IntEnum):
     @classmethod
     def lookup(cls, value: int) -> object:
         return cls._value2member_map_.get(value, f"<{cls.__name__}.UNKNOWN: {value:x}>")
 
@@ -135,56 +146,58 @@
     PSEUDO_FENCE = -312
     PSEUDO_CONTINUOUS_UPDATES = -313
     PSEUDO_CURSOR_WITH_ALPHA = -314
     PSEUDO_JPEG_FINE_GRAINED_QUALITY_LEVEL = -412  # ... -512
     CAR_CONNECTIVITY_523 = -523  # ... -528
     PSEUDO_JPEG_SUBSAMLING_LEVEL = -763  # ... -768
     VA_H264 = 0x48323634
-    VMWARE_0X574D5600 = 0x574d5600  # ... 0x574d56ff
-    PSEUDO_VMWARE_CURSOR = 0x574d5664
-    PSEUDO_VMWARE_CURSOR_STATE = 0x574d5665
-    PSEUDO_VMWARE_CURSOR_POSITION = 0x574d5666
-    PSEUDO_VMWARE_KEY_REPEAT = 0x574d5667
-    PSEUDO_VMWARE_LED_STATE = 0x574d5668
-    PSEUDO_VMWARE_DISPLAY_MODE_CHANGE = 0x574d5669
-    PSEUDO_VMWARE_VIRTUAL_MACHINE_STATE = 0x574d566a
-    PSEUDO_EXTENDED_CLIPBOARD = 0xc0a1e5ce
-    PLUGIN_STREAMING = 0xc0a1e5cf
-    KEYBOARD_LED_STATE = 0xfffe0000
-    SUPPORTED_MESSAGES = 0xfffe0001
-    SUPPORTED_ENCODINGS = 0xfffe0002
-    SERVER_IDENTITY = 0xfffe0003
-    LIBVNCSERVER_0XFFFE0004 = 0xfffe0004  # ... 0xfffe00ff
-    CACHE = 0xffff0000
-    CACHE_ENABLE = 0xffff0001
-    XOR_ZLIB = 0xffff0002
-    XOR_MONO_RECT_ZLIB = 0xffff0003
-    XOR_MULTI_COLOR_ZLIB = 0xffff0004
-    SOLID_COLOR = 0xffff0005
-    XOR_ENABLE = 0xffff0006
-    CACHE_ZIP = 0xffff0007
-    SOL_MONO_ZIP = 0xffff0008
-    ULTRA_ZIP = 0xffff0009
-    SERVER_STATE = 0xffff8000
-    ENABLE_KEEP_ALIVE = 0xffff8001
-    FTP_PROTOCOl_VERSION = 0xffff8002
-    SESSION = 0xffff8003
+    VMWARE_0X574D5600 = 0x574D5600  # ... 0x574d56ff
+    PSEUDO_VMWARE_CURSOR = 0x574D5664
+    PSEUDO_VMWARE_CURSOR_STATE = 0x574D5665
+    PSEUDO_VMWARE_CURSOR_POSITION = 0x574D5666
+    PSEUDO_VMWARE_KEY_REPEAT = 0x574D5667
+    PSEUDO_VMWARE_LED_STATE = 0x574D5668
+    PSEUDO_VMWARE_DISPLAY_MODE_CHANGE = 0x574D5669
+    PSEUDO_VMWARE_VIRTUAL_MACHINE_STATE = 0x574D566A
+    PSEUDO_EXTENDED_CLIPBOARD = 0xC0A1E5CE
+    PLUGIN_STREAMING = 0xC0A1E5CF
+    KEYBOARD_LED_STATE = 0xFFFE0000
+    SUPPORTED_MESSAGES = 0xFFFE0001
+    SUPPORTED_ENCODINGS = 0xFFFE0002
+    SERVER_IDENTITY = 0xFFFE0003
+    LIBVNCSERVER_0XFFFE0004 = 0xFFFE0004  # ... 0xfffe00ff
+    CACHE = 0xFFFF0000
+    CACHE_ENABLE = 0xFFFF0001
+    XOR_ZLIB = 0xFFFF0002
+    XOR_MONO_RECT_ZLIB = 0xFFFF0003
+    XOR_MULTI_COLOR_ZLIB = 0xFFFF0004
+    SOLID_COLOR = 0xFFFF0005
+    XOR_ENABLE = 0xFFFF0006
+    CACHE_ZIP = 0xFFFF0007
+    SOL_MONO_ZIP = 0xFFFF0008
+    ULTRA_ZIP = 0xFFFF0009
+    SERVER_STATE = 0xFFFF8000
+    ENABLE_KEEP_ALIVE = 0xFFFF8001
+    FTP_PROTOCOl_VERSION = 0xFFFF8002
+    SESSION = 0xFFFF8003
 
 
 class HextileEncoding(IntFlag):
     """RFC 6153 §7.7.4. Hextile Encoding."""
+
     RAW = 1
     BACKGROUND_SPECIFIED = 2
     FOREGROUND_SPECIFIED = 4
     ANY_SUBRECTS = 8
     SUBRECTS_COLORED = 16
 
 
 class AuthTypes(IntEnumLookup):
     """RFC 6143 §7.1.2. Security Handshake."""
+
     INVALID = 0
     NONE = 1
     VNC_AUTHENTICATION = 2
     REALVNC_3 = 3
     REALVNC_4 = 4
     RSA_AES = 5
     RSA_AES_UNENCRYPTED = 6
@@ -221,14 +234,15 @@
     RSA_AES256_2STEP = 133
     REALVNC_134 = 134
     REALVNC_192 = 192
 
 
 class MsgS2C(IntEnumLookup):
     """RFC 6143 §7.6. Server-to-Client Messages."""
+
     FRAMEBUFFER_UPDATE = 0
     SET_COLOUR_MAP_ENTRIES = 1
     BELL = 2
     SERVER_CUT_TEXT = 3
     RESIZE_FRAME_BUFFER_4 = 4
     KEY_FRAME_UPDATE = 5
     ULTRA_6 = 6
@@ -252,56 +266,56 @@
     GII_SERVER_MESSAGE = 253  # General Input Interface
     VMWARE_254 = 254
     QEMU_SERVER_MESSAGE = 255
 
 
 # keycodes
 # for KeyEvent()
-KEY_BackSpace = 0xff08
-KEY_Tab = 0xff09
-KEY_Return = 0xff0d
-KEY_Escape = 0xff1b
-KEY_Insert = 0xff63
-KEY_Delete = 0xffff
-KEY_Home = 0xff50
-KEY_End = 0xff57
-KEY_PageUp = 0xff55
-KEY_PageDown = 0xff56
-KEY_Left = 0xff51
-KEY_Up = 0xff52
-KEY_Right = 0xff53
-KEY_Down = 0xff54
-KEY_F1 = 0xffbe
-KEY_F2 = 0xffbf
-KEY_F3 = 0xffc0
-KEY_F4 = 0xffc1
-KEY_F5 = 0xffc2
-KEY_F6 = 0xffc3
-KEY_F7 = 0xffc4
-KEY_F8 = 0xffc5
-KEY_F9 = 0xffc6
-KEY_F10 = 0xffc7
-KEY_F11 = 0xffc8
-KEY_F12 = 0xffc9
+KEY_BackSpace = 0xFF08
+KEY_Tab = 0xFF09
+KEY_Return = 0xFF0D
+KEY_Escape = 0xFF1B
+KEY_Insert = 0xFF63
+KEY_Delete = 0xFFFF
+KEY_Home = 0xFF50
+KEY_End = 0xFF57
+KEY_PageUp = 0xFF55
+KEY_PageDown = 0xFF56
+KEY_Left = 0xFF51
+KEY_Up = 0xFF52
+KEY_Right = 0xFF53
+KEY_Down = 0xFF54
+KEY_F1 = 0xFFBE
+KEY_F2 = 0xFFBF
+KEY_F3 = 0xFFC0
+KEY_F4 = 0xFFC1
+KEY_F5 = 0xFFC2
+KEY_F6 = 0xFFC3
+KEY_F7 = 0xFFC4
+KEY_F8 = 0xFFC5
+KEY_F9 = 0xFFC6
+KEY_F10 = 0xFFC7
+KEY_F11 = 0xFFC8
+KEY_F12 = 0xFFC9
 KEY_F13 = 0xFFCA
 KEY_F14 = 0xFFCB
 KEY_F15 = 0xFFCC
 KEY_F16 = 0xFFCD
 KEY_F17 = 0xFFCE
 KEY_F18 = 0xFFCF
 KEY_F19 = 0xFFD0
 KEY_F20 = 0xFFD1
-KEY_ShiftLeft = 0xffe1
-KEY_ShiftRight = 0xffe2
-KEY_ControlLeft = 0xffe3
-KEY_ControlRight = 0xffe4
-KEY_MetaLeft = 0xffe7
-KEY_MetaRight = 0xffe8
-KEY_AltLeft = 0xffe9
-KEY_AltRight = 0xffea
+KEY_ShiftLeft = 0xFFE1
+KEY_ShiftRight = 0xFFE2
+KEY_ControlLeft = 0xFFE3
+KEY_ControlRight = 0xFFE4
+KEY_MetaLeft = 0xFFE7
+KEY_MetaRight = 0xFFE8
+KEY_AltLeft = 0xFFE9
+KEY_AltRight = 0xFFEA
 
 KEY_Scroll_Lock = 0xFF14
 KEY_Sys_Req = 0xFF15
 KEY_Num_Lock = 0xFF7F
 KEY_Caps_Lock = 0xFFE5
 KEY_Pause = 0xFF13
 KEY_Super_L = 0xFFEB  # windows-key, apple command key
@@ -350,17 +364,19 @@
         assert self.bpp in {8, 16, 24, 32}, f"bpp={self.bpp}"
         assert 1 <= self.depth <= self.bpp, f"depth={self.depth} <= bpp={self.bpp}"
         if self.truecolor:
             for max, shift in zip(
                 (self.redmax, self.greenmax, self.bluemax),
                 (self.redshift, self.greenshift, self.blueshift),
             ):
-                assert 1 <= max <= 0xffff, f"1 <= max={max} <= 0xffff"
+                assert 1 <= max <= 0xFFFF, f"1 <= max={max} <= 0xffff"
                 assert max & (max + 1) == 0, f"max={max} not a 2**n-1"
-                assert 0 <= shift <= self.bpp - max.bit_length(), f"shift={shift} not in bpp={self.bpp}"
+                assert (
+                    0 <= shift <= self.bpp - max.bit_length()
+                ), f"shift={shift} not in bpp={self.bpp}"
 
     @property
     def bypp(self) -> int:  # bytes-per-pixel
         return (7 + self.bpp) // 8
 
     @classmethod
     def from_bytes(cls, block: bytes) -> "PixelFormat":
@@ -410,15 +426,14 @@
 
             num_pixels += 1
             if num_pixels == pixels_in_tile:
                 return
 
 
 class RFBClient(Protocol):  # type: ignore[misc]
-
     # https://www.rfc-editor.org/rfc/rfc6143#section-7.1.1
     SUPPORTED_SERVER_VERSIONS = {
         (3, 3),
         # (3, 5),
         (3, 7),
         (3, 8),
         (3, 889),  # Apple Remote Desktop
@@ -441,16 +456,16 @@
         Encoding.ZRLE,
         Encoding.PSEUDO_CURSOR,
         Encoding.PSEUDO_DESKTOP_SIZE,
         Encoding.PSEUDO_LAST_RECT,
         Encoding.PSEUDO_QEMU_EXTENDED_KEY_EVENT,
     }
 
-    _HEADER = b'RFB 000.000\n'
-    _HEADER_TRANSLATE = bytes.maketrans(b'0123456789', b'0' * 10)
+    _HEADER = b"RFB 000.000\n"
+    _HEADER_TRANSLATE = bytes.maketrans(b"0123456789", b"0" * 10)
 
     def __init__(self) -> None:
         self._packet = bytearray()
         self._handler = self._handleInitial
         self._expected_len = 12
         self._expected_args: Tuple[Any, ...] = ()
         self._expected_kwargs: Dict[str, Any] = {}
@@ -475,15 +490,17 @@
         head = self._packet[:12]
         norm = head.translate(self._HEADER_TRANSLATE)
         if norm == self._HEADER:
             version_server = (int(head[4:7]), int(head[8:11]))
             if version_server not in self.SUPPORTED_SERVER_VERSIONS:
                 log.msg("Protocol version %d.%d not supported" % version_server)
 
-            version = max(v for v in self.SUPPORTED_SERVER_VERSIONS if v <= version_server)
+            version = max(
+                v for v in self.SUPPORTED_SERVER_VERSIONS if v <= version_server
+            )
             if version > self.MAX_CLIENT_VERSION:
                 version = self.MAX_CLIENT_VERSION
 
             del self._packet[0:12]
             log.msg("Using protocol version %d.%d" % version)
             self.transport.write(b"RFB %03d.%03d\n" % version)
             self._handler = self._handleExpected
@@ -523,15 +540,15 @@
                 self.expect(self._handleDHAuth, 4)
         else:
             log.msg(f"unknown security types: {types!r}")
             self.transport.loseConnection()
 
     def _handleAuth(self, block: bytes) -> None:
         (auth,) = unpack("!I", block)
-        #~ print(f"{auth=}")
+        # ~ print(f"{auth=}")
         if auth == AuthTypes.INVALID:
             self.expect(self._handleConnFailed, 4)
         elif auth == AuthTypes.NONE:
             self._doClientInitialization()
         elif auth == AuthTypes.VNC_AUTHENTICATION:
             self.expect(self._handleVNCAuth, 16)
         else:
@@ -579,33 +596,33 @@
         shared = long_to_bytes(pow(sk, s, m))
 
         h = MD5.new()
         h.update(shared)
         keyDigest = h.digest()
 
         cipher = AES.new(keyDigest, AES.MODE_ECB)
-        ciphertext = cipher.encrypt(userStruct.encode('utf-8'))
+        ciphertext = cipher.encrypt(userStruct.encode("utf-8"))
         self.transport.write(ciphertext + key)
 
     def ardRequestCredentials(self) -> None:
         if self.factory.username is None:
-            self.factory.username = input('username: ')
+            self.factory.username = input("username: ")
         if self.factory.password is None:
-            self.factory.password = getpass.getpass('password:')
+            self.factory.password = getpass.getpass("password:")
 
     def sendPassword(self, password: str) -> None:
         """send password"""
         key = _vnc_des(password)
         des = DES.new(key, DES.MODE_ECB)
         response = des.encrypt(self._challenge)
         self.transport.write(response)
 
     def _handleVNCAuthResult(self, block: bytes) -> None:
         (result,) = unpack("!I", block)
-        #~ print(f"{auth=}")
+        # ~ print(f"{auth=}")
         if result == 0:  # OK
             self._doClientInitialization()
             return
         elif result == 1:  # failed
             if self._version < (3, 8):
                 self.vncAuthFailed("authentication failed")
                 self.transport.loseConnection()
@@ -685,15 +702,22 @@
 
         if self.rectangles:
             self.rectangles -= 1
             self.rectanglePos.append((x, y, width, height))
             if encoding == Encoding.COPY_RECTANGLE:
                 self.expect(self._handleDecodeCopyrect, 4, x, y, width, height)
             elif encoding == Encoding.RAW:
-                self.expect(self._handleDecodeRAW, width * height * self.bypp, x, y, width, height)
+                self.expect(
+                    self._handleDecodeRAW,
+                    width * height * self.bypp,
+                    x,
+                    y,
+                    width,
+                    height,
+                )
             elif encoding == Encoding.HEXTILE:
                 self._doNextHextileSubrect(None, None, x, y, width, height, None, None)
             elif encoding == Encoding.CORRE:
                 self.expect(self._handleDecodeCORRE, 4 + self.bypp, x, y, width, height)
             elif encoding == Encoding.RRE:
                 self.expect(self._handleDecodeRRE, 4 + self.bypp, x, y, width, height)
             elif encoding == Encoding.ZRLE:
@@ -712,70 +736,77 @@
                 log.msg(f"unknown encoding received {Encoding.lookup(encoding)!r}")
                 self.transport.loseConnection()
         else:
             self._doConnection()
 
     # ---  RAW Encoding
 
-    def _handleDecodeRAW(self, block: bytes, x: int, y: int, width: int, height: int) -> None:
+    def _handleDecodeRAW(
+        self, block: bytes, x: int, y: int, width: int, height: int
+    ) -> None:
         # TODO convert pixel format?
         self.updateRectangle(x, y, width, height, block)
         self._doConnection()
 
     # ---  CopyRect Encoding
 
-    def _handleDecodeCopyrect(self, block: bytes, x: int, y: int, width: int, height: int) -> None:
+    def _handleDecodeCopyrect(
+        self, block: bytes, x: int, y: int, width: int, height: int
+    ) -> None:
         (srcx, srcy) = unpack("!HH", block)
         self.copyRectangle(srcx, srcy, x, y, width, height)
         self._doConnection()
 
     # ---  RRE Encoding
 
-    def _handleDecodeRRE(self, block: bytes, x: int, y: int, width: int, height: int) -> None:
+    def _handleDecodeRRE(
+        self, block: bytes, x: int, y: int, width: int, height: int
+    ) -> None:
         (subrects,) = unpack("!I", block[:4])
         color = block[4:]
         self.fillRectangle(x, y, width, height, color)
         if subrects:
             self.expect(self._handleRRESubRectangles, (8 + self.bypp) * subrects, x, y)
         else:
             self._doConnection()
 
     def _handleRRESubRectangles(self, block: bytes, topx: int, topy: int) -> None:
-        #~ print("_handleRRESubRectangle")
+        # ~ print("_handleRRESubRectangle")
         pos = 0
         end = len(block)
         sz = self.bypp + 8
         format = f"!{self.bypp}sHHHH"
         while pos < end:
-            (color, x, y, width, height) = unpack(format, block[pos:pos + sz])
+            (color, x, y, width, height) = unpack(format, block[pos : pos + sz])
             self.fillRectangle(topx + x, topy + y, width, height, color)
             pos += sz
         self._doConnection()
 
     # ---  CoRRE Encoding
 
-    def _handleDecodeCORRE(self, block: bytes, x: int, y: int, width: int, height: int) -> None:
+    def _handleDecodeCORRE(
+        self, block: bytes, x: int, y: int, width: int, height: int
+    ) -> None:
         (subrects,) = unpack("!I", block[:4])
         color = block[4:]
         self.fillRectangle(x, y, width, height, color)
         if subrects:
             self.expect(
-                self._handleDecodeCORRERectangles,
-                (4 + self.bypp) * subrects, x, y
+                self._handleDecodeCORRERectangles, (4 + self.bypp) * subrects, x, y
             )
         else:
             self._doConnection()
 
     def _handleDecodeCORRERectangles(self, block: bytes, topx: int, topy: int) -> None:
-        #~ print("_handleDecodeCORRERectangle")
+        # ~ print("_handleDecodeCORRERectangle")
         pos = 0
         sz = self.bypp + 4
         format = "!{self.bypp}sBBBB"
         while pos < sz:
-            (color, x, y, width, height) = unpack(format, block[pos:pos + sz])
+            (color, x, y, width, height) = unpack(format, block[pos : pos + sz])
             self.fillRectangle(topx + x, topy + y, width, height, color)
             pos += sz
         self._doConnection()
 
     # ---  Hexile Encoding
 
     def _doNextHextileSubrect(
@@ -785,15 +816,15 @@
         x: int,
         y: int,
         width: int,
         height: int,
         tx: Optional[int],
         ty: Optional[int],
     ) -> None:
-        #~ print("_doNextHextileSubrect %r" % ((color, x, y, width, height, tx, ty),))
+        # ~ print("_doNextHextileSubrect %r" % ((color, x, y, width, height, tx, ty),))
         # coords of next tile
         # its line after line of tiles
         # finished when the last line is completly received
 
         # dont inc the first time
         if tx is not None:
             assert ty is not None
@@ -805,15 +836,17 @@
         else:
             tx = x
             ty = y
         # more tiles?
         if ty >= y + height:
             self._doConnection()
         else:
-            self.expect(self._handleDecodeHextile, 1, bg, color, x, y, width, height, tx, ty)
+            self.expect(
+                self._handleDecodeHextile, 1, bg, color, x, y, width, height, tx, ty
+            )
 
     def _handleDecodeHextile(
         self,
         block: bytes,
         bg: bytes,
         color: bytes,
         x: int,
@@ -830,28 +863,49 @@
             tw = x + width - tx
         if y + height - ty < 16:
             th = y + height - ty
         # decode tile
         if subencoding & HextileEncoding.RAW:
             self.expect(
                 self._handleDecodeHextileRAW,
-                tw * th * self.bypp, bg, color, x, y, width, height, tx, ty, tw, th
+                tw * th * self.bypp,
+                bg,
+                color,
+                x,
+                y,
+                width,
+                height,
+                tx,
+                ty,
+                tw,
+                th,
             )
         else:
             numbytes = 0
             if subencoding & HextileEncoding.BACKGROUND_SPECIFIED:
                 numbytes += self.bypp
             if subencoding & HextileEncoding.FOREGROUND_SPECIFIED:
                 numbytes += self.bypp
             if subencoding & HextileEncoding.ANY_SUBRECTS:
                 numbytes += 1
             if numbytes:
                 self.expect(
                     self._handleDecodeHextileSubrect,
-                    numbytes, subencoding, bg, color, x, y, width, height, tx, ty, tw, th
+                    numbytes,
+                    subencoding,
+                    bg,
+                    color,
+                    x,
+                    y,
+                    width,
+                    height,
+                    tx,
+                    ty,
+                    tw,
+                    th,
                 )
             else:
                 self.fillRectangle(tx, ty, tw, th, bg)
                 self._doNextHextileSubrect(bg, color, x, y, width, height, tx, ty)
 
     def _handleDecodeHextileSubrect(
         self,
@@ -867,34 +921,56 @@
         ty: int,
         tw: int,
         th: int,
     ) -> None:
         subrects = 0
         pos = 0
         if subencoding & HextileEncoding.BACKGROUND_SPECIFIED:
-            bg = block[:self.bypp]
+            bg = block[: self.bypp]
             pos += self.bypp
         self.fillRectangle(tx, ty, tw, th, bg)
         if subencoding & HextileEncoding.FOREGROUND_SPECIFIED:
-            color = block[pos:pos + self.bypp]
+            color = block[pos : pos + self.bypp]
             pos += self.bypp
         if subencoding & HextileEncoding.ANY_SUBRECTS:
-            #~ (subrects, ) = unpack("!B", block)
+            # ~ (subrects, ) = unpack("!B", block)
             subrects = block[pos]
-        #~ print(subrects)
+        # ~ print(subrects)
         if subrects:
             if subencoding & HextileEncoding.SUBRECTS_COLORED:
                 self.expect(
                     self._handleDecodeHextileSubrectsColoured,
-                    (self.bypp + 2) * subrects, bg, color, subrects, x, y, width, height, tx, ty, tw, th
+                    (self.bypp + 2) * subrects,
+                    bg,
+                    color,
+                    subrects,
+                    x,
+                    y,
+                    width,
+                    height,
+                    tx,
+                    ty,
+                    tw,
+                    th,
                 )
             else:
                 self.expect(
                     self._handleDecodeHextileSubrectsFG,
-                    2 * subrects, bg, color, subrects, x, y, width, height, tx, ty, tw, th
+                    2 * subrects,
+                    bg,
+                    color,
+                    subrects,
+                    x,
+                    y,
+                    width,
+                    height,
+                    tx,
+                    ty,
+                    tw,
+                    th,
                 )
         else:
             self._doNextHextileSubrect(bg, color, x, y, width, height, tx, ty)
 
     def _handleDecodeHextileRAW(
         self,
         block: bytes,
@@ -934,17 +1010,17 @@
         end = len(block)
         while pos < end:
             pos2 = pos + self.bypp
             color = block[pos:pos2]
             xy = block[pos2]
             wh = block[pos2 + 1]
             sx = xy >> 4
-            sy = xy & 0xf
+            sy = xy & 0xF
             sw = (wh >> 4) + 1
-            sh = (wh & 0xf) + 1
+            sh = (wh & 0xF) + 1
             self.fillRectangle(tx + sx, ty + sy, sw, sh, color)
             pos += sz
         self._doNextHextileSubrect(bg, color, x, y, width, height, tx, ty)
 
     def _handleDecodeHextileSubrectsFG(
         self,
         block: bytes,
@@ -963,17 +1039,17 @@
         """all subrect with same color"""
         pos = 0
         end = len(block)
         while pos < end:
             xy = block[pos]
             wh = block[pos + 1]
             sx = xy >> 4
-            sy = xy & 0xf
+            sy = xy & 0xF
             sw = (wh >> 4) + 1
-            sh = (wh & 0xf) + 1
+            sh = (wh & 0xF) + 1
             self.fillRectangle(tx + sx, ty + sy, sw, sh, color)
             pos += 2
         self._doNextHextileSubrect(bg, color, x, y, width, height, tx, ty)
 
     # ---  ZRLE Encoding
     def _handleDecodeZRLE(
         self,
@@ -1002,20 +1078,22 @@
         tx = x
         ty = y
 
         data = self._zlib_stream.decompress(block)
         it = iter(data)
 
         def cpixel(i: Iterator[int]) -> bytearray:
-            return bytearray((
-                next(i),
-                next(i),
-                next(i),
-                0xff,
-            ))
+            return bytearray(
+                (
+                    next(i),
+                    next(i),
+                    next(i),
+                    0xFF,
+                )
+            )
 
         for subencoding in it:
             # calc tile size
             tw = th = 64
             if x + width - tx < 64:
                 tw = x + width - tx
             if y + height - ty < 64:
@@ -1094,15 +1172,17 @@
             if tx >= x + width:
                 tx = x
                 ty = ty + 64
 
         self._doConnection()
 
     # --- Pseudo Cursor Encoding
-    def _handleDecodePsuedoCursor(self, block: bytes, x: int, y: int, width: int, height: int) -> None:
+    def _handleDecodePsuedoCursor(
+        self, block: bytes, x: int, y: int, width: int, height: int
+    ) -> None:
         split = width * height * self.bypp
         image = block[:split]
         mask = block[split:]
         self.updateCursor(x, y, width, height, image, mask)
         self._doConnection()
 
     # --- Pseudo Desktop Size Encoding
@@ -1110,56 +1190,64 @@
         self.updateDesktopSize(width, height)
         self._doConnection()
 
     # ---  other server messages
 
     def _handleColourMapEntries(self, block: bytes) -> None:
         (first_color, number_of_colors) = unpack("!xHH", block)
-        self.expect(self._handleColourMapEntriesValue, 6 * number_of_colors, first_color)
+        self.expect(
+            self._handleColourMapEntriesValue, 6 * number_of_colors, first_color
+        )
 
     def _handleColourMapEntriesValue(self, block: bytes, first_color: int) -> None:
-        colors = [unpack_from("!HHH", block, offset) for offset in range(0, len(block), 6)]
+        colors = [
+            unpack_from("!HHH", block, offset) for offset in range(0, len(block), 6)
+        ]
         self.set_color_map(first_color, cast(List[Tuple[int, int, int]], colors))
         self.expect(self._handleConnection, 1)
 
     def _handleServerCutText(self, block: bytes) -> None:
-        (length, ) = unpack("!xxxI", block)
+        (length,) = unpack("!xxxI", block)
         self.expect(self._handleServerCutTextValue, length)
 
     def _handleServerCutTextValue(self, block: bytes) -> None:
         self.copy_text(block.decode("iso-8859-1"))
         self.expect(self._handleConnection, 1)
 
     # ------------------------------------------------------
     # incomming data redirector
     # ------------------------------------------------------
     def dataReceived(self, data: bytes) -> None:
-        #~ sys.stdout.write(repr(data) + '\n')
-        #~ print(f"{len(data), {len(self._packet)}")
+        # ~ sys.stdout.write(repr(data) + '\n')
+        # ~ print(f"{len(data), {len(self._packet)}")
         self._packet.extend(data)
         self._handler()
 
     def _handleExpected(self) -> None:
         if len(self._packet) >= self._expected_len:
             while len(self._packet) >= self._expected_len:
                 self._already_expecting = True
-                block = bytes(self._packet[:self._expected_len])
-                del self._packet[:self._expected_len]
-                #~ log.msg(f"handle {block!r} with {self._expected_handler.__name__!r}")
-                self._expected_handler(block, *self._expected_args, **self._expected_kwargs)
+                block = bytes(self._packet[: self._expected_len])
+                del self._packet[: self._expected_len]
+                # ~ log.msg(f"handle {block!r} with {self._expected_handler.__name__!r}")
+                self._expected_handler(
+                    block, *self._expected_args, **self._expected_kwargs
+                )
             self._already_expecting = False
 
-    def expect(self, handler: Callable[..., None], size: int, *args: Any, **kwargs: Any) -> None:
-        #~ log.msg(f"expect({handler.__name__!r}, {size!r}, {args!r}, {kwargs!r})")
+    def expect(
+        self, handler: Callable[..., None], size: int, *args: Any, **kwargs: Any
+    ) -> None:
+        # ~ log.msg(f"expect({handler.__name__!r}, {size!r}, {args!r}, {kwargs!r})")
         self._expected_handler = handler
         self._expected_len = size
         self._expected_args = args
         self._expected_kwargs = kwargs
         if not self._already_expecting:
-            self._handleExpected()   # just in case that there is already enough data
+            self._handleExpected()  # just in case that there is already enough data
 
     # ------------------------------------------------------
     # client -> server messages
     # ------------------------------------------------------
 
     def setPixelFormat(self, pixel_format: PixelFormat) -> None:
         pixformat = pixel_format.to_bytes()
@@ -1189,91 +1277,98 @@
     def keyEvent(self, key: int, down: bool = True) -> None:
         """For most ordinary keys, the "keysym" is the same as the corresponding ASCII value.
         Other common keys are shown in the KEY_ constants."""
         self.transport.write(pack("!BBxxI", 4, down, key))
 
     def pointerEvent(self, x: int, y: int, buttonmask: int = 0) -> None:
         """Indicates either pointer movement or a pointer button press or release. The pointer is
-           now at (x-position, y-position), and the current state of buttons 1 to 8 are represented
-           by bits 0 to 7 of button-mask respectively, 0 meaning up, 1 meaning down (pressed).
+        now at (x-position, y-position), and the current state of buttons 1 to 8 are represented
+        by bits 0 to 7 of button-mask respectively, 0 meaning up, 1 meaning down (pressed).
         """
         self.transport.write(pack("!BBHH", 5, buttonmask, x, y))
 
     def clientCutText(self, message: str) -> None:
         """The client has new ISO 8859-1 (Latin-1) text in its cut buffer.
-           (aka clipboard)
+        (aka clipboard)
         """
         data = message.encode("iso-8859-1")
         self.transport.write(pack("!BxxxI", 6, len(data)) + data)
 
     # ------------------------------------------------------
     # callbacks
     # override these in your application
     # ------------------------------------------------------
     def vncConnectionMade(self) -> None:
         """connection is initialized and ready.
-           typicaly, the pixel format is set here."""
+        typicaly, the pixel format is set here."""
 
     def vncRequestPassword(self) -> None:
         """a password is needed to log on, use sendPassword() to
-           send one."""
+        send one."""
         if self.factory.password is None:
             log.msg("need a password")
             self.transport.loseConnection()
             return
         self.sendPassword(self.factory.password)
 
     def vncAuthFailed(self, reason: Failure) -> None:
         """called when the authentication failed.
-           the connection is closed."""
+        the connection is closed."""
         log.msg(f"Cannot connect {reason}")
 
     def beginUpdate(self) -> None:
         """called before a series of updateRectangle(),
-           copyRectangle() or fillRectangle()."""
+        copyRectangle() or fillRectangle()."""
 
     def commitUpdate(self, rectangles: Optional[List[Rect]] = None) -> None:
         """called after a series of updateRectangle(), copyRectangle()
-           or fillRectangle() are finished.
-           typicaly, here is the place to request the next screen
-           update with FramebufferUpdateRequest(incremental=1).
-           argument is a list of tuples (x,y,w,h) with the updated
-           rectangles."""
+        or fillRectangle() are finished.
+        typicaly, here is the place to request the next screen
+        update with FramebufferUpdateRequest(incremental=1).
+        argument is a list of tuples (x,y,w,h) with the updated
+        rectangles."""
 
-    def updateRectangle(self, x: int, y: int, width: int, height: int, data: bytes) -> None:
+    def updateRectangle(
+        self, x: int, y: int, width: int, height: int, data: bytes
+    ) -> None:
         """new bitmap data. data is a string in the pixel format set
-           up earlier."""
+        up earlier."""
 
-    def copyRectangle(self, srcx: int, srcy: int, x: int, y: int, width: int, height: int) -> None:
+    def copyRectangle(
+        self, srcx: int, srcy: int, x: int, y: int, width: int, height: int
+    ) -> None:
         """used for copyrect encoding. copy the given rectangle
-           (src, srxy, width, height) to the target coords (x,y)"""
+        (src, srxy, width, height) to the target coords (x,y)"""
 
-    def fillRectangle(self, x: int, y: int, width: int, height: int, color: bytes) -> None:
+    def fillRectangle(
+        self, x: int, y: int, width: int, height: int, color: bytes
+    ) -> None:
         """fill the area with the color. the color is a string in
-           the pixel format set up earlier"""
+        the pixel format set up earlier"""
         # fallback variant, use update recatngle
         # override with specialized function for better performance
         self.updateRectangle(x, y, width, height, color * width * height)
 
-    def updateCursor(self, x: int, y: int, width: int, height: int, image: bytes, mask: bytes) -> None:
-        """ New cursor, focuses at (x, y)
-        """
+    def updateCursor(
+        self, x: int, y: int, width: int, height: int, image: bytes, mask: bytes
+    ) -> None:
+        """New cursor, focuses at (x, y)"""
 
     def updateDesktopSize(self, width: int, height: int) -> None:
-        """ New desktop size of width*height. """
+        """New desktop size of width*height."""
 
     def set_color_map(self, first: int, colors: List[Tuple[int, int, int]]) -> None:
         """The server is using a new color map."""
 
     def bell(self) -> None:
         """bell"""
 
     def copy_text(self, text: str) -> None:
         """The server has new ISO 8859-1 (Latin-1) text in its cut buffer.
-           (aka clipboard)"""
+        (aka clipboard)"""
 
 
 class RFBFactory(protocol.ClientFactory):  # type: ignore[misc]
     """A factory for remote frame buffer connections."""
 
     # the class of the protocol to build
     # should be overriden by application to use a derrived class
@@ -1282,84 +1377,94 @@
     def __init__(self, password: Optional[str] = None, shared: bool = False) -> None:
         self.password = password
         self.shared = shared
 
 
 def _vnc_des(password: str) -> bytes:
     """RFB protocol for authentication requires client to encrypt
-        challenge sent by server with password using DES method. However,
-        bits in each byte of the password are put in reverse order before
-        using it as encryption key."""
+    challenge sent by server with password using DES method. However,
+    bits in each byte of the password are put in reverse order before
+    using it as encryption key."""
     pw = f"{password:\0<8.8}"  # make sure its 8 chars long, zero padded
-    key = pw.encode("ASCII")  # unspecified https://www.rfc-editor.org/rfc/rfc6143#section-7.2.2
-    key = bytes(
-        sum((128 >> i) if (k & (1 << i)) else 0 for i in range(8))
-        for k in key
-    )
+    key = pw.encode(
+        "ASCII"
+    )  # unspecified https://www.rfc-editor.org/rfc/rfc6143#section-7.2.2
+    key = bytes(sum((128 >> i) if (k & (1 << i)) else 0 for i in range(8)) for k in key)
     return key
 
 
 # --- test code only, see vncviewer.py
 
-if __name__ == '__main__':
+if __name__ == "__main__":
+
     class RFBTest(RFBClient):
         """dummy client"""
+
         def vncConnectionMade(self) -> None:
             print(f"Screen format: {self.pixel_format}")
             print(f"Desktop name: {self.name!r}")
             self.SetEncodings([Encoding.RAW])
             self.FramebufferUpdateRequest()
 
-        def updateRectangle(self, x: int, y: int, width: int, height: int, data: bytes) -> None:
+        def updateRectangle(
+            self, x: int, y: int, width: int, height: int, data: bytes
+        ) -> None:
             print("%s " * 5 % (x, y, width, height, repr(data[:20])))
 
     class RFBTestFactory(protocol.ClientFactory):  # type: ignore[misc]
         """test factory"""
+
         protocol = RFBTest
 
         def clientConnectionLost(self, connector: IConnector, reason: Failure) -> None:
             print(reason)
             from twisted.internet import reactor
+
             reactor.stop()
-            #~ connector.connect()
+            # ~ connector.connect()
 
-        def clientConnectionFailed(self, connector: IConnector, reason: Failure) -> None:
+        def clientConnectionFailed(
+            self, connector: IConnector, reason: Failure
+        ) -> None:
             print("connection failed:", reason)
             from twisted.internet import reactor
+
             reactor.stop()
 
     class Options(usage.Options):  # type: ignore[misc]
         """command line options"""
+
         optParameters = [
-            ['display', 'd', '0', 'VNC display'],
-            ['host', 'h', 'localhost', 'remote hostname'],
-            ['outfile', 'o', None, 'Logfile [default: sys.stdout]'],
+            ["display", "d", "0", "VNC display"],
+            ["host", "h", "localhost", "remote hostname"],
+            ["outfile", "o", None, "Logfile [default: sys.stdout]"],
         ]
 
     o = Options()
     try:
         o.parseOptions()
     except usage.UsageError as errortext:
         print(f"{sys.argv[0]}: {errortext}")
         print(f"{sys.argv[0]}: Try --help for usage details.")
         raise SystemExit(1)
 
     logFile = sys.stdout
-    if o.opts['outfile']:
-        logFile = o.opts['outfile']
+    if o.opts["outfile"]:
+        logFile = o.opts["outfile"]
     log.startLogging(logFile)
 
-    host = o.opts['host']
-    port = int(o.opts['display']) + 5900
+    host = o.opts["host"]
+    port = int(o.opts["display"]) + 5900
 
     application = service.Application("rfb test")  # create Application
 
     # connect to this host and port, and reconnect if we get disconnected
     vncClient = internet.TCPClient(host, port, RFBFactory())  # create the service
     vncClient.setServiceParent(application)
 
     # this file should be run as 'twistd -y rfb.py' but it didn't work -
     # could't import crippled_des.py, so using this hack.
     # now with crippled_des.py replaced with pyDes this can be no more actual
     from twisted.internet import reactor
+
     vncClient.startService()
     reactor.run()
```

### Comparing `vncdotool-1.1.0/vncdotool.egg-info/PKG-INFO` & `vncdotool-1.2.0/vncdotool.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vncdotool
-Version: 1.1.0
+Version: 1.2.0
 Summary: Command line VNC client
 Home-page: http://github.com/sibson/vncdotool
 Author: Marc Sibson
 Author-email: sibson+vncdotool@gmail.com
 License: MIT License
 Keywords: VNC,RFB
 Classifier: Development Status :: 4 - Beta
@@ -22,15 +22,39 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE.txt
 
-.. image:: https://img.shields.io/pypi/v/vncdotool   :alt: PyPI
+.. image:: https://img.shields.io/pypi/pyversions/vncdotool.svg
+   :target: https://pypi.python.org/pypi/vncdotool
+   :alt: Python Versions
+
+.. image:: https://img.shields.io/pypi/v/vncdotool
+    :target: https://pypi.org/project/vncdotool/
+    :alt: PyPi Package
+
+.. image:: https://img.shields.io/pypi/pyversions/vncdotool.svg
+   :target: https://pypi.python.org/pypi/vncdotool
+   :alt: Python Versions
+
+.. image:: https://github.com/sibson/vncdotool/workflows/VNCDo%20CI/badge.svg
+   :target: https://github.com/sibson/vndotool/actions
+   :alt: Actions Status
+
+.. image:: https://readthedocs.org/projects/vncdotool/badge/?version=latest&style=flat
+   :target: https://vncdotool.readthedocs.io/en/latest/
+   :alt: ReadTheDocs
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+
+
 
 vncdotool
 ===========
 vncdotool is a command line VNC client.
 It can be useful to automating interactions with virtual machines or
 hardware devices that are otherwise difficult to control.
 
@@ -90,15 +114,19 @@
 
 .. _Read The Docs: http://vncdotool.readthedocs.org
 .. _GitHub: http://github.com/sibson/vncdotool
 .. _TigerVNC: http://sourceforge.net/apps/mediawiki/tigervnc/index.php?title=Main_Page
 .. _python-vnc-viewer: http://code.google.com/p/python-vnc-viewer
 .. _Stackoverflow: https://stackoverflow.com/questions/ask?tags=vncdotool
 
-1.1.0 (unreleased)
+1.2.0 (2023-06-06)
+----------------------
+  - fixes for api.shutdown and disconnect raise exceptions, #256
+
+1.1.0 (2023-04-01)
 ----------------------
 Huge thanks to @pmhahn for single handedly driving conversion to modern Python3, as well
 as cleaning up a ton of outstanding issues.
 
   - [BREAKING] drop python 2.x support, thanks @pmhahn
   - Use built-in Unittest and mock for testing
   - PEP-484 type hinting, thanks @pmhahn
```

### Comparing `vncdotool-1.1.0/vncdotool.egg-info/SOURCES.txt` & `vncdotool-1.2.0/vncdotool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

