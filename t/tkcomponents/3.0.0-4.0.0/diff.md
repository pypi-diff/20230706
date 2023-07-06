# Comparing `tmp/tkcomponents-3.0.0.tar.gz` & `tmp/tkcomponents-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkcomponents-3.0.0.tar", last modified: Mon Jul  3 04:49:04 2023, max compression
+gzip compressed data, was "tkcomponents-4.0.0.tar", last modified: Thu Jul  6 03:16:39 2023, max compression
```

## Comparing `tkcomponents-3.0.0.tar` & `tkcomponents-4.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.185560 tkcomponents-3.0.0/
--rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-3.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-03 04:49:04.185560 tkcomponents-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-3.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 04:49:04.186560 tkcomponents-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1194 2023-07-03 04:47:52.000000 tkcomponents-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.132562 tkcomponents-3.0.0/tkcomponents/
--rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-3.0.0/tkcomponents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.169561 tkcomponents-3.0.0/tkcomponents/basiccomponents/
--rw-rw-rw-   0        0        0      564 2023-07-02 09:02:35.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/__init__.py
--rw-rw-rw-   0        0        0     1592 2023-06-28 05:29:47.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/alert.py
--rw-rw-rw-   0        0        0     2302 2023-06-28 05:29:47.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/buttonlistbox.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.182560 tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/
--rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/dateticker.py
--rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/timer.py
--rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/constants.py
--rw-rw-rw-   0        0        0     3068 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/datestepper.py
--rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/labelwrapper.py
--rw-rw-rw-   0        0        0     4981 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/numberstepper.py
--rw-rw-rw-   0        0        0     2568 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/numbersteppertable.py
--rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/progressbar.py
--rw-rw-rw-   0        0        0     2861 2023-07-03 00:51:53.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/stringeditor.py
--rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/textcarousel.py
--rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/timedframe.py
--rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/timercontrol.py
--rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/togglebutton.py
--rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/verticalscrollframe.py
--rw-rw-rw-   0        0        0     7621 2023-07-01 02:53:52.000000 tkcomponents-3.0.0/tkcomponents/component.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.184561 tkcomponents-3.0.0/tkcomponents/extensions/
--rw-rw-rw-   0        0        0       74 2023-07-02 09:02:34.000000 tkcomponents-3.0.0/tkcomponents/extensions/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-07-02 09:11:53.000000 tkcomponents-3.0.0/tkcomponents/extensions/draganddrop.py
--rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-3.0.0/tkcomponents/extensions/gridhelper.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.155562 tkcomponents-3.0.0/tkcomponents.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1154 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.613004 tkcomponents-4.0.0/
+-rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-4.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-06 03:16:39.613004 tkcomponents-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-4.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 03:16:39.613004 tkcomponents-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2023-07-06 03:14:08.000000 tkcomponents-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.577003 tkcomponents-4.0.0/tkcomponents/
+-rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-4.0.0/tkcomponents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.609005 tkcomponents-4.0.0/tkcomponents/basiccomponents/
+-rw-rw-rw-   0        0        0      540 2023-07-06 03:08:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/__init__.py
+-rw-rw-rw-   0        0        0     1592 2023-06-28 05:29:47.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/alert.py
+-rw-rw-rw-   0        0        0     2302 2023-06-28 05:29:47.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/buttonlistbox.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.610005 tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/
+-rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/dateticker.py
+-rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/timer.py
+-rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/constants.py
+-rw-rw-rw-   0        0        0     3094 2023-07-06 02:31:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/datestepper.py
+-rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/labelwrapper.py
+-rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/progressbar.py
+-rw-rw-rw-   0        0        0     5471 2023-07-06 02:31:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/stepper.py
+-rw-rw-rw-   0        0        0     2795 2023-07-06 03:08:39.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/steppertable.py
+-rw-rw-rw-   0        0        0     2861 2023-07-03 00:51:53.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/stringeditor.py
+-rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/textcarousel.py
+-rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/timedframe.py
+-rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/timercontrol.py
+-rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/togglebutton.py
+-rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-4.0.0/tkcomponents/basiccomponents/verticalscrollframe.py
+-rw-rw-rw-   0        0        0     7621 2023-07-01 02:53:52.000000 tkcomponents-4.0.0/tkcomponents/component.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.612003 tkcomponents-4.0.0/tkcomponents/extensions/
+-rw-rw-rw-   0        0        0       74 2023-07-02 09:02:34.000000 tkcomponents-4.0.0/tkcomponents/extensions/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-07-02 09:11:53.000000 tkcomponents-4.0.0/tkcomponents/extensions/draganddrop.py
+-rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-4.0.0/tkcomponents/extensions/gridhelper.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:16:39.596004 tkcomponents-4.0.0/tkcomponents.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 03:16:39.000000 tkcomponents-4.0.0/tkcomponents.egg-info/top_level.txt
```

### Comparing `tkcomponents-3.0.0/LICENSE.txt` & `tkcomponents-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/PKG-INFO` & `tkcomponents-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 3.0.0
+Version: 4.0.0
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v3.0.0.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.0.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-3.0.0/README.md` & `tkcomponents-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/setup.py` & `tkcomponents-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 setup(
     name="tkcomponents",
     packages=[
         "tkcomponents", "tkcomponents.extensions", "tkcomponents.basiccomponents",
         "tkcomponents.basiccomponents.classes"
     ],
-    version="3.0.0",
+    version="4.0.0",
     license="MIT",
     description="An OOP framework for Tkinter, inspired by React",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="immijimmi",
     author_email="immijimmi1@gmail.com",
     url="https://github.com/immijimmi/tkcomponents",
-    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v3.0.0.tar.gz",
+    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.0.tar.gz",
     keywords=[
         'ui', 'gui', 'graphical', 'user', 'interface'
     ],
     install_requires=[
         'objectextensions~=2.0.2'
     ],
     classifiers=[
```

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/alert.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/alert.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/buttonlistbox.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/buttonlistbox.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/timer.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/classes/timer.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/datestepper.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/datestepper.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 from ..component import Component
 from ..extensions import GridHelper
 from .constants import Constants
 from .classes.dateticker import DateTicker
 
 
 class DateStepper(Component.with_extensions(GridHelper)):
-    def __init__(self, container, date_text_format="%Y/%m/%d",
-                 get_data=None, on_change=(lambda stepper, increment_amount: None), update_interval_ms=None, styles=None):
-        super().__init__(container, get_data=get_data, on_change=on_change,
-                         update_interval_ms=update_interval_ms, styles=styles)
+    def __init__(
+            self, container, date_text_format="%Y/%m/%d",
+            get_data=None, on_change=(lambda stepper, increment_amount: None), update_interval_ms=None, styles=None
+    ):
+        super().__init__(
+            container, get_data=get_data, on_change=on_change,
+            update_interval_ms=update_interval_ms, styles=styles
+        )
 
         self.date_text_format = date_text_format
 
         self._date_ticker = DateTicker()
 
         styles = styles or {}
         self.styles["button"] = styles.get("button", {})
```

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/labelwrapper.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/labelwrapper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/numberstepper.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/stepper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,132 @@
 from tkinter import Label, Button, StringVar
 from functools import partial
+from typing import Callable, Any, Optional
 
 from ..component import Component
 from ..extensions import GridHelper
 
 
-class NumberStepper(Component.with_extensions(GridHelper)):
-    def __init__(self, container, get_data=None, on_change=(lambda stepper, increment_amount: None),
-                 text_format="{0}", step_amounts=(1,), limits=(None, None), is_horizontal=True,
-                 update_interval_ms=None, styles=None):
+class Stepper(Component.with_extensions(GridHelper)):
+    def __init__(
+        self, container,
+        get_data: Optional[Callable[["Stepper"], Any]] = None,
+        on_change: Callable[["Stepper", Any], None] = (lambda stepper, step_amount: None),
+        before_steps: tuple[tuple[str,  Any], ...] = (("-", -1),),
+        after_steps: tuple[tuple[str,  Any], ...] = (("+", 1),),
+        format_label: Callable[["Stepper"], str] = (lambda stepper: str(stepper.value)),
+        limits: Optional[tuple[Any, Any]] = (None, None), is_horizontal: bool = True,
+        update_interval_ms=None, styles=None
+    ):
         super().__init__(container, get_data=get_data, on_change=on_change,
                          update_interval_ms=update_interval_ms, styles=styles)
 
-        self.text_format = text_format
+        self.before_steps = before_steps
+        self.after_steps = after_steps
+        self.format_label = format_label
+        self.is_horizontal = is_horizontal
 
         self.min = limits[0]
         self.max = limits[1]
 
-        self.is_horizontal = is_horizontal
-        self.step_amounts = step_amounts  # Provide only positive values, they will be mirrored for negative values
-
         styles = styles or {}
         self.styles["button"] = styles.get("button", {})
         self.styles["label"] = styles.get("label", {})
 
         self.value = self._get_data(self) if self._get_data else 0
 
-        self._value__var = StringVar()
-        self._value__var.set(self.text_format.format(self.value))
+        self._label_var = StringVar()
+        self._label_var.set(self.format_label(self.value))
 
     def _update(self):
         if self._get_data:
             self.value = self._get_data(self)
 
-        self._value__var.set(self.text_format.format(self.value))
+        self._label_var.set(self.format_label(self.value))
 
         self._set_button_states()
 
     def _render(self):
-        self.children["minus_buttons"] = []
-        self.children["plus_buttons"] = []
+        self.children["before_buttons"] = []
+        self.children["after_buttons"] = []
         self.children["label"] = None
 
-        row_stretch = [0] if self.is_horizontal else [len(self.step_amounts)]
-        column_stretch = [len(self.step_amounts)] if self.is_horizontal else [0]
+        row_stretch = [0] if self.is_horizontal else [len(self.before_steps)]
+        column_stretch = [len(self.before_steps)] if self.is_horizontal else [0]
         self._apply_frame_stretch(rows=row_stretch, columns=column_stretch)
 
         row_index, column_index = 0, 0
 
         if self.is_horizontal:
-            for step_amount in reversed(self.step_amounts):
-                button = Button(self._frame, text="-{0}".format("" if step_amount == 1 else step_amount),
-                                command=partial(self._handle_click, -step_amount), **self.styles["button"])
-                self.children["minus_buttons"].append(button)
+            for step_label, step_amount in self.before_steps:
+                button = Button(
+                    self._frame, text=step_label,
+                    command=partial(self._handle_click, step_amount), **self.styles["button"]
+                )
+                self.children["before_buttons"].append(((step_label, step_amount), button))
                 button.grid(row=row_index, column=column_index, sticky="nswe")
                 column_index += 1
 
-            self.children["label"] = Label(self._frame, textvariable=self._value__var, **self.styles["label"])
-            self.children["label"].grid(row=row_index, column=column_index, sticky="nswe")
+            label = Label(self._frame, textvariable=self._label_var, **self.styles["label"])
+            self.children["label"] = label
+            label.grid(row=row_index, column=column_index, sticky="nswe")
             column_index += 1
 
-            for step_amount in self.step_amounts:
-                button = Button(self._frame, text="+{0}".format("" if step_amount == 1 else step_amount),
-                                command=partial(self._handle_click, step_amount), **self.styles["button"])
-                self.children["plus_buttons"].append(button)
+            for step_label, step_amount in self.after_steps:
+                button = Button(
+                    self._frame, text=step_label,
+                    command=partial(self._handle_click, step_amount), **self.styles["button"]
+                )
+                self.children["after_buttons"].append(((step_label, step_amount), button))
                 button.grid(row=row_index, column=column_index, sticky="nswe")
                 column_index += 1
 
         else:
-            for step_amount in reversed(self.step_amounts):
-                button = Button(self._frame, text="+{0}".format("" if step_amount == 1 else step_amount),
-                                command=partial(self._handle_click, step_amount), **self.styles["button"])
-                self.children["plus_buttons"].append(button)
+            for step_label, step_amount in self.before_steps:
+                button = Button(
+                    self._frame, text=step_label,
+                    command=partial(self._handle_click, step_amount), **self.styles["button"]
+                )
+                self.children["before_buttons"].append(((step_label, step_amount), button))
                 button.grid(row=row_index, column=column_index, sticky="nswe")
                 row_index += 1
 
-            self.children["label"] = Label(self._frame, textvariable=self._value__var, **self.styles["label"])
-            self.children["label"].grid(row=row_index, column=column_index, sticky="nswe")
+            label = Label(self._frame, textvariable=self._label_var, **self.styles["label"])
+            self.children["label"] = label
+            label.grid(row=row_index, column=column_index, sticky="nswe")
             row_index += 1
 
-            for step_amount in self.step_amounts:
-                button = Button(self._frame, text="-{0}".format("" if step_amount == 1 else step_amount),
-                                command=partial(self._handle_click, -step_amount), **self.styles["button"])
-                self.children["minus_buttons"].append(button)
+            for step_label, step_amount in self.after_steps:
+                button = Button(
+                    self._frame, text=step_label,
+                    command=partial(self._handle_click, step_amount), **self.styles["button"]
+                )
+                self.children["after_buttons"].append(((step_label, step_amount), button))
                 button.grid(row=row_index, column=column_index, sticky="nswe")
                 row_index += 1
 
         self._set_button_states()
 
-    def _handle_click(self, increment_amount):
-        if self._get_data:
-            self.value = self._get_data(self)
+    def _handle_click(self, step_amount):
+        self.value += step_amount
 
-        self.value += increment_amount
+        # Added for redundancy
         if self.min is not None:
             self.value = max(self.min, self.value)
         if self.max is not None:
             self.value = min(self.max, self.value)
 
-        self._on_change(self, increment_amount)
+        self._on_change(self, step_amount)
 
         if self.exists:
             self._update()
 
     def _set_button_states(self):
-        for button in self.children["minus_buttons"]:
-            button.config(state="disabled" if self.value == self.min else "normal")
+        all_buttons = self.children["before_buttons"] + self.children["after_buttons"]
+
+        for (step_label, step_amount), button in all_buttons:
+            value_after_button_press = self.value + step_amount
 
-        for button in self.children["plus_buttons"]:
-            button.config(state="disabled" if self.value == self.max else "normal")
+            if (value_after_button_press < self.min) or (value_after_button_press > self.max):
+                button.config(state="disabled")
+            else:
+                button.config(state="normal")
```

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/numbersteppertable.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/steppertable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from functools import partial
 from tkinter import Label
+from typing import Any, Optional, Callable
 
 from ..component import Component
 from ..extensions import GridHelper
-from .numberstepper import NumberStepper
+from .stepper import Stepper
 
 
-class NumberStepperTable(Component.with_extensions(GridHelper)):
-    def __init__(self, container, axis_labels, axis_values,
-                 get_data=None, on_change=(lambda x_value, y_value, stepper, increment_amount: None),
-                 text_format="{0}", step_amounts=(1,), limits=(None, None), is_horizontal=True,
-                 update_interval_ms=None, styles=None):
+class StepperTable(Component.with_extensions(GridHelper)):
+    def __init__(
+        self, container,
+        axis_labels: tuple[tuple[str, ...], tuple[str, ...]], axis_values: tuple[tuple[Any, ...], tuple[Any, ...]],
+        get_data: Optional[Callable[[Any, Any, Stepper], Any]] = None,
+        on_change=(lambda x_value, y_value, stepper, step_amount: None),
+        before_steps=(("-", -1),), after_steps=(("+", 1),),
+        format_label=(lambda stepper: str(stepper.value)), limits=(None, None), is_horizontal=True,
+        update_interval_ms=None, styles=None
+    ):
         super().__init__(container, get_data=get_data, on_change=on_change, styles=styles)
 
+        styles = styles or {}
+        self.styles["x_label"] = styles.get("x_label", {})
+        self.styles["y_label"] = styles.get("y_label", {})
+
         self._stepper_kwargs = {
-            "text_format": text_format,
-            "step_amounts": step_amounts,
+            "before_steps": before_steps,
+            "after_steps": after_steps,
+            "format_label": format_label,
             "limits": limits,
-            "update_interval_ms": update_interval_ms,
             "is_horizontal": is_horizontal,
-            "styles": styles.get("number_stepper", {})
+            "update_interval_ms": update_interval_ms,
+            "styles": styles.get("stepper", {})
         }
 
         self.axis_labels = axis_labels
         self.axis_values = axis_values
 
-        styles = styles or {}
-        self.styles["x_label"] = styles.get("x_label", {})
-        self.styles["y_label"] = styles.get("y_label", {})
-
     def _render(self):
         self.children["axis_labels"] = [[], []]
-        self.children["number_steppers"] = {}
+        self.children["steppers"] = {}
 
         self._apply_frame_stretch(columns=[0], rows=[1])
 
         for x_index, x_label in enumerate(self.axis_labels[0]):
             label = Label(self._frame, text=x_label, **self.styles["x_label"])
             self.children["axis_labels"][0].append(label)
             label.grid(row=0, column=x_index+1, sticky="nswe")
@@ -43,15 +50,15 @@
         for y_index, y_label in enumerate(self.axis_labels[1]):
             label = Label(self._frame, text=y_label, **self.styles["y_label"])
             self.children["axis_labels"][1].append(label)
             label.grid(row=y_index+2, column=0, sticky="nswe")
 
         for x_index, x_value in enumerate(self.axis_values[0]):
             for y_index, y_value in enumerate(self.axis_values[1]):
-                number_stepper = NumberStepper(
+                stepper = Stepper(
                     self._frame,
                     get_data=partial(self._get_data, x_value, y_value) if self._get_data else None,
                     on_change=partial(self._on_change, x_value, y_value),
                     **self._stepper_kwargs
                 )
-                self.children["number_steppers"][(x_index, y_index)] = number_stepper
-                number_stepper.render().grid(row=y_index+2, column=x_index+1, sticky="nswe")
+                self.children["steppers"][(x_index, y_index)] = stepper
+                stepper.render().grid(row=y_index+2, column=x_index+1, sticky="nswe")
```

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/progressbar.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/progressbar.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/stringeditor.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/stringeditor.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/textcarousel.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/textcarousel.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/timedframe.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/timedframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/timercontrol.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/timercontrol.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/togglebutton.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/togglebutton.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/basiccomponents/verticalscrollframe.py` & `tkcomponents-4.0.0/tkcomponents/basiccomponents/verticalscrollframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/component.py` & `tkcomponents-4.0.0/tkcomponents/component.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/extensions/draganddrop.py` & `tkcomponents-4.0.0/tkcomponents/extensions/draganddrop.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents/extensions/gridhelper.py` & `tkcomponents-4.0.0/tkcomponents/extensions/gridhelper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-3.0.0/tkcomponents.egg-info/PKG-INFO` & `tkcomponents-4.0.0/tkcomponents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 3.0.0
+Version: 4.0.0
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v3.0.0.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v4.0.0.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-3.0.0/tkcomponents.egg-info/SOURCES.txt` & `tkcomponents-4.0.0/tkcomponents.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 tkcomponents.egg-info/top_level.txt
 tkcomponents/basiccomponents/__init__.py
 tkcomponents/basiccomponents/alert.py
 tkcomponents/basiccomponents/buttonlistbox.py
 tkcomponents/basiccomponents/constants.py
 tkcomponents/basiccomponents/datestepper.py
 tkcomponents/basiccomponents/labelwrapper.py
-tkcomponents/basiccomponents/numberstepper.py
-tkcomponents/basiccomponents/numbersteppertable.py
 tkcomponents/basiccomponents/progressbar.py
+tkcomponents/basiccomponents/stepper.py
+tkcomponents/basiccomponents/steppertable.py
 tkcomponents/basiccomponents/stringeditor.py
 tkcomponents/basiccomponents/textcarousel.py
 tkcomponents/basiccomponents/timedframe.py
 tkcomponents/basiccomponents/timercontrol.py
 tkcomponents/basiccomponents/togglebutton.py
 tkcomponents/basiccomponents/verticalscrollframe.py
 tkcomponents/basiccomponents/classes/dateticker.py
```

