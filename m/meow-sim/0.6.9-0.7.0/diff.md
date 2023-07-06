# Comparing `tmp/meow-sim-0.6.9.tar.gz` & `tmp/meow-sim-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.9.tar", last modified: Mon Jun 26 16:36:12 2023, max compression
+gzip compressed data, was "meow-sim-0.7.0.tar", last modified: Thu Jul  6 21:21:34 2023, max compression
```

## Comparing `meow-sim-0.6.9.tar` & `meow-sim-0.7.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-26 16:36:07.000000 meow-sim-0.6.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-26 16:36:12.082835 meow-sim-0.6.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-26 16:36:07.000000 meow-sim-0.6.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.078835 meow-sim-0.6.9/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.078835 meow-sim-0.6.9/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     8324 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     3298 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.078835 meow-sim-0.6.9/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6063 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     4924 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/propagate.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10442 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      708 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-26 16:36:07.000000 meow-sim-0.6.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 16:36:12.082835 meow-sim-0.6.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/tests/
--rw-r--r--   0 root         (0) root         (0)     4135 2023-06-26 16:36:07.000000 meow-sim-0.6.9/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-06-26 16:36:07.000000 meow-sim-0.6.9/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-26 16:36:07.000000 meow-sim-0.6.9/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.937969 meow-sim-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-07-06 21:21:30.000000 meow-sim-0.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-07-06 21:21:34.937969 meow-sim-0.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-06 21:21:30.000000 meow-sim-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     8650 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/propagate.py
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    12464 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    12796 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17433 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-06 21:21:30.000000 meow-sim-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 21:21:34.937969 meow-sim-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.937969 meow-sim-0.7.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-06 21:21:30.000000 meow-sim-0.7.0/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-07-06 21:21:30.000000 meow-sim-0.7.0/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-07-06 21:21:30.000000 meow-sim-0.7.0/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.9/LICENSE` & `meow-sim-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/PKG-INFO` & `meow-sim-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.9
+Version: 0.7.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.9/README.md` & `meow-sim-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/__init__.py` & `meow-sim-0.7.0/meow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.9"
+__version__ = "0.7.0"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.9/meow/assets/silicon.csv` & `meow-sim-0.7.0/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/assets/silicon_oxide.csv` & `meow-sim-0.7.0/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/base_model.py` & `meow-sim-0.7.0/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/cache.py` & `meow-sim-0.7.0/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/cell.py` & `meow-sim-0.7.0/meow/cell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 """ an EME Cell """
 
-from typing import List, Tuple, Union, cast
+from typing import Dict, List, Tuple, Union, cast
 
 import numpy as np
 from pydantic import Field
 from scipy.ndimage import convolve
 
 from .base_model import BaseModel, _array, cached_property
-from .mesh import Mesh2d
+from .materials import Material
+from .mesh import Mesh2D
 from .structures import (
-    Structure,
+    Structure2D,
+    Structure3D,
     classify_structures_by_mesh_order_and_material,
     sort_structures,
 )
 
 
 class Cell(BaseModel):
-    """A `Cell` defines a location in a `Structure` associated with a `Mesh`"""
+    """A Cell defines an interval in z (the direction of propagation) within
+    the simulation domain. The intersecting Structure3Ds are discretized by
+    a given mesh at the center of the Cell"""
 
-    structures: List[Structure] = Field(
-        description="the structures which will be sliced by the cell"
+    structures: List[Structure3D] = Field(
+        description="the 3D structures which will be sliced by the cell"
     )
-    mesh: Mesh2d = Field(description="the mesh to slice the structures with")
+    mesh: Mesh2D = Field(description="the mesh to discretize the structures with")
     z_min: float = Field(description="the starting z-coordinate of the cell")
     z_max: float = Field(description="the ending z-coordinate of the cell")
 
-    ez_interfaces: bool = Field(
-        default=False,
-        description=(
-            "when enabled, the meshing algorithm will throw away any index values "
-            "at the interfaces which are not on even (Ez) half-grid locations. "
-            "Enabling this should result in more symmetric modes."
-        ),
-    )
-
     @property
     def z(self):
         return 0.5 * (self.z_min + self.z_max)
 
     @property
     def length(self):
         return np.abs(self.z_max - self.z_min)
@@ -47,27 +42,27 @@
         materials = {}
         for i, structure in enumerate(sort_structures(self.structures), start=1):
             if not structure.material in materials:
                 materials[structure.material] = i
         return materials
 
     @cached_property
+    def structures_2d(self) -> List[Structure2D]:
+        z = 0.5 * (self.z_min + self.z_max)
+        list_of_list = [s._project(z) for s in self.structures]
+        structures = [s for ss in list_of_list for s in ss]
+        return structures
+
+    @cached_property
     def m_full(self):
-        m_full = np.zeros_like(self.mesh.X_full, dtype=np.int_)
-        structures_dict = classify_structures_by_mesh_order_and_material(
-            self.structures, self.materials
+        return _create_full_material_array(
+            mesh=self.mesh,
+            structures=self.structures_2d,
+            materials=self.materials,
         )
-        for structures in structures_dict.values():
-            _m_full = _create_material_array(self, structures, self.ez_interfaces)
-            mask = _m_full > 0
-            m_full[mask] = _m_full[mask]
-
-        m_full = _fill_single_pixel_gaps(m_full)
-
-        return m_full.view(_array)
 
     def _visualize(self, ax=None, cbar=True, show=True):
         import matplotlib.pyplot as plt  # fmt: skip
         from matplotlib.colors import ListedColormap, to_rgba  # fmt: skip
         from mpl_toolkits.axes_grid1 import make_axes_locatable  # fmt: skip
 
         colors = [(0, 0, 0, 0)] + [
@@ -101,56 +96,77 @@
             _cbar.ax.set_yticklabels(labels, rotation=90, va="center")
             plt.sca(ax)
         if show:
             plt.show()
 
 
 def create_cells(
-    structures: List[Structure],
-    mesh: Union[Mesh2d, List[Mesh2d]],
+    structures: List[Structure3D],
+    mesh: Union[Mesh2D, List[Mesh2D]],
     Ls: np.ndarray[Tuple[int], np.dtype[np.float_]],
     z_min: float = 0.0,
-    ez_interfaces: bool = False,
 ) -> List[Cell]:
     """easily create multiple `Cell` objects given a `Mesh` and a collection of cell lengths"""
 
     Ls = np.asarray(Ls, float)
     if Ls.ndim != 1:
         raise ValueError(f"Ls should be 1D. Got shape: {Ls.shape}.")
     if Ls.shape[0] < 0:
         raise ValueError(f"length of Ls array should be nonzero. Got: {Ls}.")
 
-    meshes = [mesh] * Ls.shape[0] if isinstance(mesh, Mesh2d) else mesh
+    meshes = [mesh] * Ls.shape[0] if isinstance(mesh, Mesh2D) else mesh
     if len(Ls) != len(meshes):
         raise ValueError(
             f"Number of meshes should correspond to number of lengths (length of Ls). Got {len(meshes)} != {len(Ls)}."
         )
 
     z = np.cumsum(np.concatenate([np.asarray([z_min], float), Ls]))
     cells = [
         Cell(
             structures=structures,
             mesh=mesh,
             z_min=z_min,
             z_max=z_max,
-            ez_interfaces=ez_interfaces,
         )
         for mesh, (z_min, z_max) in zip(meshes, zip(z[:-1], z[1:]))
     ]
 
     return cells
 
 
-def _create_material_array(cell, structures, ez_interfaces):
-    m_full = np.zeros_like(cell.mesh.X_full, dtype=np.int_)
+def _create_full_material_array(
+    mesh: Mesh2D,
+    structures: List[Structure2D],
+    materials: Dict[Material, int],
+):
+    m_full = np.zeros_like(mesh.X_full, dtype=np.int_)
+    structures_dict = classify_structures_by_mesh_order_and_material(
+        structures, materials
+    )
+    for structures in structures_dict.values():
+        _m_full = _create_material_array(mesh, materials, structures)
+        mask = _m_full > 0
+        m_full[mask] = _m_full[mask]
+
+    m_full = _fill_single_pixel_gaps(m_full)
+
+    return m_full.view(_array)
+
+
+def _create_material_array(
+    mesh: Mesh2D,
+    materials: Dict[Material, int],
+    structures: List[Structure2D],
+) -> np.ndarray:
+    m_full = np.zeros_like(mesh.X_full, dtype=np.int_)
     for structure in structures:
-        mask = structure.geometry._mask2d(cell.mesh.X_full, cell.mesh.Y_full, cell.z)
-        m_full[mask] = cell.materials[structure.material]
+        mask = structure.geometry._mask(mesh.X_full, mesh.Y_full)
+        m_full[mask] = materials[structure.material]
 
-    if ez_interfaces:
+    if mesh.ez_interfaces:
         mask_ez_horizontal = np.zeros_like(m_full, dtype=bool)
         mask_ez_horizontal[:, ::2] = True
         mask_ez_vertical = np.zeros_like(m_full, dtype=bool)
         mask_ez_vertical[::2, :] = True
         mask_boundaries_vertical = _get_boundary_mask_vertical(m_full)
         mask_boundaries_vertical = mask_boundaries_vertical & (~mask_ez_vertical)
         mask_boundaries_horizontal = _get_boundary_mask_horizontal(m_full)
```

### Comparing `meow-sim-0.6.9/meow/eme/__init__.py` & `meow-sim-0.7.0/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/eme/common.py` & `meow-sim-0.7.0/meow/eme/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ SAX backend for EME (default backend) """
 
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 
+from ..cell import Cell
 from ..mode import Mode
 from ..mode import inner_product as inner_product_normal
 from ..mode import inner_product_conj
 
 DEFAULT_CONJUGATE = True
 DEFAULT_ENFORCE_RECIPROCITY = False
 DEFAULT_ENFORCE_LOSSY_UNITARITY = False
@@ -121,46 +122,49 @@
             enforce_reciprocity=enforce_reciprocity,
             enforce_lossy_unitarity=enforce_lossy_unitarity,
         )
         for i, (modes1, modes2) in enumerate(zip(modes[:-1], modes[1:]))
     }
 
 
-def compute_propagation_s_matrix(
-    modes: List[Mode], override_cell_length: Optional[float] = None
-):
+def compute_propagation_s_matrix(modes: List[Mode], cell_length: float):
     """get the propagation S-matrix of each `Mode` belonging to a `CrossSection` in a `Cell` with a certain length."""
-    cell_length = modes[0].cell.length
-    if override_cell_length is not None:
-        cell_length = override_cell_length
-
     s_dict = {
         (f"left@{i}", f"right@{i}"): np.exp(
             2j * np.pi * mode.neff / mode.env.wl * cell_length
         )
         for i, mode in enumerate(modes)
     }
     s_dict = {**s_dict, **{(p2, p1): v for (p1, p2), v in s_dict.items()}}
     return s_dict
 
 
 def compute_propagation_s_matrices(
-    modes: List[List[Mode]], override_cell_lengths: Optional[List[float]] = None
+    modes: List[List[Mode]],
+    cells: Optional[List[Cell]] = None,
+    cell_lengths: Optional[List[float]] = None,
 ):
     """get all the propagation S-matrices of all the `Modes` belonging to each `CrossSection`"""
-    if override_cell_lengths:
-        if not len(override_cell_lengths) == len(modes):
-            raise ValueError(
-                f"len(override_cell_lengths) != len(modes): {len(override_cell_lengths)} != {len(modes)}"
-            )
-        cell_lengths = override_cell_lengths
-    else:
-        cell_lengths = [None for _ in modes]
+    if cells is None and cell_lengths is None:
+        raise ValueError(
+            "Please specify one of both when calculating the S-matrix: `cells` or `cell_lengths`."
+        )
+    if cells is not None and cell_lengths is not None:
+        raise ValueError("Please specify EITHER `cells` OR `cell_lengths` (not both).")
+
+    if cells:
+        cell_lengths = [cell.length for cell in cells]
+
+    assert cell_lengths is not None
+    if not len(cell_lengths) == len(modes):
+        raise ValueError(
+            f"len(cell_lengths) != len(modes): {len(cell_lengths)} != {len(modes)}"
+        )
     return {
-        f"p_{i}": compute_propagation_s_matrix(modes_, override_cell_length=cell_length)
+        f"p_{i}": compute_propagation_s_matrix(modes_, cell_length=cell_length)
         for i, (modes_, cell_length) in enumerate(zip(modes, cell_lengths))
     }
 
 
 def select_ports(
     S: np.ndarray[Any, np.dtype[np.float_]], port_map: Dict[str, int], ports: List[str]
 ):
```

### Comparing `meow-sim-0.6.9/meow/eme/propagate.py` & `meow-sim-0.7.0/meow/eme/propagate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Propagating fields throug devices"""
 
 import jax.numpy as np
-import matplotlib.pyplot as plt
 import numpy as onp
 import sax
 from sax.backends import circuit_backends
 
 from meow.eme import (
     compute_interface_s_matrices,
     compute_interface_s_matrix,
@@ -99,26 +98,25 @@
     RHS = u21 @ excitation_l + u22 @ v12 @ excitation_r
     LHS = np.diag(np.ones(m)) - u22 @ v11
     forward = np.linalg.solve(LHS, RHS)
     backward = v12 @ excitation_r + v11 @ forward  # Attention v21 was v12
     return forward, backward
 
 
-def plot_fields(modes, forwards, backwards, y, z, lim=1):
+def plot_fields(modes, cells, forwards, backwards, y, z, lim=1):
     mode_set = modes[0]
-    mesh_y = mode_set[0].cell.mesh.y
-    mesh_x = mode_set[0].cell.mesh.x
+    mesh_y = cells[0].mesh.y
+    mesh_x = cells[0].mesh.x
     mesh_x = mesh_x[:-1] + np.diff(mesh_x) / 2
     i_y = np.argmin(np.abs(mesh_y - y))
 
     lim = None
     E_tot = onp.zeros((len(z), len(mesh_x)), dtype=complex)
-    for mode_set, forward, backward in zip(modes, forwards, backwards):
-        Ex = 0 + 0j
-        cell = mode_set[0].cell
+    for mode_set, forward, backward, cell in zip(modes, forwards, backwards, cells):
+        Ex = np.array(0 + 0j)
         i_min = np.argmax(z >= cell.z_min)
         i_max = np.argmax(z > cell.z_max)
         if i_max == 0:
             z_ = z[i_min:]
         else:
             z_ = z[i_min:i_max]
 
@@ -142,16 +140,16 @@
         # X, Y = np.meshgrid(z_, mesh_x)
         # plt.pcolormesh(X, Y, np.abs(Ex), vmin = -lim, vmax = lim)
     # plt.xlabel("z in um")
     # plt.ylabel("x in um")
     return E_tot, mesh_x
 
 
-def propagate_modes(modes, ex_l, ex_r, y, z):
-    propagations = compute_propagation_s_matrices(modes)
+def propagate_modes(modes, cells, ex_l, ex_r, y, z):
+    propagations = compute_propagation_s_matrices(modes, cells)
     interfaces = compute_interface_s_matrices(
         modes,
         enforce_reciprocity=False,
     )
     identity = compute_interface_s_matrix(
         modes[0],
         modes[0],
@@ -159,8 +157,8 @@
     )
 
     pairs = pi_pairs(propagations, interfaces)
     l2rs = l2r_matrices(pairs, identity)
     r2ls = r2l_matrices(pairs)
 
     forwards, backwards = propagate(l2rs, r2ls, ex_l, ex_r)
-    return plot_fields(modes, forwards, backwards, y, z)
+    return plot_fields(modes, cells, forwards, backwards, y, z)
```

### Comparing `meow-sim-0.6.9/meow/eme/sax.py` & `meow-sim-0.7.0/meow/eme/sax.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np
 import sax
 from sax.backends import circuit_backends
 from sax.utils import get_ports
 
 from ..base_model import _array
+from ..cell import Cell
 from ..mode import Mode
 from .common import (
     DEFAULT_CONJUGATE,
     DEFAULT_ENFORCE_LOSSY_UNITARITY,
     DEFAULT_ENFORCE_RECIPROCITY,
     compute_interface_s_matrices,
     compute_propagation_s_matrices,
@@ -29,15 +30,14 @@
     """get the netlist of a stack of `Modes`"""
 
     instances = {
         **{k: S for k, S in propagations.items()},
         **{k: S for k, S in interfaces.items()},
     }
 
-    interface_keys = list(interfaces)
     propagation_keys = list(propagations)
     connections = {}
     for i in range(len(interfaces)):
         for port_mode in get_ports(interfaces[f"i_{i}_{i+1}"]):
             other_port_mode = _other_port(port_mode)
             if "left" in port_mode:
                 connections[f"p_{i},{other_port_mode}"] = f"i_{i}_{i+1},{port_mode}"
@@ -76,19 +76,20 @@
             f"Invalid SAX Backend. Got: {sax_backend!r}. Should be 'default' or 'klu'."
         )
     return sax_backend
 
 
 def compute_s_matrix_sax(
     modes: List[List[Mode]],
+    cells: Optional[List[Cell]] = None,
+    cell_lengths: Optional[List[float]] = None,
     sax_backend: Optional[str] = None,
     conjugate: bool = DEFAULT_CONJUGATE,
     enforce_reciprocity: bool = DEFAULT_ENFORCE_RECIPROCITY,
     enforce_lossy_unitarity: bool = DEFAULT_ENFORCE_LOSSY_UNITARITY,
-    override_cell_lengths: Optional[List[float]] = None,
     **kwargs,
 ):
     """Calculate the S-matrix for given sets of modes, each set belonging to a `Cell`
 
     Args:
         modes: Each collection of modes for each of the `Cell` objects
         backend: which SAX backend to use to calculate the final S-matrix.
@@ -97,29 +98,42 @@
     _compute_propagation_s_matrices = kwargs.pop(
         "compute_propagation_s_matrices", compute_propagation_s_matrices
     )
     _compute_interface_s_matrices = kwargs.pop(
         "compute_interface_s_matrices", compute_interface_s_matrices
     )
     propagations = _compute_propagation_s_matrices(
-        modes, override_cell_lengths=override_cell_lengths
+        modes, cells, cell_lengths=cell_lengths
     )
     interfaces = _compute_interface_s_matrices(
         modes,
         conjugate=conjugate,
         enforce_reciprocity=enforce_reciprocity,
         enforce_lossy_unitarity=enforce_lossy_unitarity,
         **kwargs,
     )
 
     # TODO: fix SAX Multimode to reduce this ad-hoc SAX-hacking.
     net = _get_netlist(propagations, interfaces)
     evaluate_circuit = circuit_backends[sax_backend]
-    S, pm = sax.sdense(
+    S, port_map = sax.sdense(
         evaluate_circuit(
             instances=net["instances"],
             connections=net["connections"],
             ports=net["ports"],
         )
     )
     S = np.asarray(S).view(_array)
-    return S, pm
+
+    # final sorting of result:
+    current_port_map = {
+        (p, int(i)): j
+        for (p, i), j in {
+            tuple(pm.split("@")): idx for pm, idx in port_map.items()
+        }.items()
+    }
+    desired_port_map = {pm: i for i, pm in enumerate(sorted(current_port_map))}
+    idxs = [current_port_map[pm] for pm in desired_port_map]
+    S = S[idxs, :][:, idxs]
+    port_map = {f"{p}@{m}": v for (p, m), v in desired_port_map.items()}
+
+    return S, port_map
```

### Comparing `meow-sim-0.6.9/meow/environment.py` & `meow-sim-0.7.0/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/fde/lumerical.py` & `meow-sim-0.7.0/meow/fde/lumerical.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 from pydantic.types import PositiveInt
 
 from ..cross_section import CrossSection
 from ..environment import Environment
 from ..mode import Mode, normalize_product, zero_phase
-from ..structures import Structure
+from ..structures import Structure3D
 
 _global = {"sim": None}
 
 
 def get_sim(**kwargs):
     sim = kwargs.get("sim", None)
     if sim is not None:
@@ -22,15 +22,15 @@
             "Please either pass the `lumapi.MODE` simulation object as an argument to `compute_modes_lumerical` or "
             "use `set_sim(sim)` to globally set the lumapi.MODE simulation object."
         )
     return sim
 
 
 def create_lumerical_geometries(
-    sim, structures: list[Structure], env: Environment, unit: float
+    sim, structures: list[Structure3D], env: Environment, unit: float
 ):
     sim = get_sim(sim=sim)
     sim.switchtolayout()
     sim.deleteall()
     for s in structures:
         s._lumadd(sim, env, unit, "yzx")
 
@@ -48,59 +48,62 @@
         sim: the lumerical simulation object
         spec: The FDE simulation specification
         unit: Conversion factor between MEOW unit (probably um) and Lumerical unit (probably m).
     """
     from lumapi import LumApiError  # fmt: skip # type: ignore
 
     sim = get_sim(sim=sim)
-    _assert_default_mesh_setting(cs.cell.mesh.angle_phi == 0, "angle_phi")
-    _assert_default_mesh_setting(cs.cell.mesh.angle_theta == 0, "angle_theta")
-    _assert_default_mesh_setting(cs.cell.mesh.bend_radius is None, "bend_radius")
+    cell = cs._cell
+    assert cell is not None
+
+    _assert_default_mesh_setting(cell.mesh.angle_phi == 0, "angle_phi")
+    _assert_default_mesh_setting(cell.mesh.angle_theta == 0, "angle_theta")
+    _assert_default_mesh_setting(cell.mesh.bend_radius is None, "bend_radius")
 
     assert sim is not None
-    create_lumerical_geometries(sim, cs.cell.structures, cs.env, unit)
+    create_lumerical_geometries(sim, cell.structures, cs.env, unit)
     sim.select("FDE")
     sim.delete()
     pml_settings = {}
     num_pml_y, num_pml_z = 0, 0
-    if cs.cell.mesh.num_pml[0] > 0:
+    if cell.mesh.num_pml[0] > 0:
         pml_settings.update(
             {
                 "y_min_bc": "PML",
                 "y_max_bc": "PML",
             }
         )
         num_pml_y = 22  # TODO: allow adjusting these values
-    if cs.cell.mesh.num_pml[1] > 0:
+    if cell.mesh.num_pml[1] > 0:
         pml_settings.update(
             {
                 "z_min_bc": "PML",
                 "z_max_bc": "PML",
             }
         )
         num_pml_z = 22  # TODO: allow adjusting these values
     sim.addfde(
         background_index=1.0,
         solver_type="2D X normal",
-        x=float(cs.cell.z * unit),
-        y_min=float(cs.cell.mesh.x.min() * unit),
-        y_max=float(cs.cell.mesh.x.max() * unit),
-        z_min=float(cs.cell.mesh.y.min() * unit),
-        z_max=float(cs.cell.mesh.y.max() * unit),
+        x=float(cell.z * unit),
+        y_min=float(cell.mesh.x.min() * unit),
+        y_max=float(cell.mesh.x.max() * unit),
+        z_min=float(cell.mesh.y.min() * unit),
+        z_max=float(cell.mesh.y.max() * unit),
         define_y_mesh_by="number of mesh cells",
         define_z_mesh_by="number of mesh cells",
-        mesh_cells_y=cs.cell.mesh.x_.shape[0],
-        mesh_cells_z=cs.cell.mesh.y_.shape[0],
+        mesh_cells_y=cell.mesh.x_.shape[0],
+        mesh_cells_z=cell.mesh.y_.shape[0],
         **pml_settings,
     )
     # set mesh size again, because PML messes with it:
-    if cs.cell.mesh.num_pml[0] > 0:
-        sim.setnamed("FDE", "mesh cells y", cs.cell.mesh.x_.shape[0] - num_pml_y)
-    if cs.cell.mesh.num_pml[1] > 0:
-        sim.setnamed("FDE", "mesh cells z", cs.cell.mesh.y_.shape[0] - num_pml_z)
+    if cell.mesh.num_pml[0] > 0:
+        sim.setnamed("FDE", "mesh cells y", cell.mesh.x_.shape[0] - num_pml_y)
+    if cell.mesh.num_pml[1] > 0:
+        sim.setnamed("FDE", "mesh cells z", cell.mesh.y_.shape[0] - num_pml_z)
     sim.setanalysis("number of trial modes", int(num_modes))
     sim.setanalysis("search", "near n")
     sim.setanalysis("use max index", True)
     sim.setanalysis("wavelength", float(cs.env.wl * unit))
     sim.findmodes()
     modes = []
     for j in range(1, num_modes + 1):
```

### Comparing `meow-sim-0.6.9/meow/fde/tidy3d.py` & `meow-sim-0.7.0/meow/fde/tidy3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,33 +43,33 @@
         eps_cross = [cs.nx**2, od, od, od, cs.ny**2, od, od, od, cs.nz**2]
     else:
         eps_cross = [cs.nx**2, cs.ny**2, cs.nz**2]
 
     mode_spec = SimpleNamespace(  # tidy3d.ModeSpec alternative (prevents type checking)
         num_modes=num_modes,
         target_neff=target_neff,
-        num_pml=cs.cell.mesh.num_pml,
+        num_pml=cs.mesh.num_pml,
         filter_pol=None,
-        angle_theta=cs.cell.mesh.angle_theta,
-        angle_phi=cs.cell.mesh.angle_phi,
-        bend_radius=cs.cell.mesh.bend_radius,
+        angle_theta=cs.mesh.angle_theta,
+        angle_phi=cs.mesh.angle_phi,
+        bend_radius=cs.mesh.bend_radius,
         precision=precision,
-        bend_axis=cs.cell.mesh.bend_axis,
+        bend_axis=cs.mesh.bend_axis,
         track_freq="central",
         group_index_step=False,
     )
 
     ((Ex, Ey, Ez), (Hx, Hy, Hz)), neffs = (
         x.squeeze()
         for x in _compute_modes(
             eps_cross=eps_cross,
-            coords=[cs.cell.mesh.x, cs.cell.mesh.y],
+            coords=[cs.mesh.x, cs.mesh.y],
             freq=c / (cs.env.wl * 1e-6),
             mode_spec=mode_spec,
-        )
+        )[:2]
     )
 
     if num_modes == 1:
         modes = [
             Mode(
                 cs=cs,
                 Ex=Ex,
```

### Comparing `meow-sim-0.6.9/meow/gds_structures.py` & `meow-sim-0.7.0/meow/gds_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import shapely.geometry as sg
 from pydantic import Field
 
 from .base_model import BaseModel
 from .geometries import Prism
 from .materials import Material
-from .structures import Structure
+from .structures import Structure3D
 
 # TODO: Maybe it makes more sense to use native GDSFactory tooling for this
 
 
 class GdsExtrusionRule(BaseModel):
     """a `GdsExtrusionRule` describes a single extrusion rule.
     Multiple of such rules can later be associated with a gds layer tuple."""
@@ -22,28 +22,28 @@
     h_min: float = Field(description="the extrusion starting height")
     h_max: float = Field(description="the extrusion ending height")
     buffer: float = Field(
         default=0.0,
         description="an extra buffer (=grow or shrink) operation applied to the polygon",
     )
     mesh_order: int = Field(
-        default=5.0, description="the mesh order of the resulting `Structure`"
+        default=5.0, description="the mesh order of the resulting `Structure3D`"
     )
 
-    def __call__(self, poly) -> Structure:
+    def __call__(self, poly) -> Structure3D:
         if self.buffer > 0:
             try:
                 poly = np.asarray(sg.Polygon(poly).buffer(self.buffer).boundary.coords)
             except NotImplementedError:
                 import gdspy  # fmt: skip
 
                 polygonset = gdspy.offset(gdspy.Polygon(poly), 0.25)
                 assert polygonset is not None
                 poly = polygonset.polygons[0]
-        return Structure(
+        return Structure3D(
             material=self.material,
             geometry=Prism(
                 poly=poly,
                 h_min=self.h_min,
                 h_max=self.h_max,
                 axis="y",
             ),
```

### Comparing `meow-sim-0.6.9/meow/geometries.py` & `meow-sim-0.7.0/meow/geometries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,152 @@
-""" Geometries """
-
 import warnings
 from secrets import token_hex
 from typing import Dict, List, Literal, Tuple, Union, cast
 
+import matplotlib.pyplot as plt
 import numpy as np
 import shapely.geometry as sg
+from matplotlib.patches import Rectangle as MplRect
 from pydantic import Field, validator
 
-from .base_model import BaseModel
+from meow.base_model import BaseModel
+
+GEOMETRIES_3D: Dict[str, type] = {}
+GEOMETRIES_2D: Dict[str, type] = {}
+AxisDirection = Union[Literal["x"], Literal["y"], Literal["z"]]
+
+
+class Geometry2D(BaseModel):
+    type: str = ""
+
+    def __init_subclass__(cls):
+        GEOMETRIES_2D[cls.__name__] = cls
+
+    def __new__(cls, **kwargs):
+        cls = GEOMETRIES_2D.get(kwargs.get("type", cls.__name__), cls)
+        return BaseModel.__new__(cls)  # type: ignore
+
+    @validator("type", pre=True, always=True)
+    def validate_type(cls, value):
+        if not value:
+            value = getattr(cls, "__name__", "Geometry")
+        if value not in GEOMETRIES_2D:
+            raise ValueError(
+                f"Invalid Geometry type. Got: {value!r}. Valid types: {GEOMETRIES_2D}."
+            )
+        return value
+
+    def _mask(self, X, Y):
+        raise NotImplementedError(f"{self.__class__.__name__!r} cannot be masked.")
+
+    def _visualize(self, color=None):
+        raise NotImplementedError(f"{self.__class__.__name__!r} cannot be visualized.")
+
+
+class Rectangle(Geometry2D):
+    """a Rectangle"""
+
+    x_min: float = Field(description="the minimum x-value of the box")
+    x_max: float = Field(description="the maximum x-value of the box")
+    y_min: float = Field(description="the minimum y-value of the box")
+    y_max: float = Field(description="the maximum y-value of the box")
+
+    def _mask(self, X, Y):
+        mask = (
+            (self.x_min <= X)
+            & (X <= self.x_max)
+            & (self.y_min <= Y)
+            & (Y <= self.y_max)
+        )
+        return mask
 
-GEOMETRIES: Dict[str, type] = {}
+    def _visualize(self, ax=None, show=True, color=None):
+        if ax is None:
+            ax = plt.gca()
+        if color is None:
+            color = "grey"
+        width = self.x_max - self.x_min
+        height = self.y_max - self.y_min
+        mpl_rect = MplRect(
+            xy=(self.x_min, self.y_min),
+            width=width,
+            height=height,
+            color=color,
+        )
+        ax.add_patch(mpl_rect)
+        ax.set_xlim(self.x_min - 0.1 * width, self.x_max + 0.1 * width)
+        ax.set_ylim(self.y_min - 0.1 * width, self.y_max + 0.1 * width)
+        ax.set_xlabel("x")
+        ax.set_ylabel("y")
+        plt.grid(True)
+        if show:
+            plt.show()
 
 
-class Geometry(BaseModel):
+class Geometry3D(BaseModel):
     type: str = ""
 
     def __init_subclass__(cls):
-        GEOMETRIES[cls.__name__] = cls
+        GEOMETRIES_3D[cls.__name__] = cls
 
     def __new__(cls, **kwargs):
-        cls = GEOMETRIES.get(kwargs.get("type", cls.__name__), cls)
+        cls = GEOMETRIES_3D.get(kwargs.get("type", cls.__name__), cls)
         return BaseModel.__new__(cls)  # type: ignore
 
     @validator("type", pre=True, always=True)
     def validate_type(cls, value):
         if not value:
             value = getattr(cls, "__name__", "Geometry")
-        if value not in GEOMETRIES:
+        if value not in GEOMETRIES_3D:
             raise ValueError(
-                f"Invalid Geometry type. Got: {value!r}. Valid types: {GEOMETRIES}."
+                f"Invalid Geometry type. Got: {value!r}. Valid types: {GEOMETRIES_3D}."
             )
         return value
 
+    def _project(self, z: float) -> List[Geometry2D]:
+        raise NotImplementedError(f"{self.__class__.__name__!r} cannot be projected.")
+
     def _visualize(self, scale=None):
         from trimesh.scene import Scene  # fmt: skip
         from trimesh.transformations import rotation_matrix  # fmt: skip
 
         scene = Scene()
         scene.add_geometry(self._trimesh(scale=scale))
         scene.apply_transform(rotation_matrix(-np.pi / 6, (0, 1, 0)))
         return scene.show()
 
-    def _mask2d(self, X, Y, z):
-        raise NotImplementedError(f"{self.__class__.__name__!r} cannot be masked.")
-
     def _lumadd(self, sim, material_name, mesh_order, unit=1e-6, xyz="yzx"):
         raise NotImplementedError(
             f"{self.__class__.__name__!r} cannot be added to Lumerical."
         )
 
     def _trimesh(self, **kwargs):
         raise NotImplementedError(f"{self.__class__.__name__!r} cannot be visualized.")
 
 
-Geometries = List[Geometry]
-
-
-class Box(Geometry):
+class Box(Geometry3D):
     """A Box is a simple rectangular cuboid"""
 
     x_min: float = Field(description="the minimum x-value of the box")
     x_max: float = Field(description="the maximum x-value of the box")
     y_min: float = Field(description="the minimum y-value of the box")
     y_max: float = Field(description="the maximum y-value of the box")
     z_min: float = Field(description="the minimum z-value of the box")
     z_max: float = Field(description="the maximum z-value of the box")
 
-    def _mask2d(self, X, Y, z):
-        if (z < self.z_min) or (self.z_max < z):
-            return np.zeros_like(X, dtype=bool)
-        return (
-            (self.x_min <= X)
-            & (X <= self.x_max)
-            & (self.y_min <= Y)
-            & (Y <= self.y_max)
+    def _project(self, z: float) -> List[Geometry2D]:
+        if z < self.z_min or z > self.z_max:
+            return []
+        rect = Rectangle(
+            x_min=self.x_min,
+            x_max=self.x_max,
+            y_min=self.y_min,
+            y_max=self.y_max,
         )
+        return [rect]
 
     def _lumadd(self, sim, material_name, mesh_order, unit, xyz):
         x, y, z = xyz
         name = token_hex(4)
         kwargs = {
             f"{x}_min": float(self.x_min * unit),
             f"{x}_max": float(self.x_max * unit),
@@ -112,106 +179,107 @@
         prism = extrude_polygon(poly, self.z_max * sz - self.z_min * sz)
         prism = cast(Trimesh, prism.apply_translation((0, 0, self.z_min * sz)))
         if color is not None:
             prism.visual.face_colors = _to_rgba(color)  # type: ignore
         return prism
 
 
-AxisDirection = Union[Literal["x"], Literal["y"], Literal["z"]]
-
-
-class Prism(Geometry):
-    """A prism is a 2D Polygon extruded along a certain axis direction ('x', 'y', or 'z').
-
-    Note:
-        currently only extrusions along 'y' (perpendicular to the chip)
-        are fully supported!
-    """
+class Prism(Geometry3D):
+    """A prism is a 2D Polygon extruded along a certain axis direction ('x', 'y', or 'z')."""
 
     poly: np.ndarray[Tuple[int, Literal[2]], np.dtype[np.float_]] = Field(
         description="the 2D array (Nx2) with polygon vertices"
     )
     h_min: float = Field(description="the start height of the extrusion")
     h_max: float = Field(description="the end height of the extrusion")
     axis: AxisDirection = Field(
         default="y",
         description="the axis along which the polygon will be extruded ('x', 'y', or 'z').",
     )
 
-    def _mask2d_axis_x(self, X, Y, z):
+    def _project_axis_x(self, z):
         # x, y, z -> y, z, x
         poly = sg.Polygon(self.poly)
         y_min, _ = self.poly.min(0)
         y_max, _ = self.poly.max(0)
         line = sg.LineString([(y_min, z), (y_max, z)])
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=RuntimeWarning, module="shapely")
             intersections = poly.intersection(line)
 
         if not isinstance(intersections, sg.MultiLineString):
             intersection_array = np.asarray(intersections.coords)
             if not intersection_array.shape[0]:
-                return np.zeros_like(Y, dtype=bool)
+                return []
             intersections = sg.MultiLineString([intersections])
 
-        mask = np.zeros_like(Y, dtype=bool)
+        geoms_2d = []
         for intersection in intersections.geoms:
             intersection = np.asarray(intersection.coords)
             if not intersection.shape[0]:
-                return np.zeros_like(X, dtype=bool)
+                continue
             (y_min, _), (y_max, _) = intersection
             y_min, y_max = min(y_min, y_max), max(y_min, y_max)
             x_min, x_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-            mask |= (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
-        return mask
+            rect = Rectangle(
+                x_min=x_min,
+                x_max=x_max,
+                y_min=y_min,
+                y_max=y_max,
+            )
+            geoms_2d.append(rect)
+        return geoms_2d
 
-    def _mask2d_axis_y(self, X, Y, z):
+    def _project_axis_y(self, z):
         # x, y, z -> z, x, y
         poly = sg.Polygon(self.poly)
         _, x_min = self.poly.min(0)
         _, x_max = self.poly.max(0)
         line = sg.LineString([(z, x_min), (z, x_max)])
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=RuntimeWarning, module="shapely")
             intersections = poly.intersection(line)
 
         if not isinstance(intersections, sg.MultiLineString):
             intersection_array = np.asarray(intersections.coords)
             if not intersection_array.shape[0]:
-                return np.zeros_like(Y, dtype=bool)
+                return []
             intersections = sg.MultiLineString([intersections])
 
-        mask = np.zeros_like(Y, dtype=bool)
+        geoms_2d = []
         for intersection in intersections.geoms:
             intersection = np.asarray(intersection.coords)
             if not intersection.shape[0]:
                 continue
             (_, x_min), (_, x_max) = intersection
             x_min, x_max = min(x_min, x_max), max(x_min, x_max)
             y_min, y_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-            mask |= (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
-        return mask
+            rect = Rectangle(
+                x_min=x_min,
+                x_max=x_max,
+                y_min=y_min,
+                y_max=y_max,
+            )
+            geoms_2d.append(rect)
+        return geoms_2d
 
-    def _mask2d_axis_z(self, X, Y, z):
+    def _project_axis_z(self, z):
         # x, y, z -> x, y, z
-        poly = sg.Polygon(self.poly)
-        if (z < self.h_min) or (self.h_max < z):
-            return np.zeros_like(X, dtype=bool)
-        return np.asarray(
-            [poly.contains(sg.Point(x, y)) for x, y in zip(X.ravel(), Y.ravel())],
-            dtype=bool,
-        ).reshape(X.shape)
+        if z < self.h_min or z < self.h_max:
+            return []
+        else:
+            return [self.poly]
 
-    def _mask2d(self, X, Y, z):
+    def _project(self, z):
         if self.axis == "x":
-            return self._mask2d_axis_x(X, Y, z)
+            return self._project_axis_x(z)
         elif self.axis == "y":
-            return self._mask2d_axis_y(X, Y, z)
+            return self._project_axis_y(z)
         else:
-            return self._mask2d_axis_z(X, Y, z)
+            return self._project_axis_z(z)
 
     def _lumadd(self, sim, material_name, mesh_order, unit=1e-6, xyz="yzx"):
         name = token_hex(4)
 
         if xyz not in ("xyz", "yzx", "zxy"):
             raise ValueError(
                 f"Prism axes should be positively oriented when adding to Lumerical. Got: {xyz!r}"
```

### Comparing `meow-sim-0.6.9/meow/integrate.py` & `meow-sim-0.7.0/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/meow/materials.py` & `meow-sim-0.7.0/meow/materials.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .base_model import BaseModel, _array
 from .environment import Environment
 
 MATERIAL_TYPES: Dict[str, type] = {}
 
 
 class Material(BaseModel):
-    """a `Material` defines the refractive index of a `Structure` within an `Environment`."""
+    """a `Material` defines the refractive index of a `Structure3D` within an `Environment`."""
 
     type: str = ""
 
     name: str = Field(description="the name of the material")
 
     meta: Dict[str, Any] = Field(
         default_factory=lambda: {}, description="metadata for the material"
```

### Comparing `meow-sim-0.6.9/meow/mesh.py` & `meow-sim-0.7.0/meow/mesh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """ a 2D Mesh """
 
+import warnings
+from functools import wraps
 from typing import Literal, Optional, Tuple
 
 import numpy as np
 from pydantic import Field
 from pydantic.types import NonNegativeInt
 
 from .base_model import BaseModel, _array, cached_property
 
 
 class Mesh(BaseModel):
-    """[BaseClass] a ``Mesh`` describes how a ``Structure`` is discretized"""
+    """[BaseClass] a ``Mesh`` describes how a ``Structure3D`` is discretized"""
 
 
-class Mesh2d(Mesh):
-    """a 2D Mesh or ``Mesh2D`` describes how a ``Structure`` is discritized into a ``Cell`` or ``CrossSection``"""
+class Mesh2D(Mesh):
+    """a 2D Mesh or ``Mesh2D`` describes how a ``Structure3D`` is discritized into a ``Cell`` or ``CrossSection``"""
 
     x: np.ndarray[Tuple[int], np.dtype[np.float_]] = Field(
         description="x-coordinates of the mesh (Ez locations, i.e. corners of the 2D cell)"
     )
     y: np.ndarray[Tuple[int], np.dtype[np.float_]] = Field(
         description="y-coordinates of the mesh (Ez locations, i.e. corners of the 2D cell)"
     )
@@ -48,14 +50,23 @@
         ),
     )
     num_pml: Tuple[NonNegativeInt, NonNegativeInt] = Field(
         default=(0, 0),
         description="Number of standard pml layers to add in the two tangential axes.",
     )
 
+    ez_interfaces: bool = Field(
+        default=False,
+        description=(
+            "when enabled, the meshing algorithm will throw away any index values "
+            "at the interfaces which are not on even (Ez) half-grid locations. "
+            "Enabling this should result in more symmetric modes."
+        ),
+    )
+
     @cached_property
     def dx(self):
         """dx at Hz locations, i.e. center of the 2D cell"""
         return (self.x[1:] - self.x[:-1]).view(_array)
 
     @cached_property
     def dy(self):
@@ -146,7 +157,16 @@
         eq = True
         for k, v in self.dict().items():
             if isinstance(v, np.ndarray):
                 eq &= bool(((v - getattr(other, k)) < 1e-6).all())
             else:
                 eq &= bool(v == getattr(other, k))
         return eq
+
+
+@wraps(Mesh2D)
+def Mesh2d(*args, **kwargs):
+    warnings.warn(
+        "Mesh2d is deprecated. Please use Mesh2D (with capital D in the end).",
+        DeprecationWarning,
+    )
+    return Mesh2D(*args, **kwargs)
```

### Comparing `meow-sim-0.6.9/meow/mode.py` & `meow-sim-0.7.0/meow/mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,29 +93,25 @@
 
     @cached_property
     def A(self):
         """mode area"""
         vecE = np.stack([self.Ex, self.Ey, self.Ez], axis=-1)
         E_sq = norm(vecE, axis=-1, ord=2)
         E_qu = E_sq**2
-        x = self.cs.cell.mesh.x_
-        y = self.cs.cell.mesh.y_
+        x = self.cs.mesh.x_
+        y = self.cs.mesh.y_
         return np.float_(integrate_2d(x, y, E_sq) ** 2 / integrate_2d(x, y, E_qu))
 
     @property
     def env(self):
         return self.cs.env
 
     @property
     def mesh(self):
-        return self.cs.cell.mesh
-
-    @property
-    def cell(self):
-        return self.cs.cell
+        return self.cs.mesh
 
     def _visualize(
         self,
         title=None,
         title_prefix="",
         fields=None,
         ax=None,
@@ -175,15 +171,15 @@
         if n_cmap is None:
             # little bit lighter colored than the one in cs._visualize:
             n_cmap = colors.LinearSegmentedColormap.from_list(
                 name="c_cmap", colors=["#ffffff", "#c1d9ed"]
             )
         self.cs._visualize(ax=ax, n_cmap=n_cmap, cbar=False, show=False)
 
-        x, y = "x", "y"  # currently only propagation in z supported, see Mesh2d
+        x, y = "x", "y"  # currently only propagation in z supported, see Mesh2D
         c = {
             "Ex": "x",
             "Ey": "y",
             "Ez": "z",
             "Hx": "y",
             "Hy": "x",
             "Hz": "z_",
@@ -435,15 +431,15 @@
 
     Returns:
         bool: whether the mode is a PML mode or not
     """
     threshold = min(max(threshold, 0.0), 1.0)
     if threshold > 0.999:
         return False
-    numx, numy = mode.cell.mesh.num_pml
+    numx, numy = mode.mesh.num_pml
     ed = energy_density(mode)
     m, n = ed.shape
     lft = ed[:numx, :]
     rgt = ed[m - numx :, :]
     top = ed[numx : m - numx, n:numy]
     btm = ed[numx : m - numx, n - numy :]
     rest = ed[numx : m - numx, numy : n - numy]
@@ -453,15 +449,15 @@
     # the size of the mesh cells would be better here
     is_pml = pml_sum > threshold * (rest_sum + pml_sum)
     return is_pml
 
 
 def te_fraction(mode: Mode) -> float:
     """the TE polarization fraction of the `Mode`"""
-    epsx = mode.cs.nx**2
+    epsx = np.real(mode.cs.nx**2)
     e = np.sum(0.5 * eps0 * epsx * np.abs(mode.Ex) ** 2)
     h = np.sum(0.5 * mu0 * np.abs(mode.Hx) ** 2)
     return float(e / (e + h))
 
 
 def _average(field, direction="forward", axis=0):
     direction = direction.lower()
```

### Comparing `meow-sim-0.6.9/meow/visualize.py` & `meow-sim-0.7.0/meow/visualize.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 
 from meow.structures import visualize_structures
 
 try:
     import matplotlib.pyplot as plt  # fmt: skip
 
+
 except ImportError:
     plt = None
 
 try:
     import gdsfactory as gf  # fmt: skip
 except ImportError:
     gf = None
@@ -183,16 +184,16 @@
         x, y = obj  # type: ignore
         return True
     except Exception:
         return False
 
 
 def _figsize_visualize_mode(cs, W0):
-    x_min, x_max = cs.cell.mesh.x.min(), cs.cell.mesh.x.max()
-    y_min, y_max = cs.cell.mesh.y.min(), cs.cell.mesh.y.max()
+    x_min, x_max = cs.mesh.x.min(), cs.mesh.x.max()
+    y_min, y_max = cs.mesh.y.min(), cs.mesh.y.max()
     delta_x = x_max - x_min
     delta_y = y_max - y_min
     aspect = delta_y / delta_x
     W, H = W0 + 1, W0 * aspect + 1
     return W, H
 
 
@@ -247,17 +248,17 @@
 
 
 def _is_mode_list(obj: Any) -> bool:
     from .mode import Mode  # fmt: skip
     return isinstance(obj, Iterable) and all(isinstance(o, Mode) for o in obj)
 
 
-def _is_structure_list(obj: Any) -> bool:
-    from .structures import Structure  # fmt: skip
-    return isinstance(obj, Iterable) and all(isinstance(o, Structure) for o in obj)
+def _is_structure_3d_list(obj: Any) -> bool:
+    from .structures import Structure3D  # fmt: skip
+    return isinstance(obj, Iterable) and all(isinstance(o, Structure3D) for o in obj)
 
 
 def _is_base_model(obj: Any) -> bool:
     from .base_model import BaseModel  # fmt: skip
     return isinstance(obj, BaseModel)
 
 
@@ -285,15 +286,15 @@
 def _is_gf_component(obj):
     return gf is not None and isinstance(obj, gf.Component)
 
 
 VISUALIZATION_MAPPING: dict[Callable, Callable] = {
     _is_base_model: _visualize_base_model,
     _is_mode_list: _visualize_modes,
-    _is_structure_list: visualize_structures,
+    _is_structure_3d_list: visualize_structures,
     _is_mode_overlap: _visualize_overlap_density,
     _is_s_matrix: _visualize_s_matrix,
     _is_s_pm_matrix: _visualize_s_pm_matrix,
     _is_gf_component: _visualize_gf_component,
 }
```

### Comparing `meow-sim-0.6.9/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.7.0/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.9
+Version: 0.7.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.9/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.7.0/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.9/pyproject.toml` & `meow-sim-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.9"
+version = "0.7.0"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.6.9/tests/test_nbs.py` & `meow-sim-0.7.0/tests/test_nbs.py`

 * *Files identical despite different names*

