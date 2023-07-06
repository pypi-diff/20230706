# Comparing `tmp/tkcomponents-4.0.1.tar.gz` & `tmp/tkcomponents-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkcomponents-4.0.1.tar", last modified: Thu Jul  6 03:32:54 2023, max compression
+gzip compressed data, was "tkcomponents-4.0.2.tar", last modified: Thu Jul  6 03:46:05 2023, max compression
```

## Comparing `tkcomponents-4.0.1.tar` & `tkcomponents-4.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.149088 tkcomponents-4.0.1/
--rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-4.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-4.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-06 03:32:54.148086 tkcomponents-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-4.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 03:32:54.149088 tkcomponents-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1194 2023-07-06 03:32:30.000000 tkcomponents-4.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.120086 tkcomponents-4.0.1/tkcomponents/
--rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-4.0.1/tkcomponents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.144088 tkcomponents-4.0.1/tkcomponents/basiccomponents/
--rw-rw-rw-   0        0        0      540 2023-07-06 03:08:39.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/__init__.py
--rw-rw-rw-   0        0        0     1592 2023-06-28 05:29:47.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/alert.py
--rw-rw-rw-   0        0        0     2302 2023-06-28 05:29:47.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/buttonlistbox.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.145087 tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/
--rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/dateticker.py
--rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/timer.py
--rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/constants.py
--rw-rw-rw-   0        0        0     3094 2023-07-06 02:31:39.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/datestepper.py
--rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/labelwrapper.py
--rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/progressbar.py
--rw-rw-rw-   0        0        0     5459 2023-07-06 03:28:51.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/stepper.py
--rw-rw-rw-   0        0        0     2795 2023-07-06 03:08:39.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/steppertable.py
--rw-rw-rw-   0        0        0     2861 2023-07-03 00:51:53.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/stringeditor.py
--rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/textcarousel.py
--rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/timedframe.py
--rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/timercontrol.py
--rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/togglebutton.py
--rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-4.0.1/tkcomponents/basiccomponents/verticalscrollframe.py
--rw-rw-rw-   0        0        0     7621 2023-07-01 02:53:52.000000 tkcomponents-4.0.1/tkcomponents/component.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.147087 tkcomponents-4.0.1/tkcomponents/extensions/
--rw-rw-rw-   0        0        0       74 2023-07-02 09:02:34.000000 tkcomponents-4.0.1/tkcomponents/extensions/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-07-02 09:11:53.000000 tkcomponents-4.0.1/tkcomponents/extensions/draganddrop.py
--rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-4.0.1/tkcomponents/extensions/gridhelper.py
-drwxrwxrwx   0        0        0        0 2023-07-06 03:32:54.131088 tkcomponents-4.0.1/tkcomponents.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 03:32:54.000000 tkcomponents-4.0.1/tkcomponents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:05.531756 tkcomponents-4.0.2/
+-rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-4.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-4.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-06 03:46:05.530757 tkcomponents-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-4.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:46:05.531756 tkcomponents-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2023-07-06 03:45:14.000000 tkcomponents-4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:05.502756 tkcomponents-4.0.2/tkcomponents/
+-rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-4.0.2/tkcomponents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:05.526759 tkcomponents-4.0.2/tkcomponents/basiccomponents/
+-rw-rw-rw-   0        0        0      540 2023-07-06 03:08:39.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/__init__.py
+-rw-rw-rw-   0        0        0     1592 2023-06-28 05:29:47.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/alert.py
+-rw-rw-rw-   0        0        0     2302 2023-06-28 05:29:47.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/buttonlistbox.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:05.527758 tkcomponents-4.0.2/tkcomponents/basiccomponents/classes/
+-rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/classes/dateticker.py
+-rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/classes/timer.py
+-rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/constants.py
+-rw-rw-rw-   0        0        0     3094 2023-07-06 02:31:39.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/datestepper.py
+-rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/labelwrapper.py
+-rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/progressbar.py
+-rw-rw-rw-   0        0        0     5578 2023-07-06 03:36:18.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/stepper.py
+-rw-rw-rw-   0        0        0     2795 2023-07-06 03:08:39.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/steppertable.py
+-rw-rw-rw-   0        0        0     2861 2023-07-03 00:51:53.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/stringeditor.py
+-rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/textcarousel.py
+-rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/timedframe.py
+-rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/timercontrol.py
+-rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/togglebutton.py
+-rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-4.0.2/tkcomponents/basiccomponents/verticalscrollframe.py
+-rw-rw-rw-   0        0        0     7621 2023-07-01 02:53:52.000000 tkcomponents-4.0.2/tkcomponents/component.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:05.530757 tkcomponents-4.0.2/tkcomponents/extensions/
+-rw-rw-rw-   0        0        0       74 2023-07-02 09:02:34.000000 tkcomponents-4.0.2/tkcomponents/extensions/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-07-02 09:11:53.000000 tkcomponents-4.0.2/tkcomponents/extensions/draganddrop.py
+-rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-4.0.2/tkcomponents/extensions/gridhelper.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:46:05.513757 tkcomponents-4.0.2/tkcomponents.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-06 03:46:05.000000 tkcomponents-4.0.2/tkcomponents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-07-06 03:46:05.000000 tkcomponents-4.0.2/tkcomponents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:46:05.000000 tkcomponents-4.0.2/tkcomponents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-06 03:46:05.000000 tkcomponents-4.0.2/tkcomponents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 03:46:05.000000 tkcomponents-4.0.2/tkcomponents.egg-info/top_level.txt
```

### Comparing `tkcomponents-4.0.1/LICENSE.txt` & `tkcomponents-4.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/PKG-INFO` & `tkcomponents-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 4.0.1
+Version: 4.0.2
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.1.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.2.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-4.0.1/README.md` & `tkcomponents-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/setup.py` & `tkcomponents-4.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 setup(
     name="tkcomponents",
     packages=[
         "tkcomponents", "tkcomponents.extensions", "tkcomponents.basiccomponents",
         "tkcomponents.basiccomponents.classes"
     ],
-    version="4.0.1",
+    version="4.0.2",
     license="MIT",
     description="An OOP framework for Tkinter, inspired by React",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="immijimmi",
     author_email="immijimmi1@gmail.com",
     url="https://github.com/immijimmi/tkcomponents",
-    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.1.tar.gz",
+    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.2.tar.gz",
     keywords=[
         'ui', 'gui', 'graphical', 'user', 'interface'
     ],
     install_requires=[
         'objectextensions~=2.0.2'
     ],
     classifiers=[
```

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/__init__.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/__init__.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/alert.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/alert.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/buttonlistbox.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/buttonlistbox.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/classes/timer.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/classes/timer.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/datestepper.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/datestepper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/labelwrapper.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/labelwrapper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/progressbar.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/progressbar.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/stepper.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/stepper.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,11 +122,13 @@
 
     def _set_button_states(self):
         all_buttons = self.children["before_buttons"] + self.children["after_buttons"]
 
         for (step_label, step_amount), button in all_buttons:
             value_after_button_press = self.value + step_amount
 
-            if (value_after_button_press < self.min) or (value_after_button_press > self.max):
+            if (self.min is not None) and (value_after_button_press < self.min):
+                button.config(state="disabled")
+            elif (self.max is not None) and (value_after_button_press > self.max):
                 button.config(state="disabled")
             else:
                 button.config(state="normal")
```

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/steppertable.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/steppertable.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/stringeditor.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/stringeditor.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/textcarousel.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/textcarousel.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/timedframe.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/timedframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/timercontrol.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/timercontrol.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/togglebutton.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/togglebutton.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/basiccomponents/verticalscrollframe.py` & `tkcomponents-4.0.2/tkcomponents/basiccomponents/verticalscrollframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/component.py` & `tkcomponents-4.0.2/tkcomponents/component.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/extensions/draganddrop.py` & `tkcomponents-4.0.2/tkcomponents/extensions/draganddrop.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents/extensions/gridhelper.py` & `tkcomponents-4.0.2/tkcomponents/extensions/gridhelper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-4.0.1/tkcomponents.egg-info/PKG-INFO` & `tkcomponents-4.0.2/tkcomponents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 4.0.1
+Version: 4.0.2
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.1.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.2.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-4.0.1/tkcomponents.egg-info/SOURCES.txt` & `tkcomponents-4.0.2/tkcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

