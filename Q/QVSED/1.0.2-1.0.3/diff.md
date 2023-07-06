# Comparing `tmp/QVSED-1.0.2.tar.gz` & `tmp/QVSED-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QVSED-1.0.2.tar", last modified: Thu Jul  6 21:38:52 2023, max compression
+gzip compressed data, was "QVSED-1.0.3.tar", last modified: Thu Jul  6 21:40:02 2023, max compression
```

## Comparing `QVSED-1.0.2.tar` & `QVSED-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 21:38:52.054874 QVSED-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 QVSED-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 QVSED-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      754 2023-07-06 21:38:52.052891 QVSED-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 21:38:52.034252 QVSED-1.0.2/QVSED/
--rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 QVSED-1.0.2/QVSED/QVSED.ui
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 QVSED-1.0.2/QVSED/__init__.py
--rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 QVSED-1.0.2/QVSED/config.py
--rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 QVSED-1.0.2/QVSED/config_default.py
--rw-rw-rw-   0        0        0     7480 2023-07-06 21:07:16.000000 QVSED-1.0.2/QVSED/qvsed.py
-drwxrwxrwx   0        0        0        0 2023-07-06 21:38:52.049997 QVSED-1.0.2/QVSED.egg-info/
--rw-rw-rw-   0        0        0      754 2023-07-06 21:38:51.000000 QVSED-1.0.2/QVSED.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-06 21:38:51.000000 QVSED-1.0.2/QVSED.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 21:38:51.000000 QVSED-1.0.2/QVSED.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-06 21:38:51.000000 QVSED-1.0.2/QVSED.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 21:38:51.000000 QVSED-1.0.2/QVSED.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 21:38:51.000000 QVSED-1.0.2/QVSED.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2040 2023-07-06 21:35:06.000000 QVSED-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 21:38:52.054874 QVSED-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-06 21:38:48.000000 QVSED-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:40:02.359702 QVSED-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 QVSED-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 QVSED-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      710 2023-07-06 21:40:02.359702 QVSED-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 21:40:02.336837 QVSED-1.0.3/QVSED/
+-rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 QVSED-1.0.3/QVSED/QVSED.ui
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 QVSED-1.0.3/QVSED/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 QVSED-1.0.3/QVSED/config.py
+-rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 QVSED-1.0.3/QVSED/config_default.py
+-rw-rw-rw-   0        0        0     7480 2023-07-06 21:07:16.000000 QVSED-1.0.3/QVSED/qvsed.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:40:02.358264 QVSED-1.0.3/QVSED.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2040 2023-07-06 21:39:45.000000 QVSED-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 21:40:02.359702 QVSED-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-07-06 21:39:53.000000 QVSED-1.0.3/setup.py
```

### Comparing `QVSED-1.0.2/LICENSE.txt` & `QVSED-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QVSED-1.0.2/PKG-INFO` & `QVSED-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: QVSED
-Version: 1.0.2
+Version: 1.0.3
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
-#QVSED - Qt-based Volatile Small Editor
-QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files.
-QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows.
-QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET.
-QVSED is licensed under the GNU General Public License version 3 or later.
+QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.0.2/QVSED/QVSED.ui` & `QVSED-1.0.3/QVSED/QVSED.ui`

 * *Files identical despite different names*

### Comparing `QVSED-1.0.2/QVSED/qvsed.py` & `QVSED-1.0.3/QVSED/qvsed.py`

 * *Files identical despite different names*

### Comparing `QVSED-1.0.2/QVSED.egg-info/PKG-INFO` & `QVSED-1.0.3/QVSED.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: QVSED
-Version: 1.0.2
+Version: 1.0.3
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
-#QVSED - Qt-based Volatile Small Editor
-QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files.
-QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows.
-QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET.
-QVSED is licensed under the GNU General Public License version 3 or later.
+QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.0.2/README.md` & `QVSED-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `QVSED-1.0.2/setup.py` & `QVSED-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='QVSED',
-    version='1.0.2',
+    version='1.0.3',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
-    long_description='#QVSED - Qt-based Volatile Small Editor\nQVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files.\nQVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows.\nQVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET.\nQVSED is licensed under the GNU General Public License version 3 or later.',
+    long_description='QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.',
     packages=find_packages(),
     license="GPL-3.0-or-later",
     url='https://github.com/That1M8Head/QVSED/',
     include_package_data=True,
     install_requires=[
         'PyQt5'
     ],
```

