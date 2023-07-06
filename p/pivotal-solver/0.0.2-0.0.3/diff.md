# Comparing `tmp/pivotal-solver-0.0.2.tar.gz` & `tmp/pivotal-solver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pivotal-solver-0.0.2.tar", last modified: Sat Jun 24 15:47:51 2023, max compression
+gzip compressed data, was "pivotal-solver-0.0.3.tar", last modified: Thu Jul  6 19:36:16 2023, max compression
```

## Comparing `pivotal-solver-0.0.2.tar` & `pivotal-solver-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.148971 pivotal-solver-0.0.2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      126 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/.flake8
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       62 2023-06-24 13:26:47.000000 pivotal-solver-0.0.2/.gitignore
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      355 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1064 2023-06-24 13:13:25.000000 pivotal-solver-0.0.2/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5560 2023-06-24 15:47:51.144971 pivotal-solver-0.0.2/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3389 2023-06-24 15:46:19.000000 pivotal-solver-0.0.2/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    16866 2023-06-24 14:54:44.000000 pivotal-solver-0.0.2/logo.svg
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.140971 pivotal-solver-0.0.2/pivotal/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      200 2023-06-24 15:47:25.000000 pivotal-solver-0.0.2/pivotal/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10871 2023-06-24 15:15:47.000000 pivotal-solver-0.0.2/pivotal/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      172 2023-06-24 13:33:47.000000 pivotal-solver-0.0.2/pivotal/errors.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6460 2023-06-24 13:36:24.000000 pivotal-solver-0.0.2/pivotal/simplex.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.140971 pivotal-solver-0.0.2/pivotal_solver.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5560 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      457 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       44 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        8 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1387 2023-06-24 15:39:54.000000 pivotal-solver-0.0.2/pyproject.toml
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.144971 pivotal-solver-0.0.2/resources/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   468869 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/resources/2_Simplex.pdf
--rw-rw-r--   0 tomas     (1000) tomas     (1000)  2807945 2023-06-16 22:01:01.000000 pivotal-solver-0.0.2/resources/cvut_fel_opt.pdf
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   677438 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/resources/mitocw.pdf
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-06-24 15:47:51.148971 pivotal-solver-0.0.2/setup.cfg
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.144971 pivotal-solver-0.0.2/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4460 2023-06-24 13:26:24.000000 pivotal-solver-0.0.2/tests/test_api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4668 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/tests/test_simplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:36:16.654345 pivotal-solver-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:36:16.642345 pivotal-solver-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:36:16.646345 pivotal-solver-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/.github/workflows/pypi_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-06 19:36:16.654345 pivotal-solver-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:36:16.646345 pivotal-solver-0.0.3/pivotal/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/pivotal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/pivotal/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/pivotal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/pivotal/simplex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:36:16.646345 pivotal-solver-0.0.3/pivotal_solver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-06 19:36:16.000000 pivotal-solver-0.0.3/pivotal_solver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 19:36:16.000000 pivotal-solver-0.0.3/pivotal_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:36:16.000000 pivotal-solver-0.0.3/pivotal_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:36:16.000000 pivotal-solver-0.0.3/pivotal_solver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 19:36:16.000000 pivotal-solver-0.0.3/pivotal_solver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:36:16.650345 pivotal-solver-0.0.3/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   468869 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/resources/2_Simplex.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  2807945 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/resources/cvut_fel_opt.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   677438 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/resources/mitocw.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:36:16.654345 pivotal-solver-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:36:16.654345 pivotal-solver-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-06 19:35:56.000000 pivotal-solver-0.0.3/tests/test_simplex.py
```

### Comparing `pivotal-solver-0.0.2/LICENSE` & `pivotal-solver-0.0.3/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) <year> <copyright holders>
+Copyright (c) Tomas Roun
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `pivotal-solver-0.0.2/PKG-INFO` & `pivotal-solver-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pivotal-solver
-Version: 0.0.2
+Version: 0.0.3
 Summary: High-level Linear Programming solver using the Simplex algorithm
 Author-email: Tomas Roun <tomas.roun8@gmail.com>
-License: Copyright (c) <year> <copyright holders>
+License: Copyright (c) Tomas Roun
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -18,14 +18,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/tomasr8/pivotal
 Project-URL: Github, https://github.com/tomasr8/pivotal
 Keywords: linear programming,linear programming solver,lp solver,lp,solver,linprog,numerical optimization,convex optimization,simplex,simplex algorithm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -153,23 +154,27 @@
 
 try:
     minimize(objective, constraints)
 except Infeasible:
     print("No solution")
 ```
 
+### Iterations & Tolerance
+
+`minimize` and `maximize` take two keyword arguments `max_iterations` and `tolerance`. `max_iterations` (default `math.inf`) controls the maximum number of iterations of the second phase of the Simplex algorithm. If the maximum number of iterations is reached a potentially non-optimal solution is returned. `tolerance` (default `1e-6`) controls the precision of floating point comparisons, e.g. when comparing against zero. Instead of `x == 0.0`, the algorithm considers a value to be zero when it is within the given tolerance: `abs(x) <= tolerance`.
+
 ## Limitations
 
 - Currently, all variables are assumed to be positive
 
 ## TODO (Contributions welcome)
 
+- ✔️ Setting tolerance & max number of iterations
 - (WIP) Arbitrary variable bounds, e.g. `a <= x <= b`
 - (WIP) Support for absolute values
-- Setting tolerance & max number of iterations
 - MILP solver with branch & bound
 
 
 ## Development
 
 ### Setting up
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pivotal-solver-0.0.2/README.md` & `pivotal-solver-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -113,23 +113,27 @@
 
 try:
     minimize(objective, constraints)
 except Infeasible:
     print("No solution")
 ```
 
+### Iterations & Tolerance
+
+`minimize` and `maximize` take two keyword arguments `max_iterations` and `tolerance`. `max_iterations` (default `math.inf`) controls the maximum number of iterations of the second phase of the Simplex algorithm. If the maximum number of iterations is reached a potentially non-optimal solution is returned. `tolerance` (default `1e-6`) controls the precision of floating point comparisons, e.g. when comparing against zero. Instead of `x == 0.0`, the algorithm considers a value to be zero when it is within the given tolerance: `abs(x) <= tolerance`.
+
 ## Limitations
 
 - Currently, all variables are assumed to be positive
 
 ## TODO (Contributions welcome)
 
+- ✔️ Setting tolerance & max number of iterations
 - (WIP) Arbitrary variable bounds, e.g. `a <= x <= b`
 - (WIP) Support for absolute values
-- Setting tolerance & max number of iterations
 - MILP solver with branch & bound
 
 
 ## Development
 
 ### Setting up
 
@@ -141,8 +145,8 @@
 pip install -e ".[dev]"
 ```
 
 ### Running tests
 
 ```python
 pytest
-```
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pivotal-solver-0.0.2/logo.svg` & `pivotal-solver-0.0.3/logo.svg`

 * *Files 0% similar despite different names*

```diff
@@ -1048,8 +1048,8 @@
 00004170: 4831 3738 2e35 3330 3032 4331 3737 2e36  H178.53002C177.6
 00004180: 3333 3435 2d32 392e 3537 3932 3234 2031  3345-29.579224 1
 00004190: 3737 2e36 3033 3737 2d32 392e 3436 3935  77.60377-29.4695
 000041a0: 3337 2031 3737 2e36 3033 3737 2d32 392e  37 177.60377-29.
 000041b0: 3130 3130 3939 562d 3233 2e35 3132 3636  101099V-23.51266
 000041c0: 5a27 202f 3e0a 2020 2020 2020 2020 3c2f  Z' />.        </
 000041d0: 673e 0a20 2020 203c 2f67 3e0a 3c2f 7376  g>.    </g>.</sv
-000041e0: 673e                                     g>
+000041e0: 673e 0a                                  g>.
```

### Comparing `pivotal-solver-0.0.2/pivotal/api.py` & `pivotal-solver-0.0.3/pivotal/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+import math
 
 import numpy as np
 
 from pivotal.simplex import LinearProgram as LP
 from pivotal.simplex import canonicalize, solve
 
 
@@ -86,18 +87,15 @@
 class Variable(Expression, Comparable):
     id_iter = itertools.count()
 
     def __init__(self, name: str | None = None, coeff=1.0, lb=0, ub=0):
         if name is None:
             id = next(self.id_iter)
             self.name = f"_{id}"
-        # TODO:
-        # elif name.startswith("_"):
-            # raise TypeError("Variables starting with an underscore are reserved for slack"
-                            # " and auxiliary variables used by the solver.")
+        # TODO: underscored variable names
         else:
             self.name = name
         self.coeff = coeff
 
     def __abs__(self):
         return Abs(self)
 
@@ -291,15 +289,15 @@
     def __init__(self, type, objective, constraints):
         self.type = type
         self.objective = objective
         self.constraints = constraints
 
     def validate(self):
         ...
-        #TODO: check for nesting
+        # TODO: check for nesting
 
         # for elt in self.objective:
         #     if not isinstance(elt, Abs):
         #         continue
         #     if self.type == LinearProgram.MIN and elt.sign == -1:
         #         raise Exception("Cannot minimize a negative absolute value")
         #     if self.type == LinearProgram.MAX and elt.sign == 1:
@@ -355,26 +353,30 @@
     def maximize(cls, objective):
         return cls(LinearProgram.MAX, objective, [])
 
     def such_that(self, *constraints):
         self.constraints = constraints
         return self
 
-    def optimize(self):
+    def optimize(self, max_iterations, tolerance):
         all_vars = sorted(list(self._get_variables()))
         A, b, c = canonicalize(*self.as_matrix())
-        value, variables = solve(LP(A, b, c, {}))
+        value, variables = solve(LP(A, b, c, {}), max_iterations=max_iterations, tolerance=tolerance)
         value = value if self.type == LinearProgram.MIN else -value
         variables = variables[:len(all_vars)]
         return value, ({all_vars[i]: v for i, v in enumerate(variables)})
 
     def __str__(self):
         constraints = "\n".join((f"  {constraint}" for constraint in self.constraints))
         return f"{self.type} {self.objective}\ns.t.\n{constraints}"
 
 
-def minimize(objective: Expression, constraints: list[Constraint]) -> tuple[float, dict[str, float]]:
-    return LinearProgram.minimize(objective).such_that(*constraints).optimize()
+def minimize(objective: Expression, constraints: list[Constraint],
+             *, max_iterations=math.inf, tolerance=1e-6) -> tuple[float, dict[str, float]]:
+    return LinearProgram.minimize(objective).such_that(*constraints).optimize(max_iterations=max_iterations,
+                                                                              tolerance=tolerance)
 
 
-def maximize(objective: Expression, constraints: list[Constraint]) -> tuple[float, dict[str, float]]:
-    return LinearProgram.maximize(objective).such_that(*constraints).optimize()
+def maximize(objective: Expression, constraints: list[Constraint],
+             *, max_iterations=math.inf, tolerance=1e-6) -> tuple[float, dict[str, float]]:
+    return LinearProgram.maximize(objective).such_that(*constraints).optimize(max_iterations=max_iterations,
+                                                                              tolerance=tolerance)
```

### Comparing `pivotal-solver-0.0.2/pivotal/simplex.py` & `pivotal-solver-0.0.3/pivotal/simplex.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
             del self.rc[row]
             del self.cr[column]
         else:
             row = self.cr[column]
             del self.rc[row]
             del self.cr[column]
 
+    def __str__(self):
+        return str(self.rc)
+
 
 class LinearProgram:
     def __init__(self, A, b, c, pivots: dict[int, int] | Pivots):
         self.M = np.block([
             [np.atleast_2d(c), np.atleast_2d(0)],
             [A, np.atleast_2d(b).T]
         ])
@@ -69,44 +72,44 @@
     def value(self):
         return -self.M[0, -1]
 
     def __str__(self):
         return f"{self.M}\n{self.pivots}"
 
 
-def zero_out_cj(program, column):
+def zero_out_cj(program, column, *, tolerance):
     row = program.pivots.get(column=column)
     cj = program.c[column]
-    if cj == 0:
+    if is_zero(cj, tolerance):
         return
     program.M[0] -= cj*program.M[row]
 
 
 def do_pivot(program, pivot):
     row, column = pivot
     program.M[row] /= program.M[row, column]
 
     for i in range(1, program.n_constraints+1):
         if i == row:
             continue
         program.M[i] -= program.M[i, column]*program.M[row]
 
 
-def find_pivot(program):
+def find_pivot(program, *, tolerance):
     for j in range(program.n_vars):
         if program.pivots.has(column=j):
             continue
-        if program.c[j] < 0:
+        if program.c[j] < -tolerance:
             min_value = math.inf
             min_i = None
             for i in range(1, program.n_constraints + 1):
-                if program.M[i, j] == 0:
+                if is_zero(program.M[i, j], tolerance):
                     continue
                 frac = program.M[i, -1]/program.M[i, j]
-                if program.M[i, j] > 0 and frac < min_value:
+                if program.M[i, j] > tolerance and (frac-min_value) < -tolerance:
                     min_value = frac
                     min_i = i
             if min_i is not None:
                 return min_i, j
     return None
 
 
@@ -116,37 +119,40 @@
     for j in range(n):
         if program.pivots.has(column=j):
             row = program.pivots.get(column=j)
             solution[j] = program.b[row-1]
     return solution
 
 
-def run_simplex(program):
-    while (pivot := find_pivot(program)) is not None:
+def run_simplex(program, *, max_iterations=math.inf, tolerance=1e-6):
+    iterations = 0
+    while (pivot := find_pivot(program, tolerance=tolerance)) is not None:
         old_pivot = program.pivots.get(row=pivot[0])
         do_pivot(program, pivot)
         program.pivots.delete(column=old_pivot)
         program.pivots.set(row=pivot[0], column=pivot[1])
-        zero_out_cj(program, pivot[1])
+        zero_out_cj(program, pivot[1], tolerance=tolerance)
 
-    if np.all(program.M[0, :-1] >= 0):
-        return
-    else:
+        iterations += 1
+        if iterations > max_iterations:
+            return
+
+    if np.any(program.c < -tolerance):
         raise Unbounded("The program is unbounded, try adding more constraints.")
 
 
-def solve(program):
-    aux_program = aux_problem(program)
-    run_simplex(aux_program)
+def solve(program, *, max_iterations, tolerance):
+    aux_program = aux_problem(program, tolerance=tolerance)
+    run_simplex(aux_program, tolerance=tolerance)
 
-    if not is_zero(aux_program.value):
+    if not is_zero(aux_program.value, tolerance):
         raise Infeasible("The program is infeasible, try removing some constraints.")
 
     if any(j >= program.n_vars for j in aux_program.pivots.cr):
-        zeros = np.isclose(aux_program.A[:, :program.n_vars], 0)
+        zeros = is_zero(aux_program.A[:, :program.n_vars], tolerance)
         sel = np.all(zeros, axis=1)
         sel = np.concatenate(([False], sel))
 
         if np.any(sel):
             aux_program.M = aux_program.M[~sel]
             for i, s in enumerate(sel):
                 if s:
@@ -159,57 +165,50 @@
                 pivots.append((aux_program.pivots.get(column=col), col))
 
         for p in pivots:
             row, col = p
             for candidate_col in range(program.n_vars):
                 if candidate_col in aux_program.pivots.cr:
                     continue
-                if is_zero(aux_program.M[row, candidate_col]):
+                if is_zero(aux_program.M[row, candidate_col], tolerance):
                     continue
                 do_pivot(aux_program, (row, candidate_col))
                 aux_program.pivots.delete(column=col)
                 aux_program.pivots.set(row=row, column=candidate_col)
                 break
 
     A = aux_program.A[:, :program.n_vars]
     b = np.copy(aux_program.b)
     c = np.copy(program.c)
     pivots = aux_program.pivots
     new_prog = LinearProgram(A, b, c, pivots)
 
     for column in pivots.cr:
-        if new_prog.c[column] != 0:
-            zero_out_cj(new_prog, column)
+        if not is_zero(new_prog.c[column], tolerance):
+            zero_out_cj(new_prog, column, tolerance=tolerance)
 
-    run_simplex(new_prog)
+    run_simplex(new_prog, max_iterations=max_iterations, tolerance=tolerance)
     return new_prog.value, get_solution(new_prog)
 
 
-def aux_problem(program):
+def aux_problem(program, *, tolerance):
     m = program.n_constraints
     A = np.copy(np.c_[program.A, np.eye(m)])
     b = np.copy(program.b)
     c = np.concatenate((np.zeros(program.n_vars), np.ones(m)))
     pivots = {program.n_vars+i: i+1 for i in range(m)}
 
     aux_program = LinearProgram(A, b, c, pivots)
     for j in range(program.n_vars, program.n_vars+m):
-        zero_out_cj(aux_program, j)
+        zero_out_cj(aux_program, j, tolerance=tolerance)
     return aux_program
 
 
-TOL = 1e-5
-
-
-def equal(a, b, tol=TOL):
-    return abs(a-b) <= tol
-
-
-def is_zero(v):
-    return equal(v, 0)
+def is_zero(v, tol):
+    return np.isclose(v, 0, rtol=0, atol=tol)
 
 
 def canonicalize(type, A, b, c, constraint_types):
     if type == 'max':
         c *= -1
 
     # convert <= to >=
```

### Comparing `pivotal-solver-0.0.2/pivotal_solver.egg-info/PKG-INFO` & `pivotal-solver-0.0.3/pivotal_solver.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pivotal-solver
-Version: 0.0.2
+Version: 0.0.3
 Summary: High-level Linear Programming solver using the Simplex algorithm
 Author-email: Tomas Roun <tomas.roun8@gmail.com>
-License: Copyright (c) <year> <copyright holders>
+License: Copyright (c) Tomas Roun
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -18,14 +18,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/tomasr8/pivotal
 Project-URL: Github, https://github.com/tomasr8/pivotal
 Keywords: linear programming,linear programming solver,lp solver,lp,solver,linprog,numerical optimization,convex optimization,simplex,simplex algorithm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -153,23 +154,27 @@
 
 try:
     minimize(objective, constraints)
 except Infeasible:
     print("No solution")
 ```
 
+### Iterations & Tolerance
+
+`minimize` and `maximize` take two keyword arguments `max_iterations` and `tolerance`. `max_iterations` (default `math.inf`) controls the maximum number of iterations of the second phase of the Simplex algorithm. If the maximum number of iterations is reached a potentially non-optimal solution is returned. `tolerance` (default `1e-6`) controls the precision of floating point comparisons, e.g. when comparing against zero. Instead of `x == 0.0`, the algorithm considers a value to be zero when it is within the given tolerance: `abs(x) <= tolerance`.
+
 ## Limitations
 
 - Currently, all variables are assumed to be positive
 
 ## TODO (Contributions welcome)
 
+- ✔️ Setting tolerance & max number of iterations
 - (WIP) Arbitrary variable bounds, e.g. `a <= x <= b`
 - (WIP) Support for absolute values
-- Setting tolerance & max number of iterations
 - MILP solver with branch & bound
 
 
 ## Development
 
 ### Setting up
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pivotal-solver-0.0.2/pyproject.toml` & `pivotal-solver-0.0.3/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 packages = ["pivotal"]
 
 [tool.setuptools.dynamic]
 version = {attr = "pivotal.__version__"}
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `pivotal-solver-0.0.2/resources/2_Simplex.pdf` & `pivotal-solver-0.0.3/resources/2_Simplex.pdf`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.2/resources/cvut_fel_opt.pdf` & `pivotal-solver-0.0.3/resources/cvut_fel_opt.pdf`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.2/resources/mitocw.pdf` & `pivotal-solver-0.0.3/resources/mitocw.pdf`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.2/tests/test_api.py` & `pivotal-solver-0.0.3/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import math
+
 import numpy as np
 from numpy.testing import assert_allclose
 
 from pivotal.api import LinearProgram, Variable
 
 
 def assert_solution_almost_equal(expected, actual):
@@ -120,15 +122,15 @@
         25*b + 50*m + 80*z
     ).such_that(
         2*b + m + z >= 8,
         2*b + 6*m + z >= 16,
         b + 3*m + 6*z >= 8,
     )
 
-    assert_solution_almost_equal((160, [3.2, 1.6, 0]), program.optimize())
+    assert_solution_almost_equal((160, [3.2, 1.6, 0]), program.optimize(max_iterations=math.inf, tolerance=1e-6))
 
 
 def test_assignment_problem():
     # Assignment problem
     # technically ILP, but the LP relaxation is always optimal
     # opt.pdf page 149, section 11.4.1
     C = np.array([
@@ -146,38 +148,39 @@
         sum(X[1][j] for j in range(3)) == 1,
         sum(X[2][j] for j in range(3)) == 1,
         sum(X[i][0] for i in range(3)) == 1,
         sum(X[i][1] for i in range(3)) == 1,
         sum(X[i][2] for i in range(3)) == 1,
     )
 
-    assert_solution_almost_equal((4, [1, 0, 0, 0, 0, 1, 0, 1, 0]), program.optimize())
+    assert_solution_almost_equal((4, [1, 0, 0, 0, 0, 1, 0, 1, 0]),
+                                 program.optimize(max_iterations=math.inf, tolerance=1e-6))
 
 
 def test_redundant_constraints():
     # OCW, page 82
     X = [Variable(f"x{i+1}") for i in range(3)]
 
     program = LinearProgram.maximize(
         X[0] + 2*X[1] - X[2]
     ).such_that(
         2*X[0] - X[1] + X[2] == 12,
         -X[0] + 2*X[1] + X[2] == 10,
         X[0] + X[1] + 2*X[2] == 22,
     )
 
-    assert_solution_almost_equal((98/3, [34/3, 32/3, 0]), program.optimize())
+    assert_solution_almost_equal((98/3, [34/3, 32/3, 0]), program.optimize(max_iterations=math.inf, tolerance=1e-6))
 
 
 def test_degenerate_solution():
     # OCW, page 84
     X = [Variable(f"x{i+1}") for i in range(4)]
 
     program = LinearProgram.minimize(
         X[0] + X[1] + 3*X[2]
     ).such_that(
         X[0] + 5*X[1] + X[2] + X[3] == 7,
         X[0] - X[1] + X[2] == 5,
         0.5*X[0] - 2*X[1] + X[2] == 5,
     )
 
-    assert_solution_almost_equal((15, [0, 0, 5, 2]), program.optimize())
+    assert_solution_almost_equal((15, [0, 0, 5, 2]), program.optimize(max_iterations=math.inf, tolerance=1e-6))
```

### Comparing `pivotal-solver-0.0.2/tests/test_simplex.py` & `pivotal-solver-0.0.3/tests/test_simplex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,40 @@
+import math
+
 import numpy as np
 import pytest
 from numpy.testing import assert_array_equal
 
-from pivotal.simplex import (TOL, LinearProgram, canonicalize, do_pivot,
-                             find_pivot, get_solution, solve, zero_out_cj)
+from pivotal.simplex import LinearProgram, canonicalize, do_pivot, find_pivot, get_solution, solve, zero_out_cj
 
 
 def test_zero_out_cj_1():
     A = np.eye(2)
     b = np.ones(2)
     c = np.zeros(2)
     program = LinearProgram(A, b, c, {0: 1, 1: 2})
     M = np.copy(program.M)
-    zero_out_cj(program, 0)
+    zero_out_cj(program, 0, tolerance=1e-6)
     assert_array_equal(M, program.M)
-    zero_out_cj(program, 1)
+    zero_out_cj(program, 1, tolerance=1e-6)
     assert_array_equal(M, program.M)
 
 
 def test_zero_out_cj_2():
     A = np.eye(2)
     b = np.ones(2)
     c = 2*np.ones(2)
     program = LinearProgram(A, b, c, {0: 1, 1: 2})
-    zero_out_cj(program, 0)
+    zero_out_cj(program, 0, tolerance=1e-6)
     assert_array_equal(program.M, np.array([
         [0, 2, -2],
         [1, 0, 1],
         [0, 1, 1],
     ]))
-    zero_out_cj(program, 1)
+    zero_out_cj(program, 1, tolerance=1e-6)
     assert_array_equal(program.M, np.array([
         [0, 0, -4],
         [1, 0, 1],
         [0, 1, 1],
     ]))
 
 
@@ -75,39 +76,39 @@
     A = np.array([
         [1, 0, 2],
         [0, 1, 7]
     ], dtype=float)
     b = [3, 5]
     c = [1, 1, 1]
     program = LinearProgram(A, b, c, {})
-    pivot = find_pivot(program)
+    pivot = find_pivot(program, tolerance=1e-6)
     assert pivot is None
 
 
 def test_find_pivot_no_pivot_negative_column():
     A = np.array([
         [1, 0, -2],
         [0, 1, -7]
     ], dtype=float)
     b = [3, 5]
     c = [1, 1, -3]
     program = LinearProgram(A, b, c, {})
-    pivot = find_pivot(program)
+    pivot = find_pivot(program, tolerance=1e-6)
     assert pivot is None
 
 
 def test_find_pivot():
     A = np.array([
         [1, 0, 2],
         [0, 1, 7]
     ], dtype=float)
     b = [3, 5]
     c = [1, 1, -2]
     program = LinearProgram(A, b, c, {0: 1, 1: 2})
-    pivot = find_pivot(program)
+    pivot = find_pivot(program, tolerance=1e-6)
     assert_array_equal(pivot, [2, 2])
 
 
 def test_get_solution_1():
     A = np.array([
         [1, 0],
         [0, 1]
@@ -182,28 +183,28 @@
         [1, 3],
         [4, 1],
     ], dtype=float)
 
     b = np.array([6, 5], dtype=float)
     c = np.array([1, 2], dtype=float)
 
-    value, X = solve(LinearProgram(A, b, c, {}))
+    value, X = solve(LinearProgram(A, b, c, {}), max_iterations=math.inf, tolerance=1e-6)
     X_true = [0.81818182, 1.72727273]
-    assert value == pytest.approx(4.27272727, TOL)
+    assert value == pytest.approx(4.27272727)
     for x, xt in zip(X, X_true):
-        assert x == pytest.approx(xt, TOL)
+        assert x == pytest.approx(xt)
 
 
 def test_program_2():
     A = np.array([
         [3, 2, 1],
         [1, 2, 2],
     ], dtype=float)
 
     b = np.array([10, 15], dtype=float)
     c = np.array([-20, -30, -40], dtype=float)
 
-    value, X = solve(LinearProgram(A, b, c, {}))
+    value, X = solve(LinearProgram(A, b, c, {}), max_iterations=math.inf, tolerance=1e-6)
     X_true = [1, 0, 7]
-    assert value == pytest.approx(-300, TOL)
+    assert value == pytest.approx(-300)
     for x, xt in zip(X, X_true):
-        assert x == pytest.approx(xt, TOL)
+        assert x == pytest.approx(xt)
```

