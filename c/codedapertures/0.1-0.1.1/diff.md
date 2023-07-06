# Comparing `tmp/codedapertures-0.1.tar.gz` & `tmp/codedapertures-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.1.tar", last modified: Tue Aug  9 02:43:40 2022, max compression
+gzip compressed data, was "codedapertures-0.1.1.tar", last modified: Thu Jul  6 00:49:31 2023, max compression
```

## Comparing `codedapertures-0.1.tar` & `codedapertures-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2022-08-09 02:43:40.596041 codedapertures-0.1/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2022-01-15 01:57:00.000000 codedapertures-0.1/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      229 2022-08-09 02:43:40.595871 codedapertures-0.1/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      974 2022-08-09 01:27:15.000000 codedapertures-0.1/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2022-08-09 02:43:40.594121 codedapertures-0.1/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2022-08-09 01:58:53.000000 codedapertures-0.1/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)     7644 2022-03-18 00:17:48.000000 codedapertures-0.1/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2022-08-09 02:43:40.595553 codedapertures-0.1/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      229 2022-08-09 02:43:40.000000 codedapertures-0.1/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2022-08-09 02:43:40.000000 codedapertures-0.1/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2022-08-09 02:43:40.000000 codedapertures-0.1/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2022-08-09 02:41:01.000000 codedapertures-0.1/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       26 2022-08-09 02:43:40.000000 codedapertures-0.1/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2022-08-09 02:43:40.000000 codedapertures-0.1/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2022-08-09 02:43:40.596146 codedapertures-0.1/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      400 2022-08-09 02:43:01.000000 codedapertures-0.1/setup.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-06 00:49:31.868273 codedapertures-0.1.1/
+-rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.1.1/LICENSE
+-rw-r--r--   0 bbudden    (501) staff       (20)      247 2023-07-06 00:49:31.868158 codedapertures-0.1.1/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)     1359 2023-07-06 00:28:10.000000 codedapertures-0.1.1/README.md
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-06 00:49:31.867342 codedapertures-0.1.1/codedapertures/
+-rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.1.1/codedapertures/__init__.py
+-rw-r--r--   0 bbudden    (501) staff       (20)     8038 2023-07-06 00:25:54.000000 codedapertures-0.1.1/codedapertures/codedapertures.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-06 00:49:31.868020 codedapertures-0.1.1/codedapertures.egg-info/
+-rw-r--r--   0 bbudden    (501) staff       (20)      247 2023-07-06 00:49:31.000000 codedapertures-0.1.1/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-06 00:49:31.000000 codedapertures-0.1.1/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:49:31.000000 codedapertures-0.1.1/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.1.1/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-06 00:49:31.000000 codedapertures-0.1.1/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-06 00:49:31.000000 codedapertures-0.1.1/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-06 00:49:31.868303 codedapertures-0.1.1/setup.cfg
+-rw-r--r--   0 bbudden    (501) staff       (20)      418 2023-07-06 00:43:35.000000 codedapertures-0.1.1/setup.py
```

### Comparing `codedapertures-0.1/LICENSE` & `codedapertures-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.1/codedapertures/codedapertures.py` & `codedapertures-0.1.1/codedapertures/codedapertures.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 
     Holds one of several types of coded aperture patterns.
     """
 
     def __init__(self):
         self.A_ij = None
     
-    def show(self, inverse=False):
+    def show(self, inverse=False, size=8):
         """
         Plots the mask to the screen
 
         Parameters
         ----------
         inverse : bool
             if True, will invert the array before plotting
+        size : int
+            size of the plot (default 8)
         """
-        plt.rcParams['figure.figsize'] = [8,8]
+        plt.rcParams['figure.figsize'] = [size,size]
         cmap = "binary_r" if inverse else "binary"
         plt.imshow(self.A_ij, cmap=cmap, aspect=1)
         plt.axis('off')
         plt.show()
 
     def get_pattern(self, inverse=False):
         """
@@ -69,32 +71,75 @@
         """
         
         new_width  = self.width  + width*2
         new_height = self.height + width*2
         new_mask   = np.zeros((new_width, new_height))
         if not empty: new_mask = new_mask +1
         new_mask[width:-width,width:-width] = self.A_ij
-        self.A_ij = new_mask
+        self.A_ij  = new_mask
 
+class rand_array(mask):
+    """
+    Random Array
+
+    Parameters
+    ----------
+    x : int
+        number of 'x' elements in the array
+    y : int
+        number of 'y' elements in the array
+    fill : float
+        fill factor fraction
+    quiet : bool
+        if True, will print mask info upon creation
+    """
+    
+    def __init__(self, x=10, y=10, fill=0.5, quiet=False):
+        self.r = x
+        self.s = y
+        self.fill = fill
+        
+        # randomly fill
+        A_ij = np.zeros([self.r, self.s])
+        for i in range(self.r):
+            for j in range(self.s):
+                if random.random() < self.fill:
+                    A_ij[i,j] = 1
+        self.A_ij = A_ij
+        self.actual_fill = np.sum(A_ij)/(self.r*self.s)
+        
+        # get width/height
+        self.width = self.A_ij.shape[0]
+        self.height = self.A_ij.shape[1]
+
+        if not quiet: self.report()
+        
+    def report(self):
+        """
+        Report on the mask information
+        """
+        print("Random Array")
+        print("x, y: %i, %i" % (self.r, self.s))
+        print("desired fill factor: %.2f" % self.fill)
+        print("actuall fill factor: %.2f" % self.actual_fill)
             
 class ura(mask):
     """
     Uniformly Redundant Array
 
     Parameters
     ----------
     rank : int
-        the rank of prime pairs to use
+        the rank of prime pairs to use (0 -> (5,3) 1 -> (13,11) etc.)
     mult : int
         the number of times to tile the pattern in both dimensions
     quiet : bool
         if True, will print information about the array upon creation
     """
 
-    
     def __init__(self, rank=4, mult=2, quiet=False):
         self.rank = rank
         self.mult = mult
         
         # get r, s
         r, s = self.__get_prime_pairs(self.rank)
         self.r = r
@@ -146,16 +191,19 @@
     def __get_prime_pairs(self, rank):
         """
         Determine prime pairs at specified rank
 
         Parmeters
         ---------
         rank : int
-            the rank of prime pairs to determine
+            the rank of prime pairs to determine (0 -> 5, 1 -> 13, etc.)
         """
+
+        assert rank >= 0, f"rank must be great than or equal to zero, got {rank}"
+
         pit = pyprimes.primes()
 
         # intialize
         p1 = next(pit)
         this_rank = -1
 
         # find primes
@@ -166,59 +214,14 @@
             else:
                 p1 = p2
             if this_rank == rank:
                 break
 
         return p1, p2
         
-class rand_array(mask):
-    """
-    Class to hold a randomly generate array
-
-    Parameters
-    ----------
-    r : int
-        number of 'x' elements in the array
-    s : int
-        number of 'y' elements in the array
-    fill : float
-        fill factor fraction
-    quiet : bool
-        if True, will print mask info upon creation
-    """
-    
-    def __init__(self, r=10, s=10, fill=0.5, quiet=False):
-        self.r = r
-        self.s = s
-        self.fill = fill
-        
-        # randomly fill
-        A_ij = np.zeros([r, s])
-        for i in range(r):
-            for j in range(s):
-                if random.random() < self.fill:
-                    A_ij[i,j] = 1
-        self.A_ij = A_ij
-        self.actual_fill = np.sum(A_ij)/(self.r*self.s)
-        
-        # get width/height
-        self.width = self.A_ij.shape[0]
-        self.height = self.A_ij.shape[1]
-
-        if not quiet: self.report()
-        
-    def report(self):
-        """
-        Report on the mask information
-        """
-        print("Random Array")
-        print("r, s: %i, %i" % (self.r, self.s))
-        print("desired fill factor: %.2f" % self.fill)
-        print("actuall fill factor: %.2f" % self.actual_fill)
-        
 class mura(mask):
     """
     Modified Uniformly Redundant Array
     """
     
     def __init__(self, rank=5, quiet=False, mult=2):
         self.rank = rank
@@ -269,15 +272,23 @@
         """
         print("Modified Uniformly Redundant Array")
         print("L: %i (rank %i)" % (self.L, self.rank))
         
     def __get_prime(self, rank):
         """
         Determine prime of specified rank
+
+        arameters
+        ----------
+        rank : int
+            the rank of prime pairs (0 -> 5, 1 -> 13, etc.)
         """
+
+        assert rank >= 0, f"rank must be great than or equal to zero, got {rank}"
+
         m = 1
         this_rank = -1
         while True:
             L = 4*m + 1
             if pyprimes.isprime(L):
                 this_rank += 1
             if this_rank == rank:
```

