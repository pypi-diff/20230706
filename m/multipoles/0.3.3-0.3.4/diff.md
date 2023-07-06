# Comparing `tmp/multipoles-0.3.3.tar.gz` & `tmp/multipoles-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multipoles-0.3.3.tar", last modified: Wed Jul  5 10:37:18 2023, max compression
+gzip compressed data, was "multipoles-0.3.4.tar", last modified: Thu Jul  6 12:00:59 2023, max compression
```

## Comparing `multipoles-0.3.3.tar` & `multipoles-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-05 10:37:18.256460 multipoles-0.3.3/
--rw-r--r--   0 mbaer    (671849960) 579947404      793 2023-07-05 10:37:18.256602 multipoles-0.3.3/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404     4678 2023-07-05 05:51:03.000000 multipoles-0.3.3/README.md
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-05 10:37:18.254203 multipoles-0.3.3/multipoles/
--rw-r--r--   0 mbaer    (671849960) 579947404       66 2023-07-05 10:36:59.000000 multipoles-0.3.3/multipoles/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404    14138 2023-07-05 10:23:31.000000 multipoles-0.3.3/multipoles/expansion.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-05 10:37:18.256141 multipoles-0.3.3/multipoles.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404      793 2023-07-05 10:37:18.000000 multipoles-0.3.3/multipoles.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      244 2023-07-05 10:37:18.000000 multipoles-0.3.3/multipoles.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-05 10:37:18.000000 multipoles-0.3.3/multipoles.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       12 2023-07-05 10:37:18.000000 multipoles-0.3.3/multipoles.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       11 2023-07-05 10:37:18.000000 multipoles-0.3.3/multipoles.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       79 2023-07-05 10:37:18.257129 multipoles-0.3.3/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404      968 2023-07-05 10:36:52.000000 multipoles-0.3.3/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-06 12:00:59.848210 multipoles-0.3.4/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1070 2023-07-06 09:50:10.000000 multipoles-0.3.4/LICENSE
+-rw-r--r--   0 mbaer    (671849960) 579947404      815 2023-07-06 12:00:59.848446 multipoles-0.3.4/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404     4677 2023-07-06 09:50:10.000000 multipoles-0.3.4/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-06 12:00:59.844660 multipoles-0.3.4/multipoles/
+-rw-r--r--   0 mbaer    (671849960) 579947404       66 2023-07-06 11:59:20.000000 multipoles-0.3.4/multipoles/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404    14360 2023-07-06 11:58:57.000000 multipoles-0.3.4/multipoles/expansion.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-06 12:00:59.847508 multipoles-0.3.4/multipoles.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404      815 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      252 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       12 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       11 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       79 2023-07-06 12:00:59.849334 multipoles-0.3.4/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404      968 2023-07-06 11:59:15.000000 multipoles-0.3.4/setup.py
```

### Comparing `multipoles-0.3.3/PKG-INFO` & `multipoles-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: multipoles
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python package for multipole expansions of electrostatic or gravitational potentials
 Home-page: https://github.com/maroba/multipoles
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: multipole expansion,physics,scientific-computing
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
 
 *multipoles* is a Python package for multipole expansions of the solutions of the Poisson equation     
        (e.g. electrostatic or gravitational potentials). It can handle discrete and continuous charge or mass distributions.
```

### Comparing `multipoles-0.3.3/README.md` & `multipoles-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # multipoles
-<p><a href="https://badge.fury.io/py/multipoles"> <img src="https://badge.fury.io/py/multipoles.svg?branch=master&kill_cache=1" alt="PyPI version"></a> <a href=""> <img src="https://github.com/maroba/multipoles/actions/workflows/python-app.yml/badge.svg" alt="build"></a><a href="https://codecov.io/gh/maroba/multipoles"> <img src="https://codecov.io/gh/maroba/multipoles/branch/master/graph/badge.svg?token=JNH9SP7BRG" alt=""></a></p>
+<p><a href="https://badge.fury.io/py/multipoles"> <img src="https://badge.fury.io/py/multipoles.svg?branch=kill_cache=1" alt="PyPI version"></a> <a href=""> <img src="https://github.com/maroba/multipoles/actions/workflows/python-app.yml/badge.svg" alt="build"></a><a href="https://codecov.io/gh/maroba/multipoles"> <img src="https://codecov.io/gh/maroba/multipoles/branch/master/graph/badge.svg?token=JNH9SP7BRG" alt=""></a></p>
 
 *multipoles* is a Python package for multipole expansions of the solutions of the Poisson equation (e.g. electrostatic or gravitational potentials). It can handle discrete and continuous charge or mass distributions.
 
 ## Background
 
-For a given function $\rho(x,y,z)$, the solution $\Ph   i(x,y,z)$ of the Poisson equation $\nabla^2\Phi=-4\pi \rho$ with vanishing Dirichlet boundary conditions at infinity is
+For a given function $\rho(x,y,z)$, the solution $\Phi(x,y,z)$ of the Poisson equation $\nabla^2\Phi=-4\pi \rho$ with vanishing Dirichlet boundary conditions at infinity is
 
-$$\Phi(x,y,z)=-\int d^3r'\frac{\rho(r')}{|r-r'|}$$
+$$\Phi(x,y,z)=\int d^3r'\frac{\rho(r')}{|r-r'|}$$
 
 Examples of this are the electrostatic and Newtonian gravitational potential.
 If you need to evaluate $\Phi(x,y,z)$ at many points, calculating the integral for each point is computationally expensive. As a faster alternative, we can express $\Phi(x,y,z)$ in terms of the multipole moments $q_{lm}$ or $I_{lm}$ (note some literature uses the subscripts $(\cdot)_{nm}$):
 
 $$\Phi(x,y,z)=\sum_{l=0}^\infty\underbrace{\sqrt{\frac{4\pi}{2l+1}}\sum_{m=-l}^lY_{lm}(\theta, \varphi)\frac{q_{lm}}{r^{l+1}}}_{\Phi^{(l)}}$$
 
 for a exterior expansion, or
@@ -115,9 +115,9 @@
 ```
 
 ## Installation
 
 Simply use `pip`:
 
 ```
-pip install multipoles
+pip install --upgrade multipoles
 ```
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # multipoles
 [PyPI_version] [build]
 *multipoles* is a Python package for multipole expansions of the solutions of
 the Poisson equation (e.g. electrostatic or gravitational potentials). It can
 handle discrete and continuous charge or mass distributions. ## Background For
-a given function $\rho(x,y,z)$, the solution $\Ph i(x,y,z)$ of the Poisson
+a given function $\rho(x,y,z)$, the solution $\Phi(x,y,z)$ of the Poisson
 equation $\nabla^2\Phi=-4\pi \rho$ with vanishing Dirichlet boundary conditions
-at infinity is $$\Phi(x,y,z)=-\int d^3r'\frac{\rho(r')}{|r-r'|}$$ Examples of
+at infinity is $$\Phi(x,y,z)=\int d^3r'\frac{\rho(r')}{|r-r'|}$$ Examples of
 this are the electrostatic and Newtonian gravitational potential. If you need
 to evaluate $\Phi(x,y,z)$ at many points, calculating the integral for each
 point is computationally expensive. As a faster alternative, we can express
 $\Phi(x,y,z)$ in terms of the multipole moments $q_{lm}$ or $I_{lm}$ (note some
 literature uses the subscripts $(\cdot)_{nm}$): $$\Phi(x,y,z)=\sum_
 {l=0}^\infty\underbrace{\sqrt{\frac{4\pi}{2l+1}}\sum_{m=-l}^lY_{lm}(\theta,
 \varphi)\frac{q_{lm}}{r^{l+1}}}_{\Phi^{(l)}}$$ for a exterior expansion, or
@@ -49,8 +49,8 @@
 which is a 3D numpy array: rho = gaussian(XYZ, (0, 0, 1), sigma) - gaussian
 (XYZ, (0, 0, -1), sigma) # Prepare the charge distribution dict for the
 MultipoleExpansion object: charge_dist = { 'discrete': False, # we have a
 continuous charge distribution here 'rho': rho, 'xyz': XYZ } # The rest is the
 same as for the discrete case: l_max = 2 # where to stop the infinite multipole
 sum; here we expand up to the quadrupole (l=2) Phi = MultipoleExpansion
 (charge_dist, l_max) x, y, z = 30.5, 30.6, 30.7 value = Phi(x, y, z) ``` ##
-Installation Simply use `pip`: ``` pip install multipoles ```
+Installation Simply use `pip`: ``` pip install --upgrade multipoles ```
```

### Comparing `multipoles-0.3.3/multipoles/expansion.py` & `multipoles-0.3.4/multipoles/expansion.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,22 @@
         """
         if not isinstance(mask[0], np.ndarray):
             mask = tuple(*mask)
         else:
             mask = mask[0]
         mp_contribs = []
         r, phi, theta = self.internal_coords_spherical
+
+        eps = 1.E-6
+        if isinstance(r, np.ndarray):
+            r[np.abs(r) < eps] = eps
+        else:
+            if abs(r) < eps:
+                r = eps
+
         for l in range(self.l_max + 1):
             phi_l = 0
             for m in range(-l, l + 1):
                 Y_lm = sph_harm(m, l, phi[mask], theta[mask])
                 q_lm = self.multipole_moments[(l, m)]
                 phi_l += np.sqrt(4 * np.pi / (2 * l + 1)) * q_lm * Y_lm / r[mask] ** (l + 1)
             mp_contribs.append(phi_l.real)
@@ -275,14 +283,21 @@
     def _multipole_contribs(self, xyz):
         if not isinstance(xyz, np.ndarray):
             xyz = np.array(xyz)
 
         xyz_internal = xyz - self.center_of_charge
         r, phi, theta = cartesian_to_spherical(*xyz_internal)
 
+        eps = 1.E-6
+        if isinstance(r, np.ndarray):
+            r[np.abs(r) < eps] = eps
+        else:
+            if abs(r) < eps:
+                r = eps
+
         mp_contribs = []
 
         for l in range(self.l_max + 1):
             phi_l = 0
             for m in range(-l, l + 1):
                 Y_lm = sph_harm(m, l, phi, theta)
                 q_lm = self.multipole_moments[(l, m)]
@@ -294,16 +309,14 @@
         return mp_contribs
 
     def _calc_multipole_moments(self):
         moments = {}
         for l in range(0, self.l_max + 1):
             for m in range(-l, l + 1):
                 moments[(l, m)] = self._calc_multipole_coef(l, m)
-                #if m != 0:
-                #    moments[(l, -m)] = (-1) ** m * np.conj(moments[(l, m)])
         return moments
 
     def _calc_multipole_coef(self, l, m):
 
         prefac = np.sqrt(4 * np.pi / (2 * l + 1))
 
         if self.charge_dist['discrete']:
```

### Comparing `multipoles-0.3.3/multipoles.egg-info/PKG-INFO` & `multipoles-0.3.4/multipoles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: multipoles
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python package for multipole expansions of electrostatic or gravitational potentials
 Home-page: https://github.com/maroba/multipoles
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: multipole expansion,physics,scientific-computing
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
 
 *multipoles* is a Python package for multipole expansions of the solutions of the Poisson equation     
        (e.g. electrostatic or gravitational potentials). It can handle discrete and continuous charge or mass distributions.
```

### Comparing `multipoles-0.3.3/setup.py` & `multipoles-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='multipoles',
-    version='0.3.3',
+    version='0.3.4',
     description='A Python package for multipole expansions of electrostatic or gravitational potentials',
     long_description="""*multipoles* is a Python package for multipole expansions of the solutions of the Poisson equation     
        (e.g. electrostatic or gravitational potentials). It can handle discrete and continuous charge or mass distributions.
     """,
 
     license='MIT',
     url='https://github.com/maroba/multipoles',
```

