# Comparing `tmp/tkcomponents-4.0.0.tar.gz` & `tmp/tkcomponents-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkcomponents-4.0.0.tar", last modified: Thu Jul  6 03:16:39 2023, max compression
+gzip compressed data, was "tkcomponents-4.0.1.tar", last modified: Thu Jul  6 03:32:54 2023, max compression
```

## Comparing `tkcomponents-4.0.0.tar` & `tkcomponents-4.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.613004 tkcomponents-4.0.0/
--rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-4.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-4.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-06 03:16:39.613004 tkcomponents-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-4.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 03:16:39.613004 tkcomponents-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1194 2023-07-06 03:14:08.000000 tkcomponents-4.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.577003 tkcomponents-4.0.0/tkcomponents/
--rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-4.0.0/tkcomponents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.609005 tkcomponents-4.0.0/tkcomponents/basiccomponents/
--rw-rw-rw-   0        0        0      540 2023-07-06 03:08:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/__init__.py
--rw-rw-rw-   0        0        0     1592 2023-06-28 05:29:47.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/alert.py
--rw-rw-rw-   0        0        0     2302 2023-06-28 05:29:47.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/buttonlistbox.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.610005 tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/
--rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/dateticker.py
--rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/timer.py
--rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/constants.py
--rw-rw-rw-   0        0        0     3094 2023-07-06 02:31:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/datestepper.py
--rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/labelwrapper.py
--rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/progressbar.py
--rw-rw-rw-   0        0        0     5471 2023-07-06 02:31:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/stepper.py
--rw-rw-rw-   0        0        0     2795 2023-07-06 03:08:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/steppertable.py
--rw-rw-rw-   0        0        0     2861 2023-07-03 00:51:53.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/stringeditor.py
--rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/textcarousel.py
--rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/timedframe.py
--rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/timercontrol.py
--rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/togglebutton.py
--rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/verticalscrollframe.py
--rw-rw-rw-   0        0        0     7621 2023-07-01 02:53:52.000000 tkcomponents-4.0.0/tkcomponents/component.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.612003 tkcomponents-4.0.0/tkcomponents/extensions/
--rw-rw-rw-   0        0        0       74 2023-07-02 09:02:34.000000 tkcomponents-4.0.0/tkcomponents/extensions/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-07-02 09:11:53.000000 tkcomponents-4.0.0/tkcomponents/extensions/draganddrop.py
--rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-4.0.0/tkcomponents/extensions/gridhelper.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.596004 tkcomponents-4.0.0/tkcomponents.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.149088 tkcomponents-4.0.1/
+-rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-4.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-4.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-06 03:32:54.148086 tkcomponents-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-4.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:32:54.149088 tkcomponents-4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2023-07-06 03:32:30.000000 tkcomponents-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.120086 tkcomponents-4.0.1/tkcomponents/
+-rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-4.0.1/tkcomponents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.144088 tkcomponents-4.0.1/tkcomponents/basiccomponents/
+-rw-rw-rw-   0        0        0      540 2023-07-06 03:08:39.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/__init__.py
+-rw-rw-rw-   0        0        0     1592 2023-06-28 05:29:47.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/alert.py
+-rw-rw-rw-   0        0        0     2302 2023-06-28 05:29:47.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/buttonlistbox.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.145087 tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/
+-rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/dateticker.py
+-rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/timer.py
+-rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/constants.py
+-rw-rw-rw-   0        0        0     3094 2023-07-06 02:31:39.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/datestepper.py
+-rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/labelwrapper.py
+-rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/progressbar.py
+-rw-rw-rw-   0        0        0     5459 2023-07-06 03:28:51.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/stepper.py
+-rw-rw-rw-   0        0        0     2795 2023-07-06 03:08:39.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/steppertable.py
+-rw-rw-rw-   0        0        0     2861 2023-07-03 00:51:53.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/stringeditor.py
+-rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/textcarousel.py
+-rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/timedframe.py
+-rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/timercontrol.py
+-rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/togglebutton.py
+-rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/verticalscrollframe.py
+-rw-rw-rw-   0        0        0     7621 2023-07-01 02:53:52.000000 tkcomponents-4.0.1/tkcomponents/component.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.147087 tkcomponents-4.0.1/tkcomponents/extensions/
+-rw-rw-rw-   0        0        0       74 2023-07-02 09:02:34.000000 tkcomponents-4.0.1/tkcomponents/extensions/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-07-02 09:11:53.000000 tkcomponents-4.0.1/tkcomponents/extensions/draganddrop.py
+-rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-4.0.1/tkcomponents/extensions/gridhelper.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.131088 tkcomponents-4.0.1/tkcomponents.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/top_level.txt
```

### Comparing `tkcomponents-4.0.0/LICENSE.txt` & `tkcomponents-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/PKG-INFO` & `tkcomponents-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 4.0.0
+Version: 4.0.1
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.0.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.1.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-4.0.0/README.md` & `tkcomponents-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/setup.py` & `tkcomponents-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 setup(
     name="tkcomponents",
     packages=[
         "tkcomponents", "tkcomponents.extensions", "tkcomponents.basiccomponents",
         "tkcomponents.basiccomponents.classes"
     ],
-    version="4.0.0",
+    version="4.0.1",
     license="MIT",
     description="An OOP framework for Tkinter, inspired by React",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="immijimmi",
     author_email="immijimmi1@gmail.com",
     url="https://github.com/immijimmi/tkcomponents",
-    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.0.tar.gz",
+    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.1.tar.gz",
     keywords=[
         'ui', 'gui', 'graphical', 'user', 'interface'
     ],
     install_requires=[
         'objectextensions~=2.0.2'
     ],
     classifiers=[
```

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/__init__.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/__init__.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/alert.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/alert.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/buttonlistbox.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/buttonlistbox.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/timer.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/timer.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/datestepper.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/datestepper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/labelwrapper.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/labelwrapper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/progressbar.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/progressbar.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/stepper.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/stepper.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,21 @@
         styles = styles or {}
         self.styles["button"] = styles.get("button", {})
         self.styles["label"] = styles.get("label", {})
 
         self.value = self._get_data(self) if self._get_data else 0
 
         self._label_var = StringVar()
-        self._label_var.set(self.format_label(self.value))
+        self._label_var.set(self.format_label(self))
 
     def _update(self):
         if self._get_data:
             self.value = self._get_data(self)
 
-        self._label_var.set(self.format_label(self.value))
+        self._label_var.set(self.format_label(self))
 
         self._set_button_states()
 
     def _render(self):
         self.children["before_buttons"] = []
         self.children["after_buttons"] = []
         self.children["label"] = None
```

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/steppertable.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/steppertable.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/stringeditor.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/stringeditor.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/textcarousel.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/textcarousel.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/timedframe.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/timedframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/timercontrol.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/timercontrol.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/togglebutton.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/togglebutton.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/basiccomponents/verticalscrollframe.py` & `tkcomponents-4.0.1/tkcomponents/basiccomponents/verticalscrollframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/component.py` & `tkcomponents-4.0.1/tkcomponents/component.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/extensions/draganddrop.py` & `tkcomponents-4.0.1/tkcomponents/extensions/draganddrop.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents/extensions/gridhelper.py` & `tkcomponents-4.0.1/tkcomponents/extensions/gridhelper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.0/tkcomponents.egg-info/PKG-INFO` & `tkcomponents-4.0.1/tkcomponents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 4.0.0
+Version: 4.0.1
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.0.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.1.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-4.0.0/tkcomponents.egg-info/SOURCES.txt` & `tkcomponents-4.0.1/tkcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

