# Comparing `tmp/datawhispers-0.2.8.5.tar.gz` & `tmp/datawhispers-0.2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.8.5.tar", last modified: Wed Jul  5 12:17:08 2023, max compression
+gzip compressed data, was "datawhispers-0.2.8.6.tar", last modified: Thu Jul  6 08:35:17 2023, max compression
```

## Comparing `datawhispers-0.2.8.5.tar` & `datawhispers-0.2.8.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-05 12:17:08.355601 datawhispers-0.2.8.5/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.5/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-05 12:17:08.355459 datawhispers-0.2.8.5/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)     1218 2023-07-04 11:44:42.000000 datawhispers-0.2.8.5/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-05 12:17:08.354524 datawhispers-0.2.8.5/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.5/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)    11578 2023-07-03 09:25:40.000000 datawhispers-0.2.8.5/datawhispers/advancedProg.py
--rw-r--r--   0 german     (501) staff       (20)    17933 2023-07-05 12:10:57.000000 datawhispers-0.2.8.5/datawhispers/datavis.py
--rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.5/datawhispers/mathFuncs.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-05 12:17:08.355224 datawhispers-0.2.8.5/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-05 12:17:08.000000 datawhispers-0.2.8.5/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      309 2023-07-05 12:17:08.000000 datawhispers-0.2.8.5/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-05 12:17:08.000000 datawhispers-0.2.8.5/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-05 12:17:08.000000 datawhispers-0.2.8.5/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-05 12:17:08.000000 datawhispers-0.2.8.5/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-05 12:17:08.355658 datawhispers-0.2.8.5/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2273 2023-07-05 12:17:01.000000 datawhispers-0.2.8.5/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:35:17.944444 datawhispers-0.2.8.6/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.6/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:35:17.944319 datawhispers-0.2.8.6/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)     1218 2023-07-05 20:19:46.000000 datawhispers-0.2.8.6/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:35:17.943414 datawhispers-0.2.8.6/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.6/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)    11593 2023-07-05 19:23:07.000000 datawhispers-0.2.8.6/datawhispers/advancedProg.py
+-rw-r--r--   0 german     (501) staff       (20)    17824 2023-07-05 13:05:34.000000 datawhispers-0.2.8.6/datawhispers/datavis.py
+-rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.6/datawhispers/mathFuncs.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-06 08:35:17.943987 datawhispers-0.2.8.6/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     2340 2023-07-06 08:35:17.000000 datawhispers-0.2.8.6/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      309 2023-07-06 08:35:17.000000 datawhispers-0.2.8.6/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-06 08:35:17.000000 datawhispers-0.2.8.6/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:35:17.000000 datawhispers-0.2.8.6/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-06 08:35:17.000000 datawhispers-0.2.8.6/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-06 08:35:17.944517 datawhispers-0.2.8.6/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2297 2023-07-06 08:35:05.000000 datawhispers-0.2.8.6/setup.py
```

### Comparing `datawhispers-0.2.8.5/LICENSE` & `datawhispers-0.2.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.5/PKG-INFO` & `datawhispers-0.2.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.5
+Version: 0.2.8.6
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.5/README.md` & `datawhispers-0.2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.5/datawhispers/advancedProg.py` & `datawhispers-0.2.8.6/datawhispers/advancedProg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from scipy.optimize import least_squares, minimize, curve_fit
 import sympy as sym
 from sympy import atan as arctan
 from sympy import sqrt, sin, cos, tan, exp, log, ln
 import matplotlib.pyplot as plt
 a, b, c, x = sym.symbols('a, b, c, x', real=True)
-
+# 
 def linReg(x_in,y):
     '''Time series linear regression. Returns coefs in polynomial descending order.
        Coefs computed analytically.
        
         Args:
             x_in: Array with x-values
             y: Array with y-values
@@ -147,14 +147,15 @@
                 Value of the cost function at the solution.
 
             func: ndarray, shape (m,)
                 Vector of residuals at the solution.
 
         Raises:
             None
+            
     '''
     return least_squares(func,x)
 
 
 def r2(y, y_pred):
         '''Coefficient of determination
         '''
```

### Comparing `datawhispers-0.2.8.5/datawhispers/datavis.py` & `datawhispers-0.2.8.6/datawhispers/datavis.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,16 +370,15 @@
                 axis.set_xlabel(self.classification_column);
                 plt.tight_layout()
                 plt.show()
         return P_Wert
     
     
     def get_all(self):
-        """Eine rundumanalyse eines Datensatzes in statistischer Form\n
-        Beachte, dass die Zielvariable kategorisch sein sollte, wenn nicht benutzte .map um es einzufügen
+        """Eine rundumanalyse eines Datensatzes in statistischer Form
         """
         print("                                   --------------------------------------------------")
         print("                                   |                     Analyse                    |")
         print("                                   --------------------------------------------------")
         res = self.get_most_relevant([self.classification_column])
         self.dfStats = res
         self.get_corr_table()
```

### Comparing `datawhispers-0.2.8.5/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.8.6/datawhispers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.5
+Version: 0.2.8.6
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.5/setup.py` & `datawhispers-0.2.8.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from distutils.core import setup
 from pathlib import Path
+import re
+import ast
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
+
+
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.8.5',      # Start with a small number and increase it with every change you make
+  version = "0.2.8.6",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

