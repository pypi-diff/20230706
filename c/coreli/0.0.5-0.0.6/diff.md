# Comparing `tmp/coreli-0.0.5.tar.gz` & `tmp/coreli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreli-0.0.5.tar", last modified: Sat Jun 24 12:59:51 2023, max compression
+gzip compressed data, was "coreli-0.0.6.tar", last modified: Thu Jul  6 07:25:19 2023, max compression
```

## Comparing `coreli-0.0.5.tar` & `coreli-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.421962 coreli-0.0.5/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1071 2023-06-24 12:55:12.000000 coreli-0.0.5/LICENSE
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4486 2023-06-24 12:59:51.421962 coreli-0.0.5/PKG-INFO
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3972 2023-06-24 12:55:12.000000 coreli-0.0.5/README.md
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.417962 coreli-0.0.5/coreli/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4028 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/Collatz_maps.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3294 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/Collatz_tilings.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      202 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/__init__.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)    14584 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/padic_integers.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     9193 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/parity_vectors.py
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.421962 coreli-0.0.5/coreli/tinytiles/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      119 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/__init__.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1406 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/interactive.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3503 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/model.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3327 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/svg_view.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     2445 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/utils.py
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.421962 coreli-0.0.5/coreli.egg-info/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4486 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/PKG-INFO
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      425 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        1 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       47 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/requires.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        7 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/top_level.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       38 2023-06-24 12:59:51.421962 coreli-0.0.5/setup.cfg
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      846 2023-06-24 12:56:15.000000 coreli-0.0.5/setup.py
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-07-06 07:25:19.812778 coreli-0.0.6/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1071 2023-06-24 12:55:12.000000 coreli-0.0.6/LICENSE
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4597 2023-07-06 07:25:19.812778 coreli-0.0.6/PKG-INFO
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4047 2023-07-06 07:24:37.000000 coreli-0.0.6/README.md
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-07-06 07:25:19.812778 coreli-0.0.6/coreli/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4028 2023-06-24 12:55:12.000000 coreli-0.0.6/coreli/Collatz_maps.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3425 2023-07-05 12:33:27.000000 coreli-0.0.6/coreli/Collatz_tilings.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      202 2023-06-24 12:55:12.000000 coreli-0.0.6/coreli/__init__.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)    14584 2023-06-24 12:55:12.000000 coreli-0.0.6/coreli/padic_integers.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     9408 2023-06-30 17:40:57.000000 coreli-0.0.6/coreli/parity_vectors.py
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-07-06 07:25:19.812778 coreli-0.0.6/coreli/tinytiles/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      119 2023-06-24 12:55:12.000000 coreli-0.0.6/coreli/tinytiles/__init__.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1597 2023-06-24 15:55:33.000000 coreli-0.0.6/coreli/tinytiles/interactive.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3799 2023-07-06 07:21:29.000000 coreli-0.0.6/coreli/tinytiles/model.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3709 2023-07-06 07:20:50.000000 coreli-0.0.6/coreli/tinytiles/svg_view.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     2445 2023-06-24 15:39:31.000000 coreli-0.0.6/coreli/utils.py
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-07-06 07:25:19.812778 coreli-0.0.6/coreli.egg-info/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4597 2023-07-06 07:25:19.000000 coreli-0.0.6/coreli.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      425 2023-07-06 07:25:19.000000 coreli-0.0.6/coreli.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        1 2023-07-06 07:25:19.000000 coreli-0.0.6/coreli.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       47 2023-07-06 07:25:19.000000 coreli-0.0.6/coreli.egg-info/requires.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        7 2023-07-06 07:25:19.000000 coreli-0.0.6/coreli.egg-info/top_level.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       38 2023-07-06 07:25:19.812778 coreli-0.0.6/setup.cfg
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      808 2023-07-06 07:24:56.000000 coreli-0.0.6/setup.py
```

### Comparing `coreli-0.0.5/LICENSE` & `coreli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `coreli-0.0.5/PKG-INFO` & `coreli-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: coreli
-Version: 0.0.5
+Version: 0.0.6
 Summary: The Collatz Research Library provides tools for experimenting and testing hypothesises related to the Collatz Process.
 Home-page: https://github.com/tcosmo/coreli
 Author: Tristan Stérin
 Author-email: tristan.sterin@mu.ie
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,14 +28,21 @@
 
 The appararent simplicity of this problem hides a very difficult mathematical problem. Actually, we believe that this problem has a lot to do with **Computer Science**. That's why we created **Coreli**, a library for experimenting and testing hypothesises regarding the Collatz process.      
 
 # Doc
 
 Coreli's doc is [hosted here](https://dna.hamilton.ie/tsterin/coreli/docs/).
 
+## Dev: deploy to pypi
+
+```
+python setup.py sdist
+twine upload dist/*
+```
+
 # References
 
 - David Applegate and Jeffrey Lagarias. Density bounds for the 3x + 1 problem. ii. krasikov
 inequalities. Mathematics of Computation - Math. Comput., 64:427–438, 01 1995. doi:
 10.2307/2153346.          
 
 - Jean Berstel, Jr. and Christophe Reutenauer. Rational Series and Their Languages. Springer-
@@ -81,7 +90,8 @@
 - Riho Terras. A stopping time problem on the positive integers. Acta Arithmetica, 30(3):241–252, 1976. URL: http://eudml.org/doc/205476.            
 
 - Günther Wirsching. On the combinatorial structure of 3n + 1 predecessor sets. Discrete Math-
 ematics, 148(1-3):265–286, January 1996. URL: https://doi.org/10.1016/0012-365x(94)00243-c, doi:10.1016/0012-365x(94)00243-c.                 
 
 - Günther J. Wirsching. The dynamical system generated by the 3n + 1 function. Springer,
 Berlin New York, 1998.
+
```

### Comparing `coreli-0.0.5/README.md` & `coreli-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 The appararent simplicity of this problem hides a very difficult mathematical problem. Actually, we believe that this problem has a lot to do with **Computer Science**. That's why we created **Coreli**, a library for experimenting and testing hypothesises regarding the Collatz process.      
 
 # Doc
 
 Coreli's doc is [hosted here](https://dna.hamilton.ie/tsterin/coreli/docs/).
 
+## Dev: deploy to pypi
+
+```
+python setup.py sdist
+twine upload dist/*
+```
+
 # References
 
 - David Applegate and Jeffrey Lagarias. Density bounds for the 3x + 1 problem. ii. krasikov
 inequalities. Mathematics of Computation - Math. Comput., 64:427–438, 01 1995. doi:
 10.2307/2153346.          
 
 - Jean Berstel, Jr. and Christophe Reutenauer. Rational Series and Their Languages. Springer-
```

### Comparing `coreli-0.0.5/coreli/Collatz_maps.py` & `coreli-0.0.6/coreli/Collatz_maps.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.5/coreli/padic_integers.py` & `coreli-0.0.6/coreli/padic_integers.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.5/coreli/parity_vectors.py` & `coreli-0.0.6/coreli/parity_vectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Tuple, Union
 from coreli.Collatz_maps import T
 from coreli.Collatz_tilings import Collatz_tileset
 from coreli.padic_integers import PadicInt, least_significant_digit
 from coreli.tinytiles.model import SquareGlues, Tiling
-from coreli.utils import int_to_base, iterate,iterates
+from coreli.utils import int_to_base, iterate, iterates
 from sympy import Rational
+import random
 
 """ Implementing Collatz parity vectors.
 
     References
     ========== 
 
     [1] A stopping time problem on the positive integers. Riho Terras. 
@@ -30,82 +31,96 @@
     [5] Binary expression of ancestors in the Collatz graph. Tristan Stérin.
         RP 2020: Proceedings of the 14th International Conference on Reachability 
         Problems, (Paris, France, October 19-21, 2020), pp 115-130. 2020.
         https://arxiv.org/abs/1907.00775
 
 """
 
+
 class ParityVector(object):
-    """ A parity vector is a list of 0s and 1s which corresponds to the 
+    """A parity vector is a list of 0s and 1s which corresponds to the
     parity of elements of a Collatz sequences (with map T).
     (i.e. which of the maps x/2 or (3x+1)/2 is taken at each step)
 
     It is known that (see [1,2,4]):
         - All parity vectors are feasible in N, i.e. for any parity vector
-        of length n there is a natural number that follows the parities given by the 
+        of length n there is a natural number that follows the parities given by the
         parity vector in its first n T-Collatz steps.
 
-        - More precisely, for any parity vector of length n, there is a smallest 
-        integer α in N such that the first n T-Collatz steps follow the parities 
+        - More precisely, for any parity vector of length n, there is a smallest
+        integer α in N such that the first n T-Collatz steps follow the parities
         given by the parity vector, and then, all integers of the form a2^n + α
-        also follow the parities given by the parity vector. We say that 
+        also follow the parities given by the parity vector. We say that
         (α,β) is the first "occurrence" of the parity vector, with β = T^n(α).
 
         - There is a bijection between parity vectors of length n and numbers < 2^n,
         i.e. two distinct numbers < 2^n have distinct length-n parity vectors.
 
-        - When considering infinite parity vectors (i.e. associated to infinite 
-        T-Collatz sequences), we get a continuous bijection Q from Z_2 to Z_2, 
-        mapping Collatz-inputs in Z_2 to their parity vector, seen as an element 
+        - When considering infinite parity vectors (i.e. associated to infinite
+        T-Collatz sequences), we get a continuous bijection Q from Z_2 to Z_2,
+        mapping Collatz-inputs in Z_2 to their parity vector, seen as an element
         of Z_2 (see [2,4]).
 
         - It is known that if Q(x) is eventually periodic then x is eventually periodic
         i.e. x is rational.
 
-        - It is conjectured that if x is eventually periodic then Q(x) is eventually 
+        - It is conjectured that if x is eventually periodic then Q(x) is eventually
         periodic, Lagarias Periodicity Conjecture [2]. If this conjecture is true,
         then there is no divergent Collatz orbit in N.
     """
+
     def __init__(self, parity_vector):
-        if len(list(filter(lambda x: x not in [0,1], parity_vector))) != 0:
-            raise ValueError(f"A parity vector must contain only 0s and 1s, which is not the case for {parity_vector}")
+        if len(list(filter(lambda x: x not in [0, 1], parity_vector))) != 0:
+            raise ValueError(
+                f"A parity vector must contain only 0s and 1s, which is not the case for {parity_vector}"
+            )
         self.parity_vector = parity_vector
-    
+
+    @classmethod
+    def get_random_parity_vector(cls, length):
+        return cls(random.choices([0, 1], k=length))
+
+    def __iter__(self):
+        for each in self.parity_vector:
+            yield each
+
     def __len__(self):
         return len(self.parity_vector)
 
     def odd_len(self):
-        """ Returns the number of 1s (odd terms) in the parity vector which is a metric that is often used
+        """Returns the number of 1s (odd terms) in the parity vector which is a metric that is often used
         when working with parity vector.
         """
-        return len(list(filter(lambda x: x==1,self.parity_vector)))
+        return len(list(filter(lambda x: x == 1, self.parity_vector)))
 
     def __repr__(self):
         return str(self)
-    
+
     def __str__(self):
         return str(self.parity_vector)
 
     @classmethod
     def from_Collatz(cls, x: Union[int, Rational, PadicInt], n: int) -> "ParityVector":
-        """ Returns the parity vector corresponding to n application of Collatz map T.
+        """Returns the parity vector corresponding to n application of Collatz map T.
         The parity vector will be of size n+1.
 
         :Example:
             >>> ParityVector.from_Collatz(23,10)
             [1, 1, 1, 0, 0, 0, 0, 1, 0, 0, 0]
         """
         return cls(list(map(least_significant_digit, iterates(T, n, x))))
 
-    def first_occurrence(self, symbolic=False) -> Union[Tuple[int,int],Tuple[str,str]]:
-        """ Returns the couple (α,β) such that α is the smallest number in N
-        such that its first n T-Collatz steps follow the parities given by 
+    def first_occurrence(
+        self, symbolic=False
+    ) -> Union[Tuple[int, int], Tuple[str, str]]:
+        """Returns the couple (α,β) such that α is the smallest number in N
+        such that its first n T-Collatz steps follow the parities given by
         the length-n parity vector. And, β = T^n(α).
 
-        There are explicit formulae for α and β, seen [4]. But here we use an iterative 
+        There are explicit formulae for α and β, seen [4]. But here we use an iterative
         algorithm described in [5].
 
         If `symbolic` is true, the function returns α in base 2 and n bits and β in base 3
         and k bits with k the number of 1s in the parity vector.
 
         :Example:
         >>> ParityVector([1,1,0,1]).first_occurrence()
@@ -117,44 +132,45 @@
         """
 
         n = len(self)
         alpha = 0
         beta = 0
         k = 0
 
-        for i,b in enumerate(self.parity_vector):
-            if b != beta%2:
+        for i, b in enumerate(self.parity_vector):
+            if b != beta % 2:
                 alpha += 2**i
 
             if b == 1:
                 k += 1
 
-            modular_inverse_of_two = (3**k+1)//2
+            modular_inverse_of_two = (3**k + 1) // 2
             if b == 0:
-                beta = (beta * modular_inverse_of_two)%(3**k)
+                beta = (beta * modular_inverse_of_two) % (3**k)
             else:
-                beta = ((3*beta + 1 )*modular_inverse_of_two)%(3**(k))
-            
-        assert(beta == iterate(T,n,alpha))
-        
+                beta = ((3 * beta + 1) * modular_inverse_of_two) % (3 ** (k))
+
+        assert beta == iterate(T, n, alpha)
+
         if not symbolic:
             return alpha, beta
 
-        return int_to_base(alpha,2,n), int_to_base(beta,3,k)
+        return int_to_base(alpha, 2, n), int_to_base(beta, 3, k)
 
     def rotate(self, n: int = 1) -> "ParityVector":
-        def rotate_list(l,n):
+        def rotate_list(l, n):
             sign = -1 if n < 0 else 1
-            n = sign*(abs(n)%len(l))
+            n = sign * (abs(n) % len(l))
             return l[n:] + l[:n]
-        rotated_pv = rotate_list(self.parity_vector,n)
+
+        rotated_pv = rotate_list(self.parity_vector, n)
         return ParityVector(rotated_pv)
 
-    def most_complex_tile(self) -> Union[None,int]:
-        """ Returns the "most complex tile" of a parity vector. 
+    def most_complex_tile(self) -> Union[None, int]:
+        """Returns the "most complex tile" of a parity vector.
         See Tristan Stérin's thesis, Chapter 1, Section 1.5, for definition.
 
         >>> ParityVector([1,1,0,1]*2).most_complex_tile()
         2
 
         >>> ParityVector([1,1,0,1]*2).rotate()
         [1, 0, 1, 1, 1, 0, 1, 1]
@@ -166,26 +182,24 @@
         >>> ParityVector([1,1,0,1]*2).rotate(-1).most_complex_tile()
         5
         """
         tiling = self.to_tiling()
         tiling.all_steps()
         tile = tiling.get_top_left_tile()
 
-        if tile is None or not isinstance(tile,int):
+        if tile is None or not isinstance(tile, int):
             return None
-        
-        return tile
-        
 
+        return tile
 
     def cyclic_rational(self) -> Rational:
-        """ Returns the unique rational x such that T^n(x) = x and the parity vector
+        """Returns the unique rational x such that T^n(x) = x and the parity vector
         corresponds to the n first Collatz steps of x.
 
-        Explicit formula deducible from 2.13 in [3] (page 41). 
+        Explicit formula deducible from 2.13 in [3] (page 41).
 
         This rational also happen to be 2-adic, 3-adic and 6-adic integer since its numerator
         is of the form 2^n - 3^k (its not a multiple of 2, 3, or 6).
 
         :Example:
             >>> ParityVector([1]).cyclic_rational()
             -1
@@ -204,44 +218,43 @@
         """
 
         indices_of_1s = [i for i, x in enumerate(self.parity_vector) if x == 1]
 
         n = len(self)
         k = self.odd_len()
         sum = 0
-        
+
         for i, s in enumerate(indices_of_1s):
-            sum += 3**(k-1-i)*2**(s)
-        
+            sum += 3 ** (k - 1 - i) * 2 ** (s)
+
         return Rational(sum, 2**n - 3**k)
 
     def to_tiling(self) -> Tiling:
-        """ Builds the Collatz tiling associated to the parity vector.
-        """
-        pos = [len(self)-1,self.odd_len()]
+        """Builds the Collatz tiling associated to the parity vector."""
+        pos = [len(self) - 1, self.odd_len()]
         tiling: Tiling = {}
-        
+
         for pbit in self.parity_vector:
             tpos = tuple(pos)
-            #print(tpos)  
+            # print(tpos)
             if pbit == 0:
                 if tpos not in tiling:
-                    tiling[tpos] = [None]*4
+                    tiling[tpos] = [None] * 4
                 tiling[tpos][0] = 0
                 pos[0] -= 1
             else:
-                tpos_east = tpos[0]+1,tpos[1]
-                tpos_south = tpos[0],tpos[1]-1
+                tpos_east = tpos[0] + 1, tpos[1]
+                tpos_south = tpos[0], tpos[1] - 1
                 if tpos_east not in tiling:
-                    tiling[tpos_east] = [None]*4
+                    tiling[tpos_east] = [None] * 4
                 if tpos_south not in tiling:
-                    tiling[tpos_south] = [None]*4
-                #print("east",tpos_east)
+                    tiling[tpos_south] = [None] * 4
+                # print("east",tpos_east)
                 tiling[tpos_east][3] = 1
                 tiling[tpos_south][0] = 0
                 pos[0] -= 1
                 pos[1] -= 1
-        
+
         for pos in tiling:
             tiling[pos] = SquareGlues(*tiling[pos])
-        
-        return Tiling(tiling, Collatz_tileset)
+
+        return Tiling(tiling, Collatz_tileset)
```

### Comparing `coreli-0.0.5/coreli/tinytiles/interactive.py` & `coreli-0.0.6/coreli/tinytiles/interactive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import ipywidgets as widgets
 from IPython.display import display
 
 from coreli.tinytiles.model import Tiling
 from coreli.tinytiles.svg_view import draw_tiling
 
-def interactive(tiling: Tiling):
+def interactive(tiling: Tiling, synchronous=False, can_build_on_null_glues=True):
 
     first_world = copy.deepcopy(tiling.tiling)
     
     button_step = widgets.Button(description="Step")
     button_steps = widgets.Button(description="All steps")
     button_reset = widgets.Button(description="Reset")
     output = widgets.Output()
@@ -19,21 +19,21 @@
         display(draw_tiling(tiling))
 
     display(output, widgets.HBox([button_step, button_steps, button_reset]))
     
     def callback_step(b):
         with output:
             output.clear_output(wait=True)
-            tiling.step()
+            tiling.step(synchronous=synchronous,can_build_on_null_glues=can_build_on_null_glues)
             display(draw_tiling(tiling))
 
     def callback_steps(b):
         with output:
             output.clear_output(wait=True)
-            tiling.all_steps()
+            tiling.all_steps(synchronous=synchronous,can_build_on_null_glues=can_build_on_null_glues)
             display(draw_tiling(tiling))
             
     def callback_reset(b):
         with output:
             output.clear_output(wait=True)
             for p in list(tiling.tiling.keys())[:]:
                 del tiling.tiling[p]
```

### Comparing `coreli-0.0.5/coreli/tinytiles/model.py` & `coreli-0.0.6/coreli/tinytiles/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,121 @@
 from typing import Dict, Tuple, List, Union
 from collections import namedtuple
 
-Coordinates = namedtuple('Coordinates', ['x','y'])
-SquareGlues = namedtuple('SquareGlues', ['north', 'east', 'south', 'west'])
-tTiling = Dict[Coordinates,SquareGlues]
+Coordinates = namedtuple("Coordinates", ["x", "y"])
+SquareGlues = namedtuple("SquareGlues", ["north", "east", "south", "west"])
+tTiling = Dict[Coordinates, SquareGlues]
 Tileset = List[SquareGlues]
 
+
 class Tiling(object):
     def __init__(self, tiling: tTiling, tileset: Tileset):
         self.tiling: tTiling = tiling
         self.tileset: Tileset = tileset
 
     def __getitem__(self, key):
         return self.tiling[key]
 
-    def get_world_boundaries(self) -> Tuple[int,int]:
-        """ Assuming positive coords only. """
+    def get_world_boundaries(self) -> Tuple[int, int]:
+        """Assuming positive coords only."""
         max_x = 0
         max_y = 0
-        for x,y in self.tiling.keys():
-            max_x = max(x,max_x)
-            max_y = max(y,max_y)
+        for x, y in self.tiling.keys():
+            max_x = max(x, max_x)
+            max_y = max(y, max_y)
         return max_x, max_y
 
-    def get_neighboring_glues(self,pos) -> SquareGlues:
-        to_ret: SquareGlues = [None]*4
-        directions = [(0,1),(1,0),(0,-1),(-1,0)]
-        for i, (dir_x,dir_y) in enumerate(directions):
-                new_pos = pos[0]+dir_x, pos[1]+dir_y
-                
-                if pos in self.tiling and self.tiling[pos][i] is not None:
-                    to_ret[i] = self.tiling[pos][i]
-                elif new_pos in self.tiling:
-                    to_ret[i] = self.tiling[new_pos][(i+2)%4]
+    def get_neighboring_glues(self, pos) -> SquareGlues:
+        to_ret: SquareGlues = [None] * 4
+        directions = [(0, 1), (1, 0), (0, -1), (-1, 0)]
+        for i, (dir_x, dir_y) in enumerate(directions):
+            new_pos = pos[0] + dir_x, pos[1] + dir_y
+
+            if pos in self.tiling and self.tiling[pos][i] is not None:
+                to_ret[i] = self.tiling[pos][i]
+            elif new_pos in self.tiling:
+                to_ret[i] = self.tiling[new_pos][(i + 2) % 4]
         return to_ret
 
-    def find_matching_tile_in_tileset(self, glues: SquareGlues, threshold:int) -> Union[None, SquareGlues]:
+    def find_matching_tile_in_tileset(
+        self, glues: SquareGlues, threshold: int
+    ) -> Union[None, SquareGlues]:
         to_ret = None
         for tile_type in self.tileset:
             score = 0
             for i in range(4):
                 if tile_type[i] == None or glues[i] == None:
                     continue
-                
+
                 if tile_type[i] == glues[i]:
                     score += 1
-                
+
                 if score >= threshold:
                     return tile_type
 
-    def get_top_left_tile(self) -> Union[None,int,SquareGlues]:
+    def get_top_left_tile(self) -> Union[None, int, SquareGlues]:
         world_w, world_h = self.get_world_boundaries()
-        
-        top_left = 0,world_h
-        
+
+        top_left = 0, world_h
+
         if top_left not in self.tiling:
             return None
-        
+
         try:
             return self.tileset.index(self.tiling[top_left])
         except ValueError as e:
             return self.tiling[top_left]
 
-    def all_steps(self, threshold=2, can_build_on_null_glues=True) -> None:
-        while self.step(threshold, can_build_on_null_glues):
+    def all_steps(
+        self, threshold=2, synchronous=False, can_build_on_null_glues=True
+    ) -> None:
+        while self.step(threshold, synchronous, can_build_on_null_glues):
             continue
-    
-    def step(self, threshold=2, can_build_on_null_glues=True) -> None:
-        """ One step of tile attachement.
+
+    def step(
+        self, threshold=2, synchronous=False, can_build_on_null_glues=True
+    ) -> None:
+        """One step of tile attachement.
         Inefficient n^2 implementation.
         """
         world_w, world_h = self.get_world_boundaries()
 
-        for x in range(world_w+1):
-            for y in range(world_h+1):
-                pos = x,y
-                
-                
+        # for synchronous mode
+        to_update = []
+
+        for x in range(world_w + 1):
+            for y in range(world_h + 1):
+                pos = x, y
+
                 if pos in self.tiling and None not in self.tiling[pos]:
                     continue
-                    
-                if pos in self.tiling and not can_build_on_null_glues and None in self.tiling[pos]:
+
+                if (
+                    pos in self.tiling
+                    and not can_build_on_null_glues
+                    and None in self.tiling[pos]
+                ):
                     continue
-                
+
                 neighboring_glues = self.get_neighboring_glues(pos)
-                
-                
-                tile = self.find_matching_tile_in_tileset(neighboring_glues,threshold)
-                #print(pos,neighboring_glues,tile)
+
+                tile = self.find_matching_tile_in_tileset(neighboring_glues, threshold)
+                # print(pos,neighboring_glues,tile)
                 if tile is not None:
-                    self.tiling[pos] = tile
-                    return True
-        return False 
+                    if synchronous:
+                        to_update.append((pos, tile))
+                    else:
+                        self.tiling[pos] = tile
+                        return True
+
+        if synchronous:
+            for pos, tile in to_update:
+                self.tiling[pos] = tile
+
+        return False
 
     from drawSvg import Drawing
+
     def draw_svg(self) -> Drawing:
         from coreli.tinytiles.svg_view import draw_tiling
-        return draw_tiling(self)
+
+        return draw_tiling(self)
```

### Comparing `coreli-0.0.5/coreli/tinytiles/svg_view.py` & `coreli-0.0.6/coreli/tinytiles/svg_view.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,122 @@
 import drawSvg as draw
 from coreli.tinytiles.model import Tileset, Tiling
 
 TILE_SIZE = 32
 null_glue_color = "#CACACA"
-color_wheel = {0:"#E6C58F",1:"#0AC52E",2:"#E37998",'S':'#3FB3F3'}
+color_wheel = {0: "#E6C58F", 1: "#0AC52E", 2: "#E37998", "S": "#3FB3F3"}
+
+
+def draw_tile(d, x, y, tile, tileset: Tileset = [], debug=False):
+    draw_x, draw_y = TILE_SIZE * x, TILE_SIZE * y
 
-def draw_tile(d,x,y,tile,tileset:Tileset=[],debug=False):
-    draw_x, draw_y = TILE_SIZE*x, TILE_SIZE*y
-    
     tile_group = draw.Group()
-    
+
     if debug:
-        r = draw.Rectangle(draw_x,draw_y,TILE_SIZE,TILE_SIZE,fill="red")
+        r = draw.Rectangle(draw_x, draw_y, TILE_SIZE, TILE_SIZE, fill="red")
         tile_group.children.append(r)
-        
-    
-    tile_center_x = draw_x+TILE_SIZE/2
-    tile_center_y = draw_y+TILE_SIZE/2
-    
-    a = [-1,1,1,-1]
-    b = [1,1,-1,-1]
-    c = [1,0,-1,0]
-    e = [0,-1,0,1]
-    
-    r = draw.Rectangle(draw_x,draw_y,TILE_SIZE,TILE_SIZE,fill=None,stroke="gray",stroke_width=1)
+
+    tile_center_x = draw_x + TILE_SIZE / 2
+    tile_center_y = draw_y + TILE_SIZE / 2
+
+    a = [-1, 1, 1, -1]
+    b = [1, 1, -1, -1]
+    c = [1, 0, -1, 0]
+    e = [0, -1, 0, 1]
+
+    r = draw.Rectangle(
+        draw_x, draw_y, TILE_SIZE, TILE_SIZE, fill=None, stroke="gray", stroke_width=1
+    )
     tile_group.children.append(r)
-    
-    
-    
-    
-    
+
     # glue colors
-    for side in range(0,4):
+    for side in range(0, 4):
         glue = tile[side]
         color = null_glue_color
         if glue is not None:
             color = color_wheel[glue]
-        p = draw.Path(stroke_width=1, stroke=None,
-              fill=color, fill_opacity=1, marker_end=None)
+        p = draw.Path(
+            stroke_width=1, stroke=None, fill=color, fill_opacity=1, marker_end=None
+        )
         p.M(tile_center_x, tile_center_y)
-        p.l(a[side]*(TILE_SIZE/2),b[side]*(TILE_SIZE/2)) 
-        p.l(c[side]*(TILE_SIZE),e[side]*(TILE_SIZE))
+        p.l(a[side] * (TILE_SIZE / 2), b[side] * (TILE_SIZE / 2))
+        p.l(c[side] * (TILE_SIZE), e[side] * (TILE_SIZE))
         p.Z()
         tile_group.children.append(p)
-        
-    p = draw.Path(stroke_width=0.4, stroke="gray",
-              fill=None, fill_opacity=0, marker_end=None)
+
+    p = draw.Path(
+        stroke_width=0.4, stroke="gray", fill=None, fill_opacity=0, marker_end=None
+    )
     p.M(draw_x, draw_y)
-    p.l(TILE_SIZE,TILE_SIZE) 
+    p.l(TILE_SIZE, TILE_SIZE)
     tile_group.children.append(p)
-    
-    p = draw.Path(stroke_width=0.4, stroke="gray",
-              fill=None, fill_opacity=0, marker_end=None)
-    p.M(draw_x+TILE_SIZE, draw_y)
-    p.l(-1*TILE_SIZE,TILE_SIZE) 
+
+    p = draw.Path(
+        stroke_width=0.4, stroke="gray", fill=None, fill_opacity=0, marker_end=None
+    )
+    p.M(draw_x + TILE_SIZE, draw_y)
+    p.l(-1 * TILE_SIZE, TILE_SIZE)
     tile_group.children.append(p)
-    
+
     # glue names
-    for side in range(0,4):
+    for side in range(0, 4):
         glue = tile[side]
         if glue is not None:
-            tile_group.children.append(draw.Text(str(glue), 8, 
-                           tile_center_x+(a[side]+c[side])*(TILE_SIZE/2)+3.7*e[side], 
-                           tile_center_y+(b[side]+e[side])*(TILE_SIZE)/2-4.2*c[side], 
-                           fill='black',text_anchor="middle",valign='middle', font_family="Arimo"))
-    
+            tile_group.children.append(
+                draw.Text(
+                    str(glue),
+                    8,
+                    tile_center_x
+                    + (a[side] + c[side]) * (TILE_SIZE / 2)
+                    + 3.7 * e[side],
+                    tile_center_y
+                    + (b[side] + e[side]) * (TILE_SIZE) / 2
+                    - 4.2 * c[side],
+                    fill="black",
+                    text_anchor="middle",
+                    valign="middle",
+                    font_family="Arimo",
+                )
+            )
+
     # tile name (if any)
     if tile in tileset:
         tweak_offset_y = 0.5
         # HACK UGLY
         tile_name = str(tileset.index(tile))
-        if tile_name == '6':
-            tile_name = 'R'
-        if tile_name == '7':
-            tile_name = 'S'
-        tile_group.children.append(draw.Text(str(tile_name), 16, 
-                           tile_center_x, tile_center_y+tweak_offset_y, fill='black',
-                           text_anchor="middle",valign='middle',font_weight="bold",font_family="Arimo")) 
-        
+        if tile_name == "6":
+            tile_name = "R"
+        if tile_name == "7":
+            tile_name = "S"
+        tile_group.children.append(
+            draw.Text(
+                str(tile_name),
+                16,
+                tile_center_x,
+                tile_center_y + tweak_offset_y,
+                fill="black",
+                text_anchor="middle",
+                valign="middle",
+                font_weight="bold",
+                font_family="Arimo",
+            )
+        )
 
-        
     d.append(tile_group)
 
-def draw_tiling(tiling: Tiling, debug=False, filter_pos=lambda x,y: True):
+
+def draw_tiling(tiling: Tiling, debug=False, filter_pos=lambda x, y: True):
     world_w, world_h = tiling.get_world_boundaries()
-    
-    draw_w, draw_h = TILE_SIZE*(world_w+1), TILE_SIZE*(world_h+1)
-    
-    d = draw.Drawing(draw_w, draw_h, origin=(0,0), displayInline=False)
+
+    draw_w, draw_h = TILE_SIZE * (world_w + 1), TILE_SIZE * (world_h + 1)
+
+    d = draw.Drawing(draw_w, draw_h, origin=(0, 0), displayInline=False)
     if debug:
-        r = draw.Rectangle(0,0,draw_w,draw_h,fill="blue")
+        r = draw.Rectangle(0, 0, draw_w, draw_h, fill="blue")
         d.append(r)
-    for x,y in tiling.tiling.keys():
-        if filter_pos(x,y):
-            draw_tile(d,x,y,tiling[x,y],tiling.tileset,debug)
+    for x, y in tiling.tiling.keys():
+        if filter_pos(x, y):
+            draw_tile(d, x, y, tiling[x, y], tiling.tileset, debug)
     if debug:
-        r = draw.Rectangle(0,0,TILE_SIZE,TILE_SIZE,fill="lime",fill_opacity=0.6)
+        r = draw.Rectangle(0, 0, TILE_SIZE, TILE_SIZE, fill="lime", fill_opacity=0.6)
         d.append(r)
-    return d
+    return d
```

### Comparing `coreli-0.0.5/coreli/utils.py` & `coreli-0.0.6/coreli/utils.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.5/coreli.egg-info/PKG-INFO` & `coreli-0.0.6/coreli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: coreli
-Version: 0.0.5
+Version: 0.0.6
 Summary: The Collatz Research Library provides tools for experimenting and testing hypothesises related to the Collatz Process.
 Home-page: https://github.com/tcosmo/coreli
 Author: Tristan Stérin
 Author-email: tristan.sterin@mu.ie
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,14 +28,21 @@
 
 The appararent simplicity of this problem hides a very difficult mathematical problem. Actually, we believe that this problem has a lot to do with **Computer Science**. That's why we created **Coreli**, a library for experimenting and testing hypothesises regarding the Collatz process.      
 
 # Doc
 
 Coreli's doc is [hosted here](https://dna.hamilton.ie/tsterin/coreli/docs/).
 
+## Dev: deploy to pypi
+
+```
+python setup.py sdist
+twine upload dist/*
+```
+
 # References
 
 - David Applegate and Jeffrey Lagarias. Density bounds for the 3x + 1 problem. ii. krasikov
 inequalities. Mathematics of Computation - Math. Comput., 64:427–438, 01 1995. doi:
 10.2307/2153346.          
 
 - Jean Berstel, Jr. and Christophe Reutenauer. Rational Series and Their Languages. Springer-
@@ -81,7 +90,8 @@
 - Riho Terras. A stopping time problem on the positive integers. Acta Arithmetica, 30(3):241–252, 1976. URL: http://eudml.org/doc/205476.            
 
 - Günther Wirsching. On the combinatorial structure of 3n + 1 predecessor sets. Discrete Math-
 ematics, 148(1-3):265–286, January 1996. URL: https://doi.org/10.1016/0012-365x(94)00243-c, doi:10.1016/0012-365x(94)00243-c.                 
 
 - Günther J. Wirsching. The dynamical system generated by the 3n + 1 function. Springer,
 Berlin New York, 1998.
+
```

### Comparing `coreli-0.0.5/setup.py` & `coreli-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="coreli",
-    version="0.0.5",
+    version="0.0.6",
     author="Tristan Stérin",
     author_email="tristan.sterin@mu.ie",
     description="The Collatz Research Library provides tools for experimenting and testing hypothesises related to the Collatz Process.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tcosmo/coreli",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
-    install_requires=[
-          'sympy==1.11.1',
-          'drawsvg==1.8.3',
-          'ipywidgets==8.0.2'
-      ],
+    python_requires=">=3.6",
+    install_requires=["sympy==1.11.1", "drawsvg==1.8.3", "ipywidgets==8.0.2"],
 )
```

