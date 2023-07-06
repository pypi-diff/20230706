# Comparing `tmp/bihc-0.0.8.2.tar.gz` & `tmp/bihc-0.0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-d8il9hxr/bihc-0.0.8.2.tar", last modified: Thu Jun 15 15:42:59 2023, max compression
+gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-mm5q8qib/bihc-0.0.8.3.tar", last modified: Thu Jul  6 08:40:33 2023, max compression
```

## Comparing `bihc-0.0.8.2.tar` & `bihc-0.0.8.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.8.2/LICENSE
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.8.2/MANIFEST.in
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-06-15 15:42:59.000000 bihc-0.0.8.2/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.8.2/README.md
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.8.2/bihc/__init__.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    28370 2023-05-31 15:03:32.000000 bihc-0.0.8.2/bihc/beam.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        0 2023-06-02 14:25:40.000000 bihc-0.0.8.2/bihc/fillingschemes.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6330 2023-05-19 11:33:18.000000 bihc-0.0.8.2/bihc/impedance.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9085 2023-05-31 14:26:46.000000 bihc-0.0.8.2/bihc/plot.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     7267 2023-06-15 15:39:26.000000 bihc-0.0.8.2/bihc/power.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      357 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/SOURCES.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/dependency_links.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/requires.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/top_level.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.8.2/pyproject.toml
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-06-15 15:42:59.000000 bihc-0.0.8.2/setup.cfg
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1082 2023-06-15 15:39:56.000000 bihc-0.0.8.2/setup.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/tests/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.8.2/tests/test_analyticBunchShapes.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.8.2/tests/test_numericBunchShapes.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-07-06 08:40:33.000000 bihc-0.0.8.3/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.8.3/LICENSE
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.8.3/MANIFEST.in
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-07-06 08:40:33.000000 bihc-0.0.8.3/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.8.3/README.md
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-07-06 08:40:33.000000 bihc-0.0.8.3/bihc/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.8.3/bihc/__init__.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    28370 2023-07-06 08:28:55.000000 bihc-0.0.8.3/bihc/beam.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        0 2023-06-02 14:25:40.000000 bihc-0.0.8.3/bihc/fillingschemes.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6606 2023-06-29 14:12:43.000000 bihc-0.0.8.3/bihc/impedance.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9085 2023-05-31 14:26:46.000000 bihc-0.0.8.3/bihc/plot.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     7365 2023-06-29 12:21:54.000000 bihc-0.0.8.3/bihc/power.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-07-06 08:40:33.000000 bihc-0.0.8.3/bihc.egg-info/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-07-06 08:40:33.000000 bihc-0.0.8.3/bihc.egg-info/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      357 2023-07-06 08:40:33.000000 bihc-0.0.8.3/bihc.egg-info/SOURCES.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-07-06 08:40:33.000000 bihc-0.0.8.3/bihc.egg-info/dependency_links.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-07-06 08:40:33.000000 bihc-0.0.8.3/bihc.egg-info/requires.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-07-06 08:40:33.000000 bihc-0.0.8.3/bihc.egg-info/top_level.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.8.3/pyproject.toml
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-07-06 08:40:33.000000 bihc-0.0.8.3/setup.cfg
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1082 2023-07-06 08:39:30.000000 bihc-0.0.8.3/setup.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-07-06 08:40:33.000000 bihc-0.0.8.3/tests/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.8.3/tests/test_analyticBunchShapes.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.8.3/tests/test_numericBunchShapes.py
```

### Comparing `bihc-0.0.8.2/LICENSE` & `bihc-0.0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.2/PKG-INFO` & `bihc-0.0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.8.2
+Version: 0.0.8.3
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.8.2/README.md` & `bihc-0.0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.2/bihc/beam.py` & `bihc-0.0.8.3/bihc/beam.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.2/bihc/impedance.py` & `bihc-0.0.8.3/bihc/impedance.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,27 @@
         self.Zr = np.zeros(len(f))
         self.Zi = np.zeros(len(f))
 
         self.isResonatorImpedance = False
         self.isRWImpedance = False
 
         if CST_file is not None:
-            self.getImpedanceFromCST(CST_file)          
+            self.getImpedanceFromCST(CST_file)     
+
+    def __add__(self, Zn):
+        Z = Impedance(self.f)
+
+        if not np.array_equal(Z.f, Zn.f):
+            Z.Zr = np.interp(Z.f, Zn.f, Zn.Zr)
+            Z.Zi = np.interp(Z.f, Zn.f, Zn.Zi)
+
+        Z.Zr = self.Zr + Zn.Zr 
+        Z.Zi = self.Zi + Zn.Zi    
+
+        return Z
         
     def getResonatorImpedance(self,Rs,Qr,fr,f=np.linspace(0.1,2e9,int(1e5))):
         """Creating the impedance curve from the broad-band resonator model.
 
         This methods creates an impedance curve using the broad-band resonator 
         model. It requires a shunt impedance value, a quality factor value, and
         the resonant frequency value.
```

### Comparing `bihc-0.0.8.2/bihc/plot.py` & `bihc-0.0.8.3/bihc/plot.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.2/bihc/power.py` & `bihc-0.0.8.3/bihc/power.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,25 +229,26 @@
             if offset1 is None:
                 offset1 = np.zeros_like(offset2)
 
             # Formula with beam offsets
             P = (2*f0*e*self.filledSlots*self.Np*S)**2
             P_loss = []
             P_density_list = []
-            for i, shift in enumerate(tau_s):
+            for i, shift in tqdm(enumerate(tau_s), "Computing 2-beam power with offset: "):
                 P_density = P*(Zreal_0+(offset1[i]+offset2[i])*Zreal_1)*(1-np.cos(2*np.pi*f*shift))
                 P_loss.append(np.sum(P_density))  
         else:
             # Simplified formula
             P = (2*f0*e*self.filledSlots*self.Np*S)**2
             P_loss = []
             P_density_list = []
-            for shift in tau_s:
+            for shift in tqdm(tau_s, "Computing 2-beam power: "):
                 P_density = P*Zreal_0*(1-np.cos(2*np.pi*f*shift))
     #           P_density_list.append(P_density)
                 P_loss.append(np.sum(P_density))  
 
         if self.verbose:
-            print(f'Computed Power loss: {P_loss} W') 
+            pass
+            #print(f'Computed Power loss: {P_loss} W') 
 
         self.P_loss = P_loss
         return P_loss
```

### Comparing `bihc-0.0.8.2/bihc.egg-info/PKG-INFO` & `bihc-0.0.8.3/bihc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.8.2
+Version: 0.0.8.3
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.8.2/setup.py` & `bihc-0.0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.8.2",
+    version="0.0.8.3",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.8.2/tests/test_analyticBunchShapes.py` & `bihc-0.0.8.3/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.2/tests/test_numericBunchShapes.py` & `bihc-0.0.8.3/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

