# Comparing `tmp/inductance-0.1.2.tar.gz` & `tmp/inductance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductance-0.1.2.tar", max compression
+gzip compressed data, was "inductance-0.1.3.tar", max compression
```

## Comparing `inductance-0.1.2.tar` & `inductance-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-04 08:01:17.006365 inductance-0.1.2/LICENSE
--rw-r--r--   0        0        0     4348 2023-07-04 08:01:17.006365 inductance-0.1.2/README.md
--rw-r--r--   0        0        0     1807 2023-07-04 08:01:39.174371 inductance-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      151 2023-07-04 08:01:17.010365 inductance-0.1.2/src/inductance/__init__.py
--rw-r--r--   0        0        0     1484 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/_numba.py
--rw-r--r--   0        0        0     5201 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/coils.py
--rw-r--r--   0        0        0    27861 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/elliptics.py
--rw-r--r--   0        0        0    14865 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/filaments.py
--rw-r--r--   0        0        0     5476 2023-07-04 08:01:39.178371 inductance-0.1.2/src/inductance/mutual.py
--rw-r--r--   0        0        0    19164 2023-07-04 08:01:39.178371 inductance-0.1.2/src/inductance/self.py
--rw-r--r--   0        0        0     5208 1970-01-01 00:00:00.000000 inductance-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-06 07:22:24.781535 inductance-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4348 2023-07-06 07:22:24.781535 inductance-0.1.3/README.md
+-rw-r--r--   0        0        0     1807 2023-07-06 07:22:43.089342 inductance-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-07-06 07:22:24.781535 inductance-0.1.3/src/inductance/__init__.py
+-rw-r--r--   0        0        0     1481 2023-07-06 07:22:43.089342 inductance-0.1.3/src/inductance/_numba.py
+-rw-r--r--   0        0        0     9912 2023-07-06 07:22:43.089342 inductance-0.1.3/src/inductance/coils.py
+-rw-r--r--   0        0        0    27861 2023-07-06 07:22:24.781535 inductance-0.1.3/src/inductance/elliptics.py
+-rw-r--r--   0        0        0    13358 2023-07-06 07:22:43.089342 inductance-0.1.3/src/inductance/filaments.py
+-rw-r--r--   0        0        0     6226 2023-07-06 07:22:43.089342 inductance-0.1.3/src/inductance/mutual.py
+-rw-r--r--   0        0        0    16355 2023-07-06 07:22:43.089342 inductance-0.1.3/src/inductance/self.py
+-rw-r--r--   0        0        0     3089 2023-07-06 07:22:43.089342 inductance-0.1.3/src/inductance/utils.py
+-rw-r--r--   0        0        0     5208 1970-01-01 00:00:00.000000 inductance-0.1.3/PKG-INFO
```

### Comparing `inductance-0.1.2/LICENSE` & `inductance-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inductance-0.1.2/README.md` & `inductance-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `inductance-0.1.2/pyproject.toml` & `inductance-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inductance"
-version = "0.1.2"
+version = "0.1.3"
 description = "Code for 2D inductance calculations"
 authors = ["Darren Garnier <dgarnier@reinrag.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dgarnier/inductance"
 repository = "https://github.com/dgarnier/inductance"
 documentation = "https://inductance.readthedocs.io"
```

### Comparing `inductance-0.1.2/src/inductance/_numba.py` & `inductance-0.1.3/src/inductance/_numba.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """Try to import numba."""
 
 import os
 
 # try to enable use without numba.  Those with guvectorize will not work.
+
 try:
     from numba import guvectorize, jit, njit, prange
 
     # if numba is diabled, redfine the jit decorator to do nothing
-    # so that coverage testing will work
     if os.getenv("NUMBA_DISABLE_JIT", "0") == "1":  # pragma: no cover
         raise ImportError
 
 except ImportError:  # pragma: no cover
     from inspect import currentframe, getframeinfo
-    from warnings import warn_explicit
+    from warnings import warn, warn_explicit
 
-    _WARNING = (
-        "Numba disabled. Mutual inductance calculations "
-        + "will not be accelerated and some API will not be available."
-    )
-    _finfo = getframeinfo(currentframe())  # type: ignore
-    warn_explicit(_WARNING, RuntimeWarning, _finfo.filename, _finfo.lineno)
+    if not os.getenv("COVERAGE_RUN", ""):  # pragma: no cover
+        _WARNING = "Numba acceleration disabled. Some API will not be available."
+        warn(_WARNING, RuntimeWarning)
 
     def _jit(*args, **kwargs):
         if len(args) == 1 and len(kwargs) == 0 and callable(args[0]):
             # called as @decorator
             return args[0]
         else:
             # called as @decorator(*args, **kwargs)
             return lambda f: f
 
     def _guvectorize(*args, **kwds):
         def fake_decorator(f):
-            warning = f"{f.__name__} requires Numba JIT."
-            finfo = getframeinfo(currentframe().f_back)  # type: ignore
-            warn_explicit(warning, RuntimeWarning, finfo.filename, finfo.lineno)
+            if not os.getenv("COVERAGE_RUN", ""):  # pragma: no cover
+                warning = f"{f.__name__} requires Numba JIT."
+                finfo = getframeinfo(currentframe().f_back)  # type: ignore
+                warn_explicit(warning, RuntimeWarning, finfo.filename, finfo.lineno)
             return lambda f: None
 
         return fake_decorator
 
     guvectorize = _guvectorize
     njit = _jit
     prange = range
     jit = _jit
+
+
+__all__ = ["guvectorize", "jit", "njit", "prange"]
```

### Comparing `inductance-0.1.2/src/inductance/coils.py` & `inductance-0.1.3/src/inductance/coils.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,57 +6,98 @@
 old Mathematica routines and other tests.
 
 Filaments are defined as an numpy 3 element vector
  - r, z, and n.
 """
 from __future__ import annotations
 
+import math
+from dataclasses import dataclass
+from enum import Enum
+
 import numpy as np
 
 from .filaments import (
     filament_coil,
     mutual_inductance_of_filaments,
     radial_force_of_filaments,
-    self_inductance_by_filaments,
     vertical_force_of_filaments,
 )
 from .self import (
     L_long_solenoid_butterworth,
     L_lorentz,
     L_lyle4,
     L_lyle6,
     L_lyle6_appendix,
     L_maxwell,
     dLdR_lyle6,
+    self_inductance_by_filaments,
 )
 
 
+class Shape(Enum):
+    """Enum for conductor shapes."""
+
+    round = "round"
+    hollow_round = "hollow_round"
+    rect = "rectangle"
+
+
+@dataclass
+class Conductor:
+    """Conductor object to keep track of conductor parameters."""
+
+    shape: Shape | str = Shape.round
+    r: float = 0.0
+    dr: float = 0.0
+    dz: float = 0.0
+    r_i: float = 0.0
+    rho: float = 0.0
+
+    def __post_init__(self):
+        """Post init."""
+        if isinstance(self.shape, str):
+            self.shape = Shape(self.shape)
+
+
 class Coil:
     """Rectangular coil object to keep track of coil parameters."""
 
-    def __init__(self, r, z, dr, dz, nt=1, at=1, nr=0, nz=0):
+    def __init__(self, r, z, dr, dz, nt=1, at=None, nr=0, nz=0, theta=0, **kwargs):
         """Create a rectangular coil object.
 
         Args:
             r (float): radial center of coil
             z (float): vertical center of coil
             dr (float): radial width of coil
             dz (float): axial height of coil
-            nt (int): number of turns in coil
+            nt (int, optional): number of turns in coil
             nr (int, optional): Number of radial sections to filament coil. Defaults to 0.
             nz (int, optional): Number of axial sections to filament coil. Defaults to 0.
-            at (float, optional): Amperage of coil. Defaults to 0.
+            at (float, optional): Amperage of coil. Defaults to nt Amps.
+            theta (float, optional): Rotation angle in radians. Defaults to 0.
+            **kwargs: Additional arguments to store in the coil object.
         """
         self.r = r
         self.z = z
         self.dr = dr
         self.dz = dz
         self.nt = nt
+        if at is None:
+            at = nt
         self.at = at
+        self.theta = theta
         self.fils = None
+        self._L = None
+        self._r_c = None
+        self._z_c = None
+
+        if kwargs:
+            for key, value in kwargs.items():
+                setattr(self, key, value)
 
         if (nr > 0) and (nz > 0):
             self.nr = nr
             self.nz = nz
             self.filamentize(nr, nz)
 
     @classmethod
@@ -86,19 +127,52 @@
     def z1(self):  # noqa: D102
         return self.z - self.dz / 2
 
     @property
     def z2(self):  # noqa: D102
         return self.z + self.dz / 2
 
+    @property
+    def r_c(self):  # noqa: D102
+        return self.r if self._r_c is None else self._r_c
+
+    @property
+    def z_c(self):  # noqa: D102
+        return self.z if self._z_c is None else self._z_c
+
+    @property
+    def conductor_length(self):  # noqa: D102
+        return self.r * self.nt * 2 * math.pi
+
+    def L_best(self):
+        """Inductance by best formula."""
+        if self.dz < 0.2 * self.r:
+            # Lyle's formula is not valid for long coils
+            # as its an expansion in dz/r
+            return self.L_Lyle6()
+        else:
+            return self.L_filament()
+
+    @property
+    def L(self):  # noqa: D102
+        if self._L is None:
+            self._L = self.L_best()
+        return self._L
+
+    @L.setter
+    def L(self, value):
+        self._L = value
+
     def filamentize(self, nr, nz):
         """Create an array of filaments to represent the coil."""
         self.nr = nr
         self.nz = nz
-        self.fils = filament_coil(self.r, self.z, self.dr, self.dz, self.nt, nr, nz)
+        self.fils = filament_coil(
+            self.r, self.z, self.dr, self.dz, self.nt, nr, nz, theta=self.theta
+        )
 
     def L_Maxwell(self):
         """Inductance by Maxwell's formula."""
         return L_maxwell(self.r, self.dr, self.dz, self.nt)
 
     def L_Lyle4(self):
         """Inductance by Lyle's formula, 4th order."""
@@ -108,19 +182,34 @@
         """Inductance by Lyle's formula, 6th order."""
         return L_lyle6(self.r, self.dr, self.dz, self.nt)
 
     def L_Lyle6A(self):
         """Inductance by Lyle's formula, 6th order, appendix."""
         return L_lyle6_appendix(self.r, self.dr, self.dz, self.nt)
 
-    def L_filament(self):
+    def L_filament(self, nr=0, nz=0):
         """Inductance by filamentation."""
-        return self_inductance_by_filaments(
-            self.fils, conductor="rect", dr=self.dr / self.nr, dz=self.dz / self.nz
-        )
+        if nr != 0 and nz != 0:
+            self.filamentize(nr, nz)
+        cond = getattr(self, "conductor", None)
+        if cond is None:
+            return self_inductance_by_filaments(
+                self.fils,
+                conductor=Shape.rect.name,
+                dr=self.dr / self.nr,
+                dz=self.dz / self.nz,
+            )
+        elif "round" in cond.shape.value:
+            return self_inductance_by_filaments(
+                self.fils, conductor=cond.shape.name, a=cond.r
+            )
+        elif "rect" in cond.shape.value:
+            return self_inductance_by_filaments(
+                self.fils, conductor=cond.shape.name, dr=cond.dr, dz=cond.dz
+            )
 
     def L_long_solenoid_butterworth(self):
         """Inductance by Butterworth's formula."""
         return L_long_solenoid_butterworth(self.r, self.dr, self.dz, self.nt)
 
     def L_lorentz(self):
         """Inductance by Lorentz's formula."""
@@ -149,15 +238,94 @@
         F_r2 = radial_force_of_filaments(self.fils, C2.fils)
         return self.at / self.nt * C2.at / C2.nt * F_r2
 
 
 class CompositeCoil(Coil):
     """A coil made of multiple rectangular coils."""
 
-    def __init__(self, coils: list[Coil]):
+    def __init__(self, coils: list[Coil], **kwargs):
         """Create a composite coil from a list of _filamented_ coils."""
         self.coils = coils
-        self.nt = sum(coil.nt for coil in coils)
-        self.at = sum(coil.at for coil in coils)
-        self.r = sum(coil.r * coil.nt for coil in coils) / self.nt
-        self.z = sum(coil.z * coil.nt for coil in coils) / self.nt
+        nt = sum(coil.nt for coil in coils)
+        at = sum(coil.at for coil in coils)
+        r1 = min(coil.r - coil.dr for coil in coils)
+        r2 = max(coil.r + coil.dr for coil in coils)
+        r = (r1 + r2) / 2
+        dr = r2 - r1
+        z1 = min(coil.z - coil.dz for coil in coils)
+        z2 = max(coil.z + coil.dz for coil in coils)
+        z = (z1 + z2) / 2
+        dz = z2 - z1
+        Coil.__init__(self, r, z, dr, dz, nt, at, **kwargs)
+        self._r_c = sum(coil.r * coil.nt for coil in coils) / nt
+        self._z_c = sum(coil.z * coil.nt for coil in coils) / nt
         self.fils = np.concatenate([coil.fils for coil in coils])
+
+    @property
+    def conductor_length(self):  # noqa: D102
+        return sum(coil.conductor_length for coil in self.coils)
+
+    def L_best(self):
+        """Inductance of composite coils by best formula."""
+        L = 0
+        for i, c1 in enumerate(self.coils):
+            for j, c2 in enumerate(self.coils):
+                if i == j:
+                    L += c1.L
+                else:
+                    L += c1.M_filament(c2)
+        return L
+
+
+def coilset_mutual_inductance(coils: list[Coil]):
+    """Get the inductance matrix of a set of coils.
+
+    Args:
+        coils (list[Coil]): set of coils
+
+    Returns:
+        np.ndarray: 2D array of inductances
+    """
+    muts = np.zeros([len(coils), len(coils)], dtype=float)
+    for i, ci in enumerate(coils):
+        for j, cj in enumerate(coils):
+            if i == j:
+                muts[i, j] = ci.L
+            else:
+                muts[i, j] = ci.M_filament(cj)
+    return muts
+
+
+def coilset_Fz_greens(coils: list[Coil]):
+    """Calculate the vertical force matrix of a set of coils.
+
+    Args:
+        coils (list[Coil]): set of coils
+
+    Returns:
+        np.ndarray: 2D array of vertical forces per amp**2
+    """
+    mfz = np.zeros([len(coils), len(coils)], dtype=float)
+    for i, ci in enumerate(coils):
+        for j, cj in enumerate(coils):
+            if i != j:
+                mfz[i, j] = ci.Fz_filament(cj)
+    return mfz
+
+
+def coilset_Fr_greens(coils: list[Coil]):
+    """Calculate the radial force matrix of a set of coils.
+
+    Args:
+        coils (list[Coil]): set of coils
+
+    Returns:
+        np.ndarray: 2D array of radial forces per amp**2
+    """
+    muts = np.zeros([len(coils), len(coils)], dtype=float)
+    for i, ci in enumerate(coils):
+        for j, cj in enumerate(coils):
+            if i == j:
+                muts[i, j] = ci.Fr_self()
+            else:
+                muts[i, j] = ci.Fr_filament(cj)
+    return muts
```

### Comparing `inductance-0.1.2/src/inductance/elliptics.py` & `inductance-0.1.3/src/inductance/elliptics.py`

 * *Files identical despite different names*

### Comparing `inductance-0.1.2/src/inductance/filaments.py` & `inductance-0.1.3/src/inductance/filaments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """Filamentary inductance calculations."""
 
+import math
+
 import numpy as np
 
 from ._numba import guvectorize, njit, prange
 from .elliptics import ellipke
-from .self import L_hollow_round, L_lyle6, L_round, _lyle_terms
+from .utils import rectangle_GMD, section_coil
 
 
 @njit
 def mutual_inductance_fil(rzn1, rzn2):
     """Mutual inductance of two filaments.
 
     Args:
         rzn1 (array): (r, z, n) of first filament
         rzn2 (array): (r, z, n) of second filament
 
     Returns:
         float: mutual inductance in Henrys
     """
-    r1 = rzn1[0]
-    r2 = rzn2[0]
-    z1 = rzn1[1]
-    z2 = rzn2[1]
-    n1 = rzn1[2]
-    n2 = rzn2[2]
+    r1, z1, n1 = rzn1
+    r2, z2, n2 = rzn2
 
     k2 = 4 * r1 * r2 / ((r1 + r2) ** 2 + (z1 - z2) ** 2)
     elk, ele = ellipke(k2)
-    amp = 2 * np.pi * r1 * 4e-7 * r2 / np.sqrt((r1 + r2) ** 2 + (z1 - z2) ** 2)
+    amp = 2 * math.pi * r1 * 4e-7 * r2 / math.sqrt((r1 + r2) ** 2 + (z1 - z2) ** 2)
     M0 = n1 * n2 * amp * ((2 - k2) * elk - 2 * ele) / k2
     return M0
 
 
 @njit
 def vertical_force_fil(rzn1, rzn2):
     """Vertical force  between two filaments per conductor amp.
@@ -39,46 +37,38 @@
     Args:
         rzn1 (array): (r, z, n) of first filament
         rzn2 (array): (r, z, n) of second filament
 
     Returns:
         float: force in Newtons/Amp^2
     """
-    r1 = rzn1[0]
-    r2 = rzn2[0]
-    z1 = rzn1[1]
-    z2 = rzn2[1]
-    n1 = rzn1[2]
-    n2 = rzn2[2]
+    r1, z1, n1 = rzn1
+    r2, z2, n2 = rzn2
 
     BrAt1 = BrGreen(r1, z1, r2, z2)
-    F = n1 * n2 * 2 * np.pi * r1 * BrAt1
+    F = n1 * n2 * 2 * math.pi * r1 * BrAt1
     return F
 
 
 @njit
 def radial_force_fil(rzn1, rzn2):
     """Radial force  between two filaments per conductor amp.
 
     Args:
         rzn1 (array): (r, z, n) of first filament
         rzn2 (array): (r, z, n) of second filament
 
     Returns:
         float: force in Newtons/Amp^2
     """
-    r1 = rzn1[0]
-    r2 = rzn2[0]
-    z1 = rzn1[1]
-    z2 = rzn2[1]
-    n1 = rzn1[2]
-    n2 = rzn2[2]
+    r1, z1, n1 = rzn1
+    r2, z2, n2 = rzn2
 
     BzAt1 = BzGreen(r1, z1, r2, z2)
-    F = n1 * n2 * 2 * np.pi * r1 * BzAt1
+    F = n1 * n2 * 2 * math.pi * r1 * BzAt1
     return F
 
 
 #
 #  Green's functions for filaments
 #
 
@@ -94,15 +84,15 @@
         b (float): vertical position of a filament
 
     Returns:
         float: Psi at r, z in Weber / Amp
     """
     k2 = 4 * a * r / ((r + a) ** 2 + (z - b) ** 2)
     elk, ele = ellipke(k2)
-    amp = 4e-7 * a / np.sqrt((r + a) ** 2 + (z - b) ** 2)
+    amp = 4e-7 * a / math.sqrt((r + a) ** 2 + (z - b) ** 2)
     return amp * ((2 - k2) * elk - 2 * ele) / k2
 
 
 @njit
 def BrGreen(r, z, a, b):
     """Br at position r, z, due to a filament with radius a, and z postion b.
 
@@ -113,15 +103,15 @@
         b (float): vertical position of a filament
 
     Returns:
         float: Br at r, z in Tesla / Amp
     """
     k2 = 4 * a * r / ((r + a) ** 2 + (z - b) ** 2)
     elk, ele = ellipke(k2)
-    amp = -2e-7 / np.sqrt((r + a) ** 2 + (z - b) ** 2)
+    amp = -2e-7 / math.sqrt((r + a) ** 2 + (z - b) ** 2)
     Gr = (a**2 + r**2 + (z - b) ** 2) / ((r - a) ** 2 + (z - b) ** 2)
     return amp * (z - b) / r * (Gr * ele - elk)
 
 
 @njit
 def BzGreen(r, z, a, b):
     """Bz at position r, z, due to a filament with radius a, and z postion b.
@@ -133,15 +123,15 @@
         b (float): vertical position of a filament
 
     Returns:
         float: Bz at r, z in Tesla / Amp
     """
     k2 = 4 * a * r / ((r + a) ** 2 + (z - b) ** 2)
     elk, ele = ellipke(k2)
-    amp = -2e-7 / np.sqrt((r + a) ** 2 + (z - b) ** 2)
+    amp = -2e-7 / math.sqrt((r + a) ** 2 + (z - b) ** 2)
     Gz = (a**2 - r**2 - (z - b) ** 2) / ((r - a) ** 2 + (z - b) ** 2)
     return amp * (Gz * ele + elk)
 
 
 @njit(parallel=True)
 def green_sum_over_filaments(gfunc, fil, r, z):
     """Calculate a greens function at position r, z, to an array of filaments.
@@ -151,24 +141,23 @@
         fil (array): filament array N x (r, z, n)
         r (float): radial position of a point
         z (float): vertical position of a point
 
     Returns:
         float: sum of the greens function at r, z, due to all filaments
     """
-    tmp = np.zeros_like(r)
-    tshp = tmp.shape
-    tmp = tmp.reshape((tmp.size,))
-    rf = r.reshape((tmp.size,))
-    zf = z.reshape((tmp.size,))
-    for j in prange(len(tmp)):
+    gr = np.zeros_like(r)  # numba must compile this in object mode
+    gf = gr.flat
+    rf = r.flat
+    zf = z.flat
+
+    for j in prange(len(gr)):  # numba will njit this loop
         for i in range(fil.shape[0]):
-            tmp.flat[j] += fil[i, 2] * gfunc(rf[j], zf[j], fil[i, 0], fil[i, 1])
-    tmp = tmp.reshape(tshp)
-    return tmp
+            gf[j] += fil[i, 2] * gfunc(rf[j], zf[j], fil[i, 0], fil[i, 1])
+    return gr
 
 
 def segment_path(pts, ds=0, close=False):
     """Segment a path into equal length segments.
 
     Args:
         pts (array): N x 3 array of points
@@ -204,15 +193,15 @@
     # segments is array of n x 3 (x,y,z)
     # segments should contain first point at start AND end.
     # r, z is r & z of loop
     M = float(0)
     for i in range(pts.shape[0] - 1):
         midp = (pts[i, :] + pts[i + 1, :]) / 2
         delta = pts[i, :] - pts[i + 1, :]
-        rs = np.sqrt(midp[0] ** 2 + midp[1] ** 2)
+        rs = math.sqrt(midp[0] ** 2 + midp[1] ** 2)
         zs = midp[2]
         rdphi = (delta[0] * midp[1] - delta[1] * midp[0]) / rs
         M += AGreen(r, z, rs, zs) * rdphi
 
     return M
 
 
@@ -247,15 +236,15 @@
     mu_0/(4*pi) * int * int ( dx1 . dx2 / norm(x1-x2)))
     do all points except where x1-x2 blows up.
     instead follow Dengler https://doi.org/10.7716/aem.v5i1.331
     which makes a approximation for that is good O(mu_0*a)
     lets just assume the thing is broken into small pieces and neglect end points
 
     this code doesn't work very well.. comparison test sorta fails
-    phi = np.linspace(0,2*np.pi,100)
+    phi = np.linspace(0,2*math.pi,100)
     test_xyz = np.array([[np.cos(p), np.sin(p), 0] for p in phi])
     L_seg = L_approx_path_rect(test_xyz, .01, .01, 1, .1)
     L_maxwell(1, .01, .01, 1), L_lyle6(1, .01, .01, 1), L_seg
     (6.898558527897293e-06, 6.8985981243869525e-06, 6.907313505254537e-06) # Y=1/4 hmmm...
     (6.898558527897293e-06, 6.8985981243869525e-06, 7.064366776069971e-06) # Y=1/2
     """
     ds = s[1] - s[0]  # the real ds and thus the real b
@@ -270,23 +259,21 @@
     for i in prange(npts):
         for j in range(npts):
             if i != j:
                 L += np.dot(dx[i], dx[j]) / np.linalg.norm(x[i] - x[j])
     return 1e-7 * (L + LS)
 
 
-def L_approx_path_rect(pts, b, c, n, ds=1):
+def L_approx_path_rect(pts, w, h, n, ds=1):
     """Approximate self inductance of a path of points with a rectangular cross section.
 
     take a path of points n x 3, with a cross section b x c
     and approximate self inductance using Dengler
     """
-    _, _, _, _, _, _, a = _lyle_terms(
-        b, c
-    )  # get Maxwell mean radius to approximate "wire" radius
+    a = rectangle_GMD(w, h)  # get Maxwell mean radius to approximate "wire" radius
     ds *= a
     segs, s = segment_path(pts, ds)
     L = n**2 * segmented_self_inductance(segs, s, a)
     return L
 
 
 # for some reason, these are slightly slower than the above.
@@ -351,38 +338,30 @@
         tmp = 0.0
         for i in range(len(fil)):
             tmp += fil[i, 2] * AGreen(r[j], z[j], fil[i, 0], fil[i, 1])
         gr[j] = tmp
 
 
 # cant jit this... meshgrid not allowed
-def filament_coil(r, z, dr, dz, nt, nr, nz, rot=0):
+def filament_coil(r, z, dr, dz, nt, nr, nz, theta=0):
     """Create an array of filaments, each with its own radius, height, and amperage.
 
     r : Major radius of coil center.
     z : Vertical center of coil.
     dr : Radial width of coil.
     dz : Height of coil.
     nt : number of turns in coil
     nr : Number of radial slices
     nz : Number of vertical slices
-    rot : Rotation of coil about phi axis
+    theta : Rotation of coil about phi axis
 
     Returns:    Array of shape (nr*nz) x 3 of R, Z, N for each filament
-
     """
-    rd = np.linspace(-dr * (nr - 1) / nr / 2, dr * (nr - 1) / nr / 2, nr)
-    zd = np.linspace(-dz * (nz - 1) / nz / 2, dz * (nz - 1) / nz / 2, nz)
-    Rg, Zg = np.meshgrid(rd, zd)
-
-    R = r + Rg * np.cos(rot) - Zg * np.sin(rot)
-    Z = z + Rg * np.sin(rot) + Zg * np.cos(rot)
-
-    N = np.full_like(R, float(nt) / (nr * nz))
-    return np.dstack([R, Z, N]).reshape(nr * nz, 3)
+    sects = section_coil(r, z, dr, dz, nt, nr, nz, theta=theta)
+    return sects[:, [0, 1, 4]]
 
 
 @njit(parallel=True)
 def sum_over_filaments(func, f1, f2):
     """Apply a function and sum over all combinations of two sets of filaments.
 
     Args:
@@ -418,42 +397,14 @@
     for i in prange(f1.shape[0]):
         for j in range(f2.shape[0]):
             M += mutual_inductance_fil(f1[i, :], f2[j, :])
     return M
 
 
 @njit(parallel=True)
-def self_inductance_by_filaments(f, conductor="round", a=0.01, dr=0.01, dz=0.01):
-    """Self inductance of filament set.
-
-    Args:
-        f (array): first filament array
-        conductor (str, optional): conductor shape. Defaults to "round".
-        a (float, optional): conductor radius. Defaults to 0.01.
-        dr (float, optional): conductor radial width. Defaults to 0.01
-        dz (float, optional): conductor vertical height. Defaults to 0.01
-
-    Returns:
-        float: self inductance of filament set in Henries
-    """
-    L = float(0)
-    for i in prange(f.shape[0]):
-        for j in range(f.shape[0]):
-            if i != j:
-                L += mutual_inductance_fil(f[i, :], f[j, :])
-        if conductor == "round":
-            L += L_round(f[i, 0], a, f[i, 2])
-        elif conductor == "hollow_round":
-            L += L_hollow_round(f[i, 0], a, f[i, 2])
-        elif conductor == "rect":
-            L += L_lyle6(f[i, 0], dr, dz, f[i, 2])
-    return L
-
-
-@njit(parallel=True)
 def vertical_force_of_filaments(f1, f2):
     """Vertical force between two sets of filaments.
 
     These should not be the same filament array,
     not setup to handle self inductance of filament.
 
     Args:
```

### Comparing `inductance-0.1.2/src/inductance/mutual.py` & `inductance-0.1.3/src/inductance/mutual.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 """
 import math
 
 import numpy as np
 
 from ._numba import njit
-
-# from .elliptics import ellipke
 from .filaments import mutual_inductance_fil, mutual_inductance_of_filaments
-
-MU0 = 4e-7 * math.pi  # permeability of free space
+from .utils import section_coil
 
 
 @njit
 def mutual_rayleigh(r1, z1, dr1, dz1, n1, r2, z2, dr2, dz2, n2):
     """Mutual inductance of two coils by Rayleigh's Quadrature Method.
 
+    reproduced in :
+    Rosa and Grover, "Formulas for the Mutual Inductance of
+    Coaxial Circular Coils of Rectangular Section,"
+    Bull. Natl. Bur. Stand., vol 8, no. 1, p. 34-35; 1911.
+
     Args:
         r1 (float): inner radius of coil 1
         z1 (float): inner height of coil 1
         dr1 (float): radial width of coil 1
         dz1 (float): height of coil 1
         n1 (int): number of turns in coil 1
         r2 (float): inner radius of coil 2
@@ -65,111 +67,125 @@
     m_ray += mutual_inductance_fil(rzn1[0, :], rzn2[2, :])
     m_ray += mutual_inductance_fil(rzn1[0, :], rzn2[3, :])
     m_ray += mutual_inductance_fil(rzn1[0, :], rzn2[4, :])
     return n1 * n2 * m_ray / 6
 
 
 @njit
-def mutual_lyle(r1, z1, dr1, dz1, n1, r2, z2, dr2, dz2, n2):
-    """Mutual inductance of two coils by Lyle's Method of Equivalent Filaments.
-
-    Args:
-        r1 (float): inner radius of coil 1
-        z1 (float): inner height of coil 1
-        dr1 (float): radial width of coil 1
-        dz1 (float): height of coil 1
-        n1 (int): number of turns in coil 1
-        r2 (float): inner radius of coil 2
-        z2 (float): inner height of coil 2
-        dr2 (float): radial width of coil 2
-        dz2 (float): height of coil 2
-        n2 (int): number of turns in coil 2
+def lyle_equivalent_filaments(r, z, dr, dz, nt, fils):
+    """Compute the equivalent filament locations for Lyle's method.
 
-    Returns:
-        float: mutual inductance of the two coils
-    """
-    fils1 = _lyle_equivalent_filaments(r1, z1, dr1, dz1)
-    fils2 = _lyle_equivalent_filaments(r2, z2, dr2, dz2)
-    return n1 * n2 * mutual_inductance_of_filaments(fils1, fils2)
+    Using Lyle's Method of Equivalent Filaments.
 
+    originally from:
+        Lyle, Phil. Mag., 3, p. 310; 1902.
 
-@njit
-def _lyle_equivalent_filaments(r, z, dr, dz):
-    """Compute the equivalent filament locations for Lyle's method.
+    reproduced in:
+        Rosa and Grover, "Formulas for the Mutual Inductance of
+        Coaxial Circular Coils of Rectangular Section,"
+        Bull. Natl. Bur. Stand., vol 8, no. 1, p. 38-39; 1911.
 
     Args:
         r (float): inner radius of coil
         z (float): inner height of coil
         dr (float): radial width of coil
         dz (float): height of coil
-
-    Returns:
-        numpy.ndarray: equivalent filament locations
+        nt (float): number of turns in coil
+        fils (numpy.ndarray): array of filaments 2 x (r, z, n)
     """
     if dr < dz:
         req = r * (1 + dr**2 / (24 * r**2))
         beta = math.sqrt((dz**2 - dr**2) / 12)
-        fils = [[req, z - beta, 0.5], [req, z + beta, 0.5]]
+        fils[:, 0] = req
+        fils[:, 1] = z - beta, z + beta
     elif dr > dz:
         req = r * (1 + dz**2 / (24 * r**2))
-        delta = math.sqrt((dz**2 - dr**2) / 12)
-        fils = [[req - delta, z, 0.5], [req + delta, z, 0.5]]
+        delta = math.sqrt((dr**2 - dz**2) / 12)
+        fils[:, 0] = req - delta, req + delta
+        fils[:, 1] = z
     else:
         req = r * (1 + dz**2 / (24 * r**2))
-        fils = [[req, z, 1]]
+        fils[:, 0] = req
+        fils[:, 1] = z
+    fils[:, 2] = 0.5 * nt
 
-    return np.array(fils)
 
+@njit
+def mutual_lyles_method(r1, z1, dr1, dz1, nt1, r2, z2, dr2, dz2, nt2):
+    """Mutual inductance of two coils by Lyle's method.
 
-def section_coil(r, z, dr, dz, nt, nr, nz):
-    """Create an array of filaments, each with its own radius, height, and amperage.
+    Using Lyle's Method of Equivalent Filaments.
 
-    r : Major radius of coil center.
-    z : Vertical center of coil.
-    dr : Radial width of coil.
-    dz : Height of coil.
-    nt : number of turns in coil
-    nr : Number of radial slices
-    nz : Number of vertical slices
+    originally from:
+    Lyle, Phil. Mag., 3, p. 310; 1902.
 
-    Returns:    Array of shape (nr*nz) x 5 of r, z, dr, dz, n for each section
+    reproduced:
+    Rosa and Grover, "Formulas for the Mutual Inductance of
+    Coaxial Circular Coils of Rectangular Section,"
+    Bull. Natl. Bur. Stand., vol 8, no. 1, p. 38-39; 1911.
 
+    Args:
+        r1 (float): inner radius of coil 1
+        z1 (float): inner height of coil 1
+        dr1 (float): radial width of coil 1
+        dz1 (float): height of coil 1
+        nt1 (int): number of turns in coil 1
+        r2 (float): inner radius of coil 2
+        z2 (float): inner height of coil 2
+        dr2 (float): radial width of coil 2
+        dz2 (float): height of coil 2
+        nt2 (int): number of turns in coil 2
+
+    Returns:
+        float: mutual inductance of the two coils
     """
-    rd = np.linspace(-dr * (nr - 1) / nr / 2, dr * (nr - 1) / nr / 2, nr)
-    zd = np.linspace(-dz * (nz - 1) / nz / 2, dz * (nz - 1) / nz / 2, nz)
-    Rg, Zg = np.meshgrid(rd, zd)
+    fils1 = np.zeros(2, 3)
+    fils2 = np.zeros(2, 3)
+
+    lyle_equivalent_filaments(r1, z1, dr1, dz1, nt1, fils1)
+    lyle_equivalent_filaments(r2, z2, dr2, dz2, nt2, fils1)
+    return mutual_inductance_of_filaments(fils1, fils2)
 
-    R = r + Rg
-    Z = z + Zg
 
-    DR = np.full_like(R, dr / nr)
-    DZ = np.full_like(R, dz / nz)
-    NT = np.full_like(R, float(nt) / (nr * nz))
+@njit
+def lyle_equivalent_subcoil_filaments(subcoils):
+    """Compute the equivalent filament locations for set of subcoils."""
+    fils = np.zeros((subcoils.shape[0], 2, 3))
+    for i in range(subcoils.shape[0]):
+        lyle_equivalent_filaments(*subcoils[i, :], fils[i, :, :])
+    return fils
 
-    return np.dstack([R, Z, DR, DZ, NT]).reshape(nr * nz, 5)
 
+def mutual_sectioning_lyle(
+    r1, z1, dr1, dz1, nt1, nr1, nz1, r2, z2, dr2, dz2, nt2, nr2, nz2
+):
+    """Mutual inductance by sectioning of two coils by Lyle's Method.
 
-def mutual_sectioning_lyle(r1, z1, dr1, dz1, n1, r2, z2, dr2, dz2, n2):
-    """Mutual inductance by sectioning of two coils by Lyle's Method of Equivalent Filaments.
+    Section cois into subcoils and compute mutual inductance of each set
+    of subcoil using Lyle's method of equivalent filaments.
 
     Args:
         r1 (float): inner radius of coil 1
         z1 (float): inner height of coil 1
         dr1 (float): radial width of coil 1
         dz1 (float): height of coil 1
-        n1 (int): number of turns in coil 1
+        nt1 (float): number of turns in coil 1
+        nr1 (int): number of radial sections in coil 1
+        nz1 (int): number of vertical sections in coil 1
         r2 (float): inner radius of coil 2
         z2 (float): inner height of coil 2
         dr2 (float): radial width of coil 2
         dz2 (float): height of coil 2
-        n2 (int): number of turns in coil 2
+        nt2 (float): number of turns in coil 2
+        nr2 (int): number of radial sections in coil 2
+        nz2 (int): number of vertical sections in coil 2
 
     Returns:
         float: mutual inductance of the two coils
     """
-    # FIXME
-    # use section_coil
-    # need to be clever to keep it numba compatible
-
-    fils1 = _lyle_equivalent_filaments(r1, z1, dr1, dz1)
-    fils2 = _lyle_equivalent_filaments(r2, z2, dr2, dz2)
-    return n1 * n2 * mutual_inductance_of_filaments(fils1, fils2)
+    subs_1 = section_coil(r1, z1, dr1, dz1, nt1, nr1, nz1)
+    subs_2 = section_coil(r2, z2, dr2, dz2, nt2, nr2, nz2)
+
+    fils_1 = lyle_equivalent_subcoil_filaments(subs_1).reshape(-1, 3)
+    fils_2 = lyle_equivalent_subcoil_filaments(subs_2).reshape(-1, 3)
+
+    return mutual_inductance_of_filaments(fils_1, fils_2)
```

### Comparing `inductance-0.1.2/src/inductance/self.py` & `inductance-0.1.3/src/inductance/self.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,89 +19,24 @@
 numba-scipy can be fragile and sometimes needs to be "updated" before installation
 to the newest version of numba.
 """
 import math
 
 import numpy as np
 
-from ._numba import njit
+from ._numba import njit, prange
 from .elliptics import ellipke
-
-try:
-    from mpmath import mp  # type: ignore
-
-    USE_MPMATH = True
-except ImportError:  # pragma: no cove
-    USE_MPMATH = False
+from .filaments import mutual_inductance_fil
+from .mutual import lyle_equivalent_subcoil_filaments, mutual_lyles_method
+from .utils import _lyle_terms, section_coil
 
 MU0 = 4e-7 * math.pi  # permeability of free space
 
 
 @njit
-def _lyle_terms(b, c):
-    #  helper functions for most self inductance equations.
-    # b : cylindrical height of coil
-    # c : radial width of coil
-
-    # FIXME:  when b/c or c/b is very large or small, this diverges
-    #         and gives inaccurate results when b/c ~ 1e6 or 1e-6
-    # phi should approach 1.5 and GMD should approach (b+c)*exp(-1.5)
-
-    # for small b/c, u and wp need to be calculated with more precision
-    # for small c/b, v and w need more precision
-    # will try to use limit functions
-
-    boc2 = (b / c) ** 2
-    if b == 0:
-        u, v, w, p = 0, 1, 0, 1
-    elif c == 0:
-        u, v, w, p = 1, 0, 1, 0
-    elif boc2 < 1e-8:
-        u = -boc2 * math.log(boc2) + boc2**2 - boc2**3 / 2
-        v = 1 - boc2 / 2 + boc2**2 / 3
-        w = math.pi / 2 * (b / c) - boc2 + boc2**2 / 3
-        p = 1 - boc2 / 3 + boc2**2 / 5
-    elif boc2 > 1e8:
-        cob2 = (c / b) ** 2
-        u = 1 - cob2 / 2 + cob2**2 / 3
-        v = -cob2 * math.log(cob2) + cob2**2 - cob2**3 / 2
-        w = 1 - cob2 / 3 + cob2**2 / 5  # taylor series
-        p = math.pi / 2 * (c / b) - cob2 + cob2**2 / 3  # laurent series
-    else:
-        u = ((b / c) ** 2) * math.log(1 + (c / b) ** 2)
-        v = ((c / b) ** 2) * math.log(1 + (b / c) ** 2)
-        w = (b / c) * math.atan2(c, b)
-        p = (c / b) * math.atan2(b, c)
-
-    d = np.sqrt(b**2 + c**2)  # diagnonal length
-    phi = (u + v + 25) / 12 - 2 * (w + p) / 3
-    GMD = d * np.exp(-phi)  # geometric mean radius of section GMD
-
-    return d, u, v, w, p, phi, GMD
-
-
-if USE_MPMATH:  # pragma: no cover
-
-    def _lyle_terms_mp(b, c):
-        # b : cylindrical height of coil
-        # c : radial width of coil
-
-        # this does NOT fix problem with b/c ~ 1e6 or 1e-6
-
-        d = mp.sqrt(b**2 + c**2)  # diagnonal length
-        u = ((b / c) ** 2) * 2 * mp.log(d / b)
-        v = ((c / b) ** 2) * 2 * mp.log(d / c)
-        w = (b / c) * mp.atan(c / b)
-        wp = (c / b) * mp.atan(b / c)
-        phi = (u + v + 25) / 12 - 2 * (w + wp) / 3
-        GMD = d * mp.exp(-phi)  # geometric mean radius of section GMD
-        return d, u, v, w, wp, phi, GMD
-
-
-@njit
 def L_maxwell(r, dr, dz, n):
     """Self inductance of a rectangular coil with constant current density by Maxwell.
 
     Args:
         r (float): coil centerline radius
         dr (float): coil radial width
         dz (float): coil height
@@ -147,15 +82,15 @@
         float: coil self inductance in Henrys
     """
     L = MU0 * (n**2) * r * (math.log(8 * r / a) - 2)
     return L
 
 
 @njit
-def L_lyle4_eq3(r, dr, dz, n):
+def L_lyle4(r, dr, dz, n):
     """Self inductance of a rectangular coil via Lyle to 4th order, Eq3.
 
     Args:
         r (float): coil centerline radius
         dr (float): coil radial width
         dz (float): coil height
         n (int): number of turns
@@ -211,20 +146,24 @@
     )
     return eq3
 
 
 # equation 4.. slightly different result... not sure which is better.
 # equation 3 above matches what I did for the 6th order.
 # and it also seems to match the 4th order in the paper.
+# and in other papers with examples
 
 
 @njit
 def L_lyle4_eq4(r, dr, dz, n):
     """Self inductance of a rectangular coil via Lyle to 4th order, Eq4.
 
+    this doesn't give quite the same answer as eq3 above.
+    and it doesn't seem to work as well.
+
     Args:
         r (float): coil centerline radius
         dr (float): coil radial width
         dz (float): coil height
         n (int): number of turns
 
     Returns:
@@ -275,17 +214,14 @@
     A = a * (1 + m1 * (d / a) ** 2 + m2 * (d / a) ** 4)
     R = GMD * (1 + n1 * (d / a) ** 2 + n2 * (d / a) ** 4 + n3 * (d / a) ** 6)
 
     eq4 = MU0 * (n**2) * A * (np.log(8 * A / R) - 2)
     return eq4
 
 
-L_lyle4 = L_lyle4_eq3
-
-
 @njit
 def L_lyle6(r, dr, dz, n):
     """Self inductance of a rectangular coil via Lyle to 6th order.
 
     Args:
         r (float): coil centerline radius
         dr (float): coil radial width
@@ -443,97 +379,46 @@
             - 617423 / (2**2 * 3**2 * 5) * b**4 * c**2
             - 8329 / (2**2 * 3 * 5) * b**2 * c**4
             + 4308631 / (2**3 * 3 * 5 * 7) * c**6
         )
     )
 
     # just add the correction to the 4th order solution
-    L6 = L_lyle4_eq3(r, dr, dz, n) + 4e-7 * np.pi * (n**2) * a * (d / a) ** 6 * (
+    L6 = L_lyle4(r, dr, dz, n) + 4e-7 * np.pi * (n**2) * a * (d / a) ** 6 * (
         p6 * np.log(8 * a / d) + q6
     )
     # print("Lyle6A r: %.4g, dr: %.4g, dz: %4g, n: %d, L: %.8g"%(a,c,b,n,L6))
     return L6
 
 
-if USE_MPMATH:
-
-    def L_lyle6_mp(r, dr, dz, n):
-        """Self inductance of a rectangular coil via Lyle to 6th order.
+@njit
+def L_lyle_sectioning(r, dr, dz, nt, nr, nz):
+    """Self inductance by sectioning, Lyle's method, and Lyle's 4th order.
 
-        This function uses the mpmath arbitrary precision library to
-        calculate to arbitrary precision.  The default precision is 30.
+    Args:
+        r (float): coil centerline radius
+        dr (float): coil radial width
+        dz (float): coil height
+        nt (float): number of turns
+        nr (int): number of radial sections
+        nz (int): number of axial sections
 
-        Args:
-            r (float): coil centerline radius
-            dr (float): coil radial width
-            dz (float): coil height
-            n (int): number of turns
-
-        Returns:
-            float: coil self inductance in Henrys
-        """
-        mp.dps = 30
-        a = mp.mpf(r)
-        b = mp.mpf(dz)
-        c = mp.mpf(dr)
-        d, u, v, w, wp, phi, GMD = _lyle_terms_mp(b, c)
-        ML = mp.log(8 * a / d)
-
-        f = (
-            ML
-            + (u + v + 1) / 12
-            - mp.mpf(2) / 3 * (w + wp)
-            + 1
-            / (2**5 * 3 * a**2)
-            * (
-                (3 * b**2 + c**2) * ML
-                + mp.mpf(1) / 2 * b**2 * u
-                - 1.0 / 10 * c**2 * v
-                - 16.0 / 5 * b**2 * w
-                + 69.0 / 20 * b**2
-                + 221.0 / 60 * c**2
-            )
-            + mp.mpf(1)
-            / (2**11 * 3 * 5 * a**4)
-            * (
-                (-30 * b**4 + 35 * b**2 * c**2 + mp.mpf(22) / 3 * c**4) * ML
-                - (115 * b**4 - 480 * b**2 * c**2) / 12 * u
-                - mp.mpf(23) / 28 * c**4 * v
-                + (6 * b**4 - 7 * b**2 * c**2) / 21 * 2**8 * w
-                - (36590 * b**4 - 2035 * b**2 * c**2 - 11442 * c**4)
-                / (2**3 * 3 * 5 * 7)
-            )
-            + (mp.mpf(1) / (2**16 * 3 * 5 * 7 * a**6))
-            * (
-                (
-                    525 * b**6
-                    - 1610 * b**4 * c**2
-                    + 770 * b**2 * c**4
-                    + 103 * c**6
-                )
-                * ML
-                + (
-                    mp.mpf(3633) / 10 * b**6
-                    - 3220 * b**4 * c**2
-                    + 2240 * b**2 * c**4
-                )
-                * u
-                - mp.mpf(359) / 30 * c**6 * v
-                - 2**11
-                * ((25 * b**6 - 60 * b**4 * c**2 + 21 * b**2 * c**4) / 15)
-                * w
-                + mp.mpf(2161453) / (2**3 * 3 * 5 * 7) * b**6
-                - mp.mpf(617423) / ((2**2) * (3**2) * 5) * b**4 * c**2
-                - mp.mpf(8329) / ((2**2) * 3 * 5) * b**2 * c**4
-                + mp.mpf(4308631) / (2**3 * 3 * 5 * 7) * c**6
-            )
-        )
-        L = 4e-7 * mp.pi * (n**2) * a * f
-        # print("Lyle6mp r: %.4g, dr: %.4g, dz: %4g, n: %d, L: %.8g"%(a,c,b,n,L))
-        return L
+    Returns:
+        float: coil self inductance in Henrys
+    """
+    L = 0
+    subcoils = section_coil(r, dr, dz, nt, nt, nr, nz)
+    fils = lyle_equivalent_subcoil_filaments(subcoils)
+
+    for i in range(nr * nz):
+        for j in range(nr * nz):
+            if i != j:
+                L += mutual_lyles_method(*fils[i], *fils[j])
+        L += 2 * L_lyle6(*subcoils[i])
+    return L
 
 
 @njit
 def L_long_solenoid_butterworth(r, dr, dz, n):
     """Self inductance of a long solenoid by Butterworth's formula.
 
     As written in Grover, Bulletin of the Bureau of Standards, Vol. 14 pg. 558
@@ -667,7 +552,35 @@
     k3 = k2**1.5
     beta2 = beta**2
     elK, elE = ellipke(k2)
 
     f = 2 / 3 / beta2 * (((2 * k2 - 1) * elE + (1 - k2) * elK) / k3 - 1)
     Ls = MU0 * (n**2) * r * f
     return Ls
+
+
+@njit(parallel=True)
+def self_inductance_by_filaments(f, conductor="round", a=0.01, dr=0.01, dz=0.01):
+    """Self inductance of filament set.
+
+    Args:
+        f (array): first filament array
+        conductor (str, optional): conductor shape. Defaults to "round".
+        a (float, optional): conductor radius. Defaults to 0.01.
+        dr (float, optional): conductor radial width. Defaults to 0.01
+        dz (float, optional): conductor vertical height. Defaults to 0.01
+
+    Returns:
+        float: self inductance of filament set in Henries
+    """
+    L = float(0)
+    for i in prange(f.shape[0]):
+        for j in range(f.shape[0]):
+            if i != j:
+                L += mutual_inductance_fil(f[i, :], f[j, :])
+        if conductor == "round":
+            L += L_round(f[i, 0], a, f[i, 2])
+        elif conductor == "hollow_round":
+            L += L_hollow_round(f[i, 0], a, f[i, 2])
+        elif conductor == "rect":
+            L += L_lyle6(f[i, 0], dr, dz, f[i, 2])
+    return L
```

### Comparing `inductance-0.1.2/PKG-INFO` & `inductance-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductance
-Version: 0.1.2
+Version: 0.1.3
 Summary: Code for 2D inductance calculations
 Home-page: https://github.com/dgarnier/inductance
 License: MIT
 Author: Darren Garnier
 Author-email: dgarnier@reinrag.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

