# Comparing `tmp/pyniki-0.0.5.tar.gz` & `tmp/pyniki-0.0.6.tar.gz`

## Comparing `pyniki-0.0.5.tar` & `pyniki-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/curses.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/field.py
--rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/main.py
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/sim.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/ui.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyniki-0.0.5/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.5/LICENSE
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.5/README.md
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.6/src/pyniki/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pyniki-0.0.6/src/pyniki/curses.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 pyniki-0.0.6/src/pyniki/field.py
+-rw-r--r--   0        0        0    15938 2020-02-02 00:00:00.000000 pyniki-0.0.6/src/pyniki/main.py
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 pyniki-0.0.6/src/pyniki/sim.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyniki-0.0.6/src/pyniki/ui.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyniki-0.0.6/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.6/LICENSE
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.6/README.md
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.6/PKG-INFO
```

### Comparing `pyniki-0.0.5/src/pyniki/curses.py` & `pyniki-0.0.6/src/pyniki/curses.py`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.5/src/pyniki/field.py` & `pyniki-0.0.6/src/pyniki/field.py`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.5/src/pyniki/main.py` & `pyniki-0.0.6/src/pyniki/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,22 +400,33 @@
                         if filename is None:
                             active_dialog.filename.txt = old_filename
                             active_dialog.draw()
                             continue
                         active_dialog.filename.txt = filename
                         active_dialog.draw()
 
+                    if active_dialog is robot_dialog:
+                        filename = filename + '.py'
+                    else:
+                        filename = filename + '.rob'
+                    if not os.path.exists(filename):
+                        active_dialog.filename.txt = ''
+                        continue
+                    if active_dialog is robot_dialog:
+                        with open(filename, 'rt') as f:
+                            self.program = f.read()
+                    else:
+                        with open(filename, 'rb') as f:
+                            self.field = pickle.load(f)
+                            self.field.name = field_dialog.filename.txt
+
                 if active_dialog is robot_dialog:
-                    if self.program is None:
-                        self.program = ''
                     self.edit_program()
                     self.draw()
                 else:
-                    if self.field is None:
-                        self.field = Field(10, 15, 1, name=self.field_dialog.filename.txt)
                     edit_field(self.field)
                     self.draw()
             elif CMD == 'NEW':
                 active_dialog.filename.txt = 'NONAME'
                 if active_dialog is robot_dialog:
                     self.program = ''
                     self.edit_program()
```

### Comparing `pyniki-0.0.5/src/pyniki/sim.py` & `pyniki-0.0.6/src/pyniki/sim.py`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.5/src/pyniki/ui.py` & `pyniki-0.0.6/src/pyniki/ui.py`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.5/LICENSE` & `pyniki-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.5/pyproject.toml` & `pyniki-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyNIKI"
-version = "0.0.5"
+version = "0.0.6"
 description = "Classic Niki the robot in Python"
 readme = "README.md"
 license.file = "LICENSE"
 requires-python = ">=3.8"
 authors = [
     { name = "Stephan Rave", email = "stephan.rave@uni-muenster.de" },
 ]
```

### Comparing `pyniki-0.0.5/PKG-INFO` & `pyniki-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNIKI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Classic Niki the robot in Python
 Project-URL: Homepage, https://github.com/sdrave/pyniki
 Author-email: Stephan Rave <stephan.rave@uni-muenster.de>
 Maintainer-email: Stephan Rave <stephan.rave@uni-muenster.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
```

