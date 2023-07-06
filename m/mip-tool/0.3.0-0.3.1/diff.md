# Comparing `tmp/mip_tool-0.3.0-py3-none-any.whl.zip` & `tmp/mip_tool-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10552 bytes, number of entries: 10
+Zip file size: 10602 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 mip_tool/__init__.py
 -rw-r--r--  2.0 unx     3050 b- defN 80-Jan-01 00:00 mip_tool/func/__init__.py
--rw-r--r--  2.0 unx     4859 b- defN 80-Jan-01 00:00 mip_tool/util.py
--rw-r--r--  2.0 unx     2237 b- defN 80-Jan-01 00:00 mip_tool/view/__init__.py
+-rw-r--r--  2.0 unx     4876 b- defN 80-Jan-01 00:00 mip_tool/util.py
+-rw-r--r--  2.0 unx     2268 b- defN 80-Jan-01 00:00 mip_tool/view/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 mip_tool/view/__main__.py
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     2635 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      788 b- defN 16-Jan-01 00:00 mip_tool-0.3.0.dist-info/RECORD
-10 files, 24713 bytes uncompressed, 9214 bytes compressed:  62.7%
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 mip_tool-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2686 b- defN 80-Jan-01 00:00 mip_tool-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mip_tool-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 mip_tool-0.3.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      788 b- defN 16-Jan-01 00:00 mip_tool-0.3.1.dist-info/RECORD
+10 files, 24812 bytes uncompressed, 9264 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: mip_tool/view/__init__.py
 Comment: 
 
 Filename: mip_tool/view/__main__.py
 Comment: 
 
-Filename: mip_tool-0.3.0.dist-info/LICENSE
+Filename: mip_tool-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: mip_tool-0.3.0.dist-info/WHEEL
+Filename: mip_tool-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: mip_tool-0.3.0.dist-info/entry_points.txt
+Filename: mip_tool-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: mip_tool-0.3.0.dist-info/METADATA
+Filename: mip_tool-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mip_tool-0.3.0.dist-info/RECORD
+Filename: mip_tool-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mip_tool/util.py

```diff
@@ -109,15 +109,15 @@
     :param seed: seed
     :param rtco: rate of non zero in matrix
     :param var_type: variable type
     """
     rtco = max(1e-3, rtco)
     rnd = np.random.default_rng(seed)
     while True:
-        m = Model()
+        m = Model(solver_name="CBC")
         x = m.add_var_tensor((nv,), "x", var_type=var_type)
         m.objective = maximize(xsum(rnd.integers(20, 40, nv) * x))
         rem = nc
         while rem > 0:
             a = rnd.integers(10, 30, nv)
             a[rnd.random(nv) >= rtco] = 0
             if not a.sum():
```

## mip_tool/view/__init__.py

```diff
@@ -1,19 +1,21 @@
 import sys
 
 from IPython.display import HTML
 from mip import ParameterNotAvailable
 
-STYLE = ' style="text-align: left;" width="60"'
-VAR_WIDTH = 60
+STYLE = ' style="text-align: left;" width="64"'
+VAR_WIDTH = 64
 
 
 def main():
     src = f"{sys.argv[1]};" if len(sys.argv) > 1 else ""
-    exec(f"import mip_tool.view; from mip import *;m = Model();{src}print(view_model(m).data)")
+    exec(
+        f"import mip_tool.view; from mip import *;m = Model(solver_name='CBC');{src}print(view_model(m).data)"
+    )
 
 
 def var_desc(v):
     lb, ub = v.lb, v.ub
     if v.var_type == "C":
         s = "連続変数" if lb else "非負変数"
     elif v.var_type == "B":
@@ -54,15 +56,15 @@
             s = str(cnst.expr).removeprefix("+ ")
             s = s.replace("<=", "≦").replace(">=", "≧")
             lst.append(f"<tr><td>{s}</td></tr>\n")
         lst[0] = f'<tr><td rowspan="{len(lst)}"{STYLE}>制約条件</td>' + lst[0][4:]
     return f'<table width="100%">\n{"".join(lst)}</table>'
 
 
-def view_model(m, width="300", has_html=False):
+def view_model(m, width="320", has_html=False):
     try:
         obj = m.objective
     except ParameterNotAvailable:
         obj = None
     s = f"""\
 <table width="{width}">
   <tr><td style="text-align: center;">モデル</td></tr>
```

## Comparing `mip_tool-0.3.0.dist-info/LICENSE` & `mip_tool-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mip_tool-0.3.0.dist-info/METADATA` & `mip_tool-0.3.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mip-tool
-Version: 0.3.0
+Version: 0.3.1
 Summary: `mip-tool` is a package for Python-MIP.
 Home-page: https://github.com/SaitoTsutomu/mip-tool
 License: Apache-2.0
 Author: Saito Tsutomu
 Author-email: tsutomu7@hotmail.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -35,15 +35,15 @@
 Maximize y which is on points of (-2, 6), (-1, 7), (2, -2), (4, 5).
 
 ```python
 import numpy as np
 from mip import INF, Model, OptimizationStatus
 from mip_tool import add_lines, show_model
 
-m = Model()
+m = Model(solver_name="CBC")
 x = m.add_var("x", lb=-INF)
 y = m.add_var("y", obj=-1)
 curve = np.array([[-2, 6], [-1, 7], [2, -2], [4, 5]])
 add_lines(m, curve, x, y)
 m.verbose = 0
 m.optimize()
 assert m.status == OptimizationStatus.OPTIMAL
@@ -80,15 +80,15 @@
 Easy to understand using F.
 
 attention: Change Model and Var when using mip_tool.func.
 
 ```python
 from mip_tool.func import F
 
-m = Model()
+m = Model(solver_name="CBC")
 x = m.add_var("x")
 y = m.add_var("y", obj=-1)
 m += y <= F([[0, 2], [1, 3], [2, 2]], x)
 m.verbose = 0
 m.optimize()
 print(x.x, y.x)  # 1.0 3.0
 ```
@@ -104,15 +104,15 @@
 ```python
 import pandas as pd
 from mip import Model, maximize, xsum
 from mip_tool.func import addvars
 
 A = pd.DataFrame([[1, 2], [3, 1]])
 b = pd.Series([16, 18])
-m = Model()
+m = Model(solver_name="CBC")
 x = addvars(m, A, "", False)
 m.objective = maximize(xsum(x))
 m += A @ x <= b
 m.verbose = 0
 m.optimize()
 print(x.astype(float))  # [4. 6.]
 ```
```

