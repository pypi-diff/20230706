# Comparing `tmp/LogTranslate-1.2.2.tar.gz` & `tmp/LogTranslate-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-1.2.2.tar", last modified: Mon Jul  3 13:32:32 2023, max compression
+gzip compressed data, was "LogTranslate-1.2.3.tar", last modified: Thu Jul  6 17:16:38 2023, max compression
```

## Comparing `LogTranslate-1.2.2.tar` & `LogTranslate-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.297102 LogTranslate-1.2.2/
--rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.272016 LogTranslate-1.2.2/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0     3183 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3183 2023-07-03 13:32:32.296104 LogTranslate-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.285707 LogTranslate-1.2.2/log_translate/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.291121 LogTranslate-1.2.2/log_translate/business/
--rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/business/__init__.py
--rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.2/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/config_default.py
--rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/data_struct.py
--rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/gloable.py
--rw-rw-rw-   0        0        0     4448 2023-07-03 13:31:40.000000 LogTranslate-1.2.2/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     3162 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/read_log_file.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.293114 LogTranslate-1.2.2/log_translate/res/
--rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/res/log_logo.ico
--rw-rw-rw-   0        0        0     7386 2023-06-29 14:53:32.000000 LogTranslate-1.2.2/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     7374 2023-06-29 14:53:32.000000 LogTranslate-1.2.2/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 13:32:32.297102 LogTranslate-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2199 2023-07-03 13:32:14.000000 LogTranslate-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.083648 LogTranslate-1.2.3/
+-rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.072684 LogTranslate-1.2.3/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3183 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-07-06 17:16:38.000000 LogTranslate-1.2.3/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3183 2023-07-06 17:16:38.082652 LogTranslate-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.077667 LogTranslate-1.2.3/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.080659 LogTranslate-1.2.3/log_translate/business/
+-rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.3/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/gloable.py
+-rw-rw-rw-   0        0        0     4448 2023-07-03 13:31:40.000000 LogTranslate-1.2.3/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     3162 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.081656 LogTranslate-1.2.3/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     7561 2023-07-06 17:13:36.000000 LogTranslate-1.2.3/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7491 2023-07-06 17:14:47.000000 LogTranslate-1.2.3/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 17:16:38.083648 LogTranslate-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2199 2023-07-06 17:16:35.000000 LogTranslate-1.2.3/setup.py
```

### Comparing `LogTranslate-1.2.2/LICENSE.txt` & `LogTranslate-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-1.2.3/LogTranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.2/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.2.3/LogTranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/PKG-INFO` & `LogTranslate-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.2/README.md` & `LogTranslate-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/log_translate/business/AndroidCrashPattern_translator.py` & `LogTranslate-1.2.3/log_translate/business/AndroidCrashPattern_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.2.3/log_translate/business/bluetooth_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/log_translate/data_struct.py` & `LogTranslate-1.2.3/log_translate/data_struct.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/log_translate/log_translator.py` & `LogTranslate-1.2.3/log_translate/log_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/log_translate/read_log_file.py` & `LogTranslate-1.2.3/log_translate/read_log_file.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/log_translate/res/log_logo.ico` & `LogTranslate-1.2.3/log_translate/res/log_logo.ico`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.2/log_translate/ui_pyqt6.py` & `LogTranslate-1.2.3/log_translate/ui_pyqt6.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import sys
 import traceback
 
 import keyboard as keyboard
 import pkg_resources
+from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QAction, QBrush, QColor, QIcon, QFont
 from PyQt6.QtWidgets import QApplication, QMainWindow, QListWidget, QListWidgetItem, QAbstractItemView
 
 from log_translate.data_struct import Log, Level
 from log_translate.read_log_file import LogReader
 
 
 class PyQt6Window(QMainWindow):
     def __init__(self):
         super().__init__()
         self.setWindowTitle("🤖日志解析")
+        # 设置窗口标志位为 Qt.WindowStaysOnTopHint
+        self.setWindowFlags(self.windowFlags() | Qt.WindowType.WindowStaysOnTopHint)
         ico = pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
         self.setWindowIcon(QIcon(ico))
         self.list_widget = QListWidget()
         self.list_widget.setSelectionMode(QAbstractItemView.SelectionMode.NoSelection)
         self.setCentralWidget(self.list_widget)
         self.setAcceptDrops(True)
         self.create_menu()
```

### Comparing `LogTranslate-1.2.2/log_translate/ui_pyside2.py` & `LogTranslate-1.2.3/log_translate/ui_pyside2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import sys
 import traceback
 
 import keyboard as keyboard
 import pkg_resources
+from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon, QFont, QAction, QColor
 from PySide6.QtWidgets import QMainWindow, QListWidget, QAbstractItemView, QApplication, QListWidgetItem
 
 from log_translate.data_struct import Log, Level
 from log_translate.read_log_file import LogReader
 
 
 class PySide6Window(QMainWindow):
     def __init__(self):
         super().__init__()
         self.setWindowTitle("🤖日志解析")
+        self.setWindowFlags(self.windowFlags() | Qt.WindowType.WindowStaysOnTopHint)
         ico = pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
         self.setWindowIcon(QIcon(ico))
         self.list_widget = QListWidget()
         self.list_widget.setSelectionMode(QAbstractItemView.SelectionMode.NoSelection)
         self.setCentralWidget(self.list_widget)
         self.setAcceptDrops(True)
         self.create_menu()
```

### Comparing `LogTranslate-1.2.2/setup.py` & `LogTranslate-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # PACKAGE_NAME主要在使用的时候用到 pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
 PACKAGE_NAME = 'log_translate'
 # 需要写清楚路径
 ICON_PATH = 'res/*.ico'
 
 setup(
     name='LogTranslate',
-    version='1.2.2',
+    version='1.2.3',
     author='5hmlA',
     author_email='jonas.jzy@gmail.com',
     # 指定运行时需要的Python版本
     python_requires='>=3.6',
     # 找到当前目录下有哪些包 当前(setup.py)目录下的文件夹 当前目录的py不包含 打包的是把所有代码放一个文件夹下文件名为库名字
     packages=find_packages(),
     # 配置readme
```

