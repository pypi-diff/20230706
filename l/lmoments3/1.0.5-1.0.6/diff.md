# Comparing `tmp/lmoments3-1.0.5.tar.gz` & `tmp/lmoments3-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmoments3-1.0.5.tar", last modified: Tue Feb 28 20:22:57 2023, max compression
+gzip compressed data, was "lmoments3-1.0.6.tar", last modified: Thu Jul  6 18:38:41 2023, max compression
```

## Comparing `lmoments3-1.0.5.tar` & `lmoments3-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,19 @@
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 20:22:57.770939 lmoments3-1.0.5/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2338 2023-02-28 20:17:32.000000 lmoments3-1.0.5/CHANGELOG.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)    35122 2023-02-20 22:00:35.000000 lmoments3-1.0.5/LICENSE
--rw-r--r--   0 tjs       (1000) tjs       (1000)      358 2023-02-28 18:26:13.000000 lmoments3-1.0.5/MANIFEST.in
--rw-r--r--   0 tjs       (1000) tjs       (1000)     4983 2023-02-28 20:22:57.770939 lmoments3-1.0.5/PKG-INFO
--rw-r--r--   0 tjs       (1000) tjs       (1000)     3775 2023-02-27 15:48:14.000000 lmoments3-1.0.5/README.rst
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 20:22:57.764939 lmoments3-1.0.5/docs/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     6811 2023-02-20 19:25:36.000000 lmoments3-1.0.5/docs/Makefile
--rw-r--r--   0 tjs       (1000) tjs       (1000)     6488 2023-02-20 19:25:36.000000 lmoments3-1.0.5/docs/make.bat
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 20:22:57.766939 lmoments3-1.0.5/docs/source/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      510 2023-02-28 18:26:13.000000 lmoments3-1.0.5/docs/source/api.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)       33 2023-02-27 15:48:14.000000 lmoments3-1.0.5/docs/source/changes.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)     8865 2023-02-28 18:26:13.000000 lmoments3-1.0.5/docs/source/conf.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2208 2023-02-28 18:26:13.000000 lmoments3-1.0.5/docs/source/distributions.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1595 2023-02-28 18:26:13.000000 lmoments3-1.0.5/docs/source/index.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)       30 2023-02-27 15:48:14.000000 lmoments3-1.0.5/docs/source/readme.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)     4526 2023-02-28 18:26:13.000000 lmoments3-1.0.5/docs/source/usage.rst
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 20:22:57.771939 lmoments3-1.0.5/lmoments3/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     7146 2023-02-28 20:15:18.000000 lmoments3-1.0.5/lmoments3/__init__.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)      497 2023-02-28 20:22:57.771939 lmoments3-1.0.5/lmoments3/_version.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    51839 2023-02-27 15:48:14.000000 lmoments3-1.0.5/lmoments3/distr.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1902 2023-02-27 15:48:14.000000 lmoments3-1.0.5/lmoments3/stats.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 20:22:57.770939 lmoments3-1.0.5/lmoments3/tests/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     3637 2023-02-27 15:48:14.000000 lmoments3-1.0.5/lmoments3/tests/__init__.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     7734 2023-02-27 15:48:14.000000 lmoments3-1.0.5/lmoments3/tests/test_lmoments.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1510 2023-02-27 15:48:14.000000 lmoments3-1.0.5/lmoments3/tests/test_samlmu_speed.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 20:22:57.769939 lmoments3-1.0.5/lmoments3.egg-info/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     4983 2023-02-28 20:22:57.000000 lmoments3-1.0.5/lmoments3.egg-info/PKG-INFO
--rw-r--r--   0 tjs       (1000) tjs       (1000)      695 2023-02-28 20:22:57.000000 lmoments3-1.0.5/lmoments3.egg-info/SOURCES.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        1 2023-02-28 20:22:57.000000 lmoments3-1.0.5/lmoments3.egg-info/dependency_links.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        1 2023-02-20 21:53:01.000000 lmoments3-1.0.5/lmoments3.egg-info/not-zip-safe
--rw-r--r--   0 tjs       (1000) tjs       (1000)       81 2023-02-28 20:22:57.000000 lmoments3-1.0.5/lmoments3.egg-info/requires.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       10 2023-02-28 20:22:57.000000 lmoments3-1.0.5/lmoments3.egg-info/top_level.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)      289 2023-02-27 15:48:14.000000 lmoments3-1.0.5/pyproject.toml
--rw-r--r--   0 tjs       (1000) tjs       (1000)       12 2023-02-27 15:48:14.000000 lmoments3-1.0.5/requirements.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)       62 2023-02-27 15:48:14.000000 lmoments3-1.0.5/requirements_dev.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)      360 2023-02-28 20:22:57.771939 lmoments3-1.0.5/setup.cfg
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1791 2023-02-28 18:26:13.000000 lmoments3-1.0.5/setup.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    83757 2023-02-28 20:15:18.000000 lmoments3-1.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:41.773122 lmoments3-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-06 18:38:32.000000 lmoments3-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45819 2023-07-06 18:38:41.773122 lmoments3-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-06 18:38:32.000000 lmoments3-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:41.773122 lmoments3-1.0.6/lmoments3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-06 18:38:32.000000 lmoments3-1.0.6/lmoments3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 18:38:41.773122 lmoments3-1.0.6/lmoments3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51927 2023-07-06 18:38:32.000000 lmoments3-1.0.6/lmoments3/distr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-06 18:38:32.000000 lmoments3-1.0.6/lmoments3/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:41.773122 lmoments3-1.0.6/lmoments3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45819 2023-07-06 18:38:41.000000 lmoments3-1.0.6/lmoments3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 18:38:41.000000 lmoments3-1.0.6/lmoments3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:38:41.000000 lmoments3-1.0.6/lmoments3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-06 18:38:41.000000 lmoments3-1.0.6/lmoments3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 18:38:41.000000 lmoments3-1.0.6/lmoments3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-06 18:38:32.000000 lmoments3-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 18:38:41.773122 lmoments3-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 18:38:32.000000 lmoments3-1.0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83757 2023-07-06 18:38:32.000000 lmoments3-1.0.6/versioneer.py
```

### Comparing `lmoments3-1.0.5/LICENSE` & `lmoments3-1.0.6/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -668,8 +668,7 @@
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
 <http://www.gnu.org/philosophy/why-not-lgpl.html>.
-
```

### Comparing `lmoments3-1.0.5/README.rst` & `lmoments3-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `lmoments3-1.0.5/lmoments3/__init__.py` & `lmoments3-1.0.6/lmoments3/__init__.py`

 * *Files identical despite different names*

### Comparing `lmoments3-1.0.5/lmoments3/distr.py` & `lmoments3-1.0.6/lmoments3/distr.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,31 +32,28 @@
     from scipy.stats._distn_infrastructure import rv_continuous_frozen
 except ImportError:
     # Scipy < 1.9
     from scipy.stats._distn_infrastructure import rv_frozen as rv_continuous_frozen
 
 
 class LmomDistrMixin:
-    """
-    Mixin class to add L-moment methods to :class:`scipy.stats.rv_continous` distribution functions. Distributions using
-    the mixin should override the methods :meth:`._lmom_fit` and :meth:`.lmom_ratios`.
+    """Mixin class to add L-moment methods to :class:`scipy.stats.rv_continous` distribution functions.
+
+    Distributions using the mixin should override the methods :meth:`._lmom_fit` and :meth:`.lmom_ratios`.
     """
 
     def _lmom_fit(self, lmom_ratios):
         raise NotImplementedError
 
     def _lmom_ratios(self, *shapes, locs, scale, nmom):
-        """
-        When overriding, *shapes can be replaced by the actual distribution's shape parameter(s), if any.
-        """
+        """When overriding, *shapes can be replaced by the actual distribution's shape parameter(s), if any."""
         raise NotImplementedError
 
     def lmom_fit(self, data=[], lmom_ratios=[]):
-        """
-        Fit the distribution function to the given data or given L-moments.
+        """Fit the distribution function to the given data or given L-moments.
 
         :param data: Data to use in calculating the distribution parameters
         :type data: array_like
         :param lmom_ratios: L-moments (ratios) l1, l2, t3, t4, .. to use in calculating the distribution parameters
         :type lmom_ratios: array_like
         :returns: Distribution parameters in `scipy` order, e.g. scale, loc, shape
         :rtype: :class:`OrderedDict`
@@ -70,23 +67,22 @@
             raise Exception("Either `data` or `lmom_ratios` must be provided.")
         elif len(lmom_ratios) < n_min:
             raise ValueError(f"At least {n_min} number of L-moments must be provided.")
 
         return self._lmom_fit(lmom_ratios)
 
     def lmom(self, *args, nmom=5, **kwds):
-        """
-        Compute the distribution's L-moments, e.g. l1, l2, l3, l4, ..
+        """Compute the distribution's L-moments, e.g. l1, l2, l3, l4, ..
 
         :param args: Distribution parameters in order of shape(s), loc, scale
         :type args: float
         :param nmom: Number of moments to calculate
         :type nmom: int
-        :param kwds: Distribution parameters as named arguments. See :attr:`rv_continous.shapes` for names of shape
-                     parameters
+        :param kwds: Distribution parameters as named arguments.
+                     See :attr:`rv_continous.shapes` for names of shape parameters
         :type kwds: float
         :returns: List of L-moments
         :rtype: list
         """
         ratios = self.lmom_ratios(*args, nmom=nmom, **kwds)
         moments = ratios[0:2]
         moments += [ratio * moments[1] for ratio in ratios[2:]]
@@ -96,16 +92,16 @@
         """
         Compute the distribution's L-moment ratios, e.g. l1, l2, t3, t4, ..
 
         :param args: Distribution parameters in order of shape(s), loc, scale
         :type args: float
         :param nmom: Number of moments to calculate
         :type nmom: int
-        :param kwds: Distribution parameters as named arguments. See :attr:`rv_continous.shapes` for names of shape
-                     parameters
+        :param kwds: Distribution parameters as named arguments.
+                     See :attr:`rv_continous.shapes` for names of shape parameters
         :type kwds: float
         :returns: List of L-moment ratios
         :rtype: list
         """
         if nmom > 20:
             return ValueError("Parameter nmom too large. Max of 20.")
 
@@ -124,15 +120,15 @@
         # This is how scipy's nnlf requires parameters
         theta = list(shapes) + [loc, scale]
 
         # Now call the super class's nnlf
         return scipy.stats.rv_continuous.nnlf(self, x=data, theta=theta)
 
     def freeze(self, *args, **kwds):
-        # Override `freeze` because we're extending the frozen version of the distribution.
+        """Override `freeze` because we're extending the frozen version of the distribution."""
         return LmomFrozenDistr(self, *args, **kwds)
 
 
 class LmomFrozenDistr(rv_continuous_frozen):
     """
     Frozen version of the distribution returned by :class:`LmomDistrMixin`. Simply provides additional methods supported
     by the mixin.
@@ -610,14 +606,15 @@
         G = (1 - 3 * T3) / (1 + T3)
         H = HSTART
         Z = G + H * 0.725
         Xdist = BIG
 
         # Newton-Raphson Iteration
         for it in range(1, MAXIT + 1):
+            Success = 0
             for i in range(1, MAXSR + 1):
                 if G > OFLGAM:
                     raise Exception("Failed to converge")
                 if H > 0:
                     U1 = math.exp(
                         special.gammaln(1 / H) - special.gammaln(1 / H + 1 + G)
                     )
@@ -655,18 +652,20 @@
                 E2 = TAU4 - T4
 
                 DIST = max(abs(E1), abs(E2))
                 if DIST < Xdist:
                     Success = 1
                     break
                 else:
-                    DEL1 = 0.5 * DEL1
-                    DEL2 = 0.5 * DEL2
-                    G = XG - DEL1
-                    H = XH - DEL2
+                    pass
+                    # FIXME: The following variables are undefined
+                    # DEL1 = 0.5 * DEL1
+                    # DEL2 = 0.5 * DEL2
+                    # G = XG - DEL1
+                    # H = XH - DEL2
 
             if Success == 0:
                 raise Exception("Failed to converge")
 
             # Test for convergence
             if DIST < EPS:
                 TEMP = special.gammaln(1 + G)
@@ -1087,16 +1086,16 @@
             xmom.append((Y + Z) / ALAM2)
         return xmom
 
 
 wak = WakebyGen(name="wakeby", shapes="beta, gamma, delta")
 
 """
-The following distributions are available in `scipy.stats` and are redefined here with an `LmomDistrMixin` to extend the
-scipy distribution with L-moment methods.
+The following distributions are available in `scipy.stats` and are redefined
+here with an `LmomDistrMixin` to extend the scipy distribution with L-moment methods.
 """
 
 
 class GenParetoGen(LmomDistrMixin, scipy.stats._continuous_distns.genpareto_gen):
     def _lmom_fit(self, lmom_ratios):
         T3 = lmom_ratios[2]
         if lmom_ratios[1] <= 0 or abs(T3) >= 1:
```

### Comparing `lmoments3-1.0.5/lmoments3/stats.py` & `lmoments3-1.0.6/lmoments3/stats.py`

 * *Files identical despite different names*

### Comparing `lmoments3-1.0.5/versioneer.py` & `lmoments3-1.0.6/versioneer.py`

 * *Files identical despite different names*

