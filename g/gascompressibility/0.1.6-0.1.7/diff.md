# Comparing `tmp/gascompressibility-0.1.6.tar.gz` & `tmp/gascompressibility-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gascompressibility-0.1.6.tar", last modified: Thu Jun 29 18:28:54 2023, max compression
+gzip compressed data, was "gascompressibility-0.1.7.tar", last modified: Thu Jul  6 19:14:11 2023, max compression
```

## Comparing `gascompressibility-0.1.6.tar` & `gascompressibility-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.788940 gascompressibility-0.1.6/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.6/LICENSE
--rw-rw-rw-   0        0        0    11101 2023-06-29 18:28:54.788940 gascompressibility-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    10123 2023-06-28 22:59:44.000000 gascompressibility-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.740970 gascompressibility-0.1.6/gascompressibility/
--rw-rw-rw-   0        0        0      209 2023-06-28 22:34:59.000000 gascompressibility-0.1.6/gascompressibility/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.759968 gascompressibility-0.1.6/gascompressibility/pseudocritical/
--rw-rw-rw-   0        0        0    17335 2023-06-29 17:48:34.000000 gascompressibility-0.1.6/gascompressibility/pseudocritical/Piper.py
--rw-rw-rw-   0        0        0    20224 2023-06-29 17:48:34.000000 gascompressibility-0.1.6/gascompressibility/pseudocritical/Sutton.py
--rw-rw-rw-   0        0        0       56 2023-06-29 18:25:42.000000 gascompressibility-0.1.6/gascompressibility/pseudocritical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.764973 gascompressibility-0.1.6/gascompressibility/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.6/gascompressibility/utilities/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.6/gascompressibility/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.783940 gascompressibility-0.1.6/gascompressibility/z_correlation/
--rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/DAK.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/__init__.py
--rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/hall_yarborough.py
--rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/kareem.py
--rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/londono.py
--rw-rw-rw-   0        0        0     5965 2023-06-29 18:26:44.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/z_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.757969 gascompressibility-0.1.6/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0    11101 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 18:28:54.789939 gascompressibility-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1549 2023-06-29 18:28:09.000000 gascompressibility-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.787940 gascompressibility-0.1.6/tests/
--rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0    30936 2023-06-28 22:59:10.000000 gascompressibility-0.1.6/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.251023 gascompressibility-0.1.7/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0    11101 2023-07-06 19:14:11.251023 gascompressibility-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10123 2023-07-06 14:22:50.000000 gascompressibility-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.226741 gascompressibility-0.1.7/gascompressibility/
+-rw-rw-rw-   0        0        0      275 2023-07-06 19:01:31.000000 gascompressibility-0.1.7/gascompressibility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.240742 gascompressibility-0.1.7/gascompressibility/pseudocritical/
+-rw-rw-rw-   0        0        0    17335 2023-06-29 17:48:34.000000 gascompressibility-0.1.7/gascompressibility/pseudocritical/Piper.py
+-rw-rw-rw-   0        0        0    20224 2023-06-29 17:48:34.000000 gascompressibility-0.1.7/gascompressibility/pseudocritical/Sutton.py
+-rw-rw-rw-   0        0        0       56 2023-06-29 18:25:42.000000 gascompressibility-0.1.7/gascompressibility/pseudocritical/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.242741 gascompressibility-0.1.7/gascompressibility/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.7/gascompressibility/utilities/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.7/gascompressibility/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.248022 gascompressibility-0.1.7/gascompressibility/z_correlation/
+-rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/DAK.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/hall_yarborough.py
+-rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/kareem.py
+-rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/londono.py
+-rw-rw-rw-   0        0        0     8846 2023-07-06 19:01:44.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/z_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.237741 gascompressibility-0.1.7/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0    11101 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 19:14:11.251023 gascompressibility-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1522 2023-07-06 19:03:50.000000 gascompressibility-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.250023 gascompressibility-0.1.7/tests/
+-rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0    30936 2023-06-28 22:59:10.000000 gascompressibility-0.1.7/tests/test_gascomp.py
```

### Comparing `gascompressibility-0.1.6/LICENSE` & `gascompressibility-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/PKG-INFO` & `gascompressibility-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.6
+Version: 0.1.7
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.6/README.md` & `gascompressibility-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/gascompressibility/pseudocritical/Piper.py` & `gascompressibility-0.1.7/gascompressibility/pseudocritical/Piper.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/gascompressibility/pseudocritical/Sutton.py` & `gascompressibility-0.1.7/gascompressibility/pseudocritical/Sutton.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/gascompressibility/z_correlation/DAK.py` & `gascompressibility-0.1.7/gascompressibility/z_correlation/DAK.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/gascompressibility/z_correlation/hall_yarborough.py` & `gascompressibility-0.1.7/gascompressibility/z_correlation/hall_yarborough.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/gascompressibility/z_correlation/kareem.py` & `gascompressibility-0.1.7/gascompressibility/z_correlation/kareem.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/gascompressibility/z_correlation/londono.py` & `gascompressibility-0.1.7/gascompressibility/z_correlation/londono.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/gascompressibility/z_correlation/z_helper.py` & `gascompressibility-0.1.7/gascompressibility/z_correlation/z_helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,15 +59,111 @@
                 Z = optimize.newton(zmodel_func, guess, args=(Pr, Tr), **newton_kwargs)
 
     return Z
 
 
 def calc_z(sg=None, P=None, T=None, H2S=None, CO2=None, N2=None, Pr=None, Tr=None, pmodel='Piper', zmodel='DAK',
            guess=_get_guess_constant(), newton_kwargs=None, ps_props=False, ignore_conflict=False, **kwargs):
+    """
+    Calculates the gas compressibility factor, :math:`Z`.
 
+    **Basic (most common) usage:**
+
+    >>> import gascompressibility as gc
+    >>>
+    >>> gc.calc_z(sg=0.7, T=75, P=2010)
+    0.7366562810878984
+
+
+    **In presence of significant non-hydrocarbon impurities:**
+
+    >>> gc.calc_z(sg=0.7, T=75, P=2010, CO2=0.1, H2S=0.07, N2=0.05)
+    0.7765149771306533
+
+    **When pseudo-critical properties are known (not common):**
+
+    >>> gc.calc_z(Pr=1.5, Tr=1.5)
+    0.859314380561347
+
+    **Picking correlation models of your choice**
+
+    >>> gc.calc_z(sg=0.7, T=75, P=2010, zmodel='kareem', pmodel='Sutton')
+    0.7150183342641309
+
+    **Returning all associated pseudo-critical properties computed**
+
+    >>> gc.calc_z(sg=0.7, T=75, P=2010, ps_props=True)
+    {'z': 0.7366562810878984, 'Tpc': 371.4335560823552, 'Ppc': 660.6569792741872, 'J': 0.56221847, 'K': 14.450840999999999, 'Tr': 1.4394768357478496, 'Pr': 3.0646766226921294}
+
+
+
+    Parameters
+    ----------
+    sg : float
+        specific gravity of gas (dimensionless)
+    P : float
+        pressure of gas (psig)
+    T : float
+        temperature of gas (°F)
+    H2S : float
+        mole fraction of H2S (dimensionless)
+    CO2 : float
+        mole fraction of CO2 (dimensionless)
+    N2 : float
+        mole fraction of N2 (dimensionless). Available only when ``pmodel='Piper'`` (default)
+    Pr : float
+        pseudo-reduced pressure, Pr (psia)
+    Tr : float
+        pseudo-reduced temperature, Tr (°R)
+    pmodel : str
+        choice of a pseudo-critical model. Accepted inputs are: ``'Sutton'`` and ``'Piper'``.
+
+        See Also
+        --------
+        :doc:`pseudocritical`
+        Sutton.Sutton
+        Piper.Piper
+
+    zmodel : str
+        choice of a z-correlation model. Accepted inputs are: ``'DAK'``, ``'hall_yarborough'``, ``'londono'``, and ``'kareem'``
+    guess : float
+        initial guess of z-value for z-correlation models using iterative convergence (``'DAK'``, ``'hall_yarborough'``,
+        and ``'londono'``).
+    newton_kwargs
+    ps_props
+    ignore_conflict
+    kwargs
+
+    Returns
+    -------
+    bool
+        True if successful, False otherwise.
+
+        The return type is not optional. The ``Returns`` section may span
+        multiple lines and paragraphs. Following lines should be indented to
+        match the first line of the description.
+
+        The ``Returns`` section supports any reStructuredText formatting,
+        including literal blocks::
+
+            {
+                'param1': param1,
+                'param2': param2
+            }
+
+    Raises
+    ------
+    AttributeError
+        The ``Raises`` section is a list of all exceptions
+        that are relevant to the interface.
+    ValueError
+        If `param2` is equal to `param1`.
+
+
+    """
     z_model = _get_z_model(model=zmodel)
 
     # Pr and Tr are already provided:
     if Pr is not None and Tr is not None:
 
         # Explicit models
         Z = _calc_z_explicit_implicit_helper(Pr, Tr, z_model, zmodel, guess, newton_kwargs, ps_props)
@@ -156,7 +252,9 @@
                  fontsize=12, pad=10, x=0.445, y=1.06)
     ax.annotate('', xy=(-0.09, 1.05), xycoords='axes fraction', xytext=(1.05, 1.05),
                 arrowprops=dict(arrowstyle="-", color='k'))
 
     fig.tight_layout()
 
     return results, fig, ax
+
+quickstart()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gascompressibility-0.1.6/gascompressibility.egg-info/PKG-INFO` & `gascompressibility-0.1.7/gascompressibility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.6
+Version: 0.1.7
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.6/gascompressibility.egg-info/SOURCES.txt` & `gascompressibility-0.1.7/gascompressibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.6/setup.py` & `gascompressibility-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,26 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
         "notes.py",
         "testruns.ipynb",
         "papers",
         "docs",
-        "docs_save_6_24",
     ]),
     description='GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     classifiers=classifiers(),
     license='MIT',
     author='Eric Kim',
```

### Comparing `gascompressibility-0.1.6/tests/test_gascomp.py` & `gascompressibility-0.1.7/tests/test_gascomp.py`

 * *Files identical despite different names*

