# Comparing `tmp/PyNiteFEA-0.0.77.tar.gz` & `tmp/PyNiteFEA-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNiteFEA-0.0.77.tar", last modified: Thu Jul  6 16:57:37 2023, max compression
+gzip compressed data, was "PyNiteFEA-0.0.78.tar", last modified: Thu Jul  6 18:49:07 2023, max compression
```

## Comparing `PyNiteFEA-0.0.77.tar` & `PyNiteFEA-0.0.78.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:57:37.210751 PyNiteFEA-0.0.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-06 16:57:37.210751 PyNiteFEA-0.0.77/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:57:37.210751 PyNiteFEA-0.0.77/PyNite/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/BeamSegY.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/BeamSegZ.py
--rw-r--r--   0 runner    (1001) docker     (123)   154553 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/FEModel3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/FixedEndReactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/LoadCombo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/MainStyleSheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Member3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    67801 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Node3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/PhysMember.py
--rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Plate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Quad3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Report_Template.html
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Spring3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/PyNite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:57:37.210751 PyNiteFEA-0.0.77/PyNiteFEA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-06 16:57:37.000000 PyNiteFEA-0.0.77/PyNiteFEA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-06 16:57:37.000000 PyNiteFEA-0.0.77/PyNiteFEA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:57:37.000000 PyNiteFEA-0.0.77/PyNiteFEA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 16:57:37.000000 PyNiteFEA-0.0.77/PyNiteFEA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 16:57:37.000000 PyNiteFEA-0.0.77/PyNiteFEA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:57:37.210751 PyNiteFEA-0.0.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-06 16:57:27.000000 PyNiteFEA-0.0.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:07.399466 PyNiteFEA-0.0.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-06 18:49:07.399466 PyNiteFEA-0.0.78/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:07.395466 PyNiteFEA-0.0.78/PyNite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/BeamSegY.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/BeamSegZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161411 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/FEModel3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/FixedEndReactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/LoadCombo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/MainStyleSheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Member3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67801 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Node3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/PhysMember.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Plate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Quad3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Report_Template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Spring3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/PyNite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:49:07.399466 PyNiteFEA-0.0.78/PyNiteFEA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-06 18:49:07.000000 PyNiteFEA-0.0.78/PyNiteFEA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-06 18:49:07.000000 PyNiteFEA-0.0.78/PyNiteFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:49:07.000000 PyNiteFEA-0.0.78/PyNiteFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 18:49:07.000000 PyNiteFEA-0.0.78/PyNiteFEA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 18:49:07.000000 PyNiteFEA-0.0.78/PyNiteFEA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:49:07.399466 PyNiteFEA-0.0.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-06 18:48:55.000000 PyNiteFEA-0.0.78/setup.py
```

### Comparing `PyNiteFEA-0.0.77/LICENSE` & `PyNiteFEA-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PKG-INFO` & `PyNiteFEA-0.0.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.77
+Version: 0.0.78
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -77,19 +77,23 @@
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.78
+* Corrections to tension/compression only support springs. v0.0.76 and v0.0.77 were not working as expected. 3rd time's a charm.
+
 v0.0.77
 * Simplified P-Delta convergence checks
 * Fixed P-Delta bug introduced in v0.0.76
   
 v0.0.76
+* Simplified P-Delta convergence checks
 * Allowed tension/compression-only support springs to reactivate after being deactivated. Erroneous deflections were being reported on very flexible models that experienced a lot of movement with T/C support springs.
 * `matplotlib` is now an optional dependency. You'll only need to install it if you want to view plots for members.
 * Documentation for installation has been improved.
 
 v0.0.75
 * Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
```

### Comparing `PyNiteFEA-0.0.77/PyNite/BeamSegY.py` & `PyNiteFEA-0.0.78/PyNite/BeamSegY.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/BeamSegZ.py` & `PyNiteFEA-0.0.78/PyNite/BeamSegZ.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/FEModel3D.py` & `PyNiteFEA-0.0.78/PyNite/FEModel3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -2062,48 +2062,90 @@
 
                 # Check tension/compression-only spring supports
                 if log: print('- Checking for tension/compression-only support spring convergence')
                 for node in self.Nodes.values():
                     
                     # Check convergence of tension/compression-only spring supports and activate/deactivate them as necessary
                     if node.spring_DX[1] is not None:
-                        if (node.spring_DX[1] == '-' and node.DX[combo.name] > 0) or (node.spring_DX[1] == '+' and node.DX[combo.name] < 0):
+                        if ((node.spring_DX[1] == '-' and node.DX[combo.name] > 0)
+                        or (node.spring_DX[1] == '+' and node.DX[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_DX[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_DX[2] = False
-                            convergence = False
-                        else:
+                        elif ((node.spring_DX[1] == '-' and node.DX[combo.name] < 0)
+                        or (node.spring_DX[1] == '+' and node.DX[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_DX[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_DX[2] = True
                     if node.spring_DY[1] is not None:
-                        if (node.spring_DY[1] == '-' and node.DY[combo.name] > 0) or (node.spring_DY[1] == '+' and node.DY[combo.name] < 0):
+                        if ((node.spring_DY[1] == '-' and node.DY[combo.name] > 0)
+                        or (node.spring_DY[1] == '+' and node.DY[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_DY[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_DY[2] = False
-                            convergence = False
-                        else:
+                        elif ((node.spring_DY[1] == '-' and node.DY[combo.name] < 0)
+                        or (node.spring_DY[1] == '+' and node.DY[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_DY[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_DY[2] = True
                     if node.spring_DZ[1] is not None:
-                        if (node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0) or (node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0):
+                        if ((node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0)
+                        or (node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_DZ[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_DZ[2] = False
-                            convergence = False
-                        else:
+                        elif ((node.spring_DZ[1] == '-' and node.DZ[combo.name] < 0)
+                        or (node.spring_DZ[1] == '+' and node.DZ[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_DZ[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_DZ[2] = True
                     if node.spring_RX[1] is not None:
-                        if (node.spring_RX[1] == '-' and node.RX[combo.name] > 0) or (node.spring_RX[1] == '+' and node.RX[combo.name] < 0):
+                        if ((node.spring_RX[1] == '-' and node.RX[combo.name] > 0)
+                        or (node.spring_RX[1] == '+' and node.RX[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_RX[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_RX[2] = False
-                            convergence = False
-                        else:
+                        elif ((node.spring_RX[1] == '-' and node.RX[combo.name] < 0)
+                        or (node.spring_RX[1] == '+' and node.RX[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_RX[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_RX[2] = True
                     if node.spring_RY[1] is not None:
-                        if (node.spring_RY[1] == '-' and node.RY[combo.name] > 0) or (node.spring_RY[1] == '+' and node.RY[combo.name] < 0):
+                        if ((node.spring_RY[1] == '-' and node.RY[combo.name] > 0)
+                        or (node.spring_RY[1] == '+' and node.RY[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_RY[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_RY[2] = False
-                            convergence = False
-                        else:
+                        elif ((node.spring_RY[1] == '-' and node.RY[combo.name] < 0)
+                        or (node.spring_RY[1] == '+' and node.RY[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_RY[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_RY[2] = True
                     if node.spring_RZ[1] is not None:
-                        if (node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0) or (node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0):
+                        if ((node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0)
+                        or (node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_RZ[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_RZ[2] = False
-                            convergence = False
-                        else:
+                        elif ((node.spring_RZ[1] == '-' and node.RZ[combo.name] < 0)
+                        or (node.spring_RZ[1] == '+' and node.RZ[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_RZ[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_RZ[2] = True
 
                 # Check tension/compression-only springs
                 if log: print('- Checking for tension/compression-only spring convergence')
                 for spring in self.Springs.values():
 
                     if spring.active[combo.name] == True:
@@ -2515,48 +2557,90 @@
                 
                 # Check tension/compression-only spring supports
                 if log: print('- Checking for tension/compression-only support spring convergence')
                 for node in self.Nodes.values():
                     
                     # Check convergence of tension/compression-only spring supports and activate/deactivate them as necessary
                     if node.spring_DX[1] is not None:
-                        if (node.spring_DX[1] == '-' and node.DX[combo.name] > 0) or (node.spring_DX[1] == '+' and node.DX[combo.name] < 0):
+                        if ((node.spring_DX[1] == '-' and node.DX[combo.name] > 0)
+                        or (node.spring_DX[1] == '+' and node.DX[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_DX[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_DX[2] = False
-                            convergence_TC = False
-                        else:
+                        elif ((node.spring_DX[1] == '-' and node.DX[combo.name] < 0)
+                        or (node.spring_DX[1] == '+' and node.DX[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_DX[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_DX[2] = True
                     if node.spring_DY[1] is not None:
-                        if (node.spring_DY[1] == '-' and node.DY[combo.name] > 0) or (node.spring_DY[1] == '+' and node.DY[combo.name] < 0):
+                        if ((node.spring_DY[1] == '-' and node.DY[combo.name] > 0)
+                        or (node.spring_DY[1] == '+' and node.DY[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_DY[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_DY[2] = False
-                            convergence_TC = False
-                        else:
+                        elif ((node.spring_DY[1] == '-' and node.DY[combo.name] < 0)
+                        or (node.spring_DY[1] == '+' and node.DY[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_DY[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_DY[2] = True
                     if node.spring_DZ[1] is not None:
-                        if (node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0) or (node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0):
+                        if ((node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0)
+                        or (node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_DZ[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_DZ[2] = False
-                            convergence_TC = False
-                        else:
+                        elif ((node.spring_DZ[1] == '-' and node.DZ[combo.name] < 0)
+                        or (node.spring_DZ[1] == '+' and node.DZ[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_DZ[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_DZ[2] = True
                     if node.spring_RX[1] is not None:
-                        if (node.spring_RX[1] == '-' and node.RX[combo.name] > 0) or (node.spring_RX[1] == '+' and node.RX[combo.name] < 0):
+                        if ((node.spring_RX[1] == '-' and node.RX[combo.name] > 0)
+                        or (node.spring_RX[1] == '+' and node.RX[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_RX[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_RX[2] = False
-                            convergence_TC = False
-                        else:
+                        elif ((node.spring_RX[1] == '-' and node.RX[combo.name] < 0)
+                        or (node.spring_RX[1] == '+' and node.RX[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_RX[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_RX[2] = True
                     if node.spring_RY[1] is not None:
-                        if (node.spring_RY[1] == '-' and node.RY[combo.name] > 0) or (node.spring_RY[1] == '+' and node.RY[combo.name] < 0):
+                        if ((node.spring_RY[1] == '-' and node.RY[combo.name] > 0)
+                        or (node.spring_RY[1] == '+' and node.RY[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_RY[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_RY[2] = False
-                            convergence_TC = False
-                        else:
+                        elif ((node.spring_RY[1] == '-' and node.RY[combo.name] < 0)
+                        or (node.spring_RY[1] == '+' and node.RY[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_RY[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_RY[2] = True
                     if node.spring_RZ[1] is not None:
-                        if (node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0) or (node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0):
+                        if ((node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0)
+                        or (node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0)):
+                            # Check if the spring is switching from active to inactive
+                            if node.spring_RZ[2] == True: convergence = False
+                            # Make sure the spring is innactive
                             node.spring_RZ[2] = False
-                            convergence_TC = False
-                        else:
+                        elif ((node.spring_RZ[1] == '-' and node.RZ[combo.name] < 0)
+                        or (node.spring_RZ[1] == '+' and node.RZ[combo.name] > 0)):
+                            # Check if the spring is switching from inactive to active
+                            if node.spring_RZ[2] == False: convergence = False
+                            # Make sure the spring is active
                             node.spring_RZ[2] = True
 
                 # Check for tension/compression-only springs that need to be deactivated
                 if log: print('- Checking for tension/compression-only spring convergence')
                 for spring in self.Springs.values():
 
                     # Only run the tension/compression only check if the spring is still active
```

### Comparing `PyNiteFEA-0.0.77/PyNite/FixedEndReactions.py` & `PyNiteFEA-0.0.78/PyNite/FixedEndReactions.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/LoadCombo.py` & `PyNiteFEA-0.0.78/PyNite/LoadCombo.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/MainStyleSheet.css` & `PyNiteFEA-0.0.78/PyNite/MainStyleSheet.css`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Member3D.py` & `PyNiteFEA-0.0.78/PyNite/Member3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Mesh.py` & `PyNiteFEA-0.0.78/PyNite/Mesh.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Node3D.py` & `PyNiteFEA-0.0.78/PyNite/Node3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/PhysMember.py` & `PyNiteFEA-0.0.78/PyNite/PhysMember.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Plate3D.py` & `PyNiteFEA-0.0.78/PyNite/Plate3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Quad3D.py` & `PyNiteFEA-0.0.78/PyNite/Quad3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Report_Template.html` & `PyNiteFEA-0.0.78/PyNite/Report_Template.html`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Reporting.py` & `PyNiteFEA-0.0.78/PyNite/Reporting.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Spring3D.py` & `PyNiteFEA-0.0.78/PyNite/Spring3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNite/Visualization.py` & `PyNiteFEA-0.0.78/PyNite/Visualization.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/PyNiteFEA.egg-info/PKG-INFO` & `PyNiteFEA-0.0.78/PyNiteFEA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.77
+Version: 0.0.78
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -77,19 +77,23 @@
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.78
+* Corrections to tension/compression only support springs. v0.0.76 and v0.0.77 were not working as expected. 3rd time's a charm.
+
 v0.0.77
 * Simplified P-Delta convergence checks
 * Fixed P-Delta bug introduced in v0.0.76
   
 v0.0.76
+* Simplified P-Delta convergence checks
 * Allowed tension/compression-only support springs to reactivate after being deactivated. Erroneous deflections were being reported on very flexible models that experienced a lot of movement with T/C support springs.
 * `matplotlib` is now an optional dependency. You'll only need to install it if you want to view plots for members.
 * Documentation for installation has been improved.
 
 v0.0.75
 * Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
```

### Comparing `PyNiteFEA-0.0.77/PyNiteFEA.egg-info/SOURCES.txt` & `PyNiteFEA-0.0.78/PyNiteFEA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.77/README.md` & `PyNiteFEA-0.0.78/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,23 @@
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.78
+* Corrections to tension/compression only support springs. v0.0.76 and v0.0.77 were not working as expected. 3rd time's a charm.
+
 v0.0.77
 * Simplified P-Delta convergence checks
 * Fixed P-Delta bug introduced in v0.0.76
   
 v0.0.76
+* Simplified P-Delta convergence checks
 * Allowed tension/compression-only support springs to reactivate after being deactivated. Erroneous deflections were being reported on very flexible models that experienced a lot of movement with T/C support springs.
 * `matplotlib` is now an optional dependency. You'll only need to install it if you want to view plots for members.
 * Documentation for installation has been improved.
 
 v0.0.75
 * Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
```

### Comparing `PyNiteFEA-0.0.77/setup.py` & `PyNiteFEA-0.0.78/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNiteFEA",
-    version="0.0.77",
+    version="0.0.78",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="A simple elastic 3D structural finite element library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/PyNite.git",
     packages=setuptools.find_packages(include=['PyNite', 'Pynite.*']),
```

