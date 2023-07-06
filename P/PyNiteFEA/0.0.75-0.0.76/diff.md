# Comparing `tmp/PyNiteFEA-0.0.75.tar.gz` & `tmp/PyNiteFEA-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNiteFEA-0.0.75.tar", last modified: Fri Jun 30 23:37:28 2023, max compression
+gzip compressed data, was "PyNiteFEA-0.0.76.tar", last modified: Thu Jul  6 16:39:48 2023, max compression
```

## Comparing `PyNiteFEA-0.0.75.tar` & `PyNiteFEA-0.0.76.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:37:28.439580 PyNiteFEA-0.0.75/PyNite/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/BeamSegY.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/BeamSegZ.py
--rw-r--r--   0 runner    (1001) docker     (123)   154824 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/FEModel3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/FixedEndReactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/LoadCombo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/MainStyleSheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Member3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    67835 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Node3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/PhysMember.py
--rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Plate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Quad3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Report_Template.html
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Spring3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:39:48.547654 PyNiteFEA-0.0.76/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-06 16:39:48.547654 PyNiteFEA-0.0.76/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:39:48.543654 PyNiteFEA-0.0.76/PyNite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/BeamSegY.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/BeamSegZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155069 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/FEModel3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/FixedEndReactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/LoadCombo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/MainStyleSheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Member3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67801 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Node3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/PhysMember.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Plate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Quad3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Report_Template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Spring3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/PyNite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:39:48.547654 PyNiteFEA-0.0.76/PyNiteFEA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-06 16:39:48.000000 PyNiteFEA-0.0.76/PyNiteFEA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-06 16:39:48.000000 PyNiteFEA-0.0.76/PyNiteFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:39:48.000000 PyNiteFEA-0.0.76/PyNiteFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 16:39:48.000000 PyNiteFEA-0.0.76/PyNiteFEA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 16:39:48.000000 PyNiteFEA-0.0.76/PyNiteFEA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:39:48.547654 PyNiteFEA-0.0.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-06 16:39:36.000000 PyNiteFEA-0.0.76/setup.py
```

### Comparing `PyNiteFEA-0.0.75/LICENSE` & `PyNiteFEA-0.0.76/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PKG-INFO` & `PyNiteFEA-0.0.76/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.75
+Version: 0.0.76
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: Sparse Solver
+Provides-Extra: Plotting
 Provides-Extra: Visualization
 Provides-Extra: Visualization Screenshots
 Provides-Extra: Reporting
 Provides-Extra: Reviewing Derivations
 License-File: LICENSE
 
 <div align="center">
@@ -29,15 +30,17 @@
 ![GitHub last commit](https://img.shields.io/github/last-commit/JWock82/PyNite)
 ![GitHub](https://img.shields.io/github/license/JWock82/PyNite)
 [![Documentation Status](https://readthedocs.org/projects/pynite/badge/?version=latest)](https://pynite.readthedocs.io/en/latest/?badge=latest)
 
 An easy to use elastic 3D structural engineering finite element analysis library for Python.
 
 # Installation
-The easiest way to install Pynite is with pip: `pip install PyNiteFEA`
+The easiest way to install Pynite is with pip: `pip install PyniteFEA`
+
+For a more detailed discussion on installation options and dependencies see https://pynite.readthedocs.io/en/latest/installation.html
 
 # Current Capabilities
 * 3D static analysis of elastic structures.
 * P-&Delta; analysis of frame type structures.
 * Member point loads, linearly varying distributed loads, and nodal loads are supported.
 * Classify loads by load case and create load combinations from load cases.
 * Produces shear, moment, and deflection results and diagrams for each member.
@@ -65,38 +68,28 @@
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
 * Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
-# Dependencies
-PyNite depends on the following packages:
-## Required Dependencies
-* numpy: used for matrix algebra and dense matrix solver
-* matplotlib: used for plotting member diagrams
-* PrettyTable : used to format tabular output
-
-## Optional Dependencies
-* scipy: Used for sparse matrix solver to improve solution speed and memory management. In most cases you'll want to install scipy. 
-* VTK: Used for visualization - Note that VTK is a little picky about which version of Python you are running. You must run a 64 bit installation of Python, rather than a 32 bit version. VTK is published by Kitware. I've noticed Kitware takes a little time updating VTK to be compatible anytime a new version of Python is released. If you're having trouble installing VTK, you can see which versions of Python are supported by visiting https://pypi.org/project/vtk/#files. VTK does not need to be installed if you don't plan to use the visualization tools built into PyNite.
-* PDFKit: Used for generating pdf reports. In order to generate pdf reports, PDFKit requires you to have wkhtmltopdf installed on your computer. This is a free program available for download at https://wkhtmltopdf.org/downloads.html. Once installed, you'll need to help PyNite find it. On Windows, this can be done by setting your PATH environment variable to include the path to "wkhtmltopdf.exe" after installation. For example, mine is installed at "C:\Program Files\wkhtmltopdf\bin"
-* IPython: Used for displaying screenshots from VTK.
-* jinja2: Used for templating reports into HTML prior to HTML-to-pdf conversion.
-* jupyterlab: Only needed if you want to view the derivations used to build PyNite.
-* sympy: Only needed if you want to view the derivations used to build PyNite.
-
 # Example Projects
-Here's a list of projects that run on PyNite:
+Here's a list of projects that use PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
+* Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.76
+* Allowed tension/compression-only support springs to reactivate after being deactivated. Erroneous deflections were being reported on very flexible models that experienced a lot of movement with T/C support springs.
+* `matplotlib` is now an optional dependency. You'll only need to install it if you want to view plots for members.
+* Documentation for installation has been improved.
+
 v0.0.75
 * Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
 
 v0.0.74
 * Bug fix for rectangular meshes with very close control points. The program now checks for mesh
 control points that are for all practical purposes the same and eliminates the duplicates.
 
@@ -133,21 +126,7 @@
 * Bug fix for P-Delta analysis. Global displacements were correct, but member internal forces were neglecting the geometric stiffness matrix. The impact of this bug was minimal, since the strain induced by correct global displacements was still being considered prior to this update. You should see a slight change to member P-Delta results.
 * Code simplification for P-Delta analysis.
 
 v0.0.66
 * Code simplification and bug fix for merging duplicate nodes.
 * When nodes are merged, support conditions for the deleted node are now assigned to the remaining node.
 * Added a linear solver for faster analysis of simple models. If you don't need P-Delta analysis or tension/compression-only analysis this solver saves time by only assembling the global stiffness matrix once.
-
-v0.0.65
-* Improved the `merge_duplicate_nodes` method. It seemed to be working, but it was hard to follow, and there may have been cases where it didn't work as expected. Simplified the code for this method to make it clear what it was doing, and to make it more efficient. Added comments explaining each step.
-* Screenshot size is now adjustable when rendering.
-* Fixed a bug for `RectangleMesh` where it could not be used repeatedly.
-* Refactoring: changed `Name` to `name` throughout code. For example, `Node3D.Name` is now `Node3D.name`.
-* Fixed obsolete method names that had not been updated.
-* Scalar bar text size can now be controlled. It had strange behavior before. It would change with the window size (until the window size was too small).
-* More work on the new `Renderer` class. This class is being built to give the user more control over the appearance and behavior of renderings.
-* Bug fix for nodal springs applied in the 'RY' and 'RZ' direction. Exceptions were being thrown in some cases.
-
-v0.0.63 thru v0.0.64
-* Fixed the `add_mesh` method. It was not working properly after version 0.0.62.
-* Made stability checks optional. Stability checks add significant solve time. If you are confident your model is stable, you can skip the stability check by toggling `check_stability` to `False` in your call to your analysis command.
```

### Comparing `PyNiteFEA-0.0.75/PyNite/BeamSegY.py` & `PyNiteFEA-0.0.76/PyNite/BeamSegY.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/BeamSegZ.py` & `PyNiteFEA-0.0.76/PyNite/BeamSegZ.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/FEModel3D.py` & `PyNiteFEA-0.0.76/PyNite/FEModel3D.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # %%
 from os import rename
 import warnings
 from math import isclose
 
-from matplotlib.pyplot import get
-
 from numpy import array, zeros, matmul, divide, subtract, atleast_2d, nanmax
 from numpy import seterr
 from numpy.linalg import solve
 
 from PyNite.Node3D import Node3D
 from PyNite.Material import Material
 from PyNite.PhysMember import PhysMember
@@ -303,15 +301,15 @@
                 name = "M" + str(len(self.Members)+count)
                 count += 1
                 
         # Create a new member
         if auxNode == None:
             new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J, A, model=self, tension_only=tension_only, comp_only=comp_only)
         else:
-            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J, A, model=self, auxnode=self.AuxNodes[auxNode], tension_only=tension_only, comp_only=comp_only)
+            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J, A, model=self, aux_node=self.AuxNodes[auxNode], tension_only=tension_only, comp_only=comp_only)
         
         # Add the new member to the list
         self.Members[name] = new_member
         
         # Flag the model as unsolved
         self.solution = None
 
@@ -911,31 +909,27 @@
         node.support_RY = support_RY
         node.support_RZ = support_RZ
 
         # Flag the model as unsolved
         self.solution = None
 
     def def_support_spring(self, node_name, dof, stiffness, direction=None):
-        """
-        Defines a spring support at a node.
+        """Defines a spring support at a node.
 
-        Parameters
-        ----------
-        node_name : str
-            The name of the node to apply the spring support to.
-        dof : str ('DX', 'DY', 'DZ', 'RX', 'RY', or 'RZ')
-            The degree of freedom to apply the spring support to.
-        stiffness : number
-            The translational or rotational stiffness of the spring support.
-        direction : str or None ('+', '-', None)
-            The direction in which the spring can act. '+' allows the spring
-            to resist positive displacements. '-' allows the spring to resist
-            negative displacements. None allows the spring to act in both
-            directions. Default is None.
-        """
+        :param node_name: The name of the node to apply the spring support to.
+        :type node_name: str
+        :param dof: The degree of freedom to apply the spring support to.
+        :type dof: str ('DX', 'DY', 'DZ', 'RX', 'RY', or 'RZ')
+        :param stiffness: The translational or rotational stiffness of the spring support.
+        :type stiffness: float
+        :param direction: The direction in which the spring can act. '+' allows the spring to resist positive displacements. '-' allows the spring to resist negative displacements. None allows the spring to act in both directions. Default is None.
+        :type direction: str or None ('+', '-', None), optional
+        :raises ValueError: Occurs when an invalid support spring direction has been specified.
+        :raises ValueError: Occurs when an invalid support spring degree of freedom has been specified.
+        """        
         
         if dof in ('DX', 'DY', 'DZ', 'RX', 'RY', 'RZ'):
             if direction in ('+', '-', None):
                 if dof == 'DX':
                     self.Nodes[node_name].spring_DX = [stiffness, direction, True]
                 elif dof == 'DY':
                     self.Nodes[node_name].spring_DY = [stiffness, direction, True]
@@ -952,24 +946,25 @@
         else:
             raise ValueError('Invalid support spring degree of freedom. Specify \'DX\', \'DY\', \'DZ\', \'RX\', \'RY\', or \'RZ\'')
         
         # Flag the model as unsolved
         self.solution = None
 
     def def_node_disp(self, node_name, direction, magnitude): 
-        '''
-        Defines a nodal displacement at a node.
+        """Defines a nodal displacement at a node.
 
-        node_name : str
-            The name of the node where the nodal displacement is being applied.
-        direction : str
-            The global direction the nodal displacement is being applied in. Displacements are 'DX', 'DY', and 'DZ'. Rotations are 'RX', 'RY', and 'RZ'.
-        magnitude : number
-            The magnitude of the displacement.
-        '''
+        :param node_name: The name of the node where the nodal displacement is being applied.
+        :type node_name: str
+        :param direction: The global direction the nodal displacement is being applied in. Displacements are 'DX', 'DY', and 'DZ'. Rotations are 'RX', 'RY', and 'RZ'.
+        :type direction: str
+        :param magnitude: The magnitude of the displacement.
+        :type magnitude: float
+        :raises ValueError: _description_
+        """
+            
         # Validate the value of Direction
         if direction not in ('DX', 'DY', 'DZ', 'RX', 'RY', 'RZ'):
             raise ValueError(f"Direction must be 'DX', 'DY', 'DZ', 'RX', 'RY', or 'RZ'. {direction} was given.")
         # Get the node
         node = self.Nodes[node_name]
 
         if direction == 'DX':
@@ -2065,51 +2060,51 @@
                 # Assume the model has converged (to be checked below)
                 convergence = True
 
                 # Check tension/compression-only spring supports
                 if log: print('- Checking for tension/compression-only support spring convergence')
                 for node in self.Nodes.values():
                     
-                    # Check if a tension/compression-only support spring has not yet converged
-                    if node.spring_DX[2] == True and node.spring_DX[1] == '-' and node.DX[combo.name] > 0:
-                        node.spring_DX[2] = False
-                        convergence = False
-                    if node.spring_DY[2] == True and node.spring_DY[1] == '-' and node.DY[combo.name] > 0:
-                        node.spring_DY[2] = False
-                        convergence = False
-                    if node.spring_DZ[2] == True and node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0:
-                        node.spring_DZ[2] = False
-                        convergence = False
-                    if node.spring_RX[2] == True and node.spring_RX[1] == '-' and node.RX[combo.name] > 0:
-                        node.spring_RX[2] = False
-                        convergence = False
-                    if node.spring_RY[2] == True and node.spring_RY[1] == '-' and node.RY[combo.name] > 0:
-                        node.spring_RY[2] = False
-                        convergence = False
-                    if node.spring_RZ[2] == True and node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0:
-                        node.spring_RZ[2] = False
-                        convergence = False
-                    if node.spring_DX[2] == True and node.spring_DX[1] == '+' and node.DX[combo.name] < 0:
-                        node.spring_DX[2] = False
-                        convergence = False
-                    if node.spring_DY[2] == True and node.spring_DY[1] == '+' and node.DY[combo.name] < 0:
-                        node.spring_DY[2] = False
-                        convergence = False
-                    if node.spring_DZ[2] == True and node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0:
-                        node.spring_DZ[2] = False
-                        convergence = False
-                    if node.spring_RX[2] == True and node.spring_RX[1] == '+' and node.RX[combo.name] < 0:
-                        node.spring_RX[2] = False
-                        convergence = False
-                    if node.spring_RY[2] == True and node.spring_RY[1] == '+' and node.RY[combo.name] < 0:
-                        node.spring_RY[2] = False
-                        convergence = False
-                    if node.spring_RZ[2] == True and node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0:
-                        node.spring_RZ[2] = False
-                        convergence = False
+                    # Check convergence of tension/compression-only spring supports and activate/deactivate them as necessary
+                    if node.spring_DX[1] is not None:
+                        if (node.spring_DX[1] == '-' and node.DX[combo.name] > 0) or (node.spring_DX[1] == '+' and node.DX[combo.name] < 0):
+                            node.spring_DX[2] = False
+                            convergence = False
+                        else:
+                            node.spring_DX[2] = True
+                    if node.spring_DY[1] is not None:
+                        if (node.spring_DY[1] == '-' and node.DY[combo.name] > 0) or (node.spring_DY[1] == '+' and node.DY[combo.name] < 0):
+                            node.spring_DY[2] = False
+                            convergence = False
+                        else:
+                            node.spring_DY[2] = True
+                    if node.spring_DZ[1] is not None:
+                        if (node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0) or (node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0):
+                            node.spring_DZ[2] = False
+                            convergence = False
+                        else:
+                            node.spring_DZ[2] = True
+                    if node.spring_RX[1] is not None:
+                        if (node.spring_RX[1] == '-' and node.RX[combo.name] > 0) or (node.spring_RX[1] == '+' and node.RX[combo.name] < 0):
+                            node.spring_RX[2] = False
+                            convergence = False
+                        else:
+                            node.spring_RX[2] = True
+                    if node.spring_RY[1] is not None:
+                        if (node.spring_RY[1] == '-' and node.RY[combo.name] > 0) or (node.spring_RY[1] == '+' and node.RY[combo.name] < 0):
+                            node.spring_RY[2] = False
+                            convergence = False
+                        else:
+                            node.spring_RY[2] = True
+                    if node.spring_RZ[1] is not None:
+                        if (node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0) or (node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0):
+                            node.spring_RZ[2] = False
+                            convergence = False
+                        else:
+                            node.spring_RZ[2] = True
 
                 # Check tension/compression-only springs
                 if log: print('- Checking for tension/compression-only spring convergence')
                 for spring in self.Springs.values():
 
                     if spring.active[combo.name] == True:
 
@@ -2160,34 +2155,26 @@
         if check_statics == True:
             self._check_statics()
         
         # Flag the model as solved
         self.solution = 'Linear TC'
 
     def analyze_linear(self, log=False, check_stability=True, check_statics=False, sparse=True):
-        '''
-        Performs first-order static analysis.
-        
-        This analysis procedure is much faster since it only assembles the global stiffness matrix
-        once, rather than once for each load combination. It is not appropriate when non-linear
-        behavior such as tension/compression only analysis or P-Delta analysis are required.
+        """Performs first-order static analysis. This analysis procedure is much faster since it only assembles the global stiffness matrix once, rather than once for each load combination. It is not appropriate when non-linear behavior such as tension/compression only analysis or P-Delta analysis are required.
 
-        Parameters
-        ----------
-        log : bool, optional
-            Prints the analysis log to the console if set to True. Default is False.
-        check_statics : bool, optional
-            When set to True, causes a statics check to be performed
-        sparse : bool, optional
-            Indicates whether the sparse matrix solver should be used. A matrix can be considered
-            sparse or dense depening on how many zero terms there are. Structural stiffness
-            matrices often contain many zero terms. The sparse solver can offer faster solutions
-            for such matrices. Using the sparse solver on dense matrices may lead to slower
-            solution times.
-        '''
+        :param log: Prints the analysis log to the console if set to True. Default is False.
+        :type log: bool, optional
+        :param check_stability: When set to True, checks the stiffness matrix for any unstable degrees of freedom and reports them back to the console. This does add to the solution time. Defaults to True.
+        :type check_stability: bool, optional
+        :param check_statics: When set to True, causes a statics check to be performed. Defaults to False.
+        :type check_statics: bool, optional
+        :param sparse: Indicates whether the sparse matrix solver should be used. A matrix can be considered sparse or dense depening on how many zero terms there are. Structural stiffness matrices often contain many zero terms. The sparse solver can offer faster solutions for such matrices. Using the sparse solver on dense matrices may lead to slower solution times. Be sure ``scipy`` is installed to use the sparse solver. Default is True.
+        :type sparse: bool, optional
+        :raises Exception: Occurs when a singular stiffness matrix is found. This indicates an unstable structure has been modeled.
+        """
 
         if log:
             print('+-------------------+')
             print('| Analyzing: Linear |')
             print('+-------------------+')
 
         # Import `scipy` features if the sparse solver is being used
@@ -2323,34 +2310,28 @@
         if check_statics == True:
             self._check_statics()
         
         # Flag the model as solved
         self.solution = 'Linear'
 
     def analyze_PDelta(self, log=False, check_stability=True, max_iter=30, tol=0.01, sparse=True):
-        """
-        Performs second order (P-Delta) analysis.
+        """Performs second order (P-Delta) analysis. This type of analysis is appropriate for most models using beams, columns and braces. Second order analysis is usually required by material specific codes. The analysis is iterative and takes longer to solve. Models with slender members and/or members with combined bending and axial loads will generally have more significant P-Delta effects. P-Delta effects in plates/quads are not considered.
 
-        Parameters
-        ----------
-        log : bool, optional
-            Prints updates to the console if set to True. Default is False.
-        max_iter : number
-            The maximum number of iterations permitted. If this value is exceeded the program will
-            report divergence.
-        tol : number
-            The deflection tolerance (as a percentage) between iterations that will be used to
-            define whether the model has converged (e.g. 0.01 = deflections must converge within 1%
-            between iterations).
-        sparse : bool, optional
-            Indicates whether the sparse matrix solver should be used. A matrix can be considered
-            sparse or dense depening on how many zero terms there are. Structural stiffness
-            matrices often contain many zero terms. The sparse solver can offer faster solutions
-            for such matrices. Using the sparse solver on dense matrices may lead to slower
-            solution times.
+        :param log: Prints updates to the console if set to True. Default is False.
+        :type log: bool, optional
+        :param check_stability: When set to True, checks the stiffness matrix for any unstable degrees of freedom and reports them back to the console. This does add to the solution time. Defaults to True.
+        :type check_stability: bool, optional
+        :param max_iter: The maximum number of iterations permitted. If this value is exceeded the program will report divergence. Defaults to 30.
+        :type max_iter: int, optional
+        :param tol: The deflection tolerance (as a percentage) between iterations that will be used to define whether the model has converged (e.g. 0.01 = deflections must converge within 1% between iterations).
+        :type tol: float, optional
+        :param sparse: Indicates whether the sparse matrix solver should be used. A matrix can be considered sparse or dense depening on how many zero terms there are. Structural stiffness matrices often contain many zero terms. The sparse solver can offer faster solutions for such matrices. Using the sparse solver on dense matrices may lead to slower solution times. Be sure ``scipy`` is installed to use the sparse solver. Default is True.
+        :type sparse: bool, optional
+        :raises ValueError: Occurs when there is a singularity in the stiffness matrix, which indicates an unstable structure.
+        :raises Exception: Occurs when a model fails to converge.
         """
         
         if log:
             print('+--------------------+')
             print('| Analyzing: P-Delta |')
             print('+--------------------+')
 
@@ -2532,75 +2513,51 @@
                 # Assume the model has converged (to be checked below)
                 convergence_TC = True
                 
                 # Check tension/compression-only spring supports
                 if log: print('- Checking for tension/compression-only support spring convergence')
                 for node in self.Nodes.values():
                     
-                    # Check if a tension/compression-only support spring has not yet converged
-                    if node.spring_DX[2] == True and node.spring_DX[1] == '-' and node.DX[combo.name] > 0:
-                        node.spring_DX[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_DY[2] == True and node.spring_DY[1] == '-' and node.DY[combo.name] > 0:
-                        node.spring_DY[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_DZ[2] == True and node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0:
-                        node.spring_DZ[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_RX[2] == True and node.spring_RX[1] == '-' and node.RX[combo.name] > 0:
-                        node.spring_RX[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_RY[2] == True and node.spring_RY[1] == '-' and node.RY[combo.name] > 0:
-                        node.spring_RY[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_RZ[2] == True and node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0:
-                        node.spring_RZ[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_DX[2] == True and node.spring_DX[1] == '+' and node.DX[combo.name] < 0:
-                        node.spring_DX[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_DY[2] == True and node.spring_DY[1] == '+' and node.DY[combo.name] < 0:
-                        node.spring_DY[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_DZ[2] == True and node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0:
-                        node.spring_DZ[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_RX[2] == True and node.spring_RX[1] == '+' and node.RX[combo.name] < 0:
-                        node.spring_RX[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_RY[2] == True and node.spring_RY[1] == '+' and node.RY[combo.name] < 0:
-                        node.spring_RY[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
-                    if node.spring_RZ[2] == True and node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0:
-                        node.spring_RZ[2] = False
-                        convergence_TC = False
-                        iter_count_PD = 0
-                        convergence_PD = False
+                    # Check convergence of tension/compression-only spring supports and activate/deactivate them as necessary
+                    if node.spring_DX[1] is not None:
+                        if (node.spring_DX[1] == '-' and node.DX[combo.name] > 0) or (node.spring_DX[1] == '+' and node.DX[combo.name] < 0):
+                            node.spring_DX[2] = False
+                            convergence = False
+                        else:
+                            node.spring_DX[2] = True
+                    if node.spring_DY[1] is not None:
+                        if (node.spring_DY[1] == '-' and node.DY[combo.name] > 0) or (node.spring_DY[1] == '+' and node.DY[combo.name] < 0):
+                            node.spring_DY[2] = False
+                            convergence = False
+                        else:
+                            node.spring_DY[2] = True
+                    if node.spring_DZ[1] is not None:
+                        if (node.spring_DZ[1] == '-' and node.DZ[combo.name] > 0) or (node.spring_DZ[1] == '+' and node.DZ[combo.name] < 0):
+                            node.spring_DZ[2] = False
+                            convergence = False
+                        else:
+                            node.spring_DZ[2] = True
+                    if node.spring_RX[1] is not None:
+                        if (node.spring_RX[1] == '-' and node.RX[combo.name] > 0) or (node.spring_RX[1] == '+' and node.RX[combo.name] < 0):
+                            node.spring_RX[2] = False
+                            convergence = False
+                        else:
+                            node.spring_RX[2] = True
+                    if node.spring_RY[1] is not None:
+                        if (node.spring_RY[1] == '-' and node.RY[combo.name] > 0) or (node.spring_RY[1] == '+' and node.RY[combo.name] < 0):
+                            node.spring_RY[2] = False
+                            convergence = False
+                        else:
+                            node.spring_RY[2] = True
+                    if node.spring_RZ[1] is not None:
+                        if (node.spring_RZ[1] == '-' and node.RZ[combo.name] > 0) or (node.spring_RZ[1] == '+' and node.RZ[combo.name] < 0):
+                            node.spring_RZ[2] = False
+                            convergence = False
+                        else:
+                            node.spring_RZ[2] = True
 
                 # Check for tension/compression-only springs that need to be deactivated
                 if log: print('- Checking for tension/compression-only spring convergence')
                 for spring in self.Springs.values():
 
                     # Only run the tension/compression only check if the spring is still active
                     if spring.active[combo.name] == True:
@@ -3240,8 +3197,8 @@
                 orphaned = True
             
             # Add the orphaned nodes to the list of orphaned nodes
             if orphaned == True:
                 orphans.append(node.name)
         
         return orphans
-      
+
```

### Comparing `PyNiteFEA-0.0.75/PyNite/FixedEndReactions.py` & `PyNiteFEA-0.0.76/PyNite/FixedEndReactions.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/LoadCombo.py` & `PyNiteFEA-0.0.76/PyNite/LoadCombo.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/MainStyleSheet.css` & `PyNiteFEA-0.0.76/PyNite/MainStyleSheet.css`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/Member3D.py` & `PyNiteFEA-0.0.76/PyNite/Member3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/Mesh.py` & `PyNiteFEA-0.0.76/PyNite/Mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,17 +358,15 @@
             
         # Return the smallest value encountered from all the elements
         return M_min
     
 #%%
 class RectangleMesh(Mesh):
 
-    def __init__(self, mesh_size, width, height, thickness, material, model, kx_mod=1, ky_mod=1, origin=[0, 0, 0],
-                 plane='XY', x_control=None, y_control=None, start_node='N1', start_element='Q1',
-                 element_type='Quad'):
+    def __init__(self, mesh_size, width, height, thickness, material, model, kx_mod=1, ky_mod=1, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node='N1', start_element='Q1', element_type='Quad'):
         """
         A rectangular mesh of elements.
 
         Parameters
         ----------
         mesh_size : number
             Desired mesh size.
```

### Comparing `PyNiteFEA-0.0.75/PyNite/Node3D.py` & `PyNiteFEA-0.0.76/PyNite/Node3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/PhysMember.py` & `PyNiteFEA-0.0.76/PyNite/PhysMember.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/Plate3D.py` & `PyNiteFEA-0.0.76/PyNite/Plate3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/Quad3D.py` & `PyNiteFEA-0.0.76/PyNite/Quad3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/Report_Template.html` & `PyNiteFEA-0.0.76/PyNite/Report_Template.html`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/Reporting.py` & `PyNiteFEA-0.0.76/PyNite/Reporting.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNite/Spring3D.py` & `PyNiteFEA-0.0.76/PyNite/Spring3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 from numpy.linalg import inv
 from math import isclose
 import PyNite.FixedEndReactions
 from PyNite.LoadCombo import LoadCombo
 
 # %%
 class Spring3D():
-    '''
-    A class representing a 3D spring element in a finite element model.
-    '''
+    """A class representing a 3D spring element in a finite element model.
+    """
 
-    # '__plt' is used to store the 'pyplot' from matplotlib once it gets imported. Setting it to 'None' for now allows
-    # us to defer importing it until it's actually needed.
+    # '__plt' is used to store the 'pyplot' from matplotlib once it gets imported. Setting it to 'None' for now allows us to defer importing it until it's actually needed.
     __plt = None
 
 #%%
     def __init__(self, name, i_node, j_node, ks, LoadCombos={'Combo 1':LoadCombo('Combo 1', factors={'Case 1':1.0})},
                  tension_only=False, comp_only=False):
         '''
         Initializes a new spring.
```

### Comparing `PyNiteFEA-0.0.75/PyNite/Visualization.py` & `PyNiteFEA-0.0.76/PyNite/Visualization.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/PyNiteFEA.egg-info/PKG-INFO` & `PyNiteFEA-0.0.76/PyNiteFEA.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.75
+Version: 0.0.76
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: Sparse Solver
+Provides-Extra: Plotting
 Provides-Extra: Visualization
 Provides-Extra: Visualization Screenshots
 Provides-Extra: Reporting
 Provides-Extra: Reviewing Derivations
 License-File: LICENSE
 
 <div align="center">
@@ -29,15 +30,17 @@
 ![GitHub last commit](https://img.shields.io/github/last-commit/JWock82/PyNite)
 ![GitHub](https://img.shields.io/github/license/JWock82/PyNite)
 [![Documentation Status](https://readthedocs.org/projects/pynite/badge/?version=latest)](https://pynite.readthedocs.io/en/latest/?badge=latest)
 
 An easy to use elastic 3D structural engineering finite element analysis library for Python.
 
 # Installation
-The easiest way to install Pynite is with pip: `pip install PyNiteFEA`
+The easiest way to install Pynite is with pip: `pip install PyniteFEA`
+
+For a more detailed discussion on installation options and dependencies see https://pynite.readthedocs.io/en/latest/installation.html
 
 # Current Capabilities
 * 3D static analysis of elastic structures.
 * P-&Delta; analysis of frame type structures.
 * Member point loads, linearly varying distributed loads, and nodal loads are supported.
 * Classify loads by load case and create load combinations from load cases.
 * Produces shear, moment, and deflection results and diagrams for each member.
@@ -65,38 +68,28 @@
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
 * Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
-# Dependencies
-PyNite depends on the following packages:
-## Required Dependencies
-* numpy: used for matrix algebra and dense matrix solver
-* matplotlib: used for plotting member diagrams
-* PrettyTable : used to format tabular output
-
-## Optional Dependencies
-* scipy: Used for sparse matrix solver to improve solution speed and memory management. In most cases you'll want to install scipy. 
-* VTK: Used for visualization - Note that VTK is a little picky about which version of Python you are running. You must run a 64 bit installation of Python, rather than a 32 bit version. VTK is published by Kitware. I've noticed Kitware takes a little time updating VTK to be compatible anytime a new version of Python is released. If you're having trouble installing VTK, you can see which versions of Python are supported by visiting https://pypi.org/project/vtk/#files. VTK does not need to be installed if you don't plan to use the visualization tools built into PyNite.
-* PDFKit: Used for generating pdf reports. In order to generate pdf reports, PDFKit requires you to have wkhtmltopdf installed on your computer. This is a free program available for download at https://wkhtmltopdf.org/downloads.html. Once installed, you'll need to help PyNite find it. On Windows, this can be done by setting your PATH environment variable to include the path to "wkhtmltopdf.exe" after installation. For example, mine is installed at "C:\Program Files\wkhtmltopdf\bin"
-* IPython: Used for displaying screenshots from VTK.
-* jinja2: Used for templating reports into HTML prior to HTML-to-pdf conversion.
-* jupyterlab: Only needed if you want to view the derivations used to build PyNite.
-* sympy: Only needed if you want to view the derivations used to build PyNite.
-
 # Example Projects
-Here's a list of projects that run on PyNite:
+Here's a list of projects that use PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
+* Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.76
+* Allowed tension/compression-only support springs to reactivate after being deactivated. Erroneous deflections were being reported on very flexible models that experienced a lot of movement with T/C support springs.
+* `matplotlib` is now an optional dependency. You'll only need to install it if you want to view plots for members.
+* Documentation for installation has been improved.
+
 v0.0.75
 * Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
 
 v0.0.74
 * Bug fix for rectangular meshes with very close control points. The program now checks for mesh
 control points that are for all practical purposes the same and eliminates the duplicates.
 
@@ -133,21 +126,7 @@
 * Bug fix for P-Delta analysis. Global displacements were correct, but member internal forces were neglecting the geometric stiffness matrix. The impact of this bug was minimal, since the strain induced by correct global displacements was still being considered prior to this update. You should see a slight change to member P-Delta results.
 * Code simplification for P-Delta analysis.
 
 v0.0.66
 * Code simplification and bug fix for merging duplicate nodes.
 * When nodes are merged, support conditions for the deleted node are now assigned to the remaining node.
 * Added a linear solver for faster analysis of simple models. If you don't need P-Delta analysis or tension/compression-only analysis this solver saves time by only assembling the global stiffness matrix once.
-
-v0.0.65
-* Improved the `merge_duplicate_nodes` method. It seemed to be working, but it was hard to follow, and there may have been cases where it didn't work as expected. Simplified the code for this method to make it clear what it was doing, and to make it more efficient. Added comments explaining each step.
-* Screenshot size is now adjustable when rendering.
-* Fixed a bug for `RectangleMesh` where it could not be used repeatedly.
-* Refactoring: changed `Name` to `name` throughout code. For example, `Node3D.Name` is now `Node3D.name`.
-* Fixed obsolete method names that had not been updated.
-* Scalar bar text size can now be controlled. It had strange behavior before. It would change with the window size (until the window size was too small).
-* More work on the new `Renderer` class. This class is being built to give the user more control over the appearance and behavior of renderings.
-* Bug fix for nodal springs applied in the 'RY' and 'RZ' direction. Exceptions were being thrown in some cases.
-
-v0.0.63 thru v0.0.64
-* Fixed the `add_mesh` method. It was not working properly after version 0.0.62.
-* Made stability checks optional. Stability checks add significant solve time. If you are confident your model is stable, you can skip the stability check by toggling `check_stability` to `False` in your call to your analysis command.
```

### Comparing `PyNiteFEA-0.0.75/PyNiteFEA.egg-info/SOURCES.txt` & `PyNiteFEA-0.0.76/PyNiteFEA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.75/README.md` & `PyNiteFEA-0.0.76/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 ![GitHub last commit](https://img.shields.io/github/last-commit/JWock82/PyNite)
 ![GitHub](https://img.shields.io/github/license/JWock82/PyNite)
 [![Documentation Status](https://readthedocs.org/projects/pynite/badge/?version=latest)](https://pynite.readthedocs.io/en/latest/?badge=latest)
 
 An easy to use elastic 3D structural engineering finite element analysis library for Python.
 
 # Installation
-The easiest way to install Pynite is with pip: `pip install PyNiteFEA`
+The easiest way to install Pynite is with pip: `pip install PyniteFEA`
+
+For a more detailed discussion on installation options and dependencies see https://pynite.readthedocs.io/en/latest/installation.html
 
 # Current Capabilities
 * 3D static analysis of elastic structures.
 * P-&Delta; analysis of frame type structures.
 * Member point loads, linearly varying distributed loads, and nodal loads are supported.
 * Classify loads by load case and create load combinations from load cases.
 * Produces shear, moment, and deflection results and diagrams for each member.
@@ -46,38 +48,28 @@
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
 * Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
-# Dependencies
-PyNite depends on the following packages:
-## Required Dependencies
-* numpy: used for matrix algebra and dense matrix solver
-* matplotlib: used for plotting member diagrams
-* PrettyTable : used to format tabular output
-
-## Optional Dependencies
-* scipy: Used for sparse matrix solver to improve solution speed and memory management. In most cases you'll want to install scipy. 
-* VTK: Used for visualization - Note that VTK is a little picky about which version of Python you are running. You must run a 64 bit installation of Python, rather than a 32 bit version. VTK is published by Kitware. I've noticed Kitware takes a little time updating VTK to be compatible anytime a new version of Python is released. If you're having trouble installing VTK, you can see which versions of Python are supported by visiting https://pypi.org/project/vtk/#files. VTK does not need to be installed if you don't plan to use the visualization tools built into PyNite.
-* PDFKit: Used for generating pdf reports. In order to generate pdf reports, PDFKit requires you to have wkhtmltopdf installed on your computer. This is a free program available for download at https://wkhtmltopdf.org/downloads.html. Once installed, you'll need to help PyNite find it. On Windows, this can be done by setting your PATH environment variable to include the path to "wkhtmltopdf.exe" after installation. For example, mine is installed at "C:\Program Files\wkhtmltopdf\bin"
-* IPython: Used for displaying screenshots from VTK.
-* jinja2: Used for templating reports into HTML prior to HTML-to-pdf conversion.
-* jupyterlab: Only needed if you want to view the derivations used to build PyNite.
-* sympy: Only needed if you want to view the derivations used to build PyNite.
-
 # Example Projects
-Here's a list of projects that run on PyNite:
+Here's a list of projects that use PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
+* Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.76
+* Allowed tension/compression-only support springs to reactivate after being deactivated. Erroneous deflections were being reported on very flexible models that experienced a lot of movement with T/C support springs.
+* `matplotlib` is now an optional dependency. You'll only need to install it if you want to view plots for members.
+* Documentation for installation has been improved.
+
 v0.0.75
 * Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
 
 v0.0.74
 * Bug fix for rectangular meshes with very close control points. The program now checks for mesh
 control points that are for all practical purposes the same and eliminates the duplicates.
 
@@ -113,22 +105,8 @@
 * Refactoring: deprecated old method names for member results. You may now have some errors show up if you still try to get member results using the old method names.
 * Bug fix for P-Delta analysis. Global displacements were correct, but member internal forces were neglecting the geometric stiffness matrix. The impact of this bug was minimal, since the strain induced by correct global displacements was still being considered prior to this update. You should see a slight change to member P-Delta results.
 * Code simplification for P-Delta analysis.
 
 v0.0.66
 * Code simplification and bug fix for merging duplicate nodes.
 * When nodes are merged, support conditions for the deleted node are now assigned to the remaining node.
-* Added a linear solver for faster analysis of simple models. If you don't need P-Delta analysis or tension/compression-only analysis this solver saves time by only assembling the global stiffness matrix once.
-
-v0.0.65
-* Improved the `merge_duplicate_nodes` method. It seemed to be working, but it was hard to follow, and there may have been cases where it didn't work as expected. Simplified the code for this method to make it clear what it was doing, and to make it more efficient. Added comments explaining each step.
-* Screenshot size is now adjustable when rendering.
-* Fixed a bug for `RectangleMesh` where it could not be used repeatedly.
-* Refactoring: changed `Name` to `name` throughout code. For example, `Node3D.Name` is now `Node3D.name`.
-* Fixed obsolete method names that had not been updated.
-* Scalar bar text size can now be controlled. It had strange behavior before. It would change with the window size (until the window size was too small).
-* More work on the new `Renderer` class. This class is being built to give the user more control over the appearance and behavior of renderings.
-* Bug fix for nodal springs applied in the 'RY' and 'RZ' direction. Exceptions were being thrown in some cases.
-
-v0.0.63 thru v0.0.64
-* Fixed the `add_mesh` method. It was not working properly after version 0.0.62.
-* Made stability checks optional. Stability checks add significant solve time. If you are confident your model is stable, you can skip the stability check by toggling `check_stability` to `False` in your call to your analysis command.
+* Added a linear solver for faster analysis of simple models. If you don't need P-Delta analysis or tension/compression-only analysis this solver saves time by only assembling the global stiffness matrix once.
```

### Comparing `PyNiteFEA-0.0.75/setup.py` & `PyNiteFEA-0.0.76/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNiteFEA",
-    version="0.0.75",
+    version="0.0.76",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="A simple elastic 3D structural finite element library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/PyNite.git",
     packages=setuptools.find_packages(include=['PyNite', 'Pynite.*']),
@@ -17,19 +17,19 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'numpy',
-        'matplotlib',
         'PrettyTable'
     ],
     extras_require = {
         'Sparse Solver': ['scipy'],
+        'Plotting': ['matplotlib'],
         'Visualization':  ['vtk'],
         'Visualization Screenshots': ['IPython'],
         'Reporting': ['pdfkit', 'Jinja2'],
         'Reviewing Derivations': ['jupyterlab', 'sympy']
     },
     include_package_data = True,
     python_requires = '>=3.6',
```

