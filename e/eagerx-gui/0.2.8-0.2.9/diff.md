# Comparing `tmp/eagerx_gui-0.2.8.tar.gz` & `tmp/eagerx_gui-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagerx_gui-0.2.8.tar", max compression
+gzip compressed data, was "eagerx_gui-0.2.9.tar", max compression
```

## Comparing `eagerx_gui-0.2.8.tar` & `eagerx_gui-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2022-08-02 09:15:30.604617 eagerx_gui-0.2.8/LICENSE
--rw-r--r--   0        0        0     2165 2022-08-02 09:15:38.493094 eagerx_gui-0.2.8/eagerx_gui/__init__.py
--rw-r--r--   0        0        0     1117 2022-08-02 09:15:30.604617 eagerx_gui-0.2.8/eagerx_gui/configuration.py
--rw-r--r--   0        0        0     8392 2022-08-02 09:15:30.608617 eagerx_gui-0.2.8/eagerx_gui/gui.py
--rw-r--r--   0        0        0    12841 2022-08-02 09:15:30.608617 eagerx_gui-0.2.8/eagerx_gui/gui_node.py
--rw-r--r--   0        0        0    13688 2022-08-02 09:15:30.608617 eagerx_gui-0.2.8/eagerx_gui/gui_terminal.py
--rw-r--r--   0        0        0      958 2022-08-02 09:15:30.608617 eagerx_gui-0.2.8/eagerx_gui/gui_view.py
--rw-r--r--   0        0        0     1907 2022-08-02 09:15:30.608617 eagerx_gui-0.2.8/eagerx_gui/pyqtgraph_utils.py
--rw-r--r--   0        0        0    11130 2022-08-02 09:15:30.608617 eagerx_gui-0.2.8/eagerx_gui/utils.py
--rw-r--r--   0        0        0     1033 2022-08-02 09:15:38.493094 eagerx_gui-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      776 2022-08-02 09:15:44.710691 eagerx_gui-0.2.8/setup.py
--rw-r--r--   0        0        0      844 2022-08-02 09:15:44.710981 eagerx_gui-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2482 2022-08-02 14:23:32.847695 eagerx_gui-0.2.9/eagerx_gui/__init__.py
+-rw-r--r--   0        0        0     1117 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/eagerx_gui/configuration.py
+-rw-r--r--   0        0        0     8392 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/eagerx_gui/gui.py
+-rw-r--r--   0        0        0    12841 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/eagerx_gui/gui_node.py
+-rw-r--r--   0        0        0    13688 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/eagerx_gui/gui_terminal.py
+-rw-r--r--   0        0        0      958 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/eagerx_gui/gui_view.py
+-rw-r--r--   0        0        0     1907 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/eagerx_gui/pyqtgraph_utils.py
+-rw-r--r--   0        0        0    11130 2022-08-02 14:23:20.951256 eagerx_gui-0.2.9/eagerx_gui/utils.py
+-rw-r--r--   0        0        0     1033 2022-08-02 14:23:32.847695 eagerx_gui-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      776 2022-08-02 14:23:41.313053 eagerx_gui-0.2.9/setup.py
+-rw-r--r--   0        0        0      844 2022-08-02 14:23:41.313413 eagerx_gui-0.2.9/PKG-INFO
```

### Comparing `eagerx_gui-0.2.8/LICENSE` & `eagerx_gui-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/eagerx_gui/__init__.py` & `eagerx_gui-0.2.9/eagerx_gui/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 import os
 
 # Set PyQt backend
 for lib in ["PyQt6", "PyQt5"]:
     try:
         __import__(lib)
@@ -11,20 +11,22 @@
     except ImportError:
         pass
 
 import pyqtgraph as pg
 import pyqtgraph.exporters
 import sys
 import numpy as np
+import atexit
 from pyqtgraph.Qt import QtWidgets, QtGui
 from eagerx_gui.gui import Gui
 
 
 def launch_gui(state, is_engine=False):
     app = QtWidgets.QApplication(sys.argv)
+    atexit.register(app.quit)
 
     ## Create main window with grid layout
     win = QtWidgets.QMainWindow()
     win.setWindowTitle("EAGERx Graph")
     cw = QtWidgets.QWidget()
     win.setCentralWidget(cw)
     layout = QtWidgets.QGridLayout()
@@ -40,19 +42,20 @@
 
     app.exec()
     state["gui_state"] = rx_gui.graph._state["gui_state"]
     app.quit()
     return state
 
 
-def render_gui(state, shape=None, is_engine=False):
-    if shape is None:
-        shape = [1920, 1080]
+def render_gui(state, resolution=None, is_engine=False, filename=None):
+    if resolution is None:
+        resolution = [1920, 1080]
 
     app = QtWidgets.QApplication(sys.argv)
+    atexit.register(app.quit)
 
     ## Create main window with grid layout
     win = QtWidgets.QMainWindow()
     win.setWindowTitle("EAGERx Graph")
     cw = QtWidgets.QWidget()
     win.setCentralWidget(cw)
     layout = QtWidgets.QGridLayout()
@@ -62,17 +65,23 @@
     w = rx_gui.widget()
 
     # Add flowchart control panel to the main window
     layout.addWidget(w, 0, 0, 2, 1)
 
     win.show()
 
+    if filename is not None:
+        if not filename.endswith(".svg"):
+            filename += ".svg"
+        svgexporter = pg.exporters.SVGExporter(w.view.scene())
+        svgexporter.export(filename)
+
     exporter = pg.exporters.ImageExporter(w.view.scene())
-    exporter.parameters()["width"] = shape[0]
-    exporter.parameters()["height"] = shape[1]
+    exporter.parameters()["width"] = resolution[0]
+    exporter.parameters()["height"] = resolution[1]
 
     png = exporter.export(toBytes=True)
     png.convertToFormat(QtGui.QImage.Format.Format_RGB32)
 
     width = png.width()
     height = png.height()
```

### Comparing `eagerx_gui-0.2.8/eagerx_gui/configuration.py` & `eagerx_gui-0.2.9/eagerx_gui/configuration.py`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/eagerx_gui/gui.py` & `eagerx_gui-0.2.9/eagerx_gui/gui.py`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/eagerx_gui/gui_node.py` & `eagerx_gui-0.2.9/eagerx_gui/gui_node.py`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/eagerx_gui/gui_terminal.py` & `eagerx_gui-0.2.9/eagerx_gui/gui_terminal.py`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/eagerx_gui/gui_view.py` & `eagerx_gui-0.2.9/eagerx_gui/gui_view.py`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/eagerx_gui/pyqtgraph_utils.py` & `eagerx_gui-0.2.9/eagerx_gui/pyqtgraph_utils.py`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/eagerx_gui/utils.py` & `eagerx_gui-0.2.9/eagerx_gui/utils.py`

 * *Files identical despite different names*

### Comparing `eagerx_gui-0.2.8/pyproject.toml` & `eagerx_gui-0.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "eagerx_gui"
-version = "0.2.8"
+version = "0.2.9"
 license = "Apache2.0"
 description = "GUI to visualise graphs in EAGERx."
 authors = ["Jelle Luijkx <j.d.luijkx@tudelft.nl>", "Bas van der Heijden <d.s.vanderheijden@tudelft.nl>"]
 homepage = "https://github.com/eager-dev/eagerx_gui"
 repository = "https://github.com/eager-dev/eagerx_gui"
 documentation = "https://eagerx.readthedocs.io/en/master/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-eagerx = "^0.1.27"
+eagerx = "^0.1.30"
 opencv-python = "^4.5"
 pyqtgraph = "^0.12.4"
 PyQt6 = "^6.2.3"
 PyVirtualDisplay = "^3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
```

### Comparing `eagerx_gui-0.2.8/setup.py` & `eagerx_gui-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyQt6>=6.2.3,<7.0.0',
  'PyVirtualDisplay>=3.0,<4.0',
- 'eagerx>=0.1.27,<0.2.0',
+ 'eagerx>=0.1.30,<0.2.0',
  'opencv-python>=4.5,<5.0',
  'pyqtgraph>=0.12.4,<0.13.0']
 
 setup_kwargs = {
     'name': 'eagerx-gui',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'GUI to visualise graphs in EAGERx.',
     'long_description': None,
     'author': 'Jelle Luijkx',
     'author_email': 'j.d.luijkx@tudelft.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/eager-dev/eagerx_gui',
```

### Comparing `eagerx_gui-0.2.8/PKG-INFO` & `eagerx_gui-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: eagerx-gui
-Version: 0.2.8
+Version: 0.2.9
 Summary: GUI to visualise graphs in EAGERx.
 Home-page: https://github.com/eager-dev/eagerx_gui
 License: Apache2.0
 Author: Jelle Luijkx
 Author-email: j.d.luijkx@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyQt6 (>=6.2.3,<7.0.0)
 Requires-Dist: PyVirtualDisplay (>=3.0,<4.0)
-Requires-Dist: eagerx (>=0.1.27,<0.2.0)
+Requires-Dist: eagerx (>=0.1.30,<0.2.0)
 Requires-Dist: opencv-python (>=4.5,<5.0)
 Requires-Dist: pyqtgraph (>=0.12.4,<0.13.0)
 Project-URL: Documentation, https://eagerx.readthedocs.io/en/master/
 Project-URL: Repository, https://github.com/eager-dev/eagerx_gui
```

