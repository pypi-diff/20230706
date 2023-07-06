# Comparing `tmp/CRYSTALpytools-2023.6.7.tar.gz` & `tmp/CRYSTALpytools-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CRYSTALpytools-2023.6.7.tar", last modified: Tue Jun  6 15:12:36 2023, max compression
+gzip compressed data, was "CRYSTALpytools-2023.7.6.tar", last modified: Thu Jul  6 11:04:33 2023, max compression
```

## Comparing `CRYSTALpytools-2023.6.7.tar` & `CRYSTALpytools-2023.7.6.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.795747 CRYSTALpytools-2023.6.7/
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.791361 CRYSTALpytools-2023.6.7/CRYSTALpytools/
--rw-r--r--   0 brunocamino   (501) staff       (20)      467 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/__init__.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      577 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/adsorb.py
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.795317 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/
--rw-r--r--   0 brunocamino   (501) staff       (20)      122 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/__init__.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    11964 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/basisset.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    47067 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/crysd12.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     9266 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/base/inputbase.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      757 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/calculate.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    16727 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/convert.py
--rw-r--r--   0 brunocamino   (501) staff       (20)   103231 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/crystal_io.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     3613 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/execute.py
--rw-r--r--   0 brunocamino   (501) staff       (20)   121442 2023-04-25 17:05:03.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/plot.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    73581 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/thermodynamics.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    12902 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/unit_test.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      974 2023-02-10 08:58:41.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/units.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      693 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools/utils.py
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-06-06 15:12:36.793259 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/
--rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/PKG-INFO
--rw-r--r--   0 brunocamino   (501) staff       (20)      655 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/SOURCES.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)        1 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/dependency_links.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)       23 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/requires.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)       15 2023-06-06 15:12:36.000000 CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/top_level.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)     1167 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.6.7/LICENSE.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-06-06 15:12:36.795615 CRYSTALpytools-2023.6.7/PKG-INFO
--rw-r--r--   0 brunocamino   (501) staff       (20)     3925 2023-06-06 14:55:03.000000 CRYSTALpytools-2023.6.7/README.md
--rw-r--r--   0 brunocamino   (501) staff       (20)      105 2022-12-21 17:23:54.000000 CRYSTALpytools-2023.6.7/pyproject.toml
--rw-r--r--   0 brunocamino   (501) staff       (20)       38 2023-06-06 15:12:36.795790 CRYSTALpytools-2023.6.7/setup.cfg
--rw-r--r--   0 brunocamino   (501) staff       (20)     1043 2023-06-06 15:12:25.000000 CRYSTALpytools-2023.6.7/setup.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.185194 CRYSTALpytools-2023.7.6/
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.178927 CRYSTALpytools-2023.7.6/CRYSTALpytools/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      520 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/__init__.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1052 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/adsorb.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.184692 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      203 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/__init__.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    11964 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/basisset.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    50980 2023-07-06 11:02:41.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/crysd12.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     7467 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/crysout.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     9265 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/inputbase.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    14464 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/propout.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1233 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/calculate.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    16954 2023-06-28 15:28:44.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/convert.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   102312 2023-07-06 11:02:41.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/crystal_io.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     4426 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/execute.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   162807 2023-07-06 11:02:41.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/plot.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   122869 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/thermodynamics.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    12902 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/unit_test.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1259 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/units.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      693 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/utils.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.181538 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)      717 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)        1 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)      138 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/requires.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)       15 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/top_level.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1167 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.7.6/LICENSE.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-07-06 11:04:33.184981 CRYSTALpytools-2023.7.6/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)     4207 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/README.md
+-rw-r--r--   0 brunocamino   (501) staff       (20)      105 2022-12-21 17:23:54.000000 CRYSTALpytools-2023.7.6/pyproject.toml
+-rw-r--r--   0 brunocamino   (501) staff       (20)       38 2023-07-06 11:04:33.185239 CRYSTALpytools-2023.7.6/setup.cfg
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1190 2023-07-06 11:04:24.000000 CRYSTALpytools-2023.7.6/setup.py
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/base/basisset.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/basisset.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/base/crysd12.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/crysd12.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,15 @@
             geom_end = 1
             bs_end = 2
             end_counter = 0
             block_counter = 0
             subblock_key = ['OPTGEOM', 'FREQCALC',
                             'ANHARM', 'CPHF', 'CPKS', 'ELASTCON', 'EOS']
             for d in data_lines:
+                d = d.strip()
                 text[block_counter] += d + '\n'
                 if d in subblock_key:
                     geom_end += 1
                     bs_end += 1
                 elif 'END' in d:
                     end_counter += 1
 
@@ -147,25 +148,29 @@
                     block_counter += 1
         # Case 2: BASISSET keyword
         else:
             self.basisset._block_ed = None
             self.geom._block_ed = None
             block_counter = 0
             for d in data_lines:
+                d = d.strip()
                 if d == 'BASISSET':
                     block_counter += 1
                     text[block_counter] += d + '\n'
                 elif d in self.scf._block_key and block_counter == 1:  # Avoid same keywords. e.g. TOLDEE
                     block_counter += 1
                     text[block_counter] += d + '\n'
                 else:
                     text[block_counter] += d + '\n'
 
         # Title line
         self.geom.title(data_lines[0])
+        # The 0D geometry keyword 'MOLECULE' and the molecular crystal option 'MOLECULE'
+        if 'MOLECULE' not in data_lines[1] and 'MOLECULE' in text[0]:
+            text[0] = re.sub('MOLECULE', 'MOLEISO', text[0])
 
         self.geom.analyze_text(text[0])
         if 'BASISSET' not in data:
             self.basisset.from_string(text[1])
         else:
             self.basisset.analyze_text(text[1])
         self.scf.analyze_text(text[2])
@@ -202,26 +207,49 @@
             'EXTERNAL'  : '_basegeom',
             'DLVINPUT'  : '_basegeom',
             'SUPERCEL'  : '_sp_matrix',
             'SUPERCELL' : '_sp_matrix',
             'SUPERCON'  : '_sp_matrix',
             'SCELCONF'  : '_sp_matrix',
             'SCELPHONO' : '_sp_matrix',
+            'ATOMBSSE'  : '_atombsse',
+            'ATOMDISP'  : '_atomdisp',
+            'ATOMINSE'  : '_atominse',
+            'ATOMORDE'  : '_atomorde',
+            'ATOMREMO'  : '_atomremo',
+            'MOLEISO'   : '_moleiso', # The original 'MOLECULE' option to isolate molecules
             'EXTPRT'    : '_extprt',
             'CIFPRT'    : '_cifprt',
             'CIFPRTSYM' : '_cifprtsym',
             'TESTGEOM'  : '_testgeom',
             'OPTGEOM'   : 'optgeom',  # Sub-block properties must be named without the initial underscore
             'FREQCALC'  : 'freqcalc',
         }
         key = list(self._block_dict.keys())
         attr = list(self._block_dict.values())
         self._block_key = sorted(set(key), key=key.index)
         self._block_attr = sorted(set(attr), key=attr.index)
 
+    @property
+    def data(self):
+        """
+        Settings in all the attributes are summarized here. Covers the data
+        property in BlockBASE, to address the ambiguity of 'MOLECULE' keywords.
+        """
+        import re
+
+        self.update_block()
+        text = ''
+        for i in [self._block_bg, self._block_data, self._block_ed]:
+            if i == None:
+                continue
+            text += i
+
+        return re.sub('MOLEISO', 'MOLECULE', text)
+
     def title(self, title='Generated by CRYSTALpytools'):
         self._block_bg = '{}\n'.format(title)
 
     def crystal(self, IGR=None, latt=[], atom=[], IFLAG=0, IFHR=0, IFSO=0, origin=[]):
         """
         Define 'CRYSTAL' structure
 
@@ -235,16 +263,15 @@
             IFSO (int): See the manual
             origin (list): *IFSO > 1* See the manual
         """
         if IGR == None:  # No entry. Return keyword
             self._basegeom = super(Geom, self).assign_keyword('CRYSTAL', [])
             return
         elif IGR == '':  # Clean data
-            self._basegeom = super(
-                Geom, self).assign_keyword('CRYSTAL', [], '')
+            self._basegeom = super(Geom, self).assign_keyword('CRYSTAL', [], '')
             return
 
         if IFSO <= 1:
             shape = [3, 1]
             value = [int(IFLAG), int(IFHR), IFSO, int(IGR)]
         else:
             shape = [3, 3, 1]
@@ -254,16 +281,15 @@
         shape += [len(latt), ]
         value += [i for i in latt]
 
         atominput = super(Geom, self).set_list(len(atom), atom)
         shape += atominput[0]
         value += atominput[1]
 
-        self._basegeom = super(Geom, self).assign_keyword(
-            'CRYSTAL', shape, value)
+        self._basegeom = super(Geom, self).assign_keyword('CRYSTAL', shape, value)
 
     def slab(self, IGR=None, latt=[], atom=[]):
         """
         Define 'SLAB' structure
         """
         if IGR == None:  # No entry. Return keyword
             self._basegeom = super(Geom, self).assign_keyword('SLAB', [])
@@ -288,30 +314,28 @@
         """
         Define 'POLYMER' structure
         """
         if IGR == None:  # No entry. Return keyword
             self._basegeom = super(Geom, self).assign_keyword('POLYMER', [])
             return
         elif IGR == '':  # Clean data
-            self._basegeom = super(
-                Geom, self).assign_keyword('POLYMER', [], '')
+            self._basegeom = super(Geom, self).assign_keyword('POLYMER', [], '')
             return
 
         shape = [1, ]
         value = [int(IGR), ]
 
         shape += [len(latt), ]
         value += [i for i in latt]
 
         atominput = super(Geom, self).set_list(len(atom), atom)
         shape += atominput[0]
         value += atominput[1]
 
-        self._basegeom = super(Geom, self).assign_keyword(
-            'POLYMER', shape, value)
+        self._basegeom = super(Geom, self).assign_keyword('POLYMER', shape, value)
 
     def helix(self, N1=None, N2=0, latt=[], atom=[]):
         """
         Define 'HELIX' structure
 
         Args:
             N1 (int): See the manual
@@ -330,38 +354,41 @@
         shape += [len(latt), ]
         value += [i for i in latt]
 
         atominput = super(Geom, self).set_list(len(atom), atom)
         shape += atominput[0]
         value += atominput[1]
 
-        self._basegeom = super(Geom, self).assign_keyword(
-            'HELIX', shape, value)
+        self._basegeom = super(Geom, self).assign_keyword('HELIX', shape, value)
 
     def molecule(self, IGR=None, atom=[]):
         """
         Define 'MOLECULE' structure
         """
+        import warnings
+
+        # The 0D geometry keyword 'MOLECULE' and the molecular crystal option 'MOLECULE'
+        if hasattr(self, '_basegeom'):
+            warnings.warn("Geometry definition exists. To launch the MOLECULE option that isolates molecules from lattice, use the 'self.moleiso' method.", stacklevel=2)
+
         if IGR == None:  # No entry. Return keyword
             self._basegeom = super(Geom, self).assign_keyword('MOLECULE', [])
             return
         elif IGR == '':  # Clean data
-            self._basegeom = super(
-                Geom, self).assign_keyword('MOLECULE', [], '')
+            self._basegeom = super(Geom, self).assign_keyword('MOLECULE', [], '')
             return
 
         shape = [1, ]
         value = [int(IGR), ]
 
         atominput = super(Geom, self).set_list(len(atom), atom)
         shape += atominput[0]
         value += atominput[1]
 
-        self._basegeom = super(Geom, self).assign_keyword(
-            'MOLECULE', shape, value)
+        self._basegeom = super(Geom, self).assign_keyword('MOLECULE', shape, value)
 
     def external(self, key='EXTERNAL'):
         """
         Define 'EXTERNAL' structure
         """
         self._basegeom = super(Geom, self).assign_keyword(key, [])
 
@@ -375,40 +402,90 @@
         """
         Supercell by 'SUPERCEL' keyword
 
         Args:
             mx (array | list | str): ndimen \* ndimen matrix, [] or ''
         """
         shape, value = super(Geom, self).set_matrix(mx)
-        self._sp_matrix = super(Geom, self).assign_keyword(
-            'SUPERCEL', shape, value)
+        self._sp_matrix = super(Geom, self).assign_keyword('SUPERCEL', shape, value)
 
     def supercon(self, mx=None):
         """
         Supercell by 'SUPERCON' keyword
         """
         shape, value = super(Geom, self).set_matrix(mx)
-        self._sp_matrix = super(Geom, self).assign_keyword(
-            'SUPERCON', shape, value)
+        self._sp_matrix = super(Geom, self).assign_keyword('SUPERCON', shape, value)
 
     def scelconf(self, mx=None):
         """
         Supercell by 'SCELCONF' keyword
         """
         shape, value = super(Geom, self).set_matrix(mx)
-        self._sp_matrix = super(Geom, self).assign_keyword(
-            'SCELCONF', shape, value)
+        self._sp_matrix = super(Geom, self).assign_keyword('SCELCONF', shape, value)
 
     def scelphono(self, mx=None):
         """
         Supercell by 'SCELPHONO' keyword
         """
         shape, args = super(Geom, self).set_matrix(mx)
-        self._sp_matrix = super(Geom, self).assign_keyword(
-            'SCELPHONO', shape, value)
+        self._sp_matrix = super(Geom, self).assign_keyword('SCELPHONO', shape, value)
+
+    def atombsse(self, IAT=None, NSTAR=None, RMAX=None):
+        self._atombsse = super(Geom, self).assign_keyword('ATOMBSSE', [3, ], [IAT, NSTAR, RMAX])
+
+    def atomdisp(self, NDISP=None, atom=[]):
+        """
+        ATOMDISP keyword
+
+        Args:
+            NDISP (int): See manual
+            atom (list): NDISP\*4 list. Including LB, DX, DY, DZ
+        """
+        shape, value = super(Geom, self).set_list(NDISP, atom)
+        self._atomdisp = super(Geom, self).assign_keyword('ATOMDISP', shape, value)
+
+    def atominse(self, NINS=None, atom=[]):
+        """
+        ATOMINSE keyword
+
+        Args:
+            NINS (int): See manual
+            atom (list): NINS\*4 list. Including NA, X, Y, Z
+        """
+        shape, value = super(Geom, self).set_list(NINS, atom)
+        self._atominse = super(Geom, self).assign_keyword('ATOMINSE', shape, value)
+
+    def atomorde(self, key='ATOMORDE'):
+        self._atomorde = super(Geom, self).assign_keyword(key, [])
+
+    def atomremo(self, NL=None, atom=[]):
+        """
+        ATOMREMO keyword
+
+        Args:
+            NL (int): See manual
+            atom (list): NL\*1 list. Including LB
+        """
+        shape, value = super(Geom, self).set_list(NL, atom)
+        self._atomremo = super(Geom, self).assign_keyword('ATOMREMO', shape, value)
+
+    def moleiso(self, NMOL=None, atom=[]):
+        """
+        .. note::
+
+            Corresponds to the **option** MOLECULE to isolate molecules from
+            lattice. Only the method's name is changed to avoid ambiguity with
+            the one to set 0D geometry.
+
+        Args:
+            NMOL (int)
+            atom (list[list[int]]): NMOL\*4 list. See CRYSTAL manual.
+        """
+        shape, value = super(Geom, self).set_list(NMOL, atom)
+        self._moleiso = super(Geom, self).assign_keyword('MOLECULE', shape, value)
 
     def extprt(self, key='EXTPRT'):
         self._extprt = super(Geom, self).assign_keyword(key, [])
 
     def cifprt(self, key='CIFPRT'):
         self._cifprt = super(Geom, self).assign_keyword(key, [])
 
@@ -514,15 +591,22 @@
             'FRAGMENT'    : '_fragment',
             'RESTART'     : '_restart',
             'FINALRUN'    : '_finalrun',
             'EXTPRESS'    : '_extpress',
             'ALLOWTRUSTR' : '_usetrustr',
             'NOTRUSTR'    : '_usetrustr',
             'MAXTRADIUS'  : '_maxtradius',
-            'TRUSTRADIUS' : '_trustradius'
+            'TRUSTRADIUS' : '_trustradius',
+            'ONELOG'      : '_printonelog',
+            'NOXYZ'       : '_printxyz',
+            'NOSYMMOPS'   : '_printsymmops',
+            'PRINTFORCES' : '_printforces',
+            'PRINTHESS'   : '_printhess',
+            'PRINTOPT'    : '_printopt',
+            'PRINT'       : '_print',
         }
         key = list(self._block_dict.keys())
         attr = list(self._block_dict.values())
         self._block_key = sorted(set(key), key=key.index)
         self._block_attr = sorted(set(attr), key=attr.index)
 
     def fulloptg(self, key='FULLOPTG'):
@@ -558,65 +642,78 @@
     def toldex(self, TX=None):
         self._toldex = super(Optgeom, self).assign_keyword('TOLDEX', [1, ], TX)
 
     def toldee(self, IG=None):
         self._toldee = super(Optgeom, self).assign_keyword('TOLDEE', [1, ], IG)
 
     def maxcycle(self, MAX=None):
-        self._maxcycle = super(Optgeom, self).assign_keyword(
-            'MAXCYCLE', [1, ], MAX)
+        self._maxcycle = super(Optgeom, self).assign_keyword('MAXCYCLE', [1, ], MAX)
 
     def fragment(self, NL=None, LB=[]):
         """
         Args:
             NL (int | str): Number of atoms. See manual. Or ''
             LB (list[int]): Label of atoms. See manual
         """
         shape, value = super(Optgeom, self).set_list(NL, LB)
-        self._fragment = super(Optgeom, self).assign_keyword(
-            'FRAGMENT', shape, value)
+        self._fragment = super(Optgeom, self).assign_keyword('FRAGMENT', shape, value)
 
     def restart(self, key='RESTART'):
         self._restart = super(Optgeom, self).assign_keyword(key, [])
 
     def finalrun(self, ICODE=None):
-        self._finalrun = super(Optgeom, self).assign_keyword(
-            'FINALRUN', [1, ], ICODE)
+        self._finalrun = super(Optgeom, self).assign_keyword('FINALRUN', [1, ], ICODE)
 
     def extpress(self, pres=None):
-        self._extpress = super(Optgeom, self).assign_keyword(
-            'EXTPRESS', [1, ], pres)
+        self._extpress = super(Optgeom, self).assign_keyword('EXTPRESS', [1, ], pres)
 
     def allowtrustr(self, key='ALLOWTRUSTR'):
         self._usetrustr = super(Optgeom, self).assign_keyword(key, [])
 
     def notrustr(self, key='NOTRUSTR'):
         self._usetrustr = super(Optgeom, self).assign_keyword(key, [])
 
     def maxtradius(self, TRMAX=None):
         import warnings
 
         if hasattr(self, '_usetrustr'):
             if self._usetrustr == 'NOTRUSTR\n':
-                warnings.warn(
-                    "The pre-set 'NOTRUSTR' keyword will be removed.")
+                warnings.warn("The pre-set 'NOTRUSTR' keyword will be removed.", stacklevel=2)
                 self.notrustr('')
-        self._maxtradius = super(Optgeom, self).assign_keyword(
-            'MAXTRADIUS', [1, ], TRMAX)
+        self._maxtradius = super(Optgeom, self).assign_keyword('MAXTRADIUS', [1, ], TRMAX)
 
     def trustradius(self, TRADIUS=None):
         import warnings
 
         if hasattr(self, '_usetrustr'):
             if self._usetrustr == 'NOTRUSTR\n':
-                warnings.warn(
-                    "The pre-set 'NOTRUSTR' keyword will be removed.")
+                warnings.warn("The pre-set 'NOTRUSTR' keyword will be removed.", stacklevel=2)
                 self.notrustr('')
-        self._trustradius = super(Optgeom, self).assign_keyword(
-            'TRUSTRADIUS', [1, ], TRADIUS)
+        self._trustradius = super(Optgeom, self).assign_keyword('TRUSTRADIUS', [1, ], TRADIUS)
+
+    def onelog(self, key='ONELOG'):
+        self._printonelog = super(Optgeom, self).assign_keyword(key, [])
+
+    def noxyz(self, key='NOXYZ'):
+        self._printxyz = super(Optgeom, self).assign_keyword(key, [])
+
+    def nosymmops(self, key='NOSYMMOPS'):
+        self._printsymmops = super(Optgeom, self).assign_keyword(key, [])
+
+    def printforces(self, key='PRINTFORCES'):
+        self._printforces = super(Optgeom, self).assign_keyword(key, [])
+
+    def printhess(self, key='PRINTHESS'):
+        self._printhess = super(Optgeom, self).assign_keyword(key, [])
+
+    def printopt(self, key='PRINTOPT'):
+        self._printopt = super(Optgeom, self).assign_keyword(key, [])
+
+    def print(self, key='PRINT'):
+        self._print = super(Optgeom, self).assign_keyword(key, [])
 
 
 class Freqcalc(BlockBASE):
     """
     FREQCALC block object
     """
 
@@ -683,19 +780,18 @@
     def dispersion(self, key='DISPERSION'):
         self._dispersion = super(Freqcalc, self).assign_keyword(key, [])
 
     def bands(self, ISS=None, NSUB=None, NLINE=None, points=[]):
         if ISS == None:
             self._bands = super(Freqcalc, self).assign_keyword('BANDS', [])
         elif ISS == '':
-            self._bands = super(Freqcalc, self).assign_keyword('BANDS', [])
+            self._bands = super(Freqcalc, self).assign_keyword('', [])
         else:
             shape, value = super(Freqcalc, self).set_list(NLINE, points)
-            self._bands = super(Freqcalc, self).assign_keyword(
-                'BANDS', [2, ] + shape, [ISS, NSUB] + value)
+            self._bands = super(Freqcalc, self).assign_keyword('BANDS', [2, ] + shape, [ISS, NSUB] + value)
 
     def modes(self, key='MODES'):
         self._modes = super(Freqcalc, self).assign_keyword(key, [])
 
     def nomodes(self, key='NOMODES'):
         self._modes = super(Freqcalc, self).assign_keyword(key, [])
 
@@ -707,20 +803,18 @@
         self._pressure = super(Freqcalc, self).assign_keyword(
             'PRESSURE', [3, ], [NP, P1, P2])
 
     def restart(self, key='RESTART'):
         self._restart = super(Freqcalc, self).assign_keyword('RESTART', [])
 
     def stepsize(self, STEP=None):
-        self._stepsize = super(Freqcalc, self).assign_keyword(
-            'NUMDERIV', [1, ], STEP)
+        self._stepsize = super(Freqcalc, self).assign_keyword('NUMDERIV', [1, ], STEP)
 
     def temperat(self, NT=None, T1=None, T2=None):
-        self._temperat = super(Freqcalc, self).assign_keyword(
-            'TEMPERAT', [3, ], [NT, T1, T2])
+        self._temperat = super(Freqcalc, self).assign_keyword('TEMPERAT', [3, ], [NT, T1, T2])
 
 
 class BasisSet(BlockBASE):
     """
     Basis Set block object
     """
 
@@ -1074,58 +1168,52 @@
         #         self._block_fixgeom._block_bg = 'GEBA\n'
         #         self._block_fixgeom._block_ed = ''
         #         self._block_fixbase = obj2
         #         self._block_fixbase._block_bg = ''
         #         self._block_fixbase._block_ed = 'END\n'
 
         else:
-            raise ValueError(
-                'Keyword error. Allowed keywords: GEOM, BASE, GEBA.')
+            raise ValueError('Keyword error. Allowed keywords: GEOM, BASE, GEBA.')
 
     def biposize(self, ISIZE=None):
-        self._biposize = super(SCF, self).assign_keyword(
-            'BIPOSIZE', [1, ], ISIZE)
+        self._biposize = super(SCF, self).assign_keyword('BIPOSIZE', [1, ], ISIZE)
 
     def exchsize(self, ISIZE=None):
-        self._exchsize = super(SCF, self).assign_keyword(
-            'EXCHSIZE', [1, ], ISIZE)
+        self._exchsize = super(SCF, self).assign_keyword('EXCHSIZE', [1, ], ISIZE)
 
     def toldee(self, ITOL=None):
         self._toldee = super(SCF, self).assign_keyword('TOLDEE', [1, ], ITOL)
 
     def guessp(self, key='GUESSP'):
         self._guessp = super(SCF, self).assign_keyword(key, [])
 
     def atomspin(self, NA=None, LA=[]):
         shape, value = super(SCF, self).set_list(NA, LA)
-        self._atomspin = super(SCF, self).assign_keyword(
-            'ATOMSPIN', shape, value)
+        self._atomspin = super(SCF, self).assign_keyword('ATOMSPIN', shape, value)
 
     def tolinteg(self, ITOL1=None, ITOL2=None, ITOL3=None, ITOL4=None, ITOL5=None):
         self._tolinteg = super(SCF, self).assign_keyword(
-            'TOLINTEG', [5, ], [ITOL1, ITOL2, ITOL3, ITOL4, ITOL5])
+            'TOLINTEG', [5, ], [ITOL1, ITOL2, ITOL3, ITOL4, ITOL5]
+        )
 
     def ldremo(self, value):
         self._ldremo = super(SCF, self).assign_keyword('LDREMO', [1, ], value)
 
     def maxcycle(self, MAX=None):
-        self._maxcycle = super(SCF, self).assign_keyword(
-            'MAXCYCLE', [1, ], MAX)
+        self._maxcycle = super(SCF, self).assign_keyword('MAXCYCLE', [1, ], MAX)
 
     def fmixing(self, IPMIX=None):
-        self._maxcycle = super(SCF, self).assign_keyword(
-            'FMIXING', [1, ], IPMIX)
+        self._maxcycle = super(SCF, self).assign_keyword('FMIXING', [1, ], IPMIX)
 
     def shrink(self, IS=None, ISP=None, IS1=None, IS2=None, IS3=None):
         if IS1 == None:
-            self._shrink = super(SCF, self).assign_keyword(
-                'SHRINK', [2, ], [IS, ISP])
+            self._shrink = super(SCF, self).assign_keyword('SHRINK', [2, ], [IS, ISP])
         else:
-            self._shrink = super(SCF, self).assign_keyword(
-                'SHRINK', [2, 3], [IS, ISP, IS1, IS2, IS3])
+            self._shrink = super(SCF, self).assign_keyword('SHRINK', [2, 3],
+                                                           [IS, ISP, IS1, IS2, IS3])
 
     def gcpauto(self, key='GCPAUTO'):
         self._gcpauto = super(SCF, self).assign_keyword(key, [])
 
     def smear(self, WIDTH=None):
         self._smear = super(SCF, self).assign_keyword('SMEAR', [1, ], WIDTH)
 
@@ -1139,33 +1227,36 @@
         self._diis = super(SCF, self).assign_keyword(key, [])
 
     def diisallk(self, key='DIISALLK'):
         import warnings
 
         if hasattr(self, '_diis'):
             if 'NODIIS' in self._diis:
-                warnings.warn("Keyword 'NODIIS' is set. It will be removed.")
+                warnings.warn("Keyword 'NODIIS' is set. It will be removed.",
+                              stacklevel=2)
                 self._diis = ''
         self._diisallk = super(SCF, self).assign_keyword(key, [])
 
     def histdiis(self, NCYC=None):
         import warnings
 
         if hasattr(self, '_diis'):
             if 'NODIIS' in self._diis:
-                warnings.warn("Keyword 'NODIIS' is set. It will be removed.")
+                warnings.warn("Keyword 'NODIIS' is set. It will be removed.",
+                              stacklevel=2)
                 self._diis = ''
         self._histdiis = super(SCF, self).assign_keyword('HISTDIIS', [1,], NCYC)
 
     def prtdiis(self, key='PRTDIIS'):
         import warnings
 
         if hasattr(self, '_diis'):
             if 'NODIIS' in self._diis:
-                warnings.warn("Keyword 'NODIIS' is set. It will be removed.")
+                warnings.warn("Keyword 'NODIIS' is set. It will be removed.",
+                              stacklevel=2)
                 self._diis = ''
         self._prtdiis = super(SCF, self).assign_keyword(key, [])
 
 
 class DFT(BlockBASE):
     """
     DFT block object
@@ -1200,23 +1291,20 @@
         if hasattr(self, '_xcfunc'):
             raise AttributeError(
                 'Exchange-correlation functional is already set.')
         self._exchange = super(DFT, self).assign_keyword('EXCHANGE', [1, ], ex)
 
     def correlat(self, cor=None):
         if hasattr(self, '_xcfunc'):
-            raise AttributeError(
-                'Exchange-correlation functional is already set.')
-        self._correlat = super(DFT, self).assign_keyword(
-            'CORRELAT', [1, ], cor)
+            raise AttributeError('Exchange-correlation functional is already set.')
+        self._correlat = super(DFT, self).assign_keyword('CORRELAT', [1, ], cor)
 
     def xcfunc(self, xc=None):
         if hasattr(self, '_exchange') or hasattr(self, '_correlat'):
-            raise AttributeError(
-                'Separate keywords are set for exchange / correlation functionals.')
+            raise AttributeError('Separate keywords are set for exchange / correlation functionals.')
         self._xcfunc = super(DFT, self).assign_keyword(None, [1, ], xc)
 
     def lgrid(self, key='LGRID'):
         self._gridsz = super(DFT, self).assign_keyword(key, [])
 
     def oldgrid(self, key='OLDGRID'):
         self._gridsz = super(DFT, self).assign_keyword(key, [])
@@ -1228,31 +1316,27 @@
         self._gridsz = super(DFT, self).assign_keyword(key, [])
 
     def xxxlgrid(self, key='XXXLGRID'):
         self._gridsz = super(DFT, self).assign_keyword(key, [])
 
     def radial(self, NR=None, RL=[], IL=[]):
         if hasattr(self, '_gridsz'):
-            raise AttributeError(
-                "Pre-defined integrated grid '{}' is defined.".format(self._gridsz[:-1]))
+            raise AttributeError("Pre-defined integrated grid '{}' is defined.".format(self._gridsz[:-1]))
         if NR != None and NR != '':
             if len(RL) != len(IL) and NR != len(RL):
                 raise ValueError('Inconsistent definition of parameters.')
-        self._gridr = super(DFT, self).assign_keyword(
-            'RADIAL', [1, len(RL), len(IL)], [NR, ] + RL + IL)
+        self._gridr = super(DFT, self).assign_keyword('RADIAL', [1, len(RL), len(IL)], [NR, ] + RL + IL)
 
     def angular(self, NI=None, AL=[], LEV=[]):
         if hasattr(self, '_gridsz'):
-            raise AttributeError(
-                "Pre-defined integrated grid '{}' is defined.".format(self._gridsz[:-1]))
+            raise AttributeError("Pre-defined integrated grid '{}' is defined.".format(self._gridsz[:-1]))
         if NI != None and NI != '':
             if len(AL) != len(LEV) and NI != len(AL):
                 raise ValueError('Inconsistent definition of parameters.')
-        self._grida = super(DFT, self).assign_keyword(
-            'ANGULAR', [1, len(AL), len(LEV)], [NI, ] + AL + LEV)
+        self._grida = super(DFT, self).assign_keyword('ANGULAR', [1, len(AL), len(LEV)], [NI, ] + AL + LEV)
 
 
 class DFTD3(BlockBASE):
     """
     DFTD3 block object
     """
 
@@ -1277,16 +1361,15 @@
         }
         key = list(self._block_dict.keys())
         attr = list(self._block_dict.values())
         self._block_key = sorted(set(key), key=key.index)
         self._block_attr = sorted(set(attr), key=attr.index)
 
     def version(self, NAT=None):
-        self._version = super(DFTD3, self).assign_keyword(
-            'VERSION', [1, ], NAT)
+        self._version = super(DFTD3, self).assign_keyword('VERSION', [1, ], NAT)
 
     def func(self, CHAR=None):
         self._func = super(DFTD3, self).assign_keyword('FUNC', [1, ], CHAR)
 
     def abc(self, key='ABC'):
         self._abc = super(DFTD3, self).assign_keyword(key, [])
 
@@ -1305,24 +1388,21 @@
     def rs6(self, rs6=None):
         self._rs6 = super(DFTD3, self).assign_keyword('RS6', [1, ], rs6)
 
     def rs8(self, rs8=None):
         self._rs8 = super(DFTD3, self).assign_keyword('RS8', [1, ], rs8)
 
     def radius(self, radius=None):
-        self._radius = super(DFTD3, self).assign_keyword(
-            'RADIUS', [1, ], radius)
+        self._radius = super(DFTD3, self).assign_keyword('RADIUS', [1, ], radius)
 
     def cnradius(self, cnradius=None):
-        self._cnradius = super(DFTD3, self).assign_keyword(
-            'CNRADIUS', [1, ], cnradius)
+        self._cnradius = super(DFTD3, self).assign_keyword('CNRADIUS', [1, ], cnradius)
 
     def abcradius(self, abcradius=None):
-        self._abcradius = super(DFTD3, self).assign_keyword(
-            'ABCRADIUS', [1, ], abcradius)
+        self._abcradius = super(DFTD3, self).assign_keyword('ABCRADIUS', [1, ], abcradius)
 
     def printc6(self, key='PRINTC6'):
         self._printc6 = super(DFTD3, self).assign_keyword(key, [])
 
 
 class GCP(BlockBASE):
     """
@@ -1362,8 +1442,8 @@
     def eta(self, eta=None):
         self._eta = super(GCP, self).assign_keyword('ETA', [1, ], eta)
 
     def radius(self, radius=None):
         self._radius = super(GCP, self).assign_keyword('RADIUS', [1, ], radius)
 
     def printemiss(self, key='PRINTEMISS'):
-        self._printemiss = super(GCP, self).assign_keyword(key, [])
+        self._printemiss = super(GCP, self).assign_keyword(key, [])
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/base/inputbase.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/inputbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         """
         if args[0] == '':  # Clean data
             return [], ''
         elif args[0] == None:  # Keyword only
             return [], None
 
         if len(args) != 2 or int(args[0]) != len(args[1]):
-            return InputeError('Input format error. Arguments should be int + list')
+            return ValueError('Input format error. Arguments should be int + list')
 
         shape = [1, ]
         value = [int(args[0]), ]
 
         if type(args[1][0]) == list or type(args[1][0]) == tuple:  # 2D list (multi-rows)
             for i in args[1]:
                 shape += [len(i), ]
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/convert.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/convert.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,37 +6,41 @@
 
 def cry_ase2gui(structure, pbc=[True, True, True], symmetry=True):
     """
     Transform an ASE Structure object into a Pymatgen structure object and then
     a CRYSTAL structure (gui) object.
 
     Args:
-        structure (ASE Structure)
-        pbc (list[bool]): Periodic boundary conditions.
-        symmetry (bool)
+        structure (ASE Structure): ASE Structure object.
+        symmetry (bool): Perform symmetry analysis.
+        
+    Returns:
+        Crystal_gui: CRYSTAL structure (gui) object.
     """
     # First transform into pmg and then write the gui
 
     from pymatgen.io.ase import AseAtomsAdaptor
 
     pmg_structure = AseAtomsAdaptor().get_structure(structure)
 
     return cry_pmg2gui(pmg_structure, pbc=pbc, symmetry=symmetry)
 
 
 def cry_bands2pmg(output, bands, labels=None):
-    # WORK IN TRANSFORMATION
-    #Transform a CRYSTAL bands object into a pymatgen bands object
-
-    # output_file is a crystal output object
-    # bands is a crystal bands object
-        # classBandStructure(kpoints, eigenvals, lattice, efermi, labels_dict=None, coords_are_cartesian=False,
-        # structure=None, projections=None)
-    # labels are the k point labels to display in the band structure
+    """
+    Transform a CRYSTAL bands object into a Pymatgen bands object.
     
+    Args:
+        output: Crystal output object.
+        bands: Crystal bands object.
+        labels (list): K point labels to display in the band structure.
+        
+    Returns:
+        BandStructureSymmLine: Pymatgen band structure object.
+    """
     import numpy as np
     from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
     
     from pymatgen.core.lattice import Lattice
     from pymatgen.electronic_structure.core import Spin
     
     # Read the reciprocal lattice from the output file
@@ -74,18 +78,23 @@
     return BandStructureSymmLine(k_points_coordinates, eigenvals, 
                                  Lattice(output.reciprocal_lattice), 
                                  bands.efermi, labels_dict,
                                  coords_are_cartesian=False)
     
 
 def cry_gui2ase(gui_file):
-    #Transform a CRYSTAL structure (gui) file into an ASE bands object
-    #The gui file is firt transfomed into a pymatgen object
-
-    #gui_file is the CRYSTAL structure (gui) file
+    """
+    Transform a CRYSTAL structure (gui) file into an ASE atoms object.
+    
+    Args:
+        gui_file (str): Path to the CRYSTAL structure (gui) file.
+        
+    Returns:
+        Atoms: ASE atoms object.
+    """
 
     from pymatgen.io.ase import AseAtomsAdaptor
 
     return AseAtomsAdaptor().get_atoms(cry_gui2pmg(gui_file))
 
 
 def cry_gui2cif(cif_file_name, gui, symprec=0.01, angle_tolerance=5.0):
@@ -106,18 +115,25 @@
 
     CifWriter(structure,
               symprec=symprec,
               angle_tolerance=angle_tolerance).write_file(cif_file_name)
 
 
 def cry_gui2pmg(gui, vacuum=10, molecule = True):
-    #Transform a CRYSTAL structure (gui) object into a pymatgen Structure object
-    #Vacuum needs to be included because pymatgen only includes 3D symmetry
-    # molecule = True generates a Molecule pymatgen object for 0D structures
-    # molecule = False generates a Molecule pymatgen with vacuum object for 0D structures
+    """
+    Transform a CRYSTAL structure (gui) object into a Pymatgen Structure object.
+    
+    Args:
+        gui: CRYSTAL structure (gui) object.
+        vacuum (float): Vacuum distance.
+        molecule (bool): Generate a Molecule Pymatgen object for 0D structures.
+        
+    Returns:
+        Structure or Molecule: Pymatgen Structure or Molecule object.
+    """
     
     from pymatgen.core.structure import Structure, Molecule
     import numpy as np
 
     if gui.dimensionality == '0':
         if molecule == True:
             return Molecule(gui.atom_number, gui.atom_positions)
@@ -149,64 +165,81 @@
                 
         gui.lattice[2][2] = thickness_z + vacuum
 
     return Structure(gui.lattice, gui.atom_number, gui.atom_positions, coords_are_cartesian=True)
 
 
 def cry_gui2xyz(xyz_file_name, gui):
-    #Transform a CRYSTAL structure (gui) file into an ASE bands object
-    #The gui file is firt transfomed into a pymatgen object
-
-    #gui_file is the CRYSTAL structure (gui) file
+    """
+    Transform a CRYSTAL structure (gui) file into an XYZ file.
+    
+    Args:
+        xyz_file_name (str): Name (including path) of the XYZ file to be saved.
+        gui: CRYSTAL structure (gui) object.
+    """
 
     from pymatgen.io.xyz import XYZ
     import sys
 
     if gui.dimensionality != 0:
         print('WARNING: the structure is periodic, please use cry_gui2cif()')
         sys.exit(1)
     else:
         structure = cry_gui2pmg(gui, molecule=True) #this returns a pmg Molecule object
     
     XYZ(structure).write_file(xyz_file_name)
 
 
 def cry_out2ase(output, initial=False, vacuum=10):
-    #Transform a CRYSTAL output object into an ASE bands object
-    #The gui file is firt transfomed into a pymatgen object
+    """
+    Transform a CRYSTAL output object into an ASE atoms object.
 
-    # output_file is a crystal output object
-    # initial == False reads the last geometry of the output file
-    # dimensionality is the dimensionality of the system  
-    # vacuum needs to be specified because pymatgen does not have 2D symmetry tools
+    Args:
+        output: Crystal output object.
+        initial (bool): Read the last geometry of the output file.
+        vacuum (float): Vacuum distance.
+        
+    Returns:
+        Atoms: ASE atoms object.
+    """
 
     from pymatgen.io.ase import AseAtomsAdaptor
 
     return AseAtomsAdaptor().get_atoms(cry_out2pmg(output,initial=initial,vacuum=vacuum))
 
 
 def cry_out2cif(cif_file_name, output):
-    #Save a CRYSTAL structure (gui) object as a cif file
-    #The gui file is first transfomed into a pymatgen object
+    """
+    Save a CRYSTAL output object as a CIF file.
+    from pymatgen.io.cif import CifWriter
 
-    #gui_file is the CRYSTAL structure (gui) file
+    Args:
+        cif_file_name (str): Name (including path) of the CIF file to be saved.
+        output: Crystal output object.
+    """
 
-    from pymatgen.io.cif import CifWriter
 
     structure = cry_gui2pmg(output)
     
     CifWriter(structure).write_file(cif_file_name)
 
 
 def cry_out2pmg(output, vacuum=10, initial = False, molecule = True):
-    #Transform a CRYSTAL output object into a pymatgen structure object
+    """
+    Transform a CRYSTAL output object into a pymatgen structure object.
 
-    # output_file is a crystal output object
-    # initial == False reads the last geometry of the output file
-    # vacuum needs to be specified because pymatgen does not have 2D symmetry tools
+    Args:
+        output (CRYSTAL output object): CRYSTAL output object.
+        vacuum (float): Vacuum distance.
+        initial (bool): Read the last geometry of the output file.
+        molecule (bool): Generate a Molecule Pymatgen object for 0D structures.
+        
+    Returns:
+        Structure: Pymatgen Structure object.
+    """
     
     from pymatgen.core.structure import Structure, Molecule
     import numpy as np
 
     #Extract information from the output file
     dimensionality = output.get_dimensionality()
     output.get_last_geom(write_gui_file=False)
@@ -394,19 +427,21 @@
         for atom in zconv:
             gui.atom_number[atom[0]] = atom[1]
 
     return gui
 
 
 def cry_out2xyz(xyz_file_name, output):
-    #Transform a CRYSTAL structure (gui) file into an ASE bands object
-    #The gui file is firt transfomed into a pymatgen object
-
-    #gui_file is the CRYSTAL structure (gui) file
-
+    """
+    Transform a CRYSTAL output object into an XYZ file.
+    
+    Args:
+        xyz_file_name (str): Name (including path) of the XYZ file to be saved.
+        output: CRYSTAL output object.
+    """
     from pymatgen.io.xyz import XYZ
     import sys
 
     if output.dimensionality != 0:
         print('WARNING: the structure is periodic, please use cry_out2cif()')
         sys.exit(1)
     else:
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/crystal_io.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/crystal_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         """
         import re
         from pymatgen.core.structure import IStructure
 
         struc = IStructure.from_file(file)
         self.geom_from_pmg(struc, zconv, keyword, pbc, gui_name, symprec, angle_tolerance)
 
-        return
+        return self
 
     def geom_from_pmg(self, struc, zconv=None, keyword='EXTERNAL',
                       pbc=[True, True, True], gui_name='fort.34',
                       symprec=0.01, angle_tolerance=5.0):
         """
         Read geometry defined by PyMatGen structure object and put infomation
         into geom block, either as 'EXTERNAL' or 'CRYSTAL'.
@@ -67,15 +67,15 @@
             gui = cry_pmg2gui(struc, pbc=pbc, symmetry=True, zconv=zconv)
             gui.write_gui(gui_name, symm=True)
         elif re.match(r'^CRYSTAL$', keyword, re.IGNORECASE):
             self._pmg2input(struc, zconv, symprec=symprec, angle_tolerance=angle_tolerance)
         else:
             raise ValueError("Input keyword format error: {}".format(keyword))
 
-        return
+        return self
 
     def _pmg2input(self, struc, zconv=None, symprec=0.01, angle_tolerance=5.0):
         """
         Pymatgen IStructure object to 'CRYSTAL' input block
 
         .. note::
 
@@ -87,101 +87,109 @@
             lead to errors due to the inconsistent choice of periodic cell
             between CRYSTAL and pymatgen.
         """
         import numpy as np
         from pymatgen.core.structure import IStructure
         from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-        analyzer = SpacegroupAnalyzer(
-            struc, symprec=symprec, angle_tolerance=angle_tolerance)
+        analyzer = SpacegroupAnalyzer(struc, symprec=symprec, angle_tolerance=angle_tolerance)
         # Analyze the refined geometry
         struc2 = analyzer.get_refined_structure()
-        analyzer2 = SpacegroupAnalyzer(
-            struc2, symprec=symprec, angle_tolerance=angle_tolerance)
-        struc_symm = analyzer2.get_symmetrized_structure()
+        analyzer2 = SpacegroupAnalyzer(struc2, symprec=symprec, angle_tolerance=angle_tolerance)
+        struc_pri = analyzer2.get_primitive_standard_structure()
+        analyzer3 = SpacegroupAnalyzer(struc_pri, symprec=symprec, angle_tolerance=angle_tolerance)
+        struc_pri = analyzer3.get_symmetrized_structure()
 
-        sg = analyzer.get_space_group_number()
+        sg = analyzer2.get_space_group_number()
         latt = []
         if sg >= 1 and sg < 3:  # trilinic
             for i in ['a', 'b', 'c', 'alpha', 'beta', 'gamma']:
                 latt.append(round(
-                    getattr(struc_symm.lattice, i), 6
+                    getattr(struc_pri.lattice, i), 6
                 ))
         elif sg >= 3 and sg < 16:  # monoclinic
             for i in ['a', 'b', 'c', 'beta']:
                 latt.append(round(
-                    getattr(struc_symm.lattice, i), 6
+                    getattr(struc_pri.lattice, i), 6
                 ))
         elif sg >= 16 and sg < 75:  # orthorhombic
             for i in ['a', 'b', 'c']:
                 latt.append(round(
-                    getattr(struc_symm.lattice, i), 6
+                    getattr(struc_pri.lattice, i), 6
                 ))
         elif sg >= 75 and sg < 143:  # tetragonal
             for i in ['a', 'c']:
                 latt.append(round(
-                    getattr(struc_symm.lattice, i), 6
+                    getattr(struc_pri.lattice, i), 6
                 ))
-        elif sg >= 143 and sg < 168:  # trigonal
-            for i in ['a', 'alpha']:
+        elif sg >= 143 and sg < 168:  # trigonal, convert to hexagonal
+            struc_pri = analyzer3.get_conventional_standard_structure()
+            analyzer4 = SpacegroupAnalyzer(struc_pri, symprec=symprec, angle_tolerance=angle_tolerance)
+            struc_pri = analyzer4.get_symmetrized_structure()
+            for i in ['a', 'c']:
                 latt.append(round(
-                    getattr(struc_symm.lattice, i), 6
+                    getattr(struc_pri.lattice, i), 6
                 ))
-        elif sg >= 168 and sg < 195:  # hexagonal
+        elif sg >= 168 and sg < 195:  # hexagonal and trigonal
             for i in ['a', 'c']:
                 latt.append(round(
-                    getattr(struc_symm.lattice, i), 6
+                    getattr(struc_pri.lattice, i), 6
                 ))
         else:  # cubic
-            latt.append(round(struc_sym.lattice.a, 6))
+            latt.append(round(struc_pri.lattice.a, 6))
 
-        natom = len(struc_symm.equivalent_sites)
-        eq_atom = int(len(struc_symm.species) / natom)
+        natom = len(struc_pri.equivalent_sites)
+        eq_atom = int(len(struc_pri.species) / natom)
         atominfo = []
         if zconv != None:
             z_atom_index = [i[0] for i in zconv]
         for i in range(natom):
             idx_eq = int(i * eq_atom)
             if zconv == None:
-                z_input = struc_symm.species[idx_eq].Z
+                z_input = struc_pri.species[idx_eq].Z
             else:
                 try:
                     atom_to_sub = z_atom_index.index(i)
                     z_input = zconv[atom_to_sub][1]
                 except ValueError:
-                    z_input = struc_symm.species[idx_eq].Z
+                    z_input = struc_pri.species[idx_eq].Z
             atominfo.append([
                 '{:<3}'.format(z_input),
                 '{0:11.8f}'.format(
-                    round(struc_symm.equivalent_sites[i][0].frac_coords[0], 8)
+                    round(struc_pri.equivalent_sites[i][0].frac_coords[0], 8)
                 ),
                 '{0:11.8f}'.format(
-                    round(struc_symm.equivalent_sites[i][0].frac_coords[1], 8)
+                    round(struc_pri.equivalent_sites[i][0].frac_coords[1], 8)
                 ),
                 '{0:11.8f}'.format(
-                    round(struc_symm.equivalent_sites[i][0].frac_coords[2], 8)
+                    round(struc_pri.equivalent_sites[i][0].frac_coords[2], 8)
                 )
             ])
 
         super(Crystal_input, self).geom.crystal(IGR=sg, latt=latt, atom=atominfo)
 
         return
 
 
 class Crystal_output:
-    # This class reads a CRYSTAL output and generates an object
+    """This class reads a CRYSTAL output and generates an object."""
 
     def __init__(self):
-        # Initialise the Crystal_output
+        """Initialize the Crystal_output."""
 
         pass
 
     def read_cry_output(self, output_name):
-        # output_name: name of the output file
+        """Reads a CRYSTAL output file.
 
+        Args:
+            output_name (str): Name of the output file.
+        Returns:
+            CrystalOutput: Object representing the CRYSTAL output.
+        """
         import sys
         import re
 
         self.name = output_name
 
         # Check if the file exists
         try:
@@ -217,56 +225,67 @@
         # Check if the geometry optimisation converged
         self.opt_converged = False
 
         for line in self.data[::-1]:
             if bool(re.search('OPT END - CONVERGED', line) ) == True:
                 self.opt_converged = True
                 break
-        
+
         return self
 
     def get_dielectric_tensor(self):
+        """Extracts the dielectric tensor from the output.
 
+        Returns:
+            list: Dielectric tensor values.
+        """
         import re
 
         for i, line in enumerate(self.data):
             if re.match(r'^ TENSOR IN PRINCIPAL AXES SYSTEM', line):
                 # This is the end of output
                 self.dielectric_tensor = [
                     float(x) for x in self.data[i+1].split()[1::2]]
                 return self.dielectric_tensor
         return None
 
     def get_eigenvectors(self):
-
+        """Extracts eigenvectors from the output."""
         import re
 
         for i, line in enumerate(self.data):
             if re.match(r'\s NUMBER OF AO', line) != None:
                 self.num_ao = int(line.split()[3])
 
             if re.match(r'\s SHRINK. FACT.(MONKH.)', line) != None:
                 self.num_k = int(line.split()[13])
 
             if re.match(r'\s SHRINK. FACT.(MONKH.)', line) != None:
                 self.num_k = int(line.split()[13])
 
     def get_dimensionality(self):
-        # Get the dimsensionality of the system
+        """Gets the dimensionality of the system.
+
+        Returns:
+            int: Dimensionality of the system.
+        """
 
         import re
 
         for line in self.data:
             if re.match(r'\sGEOMETRY FOR WAVE FUNCTION - DIMENSIONALITY OF THE SYSTEM', line) != None:
                 self.dimensionality = int(line.split()[9])
                 return self.dimensionality
 
     def get_final_energy(self):
-        # Get the final energy of the system
+        """Get the final energy of the system.
 
+        Returns:
+            float: The final energy of the system.
+        """
         import re
 
         self.final_energy = None
         for line in self.data[self.eoo::-1]:
             if re.match(r'\s\W OPT END - CONVERGED', line) != None:
                 self.final_energy = units.H_to_eV(float(line.split()[7]))
                 return self.final_energy
@@ -276,18 +295,21 @@
 
         if self.final_energy == None:
             print('WARNING: no final energy found in the output file. energy = None')
 
         return self.final_energy
 
     def get_scf_convergence(self, all_cycles=False):
-        # Returns the scf convergence energy and energy difference
-
-        # all_cycles == True returns all the steps for a geometry opt
+        """Returns the scf convergence energy and energy difference.
 
+        Args:
+            all_cycles (bool, optional): Return all steps for a geometry opt. Defaults to False.
+        Returns:
+            tuple or list: The scf convergence energy and energy difference.
+        """
         import re
         import numpy as np
 
         self.scf_energy = []
         self.scf_deltae = []
 
         scf_energy = []
@@ -312,37 +334,46 @@
                     scf_energy = []
                     scf_deltae = []
 
             self.scf_convergence = [self.scf_energy, self.scf_deltae]
         return self.scf_convergence
 
     def get_opt_convergence_energy(self):
-        # Returns the energy for each opt step
+        """Returns the energy for each opt step.
 
+        Returns:
+            list: Energy for each optimization step.
+        """
         self.opt_energy = []
         for line in self.data:
             if re.match(r'^ == SCF ENDED - CONVERGENCE ON ENERGY', line):
                 self.opt_energy.append(units.H_to_eV(float(line.split()[8])))
 
         return self.opt_energy
 
     def get_num_cycles(self):
-        # Returns the number of scf cycles
+        """Returns the number of SCF cycles.
 
+        Returns:
+            int: Number of SCF cycles.
+        """
         import re
 
         for line in self.data[::-1]:
             if re.match(r'^ CYC ', line):
                 self.num_cycles = int(line.split()[1])
                 return self.num_cycles
         return None
 
     def get_fermi_energy(self):
-        # Returns the system Fermi energy
+        """Returns the system Fermi energy.
 
+        Returns:
+            float: Fermi energy of the system.
+        """
         import re
 
         self.fermi_energy = None
 
         for i, line in enumerate(self.data[len(self.data)::-1]):
             # This is in case the .out is from a BAND calculation
             if re.match(r'^ TTTTTTTTTTTTTTTTTTTTTTTTTTTTTT BAND', self.data[len(self.data)-(i+4)]) != None:
@@ -386,18 +417,22 @@
 
         if self.fermi_energy == None:
             print('WARNING: no Fermi energy found in the output file. efermi = None')
 
         return self.fermi_energy
 
     def get_primitive_lattice(self, initial=True):
-        # Returns the pritive lattice of the system
-
-        # Initial == False: read the last lattice vectors. Useful in case of optgeom
+        """Returns the primitive lattice of the system.
 
+        Args:
+            initial (bool): Determines whether to read the initial or last lattice vectors.
+                Useful in case of optgeom. Defaults to True.
+        Returns:
+            np.ndarray: Primitive lattice of the system.
+        """
         import re
         import numpy as np
 
         lattice = []
         self.primitive_lattice = None
         if initial == True:
             for i, line in enumerate(self.data):
@@ -418,18 +453,22 @@
 
         if lattice == []:
             print('WARNING: no lattice vectors found in the output file. lattice = []')
 
         return self.primitive_lattice
 
     def get_reciprocal_lattice(self, initial=True):
-        # Returns the reciprocal pritive lattice of the system
-
-        # Initial == False: read the last reciprocal lattice vectors. Useful in case of optgeom
+        """Returns the reciprocal primitive lattice of the system.
 
+        Args:
+            initial (bool): Determines whether to read the initial or last reciprocal lattice vectors.
+                Useful in case of optgeom. Defaults to True.
+        Returns:
+            np.ndarray: Reciprocal primitive lattice of the system.
+        """
         import re
         import numpy as np
 
         lattice = []
         if initial == True:
             for i, line in enumerate(self.data):
                 if re.match(r'^ DIRECT LATTICE VECTORS COMPON. \(A.U.\)', line):
@@ -448,16 +487,19 @@
                         lattice.append(lattice_line)
                     self.reciprocal_lattice = np.array(lattice)
                     return self.reciprocal_lattice
 
         return None
 
     def get_band_gap(self):
-        # Returns the system band gap
+        """Returns the system band gap.
 
+        Returns:
+            float or np.ndarray: Band gap of the system.
+        """
         import re
         import numpy as np
 
         # Check if the system is spin polarised
         self.spin_pol = False
         for line in self.data:
             if re.match(r'^ SPIN POLARIZED', line):
@@ -626,16 +668,19 @@
 
                 self.last_geom = [lattice.tolist(
                 ), self.atom_numbers, self.atom_positions_cart.tolist()]
 
                 return self.last_geom
 
     def get_symm_ops(self):
-        # Return the symmetry operators
+        """Return the symmetry operators
 
+        Returns:
+            numpy.ndarray: Symmetry operators
+        """
         import re
         import numpy as np
 
         symmops = []
 
         for i, line in enumerate(self.data):
             if re.match(r'^ \*\*\*\*   \d+ SYMMOPS - TRANSLATORS IN FRACTIONAL UNITS', line):
@@ -644,19 +689,23 @@
                     symmops.append([float(x)
                                     for x in self.data[i+3+j].split()[2:]])
                 self.symm_ops = np.array(symmops)
 
                 return self.symm_ops
 
     def get_forces(self, initial=False, grad=False):
-        # Return the forces from an optgeom calculation
-
-        # initial == False returns the last calculated forces
-        # grad == False does not return the gradient on atoms
+        """
+        Return the forces from an optgeom calculation
 
+        Args:
+            initial (bool, optional): Return forces from the initial calculation. Defaults to False.
+            grad (bool, optional): Return gradient information. Defaults to False.
+        Returns:
+            list or None: Forces if available, None otherwise
+        """
         if ' OPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOPT\n' not in self.data:
             print('WARNING: this is not a geometry optimisation.')
             return None
         else:
 
             import re
             import numpy as np
@@ -714,32 +763,42 @@
                             self.forces_atoms.append(
                                 [float(x) for x in self.data[j].split()[2:]])
                         self.forces_atoms = np.array(self.forces_atoms)
                         self.forces = [self.forces_cell, self.forces_atoms]
                         return self.forces
 
     def get_mulliken_charges(self):
-        # Return the Mulliken charges (PPAN keyword in input)
+        """
+        Return the Mulliken charges (PPAN keyword in input)
 
+        Returns:
+            list: Mulliken charges
+        """
         import re
 
         self.mulliken_charges = []
         for i, line in enumerate(self.data):
             if re.match(r'^ MULLIKEN POPULATION ANALYSIS', line):
                 for j in range(len(self.data[i:])):
                     line1 = self.data[i+4+j].split()
                     if line1 == []:
                         return self.mulliken_charges
                     elif line1[0].isdigit() == True:
                         self.mulliken_charges.append(float(line1[3]))
         return self.mulliken_charges
 
-    def get_config_analysis(self):
-        # Return the configuration analysis for solid solutions (CONFCON keyword in input)
+    def get_config_analysis(self,return_multiplicity=False):
+        """
+        Return the configuration analysis for solid solutions (CONFCON keyword in input)
 
+        Args:
+            return_multiplicity (bool, optional): Return multiplicity information. Defaults to False.
+        Returns:
+            list or str: Configuration analysis if available, or a warning message
+        """
         import re
         import numpy as np
 
         # Check this is a configuration analysis calculation
         try:
             begin = self.data.index(
                 '                             CONFIGURATION ANALYSIS\n')
@@ -772,325 +831,213 @@
         atom2_end = np.where(
             config_list == '<><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><>')[0]
         end = np.where(
             config_list == '===============================================================================')[0][-1]
         atom2_end = np.append(atom2_end, end)
         atom_type1 = []
         atom_type2 = []
+        multiplicity_tmp = config_list[np.where(config_list == 'MULTIPLICITY')[0]+2]
+        multiplicity = [int(x) for x in multiplicity_tmp]
         config_list = config_list.tolist()
         for i in range(len(atom1_end)):
             atom_type1.append(
                 [int(x) for x in config_list[atom1_begin[i+1]+1:atom1_end[i]]])
             atom_type2.append(
                 [int(x) for x in config_list[atom2_begin[i]+1:atom2_end[i]]])
 
         self.atom_type1 = atom_type1
         self.atom_type2 = atom_type2
 
-        return [self.atom_type1, self.atom_type2]
-
-    def _check_freq_file(self):
-        """
-        Check if the output is specified and if it is a frequency output. 
-
-        .. note::
-
-            The identifier:
-
-            +++ SYMMETRY ADAPTION OF VIBRATIONAL MODES +++
-
-        Returns:
-            is_freq (bool): True if the file is a frequency output file.
+        self.multiplicity = multiplicity
+        if return_multiplicity == True:
+            return [self.atom_type1, self.atom_type2, multiplicity]
+        else:
+            return [self.atom_type1, self.atom_type2]
 
-        :raise Exception: If the output file is not specified
+    def get_phonon(self, read_eigvt=False, rm_imaginary=True, rm_overlap=True,
+                   imaginary_tol=-1e-4, q_overlap_tol=1e-4):
         """
-        import re
-
-        if not hasattr(self, 'data'):
-            raise Exception('Output file not specified.')
-
-        is_freq = False
+        Read phonon-related properties from output file.
 
-        for line in self.data:
-            if re.match(r'^\s*\+\+\+\sSYMMETRY\sADAPTION\sOF\sVIBRATIONAL\sMODES\s\+\+\+', line):
-                is_freq = True
-                break
-            else:
-                continue
+        Args:
+            read_eigvt (bool): Whether to read phonon eigenvectors and
+                normalize it to 1.
+            rm_imaginary (bool): Remove the modes with negative frequencies and
+                set all the related properties to NaN.
+            rm_overlap (bool): *For dispersion calculations* Remove repeated q
+                points and recalculate their weights.
+            imaginary_tol (float): *``rm_imaginary`` = True only* The threshold
+                of negative frequencies.
+            q_overlap_tol (float): *``rm_overlap`` = True only* The threshold of
+                overlapping points, defined as the 2nd norm of the difference
+                of fractional q vectors
 
-        return is_freq
+        .. note::
 
-    def get_q_info(self):
-        """
-        Get DFT total energy and coordinates and weights of q points (where 
-        phonon frequencies are calculated).
+            In QHA calculations, the 'q point' dimension refer to harmonic
+            phonons computed. In other cases it refers to points in reciprocal
+            space.
 
         Returns:
-            self.edft (array[float]): Energy (in kJ/mol) reported in 'CENTERAL 
-                POINT' line (DFT + corrected energy)
+            self.edft (array[float]): :math:`E_{0}` Energy with empirical
+                correction. Unit: kJ/mol.
             self.nqpoint (int): Number of q points
-            self.qpoint (list[list[array[float], float]]): A nqpoint list of
-                2\*1 list whose first element is a 3\*1 array of q point
-                fractional coordinates and the second is its weight.
-
-        .. note::
-
-            ``self.edft`` is an array commensurate with the number of qpoints
-            to ensure the compatibility with QHA output. DFT+HA calculations
-            with various volumes generated by the QHA module make ``self.edft``
-            an array of different numbers. Otherwise, it is the array of same
-            numbers.
-
-        :raise Exception: If the output does not include the 'FREQCALC' section.
+            self.qpoint (list[list[array[float], float]]): A nqpoint\*1 list of
+                2\*1 list whose first element is a 3\*1 array of fractional
+                coordinates and the second is its weight.
+            self.nmode (array[int]): Number of modes at q point. nqpoint\*1
+                array.
+            self.frequency (array[float]): nqpoint\*nmode array ofvibrational
+                frequency. Unit: THz
+            self.intens (array[float]): nqpoint\*nmode array of harmonic
+                intensiy. Unit: km/mol
+            self.IR (array[bool]): nqpoint\*nmode array of boolean values
+                specifying whether the mode is IR active
+            self.Raman (array[bool]): nqpoint\*nmode array of boolean values
+                specifying whether the mode is Raman active
+            self.eigenvector (array[float]): *``read_eigvt = True only``*
+                nqpoint\*nmode\*natom\*3 array of eigenvectors. Normalized to 1.
         """
         import re
         import numpy as np
+        from CRYSTALpytools.base.crysout import PhononBASE
+        from CRYSTALpytools.units import H_to_kjmol
 
-        is_freq = self._check_freq_file()
-        if not is_freq:
-            raise Exception('Not a frequency calculation.')
-
-        edft = np.array([], dtype=float)
+        is_freq = False
+        self.edft = []
         self.nqpoint = 0
         self.qpoint = []
+        self.nmode = []
+        self.frequency = []
+        self.intens = []
+        self.IR = []
+        self.Raman = []
+        self.eigenvector = []
 
-        for i, line in enumerate(self.data):
-            # Keywords in gradient calculation
-            if re.match(r'\s*CENTRAL POINT', line):
-                edft = np.append(edft, units.H_to_kjmol(
-                    float(line.strip().split()[2])))
-
-            if re.search(r'EXPRESSED IN UNITS\s*OF DENOMINATOR', line):
+        countline = 0
+        while countline < len(self.data):
+            line = self.data[countline]
+            # Whether is a frequency file
+            if re.match(r'^\s*\+\+\+\sSYMMETRY\sADAPTION\sOF\sVIBRATIONAL\sMODES\s\+\+\+', line):
+                is_freq = True
+                countline += 1
+                continue
+            # E_0 with empirical corrections
+            elif re.match(r'^\s+CENTRAL POINT', line):
+                self.edft.append(float(line.strip().split()[2]))
+                countline += 1
+                continue
+            # Q point info + frequency
+            ## Dispersion
+            elif re.match(r'^.+EXPRESSED IN UNITS\s+OF DENOMINATOR', line):
                 shrink = int(line.strip().split()[-1])
-
-# Keywords in dipersion calculation
-            if re.match(r'\s*DISPERSION K POINT NUMBER', line):
+                countline += 1
+                continue
+            elif re.match(r'\s+DISPERSION K POINT NUMBER', line):
                 coord = np.array(line.strip().split()[7:10], dtype=float)
                 weight = float(line.strip().split()[-1])
                 self.qpoint.append([coord / shrink, weight])
                 self.nqpoint += 1
-
-# HA Gamma point calculation
-        if self.nqpoint == 0 and len(edft) == 1:
-            self.nqpoint = 1
-            self.qpoint = [[np.array([0, 0, 0], dtype=float), 1.]]
-            self.edft = edft
-# QHA Gamma point calculation
-        elif self.nqpoint == 0 and len(edft) > 1:
-            self.nqpoint = len(edft)
-            for i in range(self.nqpoint):
-                self.qpoint.append(
-                    [np.array([0, 0, 0], dtype=float), 1.]
-                )
-            self.edft = edft
-# HA dispersion calculation
-        elif self.nqpoint > 0 and len(edft) == 1:
-            for i in range(self.nqpoint):
-                self.qpoint[i][1] /= self.nqpoint
-            self.edft = np.array([edft[0] for i in range(self.nqpoint)], dtype=float)
-        else:
-            raise Exception('Only support: 1. HA, Gamma point 2. QHA, gamma point 3. HA dispersion.')
-
-        return self.edft, self.nqpoint, self.qpoint
-
-    def get_mode(self):
-        """
-        Get the number of modes at all q points and corresponding vibrational
-        frequencies and intensities.
-
-        Returns:
-            self.nmode (array[int]): Number of modes at q point.
-            self.frequency (array[float]): nqpoint \* nmode array of vibrational
-                frequency. Unit: THz
-            self.intens (array[float]): nqpoint \* nmode array of harmonic
-                intensiy. Unit: km/mol
-            self.IR (array[bool]): nqpoint \* nmode array of boolean values
-                specifying whether the mode is IR active
-            self.Raman (array[bool]): nqpoint \* nmode array of boolean values
-                specifying whether the mode is Raman active
-        """
-        import numpy as np
-        import re
-
-        if not hasattr(self, 'nqpoint'):
-            self.get_q_info()
-
-        self.frequency = np.array([], dtype=float)
-        self.intens = np.array([], dtype=float)
-        self.IR = np.array([], dtype=bool)
-        self.Raman = np.array([], dtype=bool)
-
-        countline = 0
-        while countline < len(self.data):
-            is_freq = False
-            if re.match(r'\s*DISPERSION K POINT NUMBER\s*\d',
-                        self.data[countline]):
                 countline += 2
-                is_freq = True
-
-            if re.match(r'\s*MODES\s*EIGV\s*FREQUENCIES\s*IRREP',
-                        self.data[countline]):
+                ## Read phonons
+                phonon = PhononBASE.readmode_basic(self.data, countline)
+                countline = phonon[0]
+                self.frequency.append(phonon[1])
+                self.intens.append(phonon[2])
+                self.IR.append(phonon[3])
+                self.Raman.append(phonon[4])
+            ## Gamma point
+            elif re.match(r'^\s+MODES\s+EIGV\s+FREQUENCIES\s+IRREP', line) and self.nqpoint == 0:
                 countline += 2
-                is_freq = True
-
-            while self.data[countline].strip() and is_freq:
-                line_data = self.data[countline].split()
-                nm_a = int(line_data[0].strip('-'))
-                nm_b = int(line_data[1])
-                freq = float(line_data[4])
-                has_spec = False
-                # IR/Raman analysis, closed by default in dispersion calcs
-                if 'A' in line_data or 'I' in line_data:
-                    has_spec = True
-                    intens = float(line_data[-2].strip(')'))
-                    IR = line_data[-4] == 'A'
-                    Raman = line_data[-1] == 'A'
-                    if (nm_b-nm_a == 1):
-                        intens = intens/2
-                    elif(nm_b-nm_a == 2):
-                        intens = intens/3
-
-                for mode in range(nm_a, nm_b + 1):
-                    self.frequency = np.append(self.frequency, freq)
-                    if has_spec:
-                        self.intens = np.append(self.intens, intens)
-                        self.IR = np.append(self.IR, IR)
-                        self.Raman = np.append(self.Raman, Raman)
-
+                ## Read phonons
+                phonon = PhononBASE.readmode_basic(self.data, countline)
+                countline = phonon[0]
+                self.frequency.append(phonon[1])
+                self.intens.append(phonon[2])
+                self.IR.append(phonon[3])
+                self.Raman.append(phonon[4])
+            ## Phonon eigenvector
+            elif re.match(r'^\s+MODES IN PHASE', line) or re.match(r'^\s+NORMAL MODES NORMALIZED', line):
+                if read_eigvt == False:
+                    countline += 1
+                    continue
+                countline += 2
+                eigvt = PhononBASE.readmode_eigenvector(self.data, countline)
+                countline = eigvt[0]
+                self.eigenvector.append(eigvt[1])
+            # Other data
+            else:
                 countline += 1
+                continue
 
-            countline += 1
-
-        self.frequency = np.reshape(self.frequency, (self.nqpoint, -1))
-        self.nmode = np.array([len(i) for i in self.frequency], dtype=int)
-
-        if has_spec:
-            self.intens = np.reshape(self.intens, (self.nqpoint, -1))
-            self.IR = np.reshape(self.IR, (self.nqpoint, -1))
-            self.Raman = np.reshape(self.Raman, (self.nqpoint, -1))
-
-        return self.nmode, self.frequency, self.intens, self.IR, self.Raman
-
-    def get_phonon_eigenvector(self):
-        """
-        Get corresponding mode eigenvectors.
-
-        Returns:
-            self.eigenvector (array[float]): nqpoint\*nmode\*natom\*3 array of 
-                eigenvectors. Normalized to 1.
-        """
-        import numpy as np
-        import re
-
-        if not hasattr(self, 'nmode'):
-            self.get_mode()
+        if is_freq == False:
+            raise Exception('Not a frequency calculation.')
 
-        total_mode = np.sum(self.nmode)
-        countline = 0
-        # Multiple blocks for 1 mode. Maximum 6 columns for 1 block.
-        if np.max(self.nmode) >= 6:
-            countmode = 6
+        # HA/QHA Gamma point calculation
+        if self.nqpoint == 0:
+            self.nqpoint = len(self.edft)
+            self.qpoint = [[np.zeros([3,]), 1.] for i in range(self.nqpoint)]
+            if len(self.edft) == 1:
+                self.edft = [self.edft[0] for i in range(self.nqpoint)]
+        # Dispersion
         else:
-            countmode = total_mode
-
-        # Read the eigenvector region as its original shape
-        block_label = False
-        total_data = []
-        while countline < len(self.data) and countmode <= total_mode:
-            # Gamma point / phonon dispersion calculation
-            if re.match(r'\s*MODES IN PHASE', self.data[countline]) or\
-               re.match(r'\s*NORMAL MODES NORMALIZED', self.data[countline]):
-                block_label = True
-            elif re.match(r'\s*MODES IN ANTI-PHASE', self.data[countline]):
-                block_label = False
-
-            # Enter a block
-            if re.match(r'\s*FREQ\(CM\*\*\-1\)', self.data[countline]) and\
-               block_label:
-                countline += 2
-                block_data = []
-                while self.data[countline].strip():
-                    # Trim annotation part (12 characters)
-                    line_data = re.findall(r'\-*[\d\.]+[E\d\-\+]*',
-                                           self.data[countline][13:])
-                    if line_data:
-                        block_data.append(line_data)
-
-                    countline += 1
-
-                countmode += len(line_data)
-                total_data.append(block_data)
+            self.qpoint = [[i[0], i[1] / self.nqpoint] for i in self.qpoint]
+            self.edft = [self.edft[0] for i in range(self.nqpoint)]
 
-            countline += 1
+        self.edft = H_to_kjmol(np.array(self.edft))
 
-        total_data = np.array(total_data, dtype=float)
+        self.frequency = np.array(self.frequency)
+        self.nmode = np.array([len(i) for i in self.frequency], dtype=int)
+        if self.intens[0] == []:
+            self.intens = []
+            self.IR = []
+            self.Raman = []
+        else:
+            self.intens = np.array(self.intens)
 
-        # Rearrage eigenvectors
-        block_per_q = len(total_data) / self.nqpoint
-        self.eigenvector = []
-        # 1st dimension, nqpoint
-        for q in range(self.nqpoint):
-            index_bg = int(q * block_per_q)
-            index_ed = int((q + 1) * block_per_q)
-            q_data = np.hstack([i for i in total_data[index_bg: index_ed]])
-        # 2nd dimension, nmode
-            q_data = np.transpose(q_data)
-        # 3rd dimension, natom
-            natom = int(self.nmode[q] / 3)
-            q_rearrange = [np.split(m, natom, axis=0) for m in q_data]
+        if self.eigenvector != []:
+            self.eigenvector = np.array(self.eigenvector)
 
-            self.eigenvector.append(q_rearrange)
 
-        self.eigenvector = np.array(self.eigenvector)
+        if rm_imaginary == True:
+            self = PhononBASE.clean_imaginary(self, threshold=imaginary_tol)
 
-        # Normalize eigenvectors of each mode to 1
-        for idx_q, q in enumerate(self.eigenvector):
-            for idx_m, m in enumerate(q):
-                self.eigenvector[idx_q, idx_m] = \
-                    self.eigenvector[idx_q, idx_m] / np.linalg.norm(m)
+        if rm_overlap == True and self.nqpoint > 1:
+            self = PhononBASE.clean_q_overlap(self, threshold=q_overlap_tol)
 
-        return self.eigenvector
+        return self
 
-    def clean_imaginary(self):
+    def get_q_info(self):
         """
-        Substitute imaginary modes and corresponding eigenvectors with numpy
-        NaN format and print warning message.
-
-        Returns:
-            self.frequency (array[float])
-            self.eigenvector (array[float])
+        Deprecated.
         """
-        import numpy as np
         import warnings
 
-        for q, freq in enumerate(self.frequency):
-            if freq[0] > -1e-4 or np.isnan(freq[0]):
-                continue
+        warnings.warn('This method is deprecated. Use `get_phonon`.', stacklevel=2)
+        return self
 
-            warnings.warn(
-                'Negative frequencies detected - Calculated thermodynamics might be inaccurate. Negative frequencies will be substituted by NaN.',
-                stacklevel=2
-            )
-
-            neg_rank = np.where(freq <= -1e-4)[0]
-            self.frequency[q, neg_rank] = np.nan
-
-            if hasattr(self, 'eigenvector'):
-                if len(self.eigenvector) != 0:
-                    natom = int(self.nmode[q] / 3)
-                    nan_eigvt = np.full([natom, 3], np.nan)
-                    self.eigenvector[q, neg_rank] = nan_eigvt
+    def get_mode(self):
+        """
+        Deprecated.
+        """
+        return self.get_q_info()
 
-        if hasattr(self, 'eigenvector'):
-            return self.frequency, self.eigenvector
-        else:
-            return self.frequency
+    def get_phonon_eigenvector(self):
+        """
+        Deprecated.
+        """
+        return self.get_q_info()
 
     def get_elatensor(self):
+        """
+        Extracts the elastic tensor from the data.
 
+        Returns:
+            list: Symmetrized elastic tensor as a 6x6 nested list.
+        """
         startstring = " SYMMETRIZED ELASTIC"
         stopstring = " ELASTIC MODULI"
         self.tensor = []
         buffer = []
         strtensor = []
         copy = False
 
@@ -1123,23 +1070,31 @@
             for j in range(6):
                 self.tensor[j][i] = self.tensor[i][j]
 
         return self.tensor
 
 
 class Properties_input:
-    # This creates a properties_input object
+    """Create a properties_input object"""
+
 
     def __init__(self, input_name=None):
-        # Initialise the object
+        """Initialise the object"""
 
         self.is_newk = False
 
     def from_file(self, input_name):
-        # input_name is the path to an existing properties input
+        """
+        Read the properties input from a file.
+
+        Args:
+            input_name (str): The name of the input file.
+        Returns:
+            self (Properties_input): The Properties_input object.
+        """
         import sys
 
         self.name = input_name
         if input_name is not None:
             try:
                 if input_name[-3:] != 'd12':
                     input_name = input_name+'.d12'
@@ -1158,36 +1113,43 @@
             else:
                 self.is_newk = False
                 self.property_block = self.data
 
         return self
 
     def make_newk_block(self, shrink1, shrink2, Fermi=1, print_option=0):
-        # Returns the newk block
+        """
+        Returns the newk block.
 
-        # shrink1 and shrink 2 are the newk shrinking factors
-        # Fermi: 1 if recalculated, 0 if not
-        # print_options: Properties printing options
+        Args:
+            shrink1 (int): The first newk shrinking factor.
+            shrink2 (int): The second newk shrinking factor.
+            Fermi (int): Fermi recalculation option (default is 1).
+            print_option (int): Properties printing option (default is 0).
+        """
 
         self.is_newk = True
 
         self.newk_block = ['NEWK\n', '%s %s\n' % (shrink1, shrink2),
                            '%s %s\n' % (Fermi, print_option)]
 
     def make_bands_block(self, k_path, n_kpoints, first_band, last_band, print_eig=0, print_option=1,
                          title='BAND STRUCTURE CALCULATION'):
-        # Return the bands block to be used in a bands calculation
+        """
+        Returns the bands block for a bands calculation.
 
-        # k_path can be:
-        # list of list
-        # pymatgen HighSymmKpath object
-        # first_band: first band for bands calculation
-        # last_band: last band for bands calculation
-        # print_eig: printing options for eigenvalues
-        # print_option: properties printing options
+        Args:
+            k_path (list or HighSymmKpath): The k-path for the bands calculation.
+            n_kpoints (int): The number of k-points along the path.
+            first_band (int): The index of the first band.
+            last_band (int): The index of the last band.
+            print_eig (int): Printing options for eigenvalues (default is 0).
+            print_option (int): Properties printing options (default is 1).
+            title (str): The title of the calculation (default is 'BAND STRUCTURE CALCULATION').
+        """
 
         import numpy as np
         import sys
 
         bands_block = []
 
         # path from a pymatgen k_path object
@@ -1236,22 +1198,25 @@
 
         self.property_block = bands_block
 
         return self
 
     def make_doss_block(self, n_points=200, band_range=None, e_range=None, plotting_option=2,
                         poly=12, print_option=1):
-        # Return the doss block to be used in a doss calculation
+        """
+        Returns the doss block for a doss calculation.
 
-        # n_points : number of points in the energy range
-        # band range: which bands to include in the doss calculation
-        # e_range: in eV
-        # plotting_options: properties printing options
-        # poly: maximum exponent for the polynomial fit
-        # print_option: properties printing options
+        Args:
+            n_points (int): The number of points in the DOS plot (default is 200).
+            band_range (list or tuple): The range of bands to include in the DOS calculation (default is None).
+            e_range (list or tuple): The energy range for the DOS calculation (default is None).
+            plotting_option (int): DOS plotting options (default is 2).
+            poly (int): Degree of the polynomial for smearing (default is 12).
+            print_option (int): Properties printing options (default is 1).
+        """
 
         import sys
 
         # either band_range or e_range needs to be specified
         doss_block = []
         if band_range == None and e_range == None:
             print('EXITING: please specify either band_range or e_range. None selected')
@@ -1282,23 +1247,28 @@
 
         self.property_block = doss_block
 
         return self
 
     def make_pdoss_block(self, projections, proj_type='atom', output_file=None, n_points=200, band_range=None,
                          e_range=None, plotting_option=2, poly=12, print_option=1):
-        # Return the pdoss block to be used in a pdoss calculation
+        """
+        Returns the pdoss block for a pdoss calculation.
 
-        # projections is a list of lists of atoms or atomic orbitals
-        # n_points : number of points in the energy range
-        # proj_type == 'atom' is an atom projected DOSS, proj_type == 'ao' is an atomic orbital projected DOSS
-        # e_range: in eV
-        # plotting_options: properties printing options
-        # poly: maximum exponent for the polynomial fit
-        # print_option: properties printing options
+        Args:
+            projections (dict): Dictionary specifying the projections for the pdoss calculation.
+            proj_type (str): Type of projection ('atom' or 'site') (default is 'atom').
+            output_file (str): Output file name (default is None).
+            n_points (int): The number of points in the DOS plot (default is 200).
+            band_range (list or tuple): The range of bands to include in the DOS calculation (default is None).
+            e_range (list or tuple): The energy range for the DOS calculation (default is None).
+            plotting_option (int): DOS plotting options (default is 2).
+            poly (int): Degree of the polynomial for smearing (default is 12).
+            print_option (int): Properties printing options (default is 1).
+        """
 
         import sys
 
         pdoss_block = []
         if band_range == None and e_range == None:
             print('EXITING: please specify either band_range or e_range. None selected')
             sys.exit(1)
@@ -1364,19 +1334,20 @@
         pdoss_block.append('END\n')
 
         self.property_block = pdoss_block
 
         return self
 
     def write_properties_input(self, input_name):
-        # Write a properties input file (to file)
+        """
+        Writes the properties input to a file.
 
-        # input_name is the name of the imput that is going to be written (.d12)
-        # property_input is a Properties_input object
-        # newk == True: perform a newk calculation
+        Args:
+            input_name (str): The name of the output file.
+        """
 
         import sys
         import itertools
 
         if self.is_newk == False:
             property_input_list = self.property_block
         if self.is_newk == True:
@@ -1385,27 +1356,29 @@
 
         with open(input_name, 'w') as file:
             for line in property_input_list:
                 file.writelines(line)
 
 
 class Properties_output:
-    # This creates a properties_output object
+    """Creates a Properties_output object."""
 
     def __init__(self):
-        # properties_output is the properties output file
+        """Initialize the Properties_output object."""
 
         pass
 
     def read_file(self, properties_output):
-        # Function to parse the properties output file.
-        # It is not meant to be calles directly, but to be used by the
-        # functions below to read the properties file.
+        """Parse the properties output file.
 
-        import sys
+        Args:
+            properties_output (str): The properties output file.
+        Returns:
+            Properties_output: The updated Properties_output object.
+        """
         import os
 
         self.file_name = properties_output
 
         try:
             file = open(self.file_name, 'r')
             self.data = file.readlines()
@@ -1415,23 +1388,26 @@
             dir_name = os.path.split(properties_output)[0]
             self.abspath = os.path.join(dir_name)
 
             # title (named "title" only to distinguish from "file_name" which means another thing)
             self.title = os.path.split(properties_output)[1]
 
         except:
-            print('EXITING: a CRYSTAL properties file needs to be specified')
-            sys.exit(1)
+            raise FileNotFoundError('EXITING: a CRYSTAL properties file needs to be specified')
 
     def read_vecfield(self, properties_output, which_prop):
-        # Reads the .f25 file to return a data array containing
-        # one or more density property between: Particle Number Density,
-        # Orbital Current Density, Spin Density and Spin-Current Density.
-        # which_prop allows to know a-priori which density property
-        # has been selected by the user to be printed in the .f25 file
+        """Reads the fort.25 file to return data arrays containing one or more vectiorial density properties.
+
+        Args:
+            properties_output (str): The properties output file.
+            which_prop (str): The density property selected by the user.
+            'm' (magnetization), 'j' (spin current), 'J' (spin current density)
+        Returns:
+            Properties_output (str): The fort.25 output file.
+        """
 
         import numpy as np
 
         self.read_file(properties_output)
 
         data = self.data
 
@@ -1467,29 +1443,29 @@
 
         blines = (nrow*ncol)/6
         if (blines % 6) == 0:
             blines = int(blines)
         else:
             blines = int(blines) + 1
 
-        # Reads the types of density property requested by the user and initializes the data arrays
+        # Reads the types of density properties requested by the user and initializes the data arrays
         check = np.zeros(3, dtype=int)
         if 'm' in which_prop:
             check[0] = 1
             self.dens_m = np.zeros((nrow, ncol, 3), dtype=float)
         if 'j' in which_prop:
             check[1] = 1
             self.dens_j = np.zeros((nrow, ncol, 3), dtype=float)
         if 'J' in which_prop:
             check[2] = 1
             self.dens_JX = np.zeros((nrow, ncol, 3), dtype=float)
             self.dens_JY = np.zeros((nrow, ncol, 3), dtype=float)
             self.dens_JZ = np.zeros((nrow, ncol, 3), dtype=float)
         if (not check[0]) and (not check[1]) and (not check[2]):
-            print('Error: Invalid Entry. Only the m, j, and J charachters are supported')
+            print('Error: Invalid Entry. Only the m, j, and J characters are supported')
             sys.exit(1)
 
         # Gathers the data
         iamhere = 0
 
         if check[0]:
             iamhere = 3
@@ -1558,135 +1534,81 @@
                         r += 1
                         s = 0
                     else:
                         s += 1
         return self
 
     def read_cry_bands(self, properties_output):
-        # This class contains the bands objects created from reading the
-        # CRYSTAL band files
-        # Returns an array where the band energy is expressed in eV
-
-        import re
-        import numpy as np
+        """
+        Deprecated.
+        """
+        import warnings
 
-        self.read_file(properties_output)
+        warnings.warn('Deprecated. Use read_electron_band instead.')
+        return self.read_electron_band(properties_output)
 
-        data = self.data
+    def read_electron_band(self, properties_output):
+        """
+        Generate bands object from CRYSTAL BAND.DAT or fort.25 file.
+        Energy unit: eV.
 
-        # Read the information about the file
-        # number of k points in the calculation
-        self.n_kpoints = int(data[0].split()[2])
-        # number of bands in the calculation
-        self.n_bands = int(data[0].split()[4])
-        self.spin = int(data[0].split()[6])  # number of spin
-        # number of tick in the band plot
-        self.n_tick = int(data[1].split()[2])+1
-        self.k_point_inp_coordinates = []
-        self.n_points = []
-        # finds all the coordinates of the ticks and the k points
-        """for i in range(self.n_tick):
-            self.n_points.append(int(data[2+i].split()[1]))
-            coord = []
-            for j in range(3):
-                l = re.findall('\d+', data[2+i].split()[2])
-                coord.append(float(l[j])/float(l[3]))
-            self.k_point_inp_coordinates.append(coord)
-        self.k_point_inp_coordinates = np.array(self.k_point_inp_coordinates)
-        self.k_point_coordinates = [self.k_point_inp_coordinates[0]]
-        for i in range(1, self.n_tick):
-            step = (self.k_point_inp_coordinates[i]-self.k_point_inp_coordinates[i-1])/float(
-                self.n_points[i]-self.n_points[i-1])
-            for j in range(self.n_points[i]-self.n_points[i-1]):
-                # coordinates of the k_points in the calculation
-                self.k_point_coordinates.append(
-                    (self.k_point_inp_coordinates[i-1]+step*float(j+1)).tolist())"""
-        self.tick_position = []  # positions of the ticks
-        self.tick_label = []  # tick labels
-        for i in range(self.n_tick):
-            self.tick_position.append(
-                float(data[16+self.n_tick+i*2].split()[4]))
-            self.tick_label.append(
-                str(data[17+self.n_tick+i*2].split()[3][2:]))
-        self.efermi = units.H_to_eV(float(data[-1].split()[3]))
-
-        # Allocate the bands as np arrays
-        self.bands = np.zeros(
-            (self.n_bands, self.n_kpoints, self.spin), dtype=float)
-
-        # Allocate the k_points a one dimensional array
-        self.k_point_plot = np.zeros(self.n_kpoints)
-
-        # line where the first band is. Written this way to help identify
-        # where the error might be if there are different file lenghts
-        first_k = 2 + self.n_tick + 14 + 2*self.n_tick + 2
-
-        # Read the bands and store them into a numpy array
-        for i, line in enumerate(data[first_k:first_k+self.n_kpoints]):
-            self.bands[:self.n_bands+1, i,
-                       0] = np.array([float(n) for n in line.split()[1:]])
-            self.k_point_plot[i] = float(line.split()[0])
-
-        if self.spin == 2:
-            # line where the first beta band is. Written this way to help identify
-            first_k_beta = first_k + self.n_kpoints + 15 + 2*self.n_tick + 2
-            for i, line in enumerate(data[first_k_beta:-1]):
-                self.bands[:self.n_bands+1, i,
-                           1] = np.array([float(n) for n in line.split()[1:]])
+        Args:
+            properties_output (str): File name
 
-        # Convert all the energy to eV
-        self.bands[:, :, :] = units.H_to_eV(self.bands[:, :, :])
+        Returns:
+            self.bands (BandsBASE): A Bands base object
+        """
+        from CRYSTALpytools.base.propout import BandsBASE
 
-        # Calculate the direct/indirect band gaps
+        self.read_file(properties_output)
+        if '-%-' in self.data[0]: #fort.25 file format
+            self.bands = BandsBASE.f25_parser(self.data)
+        else: #BAND.DAT file format
+            self.bands = BandsBASE.BAND_parser(self.data)
 
-        return self
+        return self.bands
 
     def read_cry_doss(self, properties_output):
-        # This class contains the bands objects created from reading the
-        # CRYSTAL doss files
-        # Returns an array where the band energy is expressed in eV
+        """
+        Deprecated.
+        """
+        import warnings
 
-        import re
-        import numpy as np
+        warnings.warn('Deprecated. Use read_electron_dos instead.')
+        return self.read_electron_dos(properties_output)
 
-        self.read_file(properties_output)
+    def read_electron_dos(self, properties_output):
+        """
+        Generate doss object from CRYSTAL DOSS.DAT or fort.25 file.
+        Energy unit: eV.
 
-        data = self.data
+        Args:
+            properties_output (str): File name
 
-        # Read the information about the file
-        self.n_energy = int(data[0].split()[2])
-        self.n_proj = int(data[0].split()[4])
-        self.spin = int(data[0].split()[6])
-        self.efermi = units.H_to_eV(float(data[-1].split()[3]))
-
-        first_energy = 4
-
-        # Allocate the doss as np arrays
-        self.doss = np.zeros(
-            (self.n_energy, self.n_proj+1, self.spin), dtype=float)
-
-        # Read the doss and store them into a numpy array
-        for i, line in enumerate(data[first_energy:first_energy+self.n_energy]):
-            self.doss[i, :self.n_proj+1,
-                      0] = np.array([float(n) for n in line.split()])
-
-        if self.spin == 2:
-            # line where the first beta energy is. Written this way to help identify
-            first_energy_beta = first_energy + self.n_energy + 3
-            for i, line in enumerate(data[first_energy_beta:-1]):
-                self.doss[i, :self.n_proj+1,
-                          1] = np.array([float(n) for n in line.split()])
+        Returns:
+            self.doss (DOSBASE): A DOS base object
+        """
+        from CRYSTALpytools.base.propout import DOSBASE
 
-        # Convert all the energy to eV
-        self.doss[:, 0, :] = units.H_to_eV(self.doss[:, 0, :])
+        self.read_file(properties_output)
+        if '-%-' in self.data[0]: #fort.25 file format
+            self.doss = DOSBASE.f25_parser(self.data)
+        else: #DOSS.DAT file format
+            self.doss = DOSBASE.DOSS_parser(self.data)
 
-        return self
+        return self.doss
 
     def read_cry_contour(self, properties_output):
+        """Read the CRYSTAL contour files to create the contour objects.
 
+        Args:
+            properties_output (str): The properties output file.
+        Returns:
+            Properties_output: The updated Properties_output object.
+        """
         import sys
         import re
         import pandas as pd
         import numpy as np
 
         self.read_file(properties_output)
 
@@ -1793,15 +1715,22 @@
             self.colors = colors3
             self.linestyles = ls3
             self.fmt = '%1.2f'
 
         return self
 
     def read_cry_xrd_spec(self, properties_output):
+        """
+        Read XRD spectrum data from a file.
 
+        Args:
+            properties_output (str): Path to the properties output file.
+        Returns:
+            self: The modified object with extracted XRD spectrum data.
+        """
         import sys
         import re
         import pandas as pd
 
         self.read_file(properties_output)
 
         data = self.data
@@ -1861,15 +1790,22 @@
         self.y = df['INTENS-LP']
 
         self.title = title[:-1]
 
         return self
 
     def read_cry_rholine(self, properties_output):
+        """
+        Read density line data from a file.
 
+        Args:
+            properties_output (str): Path to the properties output file.
+        Returns:
+            self: The modified object with extracted density line data.
+        """
         import sys
         import re
         import pandas as pd
 
         self.read_file(properties_output)
 
         l_dens = self.data
@@ -1899,15 +1835,22 @@
         self.y = df_dens[1]/0.148184743
 
         self.title = title[:-4]
 
         return self
 
     def read_cry_seebeck(self, properties_output):
+        """
+        Read Seebeck coefficient data from a file.
 
+        Args:
+            properties_output (str): Path to the properties output file.
+        Returns:
+            self: The modified object with extracted Seebeck coefficient data.
+        """
         import sys
         import re
         import pandas as pd
 
         self.read_file(properties_output)
 
         data = self.data
@@ -1971,15 +1914,22 @@
         self.volume = (float(str(match[2:3])[-13:-4]))
 
         self.title = title
 
         return self
 
     def read_cry_sigma(self, properties_output):
+        """
+        Read electrical conductivity data from a file.
 
+        Args:
+            properties_output (str): Path to the properties output file.
+        Returns:
+            self: The modified object with extracted electrical conductivity data.
+        """
         import sys
         import re
         import pandas as pd
 
         self.read_file(properties_output)
 
         data = self.data
@@ -2043,15 +1993,22 @@
         self.volume = (float(str(match[2:3])[-13:-4]))
 
         self.title = title
 
         return self
 
     def read_cry_lapl_profile(self, properties_output):
+        """
+        Read Laplacian profile data from a file.
 
+        Args:
+            properties_output (str): Path to the properties output file.
+        Returns:
+            self: The modified object with extracted Laplacian profile data.
+        """
         import pandas as pd
         import re
         import numpy as np
 
         data = self.data
         filename = self.abspath
         title = self.title
@@ -2101,15 +2058,22 @@
         df['dist'] = df['dist'].apply(pd.to_numeric)
         self.datax = df.dist
         self.datay = df.lapl
 
         return self
 
     def read_cry_density_profile(self, properties_output):
+        """
+        Read density profile data from a file.
 
+        Args:
+            properties_output (str): Path to the properties output file.
+        Returns:
+            self: The modified object with extracted density profile data.
+        """
         import pandas as pd
         import re
         import numpy as np
 
         self.read_file(properties_output)
 
         data = self.data
@@ -2261,24 +2225,33 @@
             else:
                 file.writelines('{:5d}{:5d}\n'.format(1, 1))
 
         file.close()
 
 
 class Crystal_density():
-    # WORK IN PROGRESS
-    # Returns a crystal_density object
+    """
+    Read density data from a .f98 file.
+    """
 
     def __init__(self):
 
         pass
 
     def read_cry_irr_density(self, fort98_unit):
-        # fort98_unit is the file containing the formatted density matrix
-
+        """
+        Read density profile data from a CRYSTAL .f98 file.
+        Args:
+            fort98_unit (str): The file containing the formatted density matrix.
+        Returns:
+            None
+        Note:
+        This is a work in progress. If you are interested in this functionality,
+        please open an Issue on GitHub.
+        """
         self.file_name = fort98_unit
         self.is_irr = True
 
         import sys
         import numpy as np
         import re
 
@@ -2531,23 +2504,29 @@
                     # characters long, this ones are 21
                     # The line below fixes that issue
                     self.la4.extend([int(x) for x in data[j].split()])
                     j += 1
 
 
 def cry_combine_density(density1, density2, density3, new_density='new_density.f98', spin_pol=False):
-    # WORK IN PROGRESS:
-    # it only works with ghost atoms at the moment
+    """
+    Combine density matrix files.
 
-    # Returns the combined density matrix
-    # density1 is the first density matrix file
-    # density2 is the second density matrix file
-    # density3 is the density matrix file for the whole system
-    # new_density is the name of the new density matrix
-    # spin_pol == False means the system is not spin polarised
+    Args:
+        density1 (str): The first density matrix file.
+        density2 (str): The second density matrix file.
+        density3 (str): The density matrix file for the whole system.
+        new_density (str, optional): The name of the new density matrix. Defaults to 'new_density.f98'.
+        spin_pol (bool, optional): Specifies if the system is spin polarized. Defaults to False.
+    Returns:
+        None
+    Note:
+        This is a work in progress. If you are interested in this functionality,
+        please open an Issue on GitHub.
+    """
 
     import sys
     import numpy as np
 
     try:
         density1_data = Crystal_density(density1)  # substrate
         density2_data = Crystal_density(density2)  # adsorbate
@@ -2632,21 +2611,29 @@
         spinor+charges+fock+density+density3_data[end:]
     with open(new_density, 'w') as file:
         for line in final_fort98:
             file.writelines(line)
 
 
 def write_cry_density(fort98_name, new_p, new_fort98):
-    # WORK IN PROGRESS
+    """
+    Write the formatted density matrix.
+
+    Args:
+        fort98_name (str): The name of the previous density matrix file.
+        new_p (list): The new density matrix.
+        new_fort98 (str): The name of the new density matrix file.
+
+        Returns:
+        None
+    Note:
+        This is a work in progress. If you are interested in this functionality,
+        please open an Issue on GitHub.
+    """
 
-    # Writes the formatted density matrix
-    # fort98_name is the name of the previous density matrix file
-    # new_p is the new density matrix
-    # new_fort_90 is the name of the new density matrix file
-    #
     import numpy as np
 
     file = open(fort98_name, 'r')
     data = file.readlines()
     file.close()
 
     density = Crystal_density(fort98_name)
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/execute.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/execute.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Fri Nov 19 18:28:54 2021
 
-@author: brunocamino
 """
 
 def set_runcry_path(path):
+    """
+    Set the path for the Runcry executable.
 
+    Args:
+        path (str): The path to the Runcry executable.
+
+    Returns:
+        None
+    """
     import re
     import os
 
     this_file = os.path.realpath(__file__)
     # Read the current settings file
     file = open(this_file, 'r')
     lines = file.readlines()
@@ -25,15 +32,23 @@
     # Write the newly defined variables to the settings file
     file = open(this_file, 'w')
     for line in lines:
         file.writelines(line)
     file.close()
 
 def set_runprop_path(path):
+    """
+    Set the path for the Runprop executable.
+
+    Args:
+        path (str): The path to the Runprop executable.
 
+    Returns:
+        None
+    """
     import re
     import os
 
     this_file = os.path.realpath(__file__)
     # Read the current settings file
     file = open(this_file, 'r')
     lines = file.readlines()
@@ -48,15 +63,24 @@
     file = open(this_file, 'w')
     for line in lines:
         file.writelines(line)
     file.close()
 
 
 def runcry(file_name, guessp=None):
+    """
+    Run Runcry calculation.
 
+    Args:
+        file_name (str): The name of the file to run the calculation.
+        guessp (str, optional): The guessp parameter. Default is None.
+
+    Returns:
+        str: The result of the calculation or an error message.
+    """
     runcry_path = '/Users/brunocamino/crystal/runcry17'
     if runcry_path is None:
         return 'Please set the runcry path before calling this function'
 
     import subprocess
     import sys
     import re
@@ -88,15 +112,24 @@
                 if re.match(r'^ EEEEEEEEEE TERMINATION', line) is not None:
                     converged = True
                     return '%s.out calculation successfully completed' % file_name
 
 
 
 def runprop(prop_name,wf_file):
+    """
+    Run Runprop calculation.
 
+    Args:
+        prop_name (str): The name of the property to calculate.
+        wf_file (str): The name of the wavefunction file.
+
+    Returns:
+        str: The result of the calculation or an error message.
+    """
     runprop_path = '/Users/brunocamino/crystal/runprop17'
     if runprop_path is None:
         return('Please set the runprop path before calling it')
 
     import subprocess
     import sys
     import re
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/plot.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/plot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on 29/03/2022
+Functions to visualize CRYSTAL outputs.
 """
-
-
-def plot_vecfield2D_m(header, dens, colormapdens, quivscale, name, dpi=400):
+def plot_vecfield2D_m(header, dens, quivscale, name='MAG', levels=150, dpi=400):
+    """
+    Plots the 2D magnetization vector field.
+
+    Args:
+        header (list): List containing information about the fort.25 header.
+        dens (numpy.ndarray): Array containing the vector field data.
+        quivscale (float): Scale factor for the quiver plot.
+        name (str, optional):  Name used for saving the plots.
+        levels (int or array-like, optional): Determines the number and positions of the contour lines/regions.
+        dpi (int, optional): DPI (dots per inch) for the output image. Default is 400.
+
+    Returns:
+        None
+    """
     import matplotlib.pyplot as plt
     import numpy as np
 
     for i in range(2, 20):
         if (header[0] % i) == 0:
             nrow_split = int(header[0]/i)
 
@@ -85,25 +97,39 @@
             projy_m[i, j] = np.dot((1/(mod_normal**2))*np.cross(ABC_normal,
                                                                 np.cross(np.array([dens[int(i*step_nrow), int(j*step_ncol, 0)], dens[int(i*step_nrow), int(j*step_ncol), 1],
                                                                                    dens[int(i*step_nrow), int(j*step_ncol), 2]]), ABC_normal)), v1)
 
     # Plotting
 
     m = plt.figure()
-    m = plt.contourf(mesh_x, mesh_y, mod_m, colormapdens, cmap='cool')
+    m = plt.contourf(mesh_x, mesh_y, mod_m, levels, cmap='cool')
     m = plt.colorbar(mappable=m)
     m = plt.quiver(mesh_projx, mesh_projy, projx_m, projy_m, scale=quivscale)
     m = plt.xlabel('$\AA$')
     m = plt.ylabel('$\AA$')
     m = plt.savefig(name, dpi=dpi)
 
     plt.show()
 
 
-def plot_vecfield2D_j(header, dens, colormapdens, quivscale, name, dpi=400):
+def plot_vecfield2D_j(header, dens, quivscale, name='SC', levels=150, dpi=400):
+    """
+    Plots the 2D vector field of the spin current.
+
+    Args:
+        header (list): List containing information about the fort.25 header.
+        dens (numpy.ndarray): Array representing the vector field.
+        quivscale (float): Scale factor for the quiver plot.
+        name (str, optional):  Name used for saving the plots.
+        levels (int or array-like, optional): Determines the number and positions of the contour lines/regions.
+        dpi (int, optional): DPI (dots per inch) for the output image. Defaults to 400.
+
+    Returns:
+        None
+    """
     import matplotlib.pyplot as plt
     import numpy as np
 
     for i in range(2, 20):
         if (header[0] % i) == 0:
             nrow_split = int(header[0]/i)
 
@@ -177,25 +203,41 @@
                                                                 np.cross(np.array([dens[int(i*step_nrow), int(j*step_ncol), 0], dens[int(i*step_nrow), int(j*step_ncol), 1],
                                                                                    dens[int(i*step_nrow), int(j*step_ncol), 2]]), ABC_normal)), v2)
             projy_j[i, j] = np.dot((1/(mod_normal**2))*np.cross(ABC_normal,
                                                                 np.cross(np.array([dens[int(i*step_nrow), int(j*step_ncol), 0], dens[int(i*step_nrow), int(j*step_ncol), 1],
                                                                                    dens[int(i*step_nrow), int(j*step_ncol), 2]]), ABC_normal)), v1)
 
     j = plt.figure()
-    j = plt.contourf(mesh_x, mesh_y, mod_j, colormapdens, cmap='winter')
+    j = plt.contourf(mesh_x, mesh_y, mod_j, levels, cmap='winter')
     j = plt.colorbar(mappable=j)
     j = plt.quiver(mesh_projx, mesh_projy, projx_j, projy_j, scale=quivscale)
     j = plt.xlabel('$\AA$')
     j = plt.ylabel('$\AA$')
     j = plt.savefig(name, dpi=dpi)
 
     plt.show()
 
 
-def plot_vecfield2D_J(header, dens_JX, dens_JY, dens_JZ, colormapdens, quivscale, name, dpi=400):
+def plot_vecfield2D_J(header, dens_JX, dens_JY, dens_JZ, quivscale, name='SCD', levels=150, dpi=400):
+    """
+    Plots the 2D spin current density vector fields.
+
+    Args:
+        header (list): List containing information about the fort.25 header.
+        dens_JX (numpy.ndarray): Array representing the X-component of the spin current density.
+        dens_JY (numpy.ndarray): Array representing the Y-component of the spin current density.
+        dens_JZ (numpy.ndarray): Array representing the Z-component of the spin current density.
+        quivscale: Scale factor for the quiver plot.
+        name (str, optional): Name used for saving the plots.
+        levels (int or array-like, optional): Determines the number and positions of the contour lines/regions.
+        dpi (int, optional): DPI (Dots per inch) for saving the plots. Defaults to 400.
+
+    Returns:
+        None
+    """
     import matplotlib.pyplot as plt
     import numpy as np
 
     for i in range(2, 20):
         if (header[0] % i) == 0:
             nrow_split = int(header[0]/i)
 
@@ -293,144 +335,307 @@
             projy_JZ[i, j] = np.dot((1/(mod_normal**2))*np.cross(ABC_normal,
                                     np.cross(np.array([dens_JZ[int(i*step_nrow), int(j*step_ncol), 0], dens_JZ[int(i*step_nrow), int(j*step_ncol), 1],
                                                        dens_JZ[int(i*step_nrow), int(j*step_ncol), 2]]), ABC_normal)), v1)
 
     # Plotting
 
     JX = plt.figure()
-    JX = plt.contourf(mesh_x, mesh_y, mod_JX, colormapdens, cmap='summer')
+    JX = plt.contourf(mesh_x, mesh_y, mod_JX, levels, cmap='summer')
     JX = plt.colorbar(mappable=JX)
     JX = plt.quiver(mesh_projx, mesh_projy, projx_JX,
                     projy_JX, scale=quivscale)
     JX = plt.xlabel('$\AA$')
     JX = plt.ylabel('$\AA$')
     JX = plt.savefig(name+'_JX', dpi=dpi)
 
     JY = plt.figure()
-    JY = plt.contourf(mesh_x, mesh_y, mod_JY, colormapdens, cmap='summer')
+    JY = plt.contourf(mesh_x, mesh_y, mod_JY, levels, cmap='summer')
     JY = plt.colorbar(mappable=JY)
     JY = plt.quiver(mesh_projx, mesh_projy, projx_JY,
                     projy_JY, scale=quivscale)
     JY = plt.xlabel('$\AA$')
     JY = plt.ylabel('$\AA$')
     JY = plt.savefig(name+'_JY', dpi=dpi)
 
     JZ = plt.figure()
-    JZ = plt.contourf(mesh_x, mesh_y, mod_JZ, colormapdens, cmap='summer')
+    JZ = plt.contourf(mesh_x, mesh_y, mod_JZ, levels, cmap='summer')
     JZ = plt.colorbar(mappable=JZ)
     JZ = plt.quiver(mesh_projx, mesh_projy, projx_JZ,
                     projy_JZ, scale=quivscale)
     JZ = plt.xlabel('$\AA$')
     JZ = plt.ylabel('$\AA$')
     JZ = plt.savefig(name+'_JZ', dpi=dpi)
 
     plt.show()
 
 
-def plot_cry_bands(bands, k_labels=None, energy_range=None, title=False, not_scaled=False, save_to_file=False, mode='single', linestl='-',
-                   linewidth=1, color='blue', fermi='forestgreen', k_range=None, labels=None, figsize=None, scheme=None,
-                   sharex=True, sharey=True):
+def plot_phonon_band(bands, unit='cm-1', k_labels=None, mode='single',
+                     not_scaled=False, energy_range=None, k_range=None,
+                     color='blue', labels=None, linestl='-', linewidth=1,
+                     line_freq0=None, title=None, figsize=None,
+                     scheme=None, sharex=True, sharey=True, save_to_file=None):
+    """
+    A wrapper of plot_cry_bands for phonon band structure.
+
+    Args:
+        bands (BandsBASE|list): Bands object generated by `CRYSTALpytools.crystal_io.Crystal_output.read_pband` or
+            a list of BandsBASE objects.
+        unit (str): The unit of frequency. Can be 'cm-1' or 'THz'.
+        k_labels (list): A list of high-symmetric k point labels. Greek alphabets should be, for example, 'Gamma'.
+        mode (str): The plotting mode. Possible values are 'single', 'multi', 'compare', and 'surface'.
+        not_scaled (bool): Whether to scale the x-axis for different volumes.
+        energy_range (array): A 2x1 array specifying the energy range.
+        k_range (array): A 2x1 array specifying the k-range.
+        color (str|list): Color of plot lines. Should be consistent with bands.
+        labels (str|list): Plot legend. Should be consistent with bands.
+        linestl (str|list): Linestyle string. Should be consistent with bands.
+        linewidth (float): The width of the plot lines.
+        line_freq0 (str): The color of the frequency=0 line.
+        title (str): The title of the plot.
+        figsize (list): The figure size specified as [width, height].
+        scheme (list|tuple): The layout of subplots.
+        sharex (bool): Whether to share the x-axis among subplots.
+        sharey (bool): Whether to share the y-axis among subplots.
+        save_to_file (str): The file name to save the plot.
+
+    Returns:
+        None
+
+    Raises:
+        ValueError: If the specified unit is unknown.
+
+    """
+    import matplotlib.pyplot as plt
+    from CRYSTALpytools.units import thz_to_cm, cm_to_thz
+    import re
+
+    if re.match(r'^cm\-1$', unit, re.IGNORECASE):
+        unit = 'cm-1'
+        is_thz = False
+    elif re.match(r'^THz$', unit, re.IGNORECASE):
+        unit = 'THz'
+        is_thz = True
+    else:
+        raise ValueError('Unknown unit.')
+
+
+    if not (isinstance(bands, list) or isinstance(bands, tuple)):
+        bands = [bands]
+
+    if line_freq0 == None:
+        line_freq0 = (1., 0., 0., 0.) # Transparent
+
+    for b in bands:
+        if unit != b.unit:
+            if unit == 'cm-1':
+                b.bands[:, :, :] = thz_to_cm(b.bands[:, :, :])
+            else:
+                b.bands[:, :, :] = cm_to_thz(b.bands[:, :, :])
+            b.unit = unit
+    if len(bands) == 1:
+        bands = bands[0]
+
+    fig = plot_cry_bands(bands, k_labels=k_labels, energy_range=energy_range, title=title,
+                         not_scaled=not_scaled, mode=mode, linestl=linestl, linewidth=linewidth,
+                         color=color, fermi=line_freq0, k_range=k_range, labels=labels,
+                         figsize=figsize, scheme=scheme, sharex=sharex, sharey=sharey)
+    if is_thz == True:
+        fig.supylabel('Frequency (THz)')
+    else:
+        fig.supylabel('Frequency (cm$^{-1}$)')
+
+    if save_to_file != None:
+        save_plot(save_to_file)
+
+    plt.show()
+
+
+def plot_electron_band(bands, unit='eV', k_labels=None, mode='single',
+                       not_scaled=False, energy_range=None, k_range=None,
+                       color='blue', labels=None, linestl='-', linewidth=1,
+                       fermi='forestgreen', title=None, figsize=None,
+                       scheme=None, sharex=True, sharey=True, save_to_file=None):
+    """
+    A wrapper of plot_cry_bands for electron band structure.
+
+    Args:
+        bands (BandsBASE|list): Bands object generated by `CRYSTALpytools.crystal_io.Properties_output.read_bands` or
+            a list of BandsBASE objects.
+        unit (str): The unit of energy. Can be 'eV' or 'Hartree'.
+        k_labels (list): A list of high-symmetric k point labels. Greek alphabets should be, for example, 'Gamma'.
+        mode (str): The plotting mode. Possible values are 'single', 'multi', 'compare', and 'surface'.
+        not_scaled (bool): Whether to scale the x-axis for different volumes.
+        energy_range (array): A 2x1 array specifying the energy range.
+        k_range (array): A 2x1 array specifying the k-range.
+        color (str|list): Color of plot lines. Should be consistent with bands.
+        labels (str|list): Plot legend. Should be consistent with bands.
+        linestl (str|list): Linestyle string. Should be consistent with bands.
+        linewidth (float): The width of the plot lines.
+        fermi (str): The color of the Fermi level line.
+        title (str): The title of the plot.
+        figsize (list): The figure size specified as [width, height].
+        scheme (list|tuple): The layout of subplots.
+        sharex (bool): Whether to share the x-axis among subplots.
+        sharey (bool): Whether to share the y-axis among subplots.
+        save_to_file (str): The file name to save the plot.
+
+    Returns:
+        None
 
+    Raises:
+        ValueError: If the specified unit is unknown.
+
+    """
+    import matplotlib.pyplot as plt
+    from CRYSTALpytools.units import eV_to_H, H_to_eV
+    import re
+
+    if re.match(r'^eV$', unit, re.IGNORECASE):
+        unit = 'eV'
+        is_ev = True
+    elif re.match(r'^Hartree$', unit, re.IGNORECASE):
+        unit = 'Hartree'
+        is_ev = False
+    else:
+        raise ValueError('Unknown unit.')
+
+    if not (isinstance(bands, list) or isinstance(bands, tuple)):
+        bands = [bands]
+
+    for b in bands:
+        if unit != b.unit:
+            if unit == 'eV':
+                b.bands[:, :, :] = H_to_eV(b.bands[:, :, :])
+            else:
+                b.bands[:, :, :] = eV_to_H(b.bands[:, :, :])
+            b.unit = unit
+    if len(bands) == 1:
+        bands = bands[0]
+
+    fig = plot_cry_bands(bands, k_labels=k_labels, energy_range=energy_range, title=title,
+                         not_scaled=not_scaled, mode=mode, linestl=linestl, linewidth=linewidth,
+                         color=color, fermi=fermi, k_range=k_range, labels=labels,
+                         figsize=figsize, scheme=scheme, sharex=sharex, sharey=sharey)
+    if is_ev == True:
+        fig.supylabel('$E-E_{F}$ (eV)')
+    else:
+        fig.supylabel('$E-E_{F}$ (Hartree)')
+
+    if save_to_file != None:
+        save_plot(save_to_file)
+
+    plt.show()
+
+def plot_cry_bands(bands, k_labels, energy_range, title, not_scaled, mode, linestl,
+                   linewidth, color, fermi, k_range, labels, figsize, scheme,
+                   sharex, sharey):
+    """
+    The base function to plot electron / phonon density of states.
+
+    Args:
+        bands (Union[List, object]): List of band objects or a single band object.
+        k_labels (Union[List[str], None]): List of strings specifying the labels for high symmetry points along the path.
+        energy_range (Union[List[Union[int, float]], None]): List of two integers or floats specifying the energy range (min, max).
+        title (Union[str, None]): Title of the plot.
+        not_scaled (bool): Flag indicating whether to scale the band structure for comparison.
+        mode (str): Mode of the plot ('single', 'multi', 'compare', 'surface').
+        linestl (Union[str, List[str]]): Line style or list of line styles for the bands.
+        linewidth (Union[int, List[int]]): Line width or list of line widths for the bands.
+        color (Union[str, List[str]]): Color or list of colors for the bands.
+        fermi (str): Color of the Fermi level.
+        k_range (Union[List[str], None]): List of two strings specifying the range of k points to plot.
+        labels (Union[List[str], None]): List of labels for the bands in multi-mode.
+        figsize (Union[Tuple[int, int], None]): Figure size.
+        scheme (Union[List[int], Tuple[int, int], None]): Subplot scheme in compare-mode (number of rows, number of columns).
+        sharex (Union[bool, str]): Flag or 'row' or 'col' specifying sharing of x-axis.
+        sharey (Union[bool, str]): Flag or 'row' or 'col' specifying sharing of y-axis.
+
+    Raises:
+        ValueError: If an invalid mode flag is specified or if there are errors in the input parameters.
+
+    Returns:
+        None
+    """
     import matplotlib.pyplot as plt
     # import matplotlib.lines as mlines
     import numpy as np
     import sys
+    import warnings
 
     greek = {'Alpha': '\u0391', 'Beta': '\u0392', 'Gamma': '\u0393', 'Delta': '\u0394', 'Epsilon': '\u0395', 'Zeta': '\u0396', 'Eta': '\u0397',
              'Theta': '\u0398', 'Iota': '\u0399', 'Kappa': '\u039A', 'Lambda': '\u039B', 'Mu': '\u039C', 'Nu': '\u039D', 'Csi': '\u039E',
              'Omicron': '\u039F', 'Pi': '\u03A0', 'Rho': '\u03A1', 'Sigma': '\u03A3', 'Tau': '\u03A4', 'Upsilon': '\u03A5', 'Phi': '\u03A6',
              'Chi': '\u03A7', 'Psi': '\u03A8', 'Omega': '\u03A9', 'Sigma_1': '\u03A3\u2081'}
 
     # Error check on the mode flag
     modes = ['single', 'multi', 'compare', 'surface']
     if mode not in modes:
-        print('Error,The selected mode '+mode+' is not among the possible ones: ' +
-              modes[0]+', ' + modes[1] + ', '+modes[2] + ', or '+modes[3])
-        sys.exit(1)
+        raise ValueError('The selected mode '+mode+' is not among the possible ones: ' + modes[0]+', ' + modes[1] + ', '+modes[2] + ', or '+modes[3])
 
     # Error chenk on k_label
     if k_labels is not None:
 
         if isinstance(k_labels, list):
             for element in k_labels:
                 if not isinstance(element, str):
-                    print('Error, k_label must be a list of strings:' +
-                          str(element)+' is not a string')
-                    sys.exit(1)
+                    raise ValueError('k_label must be a list of strings:' +str(element)+' is not a string')
 
             if isinstance(bands, list):
                 ref = bands[0].n_tick
 
                 for i, file in enumerate(bands):
                     if file.n_tick != ref:
                         i = str(i)
-                        print(
-                            'Error! The ' + i + 'element your file list has a different number of High Symmetry Point!')
-                        sys.exit(1)
+                        raise ValueError('The ' + i + 'element your file list has a different number of High Symmetry Point!')
             else:
                 ref = bands.n_tick
 
             if len(k_labels) < ref:
                 diff = str(ref-len(k_labels))
-                print('Error! You are lacking ' + diff +
-                      ' High Symmetry Points in k_labels!')
-                sys.exit(1)
+                raise ValueError('You are lacking ' + diff +' High Symmetry Points in k_labels!')
 
             elif len(k_labels) > ref:
                 diff = str(len(k_labels)-ref)
-                print('Error! You have ' + diff +
-                      'High Symmetry Points in excess in k_labels')
-                sys.exit(1)
+                raise ValueError('You have ' + diff + 'High Symmetry Points in excess in k_labels')
 
         else:
-            print('Error, k_labels must be a list of strings')
-            sys.exit(1)
+            raise ValueError('k_labels must be a list of strings')
 
     # Error check on energy range
-    if energy_range is not None:
+    if energy_range != None:
 
         if isinstance(energy_range, list):
 
             if len(energy_range) > 2:
-                print('Error, energy_range must be a list of two int or float (min,max)')
-                sys.exit(1)
+                raise ValueError('energy_range must be a list of two int or float (min,max)')
 
             for element in energy_range:
                 if (not isinstance(element, int)) and (not isinstance(element, float)):
-                    print('Error, energy_range must be a list of two int or float (min,max): ' +
-                          str(element)+', is neither a float or an int')
-                    sys.exit(1)
+                    raise ValueError('energy_range must be a list of two int or float (min,max): ' +str(element)+', is neither a float or an int')
 
         else:
-            print('Error, energy_range must be a list of two int or float (min,max)')
-            sys.exit(1)
+            raise ValueError('energy_range must be a list of two int or float (min,max)')
 
     # Error check on k_range
     if k_range is not None:
-
         if isinstance(k_range, list):
             if len(k_range) > 2:
-                print('Error, k_range must be a list of two strings')
-                sys.exit(1)
+                raise ValueError('k_range must be a list of two strings')
 
             for element in k_range:
                 if not isinstance(element, str):
-                    print('Error, k_label must be a list of two strings:' +
-                          str(element)+' is not a string')
-                    sys.exit(1)
+                    raise ValueError('k_label must be a list of two strings:' +str(element)+' is not a string')
 
         else:
-            print('Error, k_range must be a list of two strings')
-            sys.exit(1)
+            raise ValueError('k_range must be a list of two strings')
 
     # Error check on title
-    if title is not False:
+    if title != None:
         if not isinstance(title, str):
-            print('Error, title needs to be a string')
-            sys.exit(1)
+            raise ValueError('title needs to be a string')
 
     if (mode == modes[0]) or (mode == modes[1]) or (mode == modes[3]):
 
         # plotting of a single band object
         if mode == modes[0]:
 
             dx = bands.k_point_plot
@@ -441,82 +646,77 @@
             ymax = np.amax(pltband)
             xmin = min(dx)
             xmax = max(dx)
             count1 = 0
             count2 = 0
 
             # band plot
-
-            if figsize is not None:
-                plt.figure(figsize=figsize)
+            if figsize != None:
+                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey, figsize=figsize)
+            else:
+                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey)
 
             for i in range(no_bands):
 
                 if bands.spin == 1:
-                    plt.plot(dx, pltband[i, :], color=color,
-                             linestyle=linestl, linewidth=linewidth)
+                    ax.plot(dx, pltband[i, :], color=color, linestyle=linestl, linewidth=linewidth)
 
                 elif bands.spin == 2:
                     if count1 == count2:
-                        plt.plot(dx, pltband[i, :, 0], color='red',
-                                 linestyle=linestl, linewidth=linewidth, label='Alpha')
-                        plt.plot(dx, pltband[i, :, 1], color='black',
-                                 linestyle=linestl, linewidth=linewidth, label='Beta')
+                        ax.plot(dx, pltband[i, :, 0], color='red',
+                                linestyle=linestl, linewidth=linewidth, label='Alpha')
+                        ax.plot(dx, pltband[i, :, 1], color='black',
+                                linestyle=linestl, linewidth=linewidth, label='Beta')
                     else:
-                        plt.plot(dx, pltband[i, :, 0], color='red',
-                                 linestyle=linestl, linewidth=linewidth)
-                        plt.plot(dx, pltband[i, :, 1], color='black',
+                        ax.plot(dx, pltband[i, :, 0], color='red',
                                  linestyle=linestl, linewidth=linewidth)
+                        ax.plot(dx, pltband[i, :, 1], color='black',
+                                linestyle=linestl, linewidth=linewidth)
                     count1 += 1
 
         # plot of multiple band objects on a single plot
         elif mode == modes[1]:
 
             # Error check on the band on the 'multi' mode flag
             if not isinstance(bands, list):
-                print('Error, When you choose a ' +
-                      modes[1]+' plot bands needs to be a list of band objects')
-                sys.exit(1)
-
+                raise ValueError('When you choose a ' +modes[1]+' plot bands needs to be a list of band objects')
             # Error check on color for the 'multi' mode flag
             if isinstance(color, list):
-                if len(color) > len(bands):
-                    print(
-                        'Error, The number of colors is greater than the number of objects you want to plot')
-                    sys.exit(1)
-
+                if len(color) != len(bands):
+                    raise ValueError('The number of colors is inconsistent with the number of objects you want to plot')
             else:
                 color = ['dimgrey', 'blue', 'indigo', 'slateblue',
                          'thistle', 'purple', 'orchid', 'crimson']
 
             # Warning comparison with band.spin==2
             for m in bands:
                 if m.spin == 2:
-                    print(
-                        "Warning: the 'multi' plot is not fully implemented at the moment for file with NSPIN = 2")
+                    warnings.warn("The 'multi' plot is not fully implemented at the moment for file with NSPIN = 2")
 
             # scaling that enables the comparison of band structure calculated at different pressures
             if not_scaled is False:
                 reference = xmax = np.amax(bands[0].k_point_plot)
                 xmin = np.amin(bands[0].k_point_plot)
 
             else:
                 xmax = []
                 xmin = []
 
             ymin = []
             ymax = []
 
-            if figsize is not None:
-                plt.figure(figsize=figsize)
+            if figsize != None:
+                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey, figsize=figsize)
+            else:
+                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey)
 
             # plot of all the bands obj present in the list
             for index, data in enumerate(bands):
                 # scaling that enables the comparison of band structure calculated at different pressures
-                if not_scaled is False:
+                if not_scaled == False:
                     k_max = np.amax(data.k_point_plot)
                     dx = (data.k_point_plot/k_max)*reference
                 else:
                     dx = data.k_point_plot
                     xmin.append(np.amin(dx))
                     xmax.append(np.amax(dx))
 
@@ -531,156 +731,144 @@
                 # Effective plot
                 for j in range(no_bands):
 
                     if (count1 == count2) and (labels is not None):
                         if data.spin == 1:
                             if isinstance(linestl, list):
                                 if isinstance(linewidth, list):
-                                    plt.plot(dx, pltband[j, :], color=color[index],
-                                             linestyle=linestl[index], linewidth=linewidth[index], label=labels[index])
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl[index], linewidth=linewidth[index], label=labels[index])
                                 else:
-                                    plt.plot(dx, pltband[j, :], color=color[index],
-                                             linestyle=linestl[index], linewidth=linewidth, label=labels[index])
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl[index], linewidth=linewidth, label=labels[index])
                             else:
                                 if isinstance(linewidth, list):
-                                    plt.plot(dx, pltband[j, :], color=color[index],
-                                             linestyle=linestl, linewidth=linewidth[index], label=labels[index])
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl, linewidth=linewidth[index], label=labels[index])
                                 else:
-                                    plt.plot(dx, pltband[j, :], color=color[index],
-                                             linestyle=linestl, linewidth=linewidth, label=labels[index])
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl, linewidth=linewidth, label=labels[index])
                         elif data.spin == 2:
-                            plt.plot(dx, pltband[j, :, 0], color=color[index],
-                                     linestyle=linestl, linewidth=linewidth, label=labels[index]+' Alpha')
-                            plt.plot(dx, pltband[j, :, 1], color=color[index],
-                                     linestyle='--', linewidth=linewidth, label=labels[index]+' Beta')
+                            ax.plot(dx, pltband[j, :, 0], color=color[index],
+                                    linestyle=linestl, linewidth=linewidth, label=labels[index]+' Alpha')
+                            ax.plot(dx, pltband[j, :, 1], color=color[index],
+                                    linestyle='--', linewidth=linewidth, label=labels[index]+' Beta')
 
                     else:
                         if data.spin == 1:
                             if isinstance(linestl, list):
                                 if isinstance(linewidth, list):
-                                    plt.plot(dx, pltband[j, :], color=color[index],
-                                             linestyle=linestl[index], linewidth=linewidth[index])
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl[index], linewidth=linewidth[index])
                                 else:
-                                    plt.plot(dx, pltband[j, :], color=color[index],
-                                             linestyle=linestl[index], linewidth=linewidth)
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl[index], linewidth=linewidth)
                             else:
                                 if isinstance(linewidth, list):
-                                    plt.plot(
-                                        dx, pltband[j, :], color=color[index], linestyle=linestl, linewidth=linewidth[index])
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl, linewidth=linewidth[index])
                                 else:
-                                    plt.plot(
-                                        dx, pltband[j, :], color=color[index], linestyle=linestl, linewidth=linewidth)
+                                    ax.plot(dx, pltband[j, :], color=color[index],
+                                            linestyle=linestl, linewidth=linewidth)
                         elif data.spin == 2:
-                            plt.plot(
-                                dx, pltband[j, :, 0], color=color[index], linestyle=linestl, linewidth=linewidth)
-                            plt.plot(
-                                dx, pltband[j, :, 1], color=color[index], linestyle='--', linewidth=linewidth)
+                            ax.plot(dx, pltband[j, :, 0], color=color[index],
+                                    linestyle=linestl, linewidth=linewidth)
+                            ax.plot(dx, pltband[j, :, 1], color=color[index],
+                                    linestyle='--', linewidth=linewidth)
 
                     count1 += 1
 
             if (isinstance(xmin, list)) or (isinstance(xmax, list)):
                 xmin = min(xmin)
                 xmax = max(xmax)
 
             ymin = min(ymin)
             ymax = max(ymax)
 
         if mode == modes[3]:
-            print('Warning, the surface bands is not ready yet')
+            warnings.warn('The surface bands is not ready yet')
             sys.exit(0)
 
         # HSP line plot
         if isinstance(bands, list):
             hsp = bands[0].tick_position
         else:
             hsp = bands.tick_position
 
         if k_labels is not None:
             if len(hsp) != len(k_labels):
                 if len(hsp) > len(k_labels):
-                    print(
-                        'Error, you have specified a number of label smalle than the number of High Simmetry Point along the path')
+                    raise ValueError('You have specified a number of label smalle than the number of High Simmetry Point along the path')
                 elif len(hsp) < len(k_labels):
-                    print(
-                        'Error, you have more labels than the High Simmetry point along the path')
-                sys.exit(1)
+                    raise ValueError('You have more labels than the High Simmetry point along the path')
 
         hsp[len(hsp)-1] = xmax
 
-        y_band = np.linspace(ymin-3, ymax+3, 2)
+        y_band = np.linspace(ymin*1.05, ymax*1.05, 2)
 
         for j in hsp:
             x_band = np.ones(2)*j
-            plt.plot(x_band, y_band, color='black', linewidth=0.5)
+            ax.plot(x_band, y_band, color='black', linewidth=0.5)
 
         # plot of the fermi level
         x = np.linspace(xmin, xmax, 2)
         y = np.zeros(2)
-        plt.plot(x, y, color=fermi, linewidth=2.5)
+        ax.plot(x, y, color=fermi, linewidth=2.5)
 
         # definition of the plot title
-        if title is not False:
-            plt.title(title)
+        if title is not None:
+            fig.suptitle(title)
 
         if not isinstance(bands, list):
             if bands.spin == 2:
-                plt.legend()
+                fig.legend()
         else:
             if labels is not None:
-                plt.legend()
-
-        plt.ylabel('$E-E_F$ (eV)')
+                fig.legend()
 
     # compare mode plot
     elif mode == modes[2]:
 
         # Error check on type(bands)
         if not isinstance(bands, list):
-            print('Error, When you choose a ' +
-                  modes[2]+' plot bands needs to be a list of band objects')
-            sys.exit(1)
-
+            raise ValueError('When you choose a ' +modes[2]+' plot bands needs to be a list of band objects')
         # Error check on sharex and sharey option
         if (not isinstance(sharex, bool)) or (not isinstance(sharey, bool)):
             accepted_str = ['row', 'col']
 
             if (isinstance(sharex, str)) or (isinstance(sharey, str)):
                 if sharex not in accepted_str:
-                    print('Error, sharex can only be equal to row or col')
-                    sys.exit(1)
+                    raise ValueError('sharex can only be equal to row or col')
                 elif sharey not in accepted_str:
-                    print('Error, sharey can only be equal to row or col')
-                    sys.exit(1)
-
+                    raise ValueError('sharey can only be equal to row or col')
             else:
-                print('Error, sharex and sharey have to be boolean')
-                sys.exit(1)
+                raise ValueError('sharex and sharey have to be boolean')
 
         # Error check and definition of scheme
         if scheme is None:
             n_rows = 1
             n_col = len(bands)
         else:
             if (not isinstance(scheme, tuple)) and (not isinstance(scheme, list)):
-                print('Error, scheme needs to be a tuple or a list')
+                raise ValueError('scheme needs to be a tuple or a list')
                 sys.exit(1)
             elif len(scheme) > 2:
-                print(
-                    'Error, scheme needs to be a tuple or a list of two elements (nrow,ncol)')
-                sys.exit(1)
+                raise ValueError('scheme needs to be a tuple or a list of two elements (nrow,ncol)')
             else:
                 n_rows = scheme[0]
                 n_col = scheme[1]
         # Creation of the subplots
         if figsize is None:
             fig, axs = plt.subplots(nrows=n_rows, ncols=n_col,
                                     sharex=sharex, sharey=sharey, figsize=figsize)
         else:
             fig, axs = plt.subplots(nrows=n_rows, ncols=n_col,
                                     sharex=sharex, sharey=sharey, figsize=figsize)
+        if n_rows == 1 and n_col == 1: # When axs is not a list
+            axs = [axs]
         # Scaling with different size of the same brillouin zone
         if not_scaled is False:
             reference = xmax = np.amax(bands[0].k_point_plot)
             xmin = np.amin(bands[0].k_point_plot)
 
         else:
             xmax = []
@@ -756,16 +944,15 @@
                         for element in k_labels:
                             if element in k_labels:
                                 g = greek.get(element)
                                 hsp_label.append(g)
                         axs[col].set_xticks(hsp)
                         if k_labels is not None:
                             axs[col].set_xlabels(hsp_label)"""
-                        print(
-                            'Warning, the sharex = False option has not been developed yet')
+                        warnings.warn('The sharex = False option has not been developed yet')
                     axs[col].set_xlim([np.amin(dx), np.amax(dx)])
                     if (sharey is not True) and (energy_range is not None):
                         axs[col].set_ylim([energy_range[0], energy_range[1]])
                     else:
                         axs[col].set_ylim([np.amin(pltband), np.amax(pltband)])
                 else:
                     if sharex is not True:
@@ -773,29 +960,25 @@
                         for element in k_labels:
                             if element in k_labels:
                                 g = greek.get(element)
                                 hsp_label.append(g)
                         axs[row, col].set_xticks(hsp)
                         if k_labels is not None:
                             axs[row, col].set_xlabels(hsp_label)"""
-                        print(
-                            'Warning, the sharex = False option has not been developed yet')
+                        warnings.warn('The sharex = False option has not been developed yet')
                     axs[row, col].set_xlim([np.amin(dx), np.amax(dx)])
                     if (sharey is not True) and (energy_range is not False):
                         axs[row, col].set_ylim(
                             [energy_range[0], energy_range[1]])
                     else:
                         axs[row, col].set_ylim(
                             [np.amin(pltband), np.amax(pltband)])
 
                 count3 += 1
 
-        fig.text(.06, 0.5, '$E-E_F$ (eV)', ha='center',
-                 va='center', rotation='vertical')
-
         if (isinstance(ymin, list)) or (isinstance(ymax, list)):
             ymin = min(ymin)
             ymax = max(ymax)
 
     hsp_label = []
     high_sym_point = []
     if k_labels is not None:
@@ -825,147 +1008,291 @@
                         if repeat_count > repeat:
                             repeat_count = 0
         count += 1
 
     path_dict = dict(zip(high_sym_point2, hsp))
 
     # definition of the ylim
-    if (energy_range is not None) or (sharey is True):
+    if (energy_range != None) and (sharey == True):
         ymin = energy_range[0]
         ymax = energy_range[1]
 
     # definition of the xlim
-    if k_range is not None:
+    if k_range != None:
         xmin = path_dict[k_range[0]]
         xmax = path_dict[k_range[1]]
 
-    if k_labels is not None:
+    if k_labels != None:
         plt.xticks(hsp, hsp_label)
     else:
         plt.xticks(hsp)
 
     plt.ylim(ymin, ymax)
     if (mode == modes[0]) or (mode == modes[1]):
         plt.xlim(xmin, xmax)
     elif (mode == modes[2]) and (k_range is not None):
-        print('Warning, the k_range is not available yet for the compare mode')
+        warnings.warn('The k_range is not available yet for the compare mode')
 
-    if save_to_file != False:
+    return fig
+
+
+def plot_electron_dos(doss, unit='eV', beta='up', overlap=False, prj=None,
+                      energy_range=None, dos_range=None, color='blue',
+                      labels=None, linestl=None, linewidth=1, fermi='forestgreen',
+                      title=None, figsize=None, save_to_file=None):
+    """
+    A wrapper of plot_cry_doss for electron density of states.
+
+    Args:
+        doss (DOSBASE): DOS obect generated by code:`CRYSTALpytools.crystal_io.Properties_output.read_doss`.
+            Or a list of DOSBASE objects.
+        unit (str): 'eV' or 'Hartree'
+        beta (str): Plot spin-down state 'up' or 'down'
+        overlap (bool): Plotting multiple lines into the same figure
+        prj (list): Index of selected projection. Consistent with the
+            index of the 2nd dimension of :code:`doss.doss`
+        energy_range (list[float]): 2*1 list of energy range
+        dos_range (list[float]): 2*1 list of DOS range
+        color (str | list[str]): Color of plot lines. *Should be
+            consistent with number of projections.*
+        labels (str | list[str]): Plot legend. *Should be consistent with
+            number of projections.*
+        linestl (str | list[str]): linestyle string. *Should be consistent
+            with number of projections.*
+        linewidth (float)
+        fermi (str): Color of Fermi level line.
+        title (str)
+        figsize (list[float])
+        save_to_file (str): File name.
+
+    Returns:
+        None
+    """
+    import matplotlib.pyplot as plt
+    from CRYSTALpytools.units import H_to_eV, eV_to_H
+    import re
+
+    if re.match(r'^ev$', unit, re.IGNORECASE):
+        unit = 'eV'
+        is_ev = True
+    elif re.match(r'^hartree$', unit, re.IGNORECASE):
+        unit = 'Hartree'
+        is_ev = False
+    else:
+        raise ValueError('Unknown unit.')
+
+    if not (isinstance(doss, list) or isinstance(doss, tuple)):
+        doss = [doss]
+
+    for d in doss:
+        if unit != d.unit:
+            if unit == 'eV':
+                d.doss[:, 0, :] = H_to_eV(d.doss[:, 0, :])
+                d.doss[:, 1:, :] = eV_to_H(d.doss[:, 1:, :])
+            else:
+                d.doss[:, 0, :] = eV_to_H(d.doss[:, 0, :])
+                d.doss[:, 1:, :] = H_to_eV(d.doss[:, 1:, :])
+            d.unit = unit
+    if len(doss) == 1:
+        doss = doss[0]
+
+    fig = plot_cry_doss(doss, color=color, fermi=fermi, overlap=overlap,
+                        labels=labels, figsize=figsize, linestl=linestl,
+                        linewidth=linewidth, title=title, beta=beta,
+                        energy_range=energy_range, dos_range=dos_range, prj=prj)
+    if is_ev == True:
+        fig.supylabel('DOS (states/eV)')
+        fig.supxlabel('Energy (eV)')
+    else:
+        fig.supylabel('DOS (states/Hartree)')
+        fig.supxlabel('Energy (Hartree)')
+
+    if save_to_file != None:
         save_plot(save_to_file)
 
     plt.show()
 
+def plot_phonon_dos(doss, unit='cm-1', overlap=False, prj=None,
+                    freq_range=None, dos_range=None, color='blue',
+                    labels=None, linestl=None, linewidth=1, line_freq0=None,
+                    title=None, figsize=None, save_to_file=None):
+    """
+    A wrapper of plot_cry_doss for electron density of states.
+
+    Args:
+        doss (DOSBASE): DOS obect generated by code:`CRYSTALpytools.crystal_io.Crystal_output.read_pdos`.
+            Or a list of DOSBASE objects.
+        unit (str): 'cm-1' or 'THz'
+        overlap (bool): Plotting multiple lines into the same figure
+        prj (list): Index of selected projection. Consistent with the
+            index of the 2nd dimension of :code:`doss.doss`
+        freq_range (list[float]): 2*1 list of frequency range
+        dos_range (list[float]): 2*1 list of DOS range
+        color (str | list[str]): Color of plot lines. *Should be
+            consistent with number of projections.*
+        labels (str | list[str]): Plot legend. *Should be consistent with
+            number of projections.*
+        linestl (str | list[str]): linestyle string. *Should be consistent
+            with number of projections.*
+        linewidth (float)
+        line_freq0 (str): Color of frequency = 0 line.
+        title (str)
+        figsize (list[float])
+        save_to_file (str): File name.
+
+    Returns:
+        None
+    """
+    import matplotlib.pyplot as plt
+    from CRYSTALpytools.units import cm_to_thz, thz_to_cm
+    import re
+
+    if re.match(r'^cm\-1$', unit, re.IGNORECASE):
+        unit = 'cm-1'
+        is_thz = False
+    elif re.match(r'^thz$', unit, re.IGNORECASE):
+        unit = 'THz'
+        is_thz = True
+    else:
+        raise ValueError('Unknown unit.')
 
-def plot_cry_doss(doss, color='blue', fermi: str = 'forestgreen', save_to_file=False, overlap: bool = False, labels=None, figsize=None, linestl=None,
-                  linewidth=1, title: str = None, beta: str = 'up', energy_range=None, dos_range=None, prj: list = None):
+    if not (isinstance(doss, list) or isinstance(doss, tuple)):
+        doss = [doss]
 
+    for d in doss:
+        if unit != d.unit:
+            if unit == 'cm-1':
+                d.doss[:, 0, :] = thz_to_cm(d.doss[:, 0, :])
+                d.doss[:, 1:, :] = cm_to_thz(d.doss[:, 1:, :])
+            else:
+                d.doss[:, 0, :] = cm_to_thz(d.doss[:, 0, :])
+                d.doss[:, 1:, :] = thz_to_cm(d.doss[:, 1:, :])
+            d.unit = unit
+
+    if line_freq0 == None:
+        line_freq0 = (1., 0., 0., 0.) # Transparent
+    if len(doss) == 1:
+        doss = doss[0]
+
+    fig = plot_cry_doss(doss, color=color, fermi=line_freq0, overlap=overlap,
+                        labels=labels, figsize=figsize, linestl=linestl,
+                        linewidth=linewidth, title=title, beta='up',
+                        energy_range=freq_range, dos_range=dos_range, prj=prj)
+
+    if is_thz == True:
+        fig.supylabel('DOS (states/THz)')
+        fig.supxlabel('Frequency (THz)')
+    else:
+        fig.supylabel('DOS (states/cm$^{-1}$)')
+        fig.supxlabel('Frequency (cm$^{-1}$)')
+
+    if save_to_file != None:
+        save_plot(save_to_file)
+
+    plt.show()
+
+def plot_cry_doss(doss, color, fermi, overlap, labels, figsize, linestl,
+                  linewidth, title, beta, energy_range, dos_range, prj):
+    """
+    The base function to plot electron / phonon density of states.
+
+    Args:
+        doss (object): The density of states object.
+        color (str or list): The color(s) of the plot(s).
+        fermi (str): The color of the Fermi level line.
+        overlap (bool): True if the projections should overlap, False otherwise.
+        labels (str or list): The label(s) for the plot(s).
+        figsize (tuple): The figure size (width, height) in inches.
+        linestl (str or list): The line style(s) for the plot(s).
+        linewidth (float): The width of the line(s) in points.
+        title (str): The title of the plot.
+        beta (str): The beta value ('up' or 'down').
+        energy_range (tuple): The energy range (xmin, xmax) for the x-axis.
+        dos_range (tuple): The density of states range (ymin, ymax) for the y-axis.
+        prj (None or list): The projection(s) to plot.
+
+    Returns:
+        None
+    """
     import matplotlib.pyplot as plt
     import numpy as np
     import sys
+    import warnings
     from os import path
 
     # Error check on beta
     accepted_beta = ['up', 'down']
     if beta not in accepted_beta:
-        print('Error!, beta can be defined only as: ' +
-              accepted_beta[0] + ' or ' + accepted_beta[1])
-        sys.exit(1)
+        raise ValueError("Beta can be defined only as: 'up' or 'down'.")
 
     # Plot for overlap == True
     if overlap == True:
 
         # Error check on color for color in overlap == true and default list of color
         if (not isinstance(color, list)) and (doss.n_proj > 1):
-            print('Warning!, When overlap is true color has to be a list!')
+            warnings.warn('When overlap is true color has to be a list!', stacklevel=2)
             color = ['blue', 'indigo', 'midgrey', 'crimson']
             if (len(color) < doss.n_proj) or (len(color) < len(prj)):
-                print('Error!, When overlap is true color has to be a list!')
-                sys.exit(1)
+                raise ValueError('When overlap is true color has to be a list!')
 
         # Error check on labels for overlap == true
         if labels is not None:
             if not isinstance(labels, list) and (doss.n_proj > 1):
-                print('Error, When overlap is true labels has to be a list')
-                sys.exit(1)
+                raise ValueError('When overlap is true labels has to be a list')
 
         # Default for figsize
         if figsize is None:
             figsize = (12, 5)
 
         # Error check on color, labels, and linestl
         if (isinstance(color, list)) or (isinstance(labels, list)) or (isinstance(linestl, list)):
             if color is not None:
                 if prj is None:
                     if (len(color) > doss.n_proj) or (len(color) < doss.n_proj):
                         if len(color) > doss.n_proj:
-                            print(
-                                'Error!, the number of colors is greater than the number of projections!')
-                            sys.exit(1)
+                            raise ValueError('The number of colors is greater than the number of projections!')
                         elif len(color) < doss.n_proj:
-                            print(
-                                'Error!, the number of colors is greater than the number of projections!')
-                            sys.exit(1)
+                            raise ValueError('The number of colors is less than the number of projections!')
                 else:
                     if (len(color) > len(prj)) or (len(color) < len(prj)):
                         if len(color) > len(prj):
-                            print(
-                                'Error!, the number of colors is greater than the number of projections required!')
-                            sys.exit(1)
+                            raise ValueError('The number of colors is greater than the number of projections required!')
                         elif len(color) < len(prj):
-                            print(
-                                'Error!, the number of colors is greater than the number of projections required!')
-                            sys.exit(1)
+                            raise ValueError('The number of colors is less than the number of projections required!')
 
             if labels is not None:
                 if prj is None:
                     if (len(labels) > doss.n_proj) or (len(labels) < doss.n_proj):
                         if len(labels) > doss.n_proj:
-                            print(
-                                'Error!, the number of labels is greater than the number of projections!')
-                            sys.exit(1)
+                            raise ValueError('The number of labels is greater than the number of projections!')
                         elif len(labels) < doss.n_proj:
-                            print(
-                                'Error!, the number of labels is greater than the number of projections!')
-                            sys.exit(1)
+                            raise ValueError('The number of labels is less than the number of projections!')
                 else:
                     if (len(labels) > len(prj)) or (len(labels) < len(prj)):
                         if len(labels) > len(prj):
-                            print(
-                                'Error!, the number of labels is greater than the number of projections required!')
-                            sys.exit(1)
+                            raise ValueError('The number of labels is greater than the number of projections required!')
                         elif len(color) < len(prj):
-                            print(
-                                'Error!, the number of labels is greater than the number of projections required!')
-                            sys.exit(1)
+                            raise ValueError('The number of labels is less than the number of projections required!')
 
             if linestl is not None:
                 if prj is None:
                     if (len(linestl) > doss.n_proj) or (len(linestl) < doss.n_proj):
                         if len(linestl) > doss.n_proj:
-                            print(
-                                'Error!, the number of linestl is greater than the number of projections!')
-                            sys.exit(1)
+                            raise ValueError('The number of linestl is greater than the number of projections!')
                         elif len(linestl) < doss.n_proj:
-                            print(
-                                'Error!, the number of linestl is greater than the number of projections!')
-                            sys.exit(1)
+                            raise ValueError('The number of linestl is less than the number of projections!')
                 else:
                     if (len(linestl) > len(prj)) or (len(linestl) < len(prj)):
                         if len(linestl) > len(prj):
-                            print(
-                                'Error!, the number of linestl is greater than the number of projections required!')
-                            sys.exit(1)
+                            raise ValueError('The number of linestl is greater than the number of projections required!')
                         elif len(color) < len(prj):
-                            print(
-                                'Error!, the number of linestl is greater than the number of projections required!')
-                            sys.exit(1)
+                            raise ValueError('The number of linestl is less than the number of projections required!')
 
         # Creation of the figure
-        plt.figure(figsize=figsize)
-
+        fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
         # Creation of dx for the plot
         if doss.spin == 1:
             dx = doss.doss[:, 0]
         elif doss.spin == 2:
             dx = doss.doss[:, 0, :]
             dx_alpha = doss.doss[:, 0, 0]
             dx_beta = doss.doss[:, 0, 1]
@@ -973,142 +1300,130 @@
         # Determination of xmin, xmax, ymin, and ymax
         xmin = np.amin(dx)
         xmax = np.amax(dx)
         ymin = np.amin(doss.doss[1:, :, :])
         ymax = np.amax(doss.doss[1:, :, :])
 
         # Plot of all projections
-        if prj is None:
+        if prj == None:
             for projection in range(1, doss.n_proj+1):
                 # for projection in range(1, 2):
                 if doss.spin == 1:
                     if doss.n_proj > 1:
                         if linestl is None:
-                            plt.plot(dx, doss.doss[:, projection], color=color[projection-1],
-                                     label=labels[projection-1], linewidth=linewidth)
+                            ax.plot(dx, doss.doss[:, projection], color=color[projection-1],
+                                    label=labels[projection-1], linewidth=linewidth)
                         else:
-                            plt.plot(dx, doss.doss[:, projection], color=color[projection-1],
-                                     label=labels[projection-1], linestyle=linestl[projection-1], linewidth=linewidth)
+                            ax.plot(dx, doss.doss[:, projection], color=color[projection-1],
+                                    label=labels[projection-1], linestyle=linestl[projection-1], linewidth=linewidth)
                     else:
-                        plt.plot(
-                            dx, doss.doss[:, projection], color=color, linewidth=linewidth)
+                        ax.plot(dx, doss.doss[:, projection], color=color, linewidth=linewidth)
                 elif doss.spin == 2:
                     if beta == accepted_beta[0]:
                         if doss.n_proj > 1:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0], color=color[projection-1],
-                                     label=labels[projection-1], linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, -doss.doss[:, projection, 1], color=color[projection-1],
-                                     label=labels[projection-1], linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[projection-1],
+                                    label=labels[projection-1], linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, -doss.doss[:, projection, 1], color=color[projection-1],
+                                    label=labels[projection-1], linestyle='--', linewidth=linewidth)
                         else:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0],
-                                     linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, -doss.doss[:, projection, 1],
-                                     linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0],
+                                    linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, -doss.doss[:, projection, 1],
+                                    linestyle='--', linewidth=linewidth)
                     elif beta == accepted_beta[1]:
                         if doss.n_proj > 1:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0], color=color[projection-1],
-                                     label=labels[projection-1], linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, doss.doss[:, projection, 1], color=color[projection-1],
-                                     label=labels[projection-1], linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[projection-1],
+                                    label=labels[projection-1], linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color[projection-1],
+                                    label=labels[projection-1], linestyle='--', linewidth=linewidth)
 
                         else:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0], color=color,
-                                     linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, doss.doss[:, projection, 1], color=color,
-                                     linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color,
+                                    linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color,
+                                    linestyle='--', linewidth=linewidth)
 
         # Plot of selected projections
         else:
             for index, projection in enumerate(prj):
                 if doss.spin == 1:
                     if doss.n_proj > 1:
                         if linestl is None:
-                            plt.plot(dx, doss.doss[:, projection], color=color[index],
-                                     label=labels[index], linewidth=linewidth)
+                            ax.plot(dx, doss.doss[:, projection], color=color[index],
+                                    label=labels[index], linewidth=linewidth)
                         else:
-                            plt.plot(dx, doss.doss[:, projection], color=color[index],
-                                     label=labels[index], linestyle=linestl[index], linewidth=linewidth)
+                            ax.plot(dx, doss.doss[:, projection], color=color[index],
+                                    label=labels[index], linestyle=linestl[index], linewidth=linewidth)
                     else:
-                        plt.plot(
-                            dx, doss.doss[:, projection], color=color, linewidth=linewidth)
+                        ax.plot(dx, doss.doss[:, projection], color=color, linewidth=linewidth)
                 elif doss.spin == 2:
                     if beta == accepted_beta[0]:
                         if doss.n_proj > 1:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0], color=color[index],
-                                     label=labels[index], linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, -doss.doss[:, projection, 1], color=color[index],
-                                     label=labels[index], linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[index],
+                                    label=labels[index], linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, -doss.doss[:, projection, 1], color=color[index],
+                                    label=labels[index], linestyle='--', linewidth=linewidth)
                         else:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0],
-                                     linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, -doss.doss[:, projection, 1],
-                                     linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0],
+                                    linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, -doss.doss[:, projection, 1],
+                                    linestyle='--', linewidth=linewidth)
                     elif beta == accepted_beta[1]:
                         if doss.n_proj > 1:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0], color=color[index],
-                                     label=labels[index], linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, doss.doss[:, projection, 1], color=color[index],
-                                     label=labels[index], linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[index],
+                                    label=labels[index], linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color[index],
+                                    label=labels[index], linestyle='--', linewidth=linewidth)
                         else:
-                            plt.plot(dx_alpha, doss.doss[:, projection, 0], color=color,
-                                     linestyle='-', linewidth=linewidth)
-                            plt.plot(dx_beta, doss.doss[:, projection, 1], color=color,
-                                     linestyle='--', linewidth=linewidth)
+                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color,
+                                    linestyle='-', linewidth=linewidth)
+                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color,
+                                    linestyle='--', linewidth=linewidth)
 
-        yfermi_level = np.linspace(ymin-6, ymax+6, 2)
+        yfermi_level = np.linspace(ymin*1.05, ymax*1.05, 2)
         xfermi_level = np.zeros(2)
         if beta == accepted_beta[0]:
-            plt.plot(xfermi_level, yfermi_level,
-                     color=fermi, linewidth=1.5)
+            ax.plot(xfermi_level, yfermi_level, color=fermi, linewidth=1.5)
         else:
-            yfermi_level = np.linspace(-ymax-5, ymax+5, 2)
-            plt.plot(xfermi_level, yfermi_level,
-                     color=fermi, linewidth=1.5)
-
+            yfermi_level = np.linspace(ymin*1.05, ymax*1.05, 2)
+            ax.plot(xfermi_level, yfermi_level, color=fermi, linewidth=1.5)
         y_zero = np.zeros(2)
         x_zero = np.linspace(xmin, xmax, 2)
-        plt.plot(x_zero, y_zero, color='black', linewidth=0.4)
-
+        ax.plot(x_zero, y_zero, color='black', linewidth=0.4)
         if dos_range is not None:
             ymin = dos_range[0]
             ymax = dos_range[1]
             plt.ylim(ymin, ymax)
         else:
             if doss.spin == 1:
                 ymin = 0
-                plt.ylim(ymin, ymax+5)
+                plt.ylim(ymin, ymax*1.05)
             elif doss.spin == 2:
                 if beta == accepted_beta[0]:
                     ymin = 0
-                    plt.ylim(ymin, ymax+5)
+                    plt.ylim(ymin, ymax*1.05)
                 elif beta == accepted_beta[1]:
-                    plt.ylim(ymin-5, ymax+5)
-
-        plt.ylabel('DOS (a.u)')
-
-        if title is not None:
-            plt.title(title)
-
-        if labels is not None:
-            plt.legend()
+                    plt.ylim(ymin*1.05, ymax*1.05)
 
     # Plot for overlap == False
     else:
-
         # Error checks on colors, labels, and linestl
         if isinstance(color, list):
-            print('Warning!, When overlap is false color should be a string!')
+            warnings.warn('When overlap is false color should be a string!',
+                          stacklevel=2)
             color = 'blue'
 
         if isinstance(labels, list):
-            print('Warning!, When overlap is false labels should be a string!')
+            warnings.warn('When overlap is false labels should be a string!',
+                          stacklevel=2)
             labels = None
 
         if isinstance(linestl, list):
-            print('Warning!, When overlap is false color should be a string!')
+            warnings.warn('When overlap is false color should be a string!',
+                          stacklevel=2)
             linestl = '-'
 
         # Creation of dx for the plot
         if doss.spin == 1:
             dx = doss.doss[:, 0]
         elif doss.spin == 2:
             dx = doss.doss[:, 0, :]
@@ -1122,102 +1437,101 @@
         # Creation xfermi, x_zero, and y_zero
         xfermi = np.zeros(2)
         x_zero = np.linspace(xmin, xmax, 2)
         y_zero = np.zeros(2)
 
         # Creation of subplots for all projections
         if prj is None:
-            fig, axs = plt.subplots(
-                nrows=doss.n_proj, ncols=1, sharex=True, figsize=figsize)
-
+            fig, axs = plt.subplots(nrows=doss.n_proj, ncols=1, sharex=True, figsize=figsize)
+            # If only one projection is generated, axs is not subscriptable
+            if doss.n_proj == 1:
+                axs = [axs]
         # Creation of subplots for selected projections
         else:
-            fig, axs = plt.subplots(
-                nrows=len(prj), ncols=1, sharex=True, figsize=figsize)
+            fig, axs = plt.subplots(nrows=len(prj), ncols=1, sharex=True, figsize=figsize)
+            # If only one projection is generated, axs is not subscriptable
+            if len(prj) == 1:
+                axs = [axs]
 
         # Plot for all projections
         if prj is None:
             for projection in range(doss.n_proj):
                 if doss.spin == 1:
                     ymin = 0
                     ymax = np.amax(doss.doss[:, projection+1])
-                    yfermi = np.linspace(ymin, ymax, 2)
+                    yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
                     axs[projection].plot(dx, doss.doss[:, projection+1],
                                          color=color, linestyle=linestl, linewidth=linewidth)
-                    axs[projection].plot(
-                        xfermi, yfermi, color=fermi, linewidth=1.5)
+                    axs[projection].plot(xfermi, yfermi, color=fermi, linewidth=1.5)
                     if dos_range is not None:
                         ymin = dos_range[0]
                         ymax = dos_range[1]
                     axs[projection].set_ylim(ymin, ymax)
                 elif doss.spin == 2:
                     if beta == accepted_beta[0]:
                         ymin = 0
                         ymax = np.amax(doss.doss[:, projection+1, :])
                         yfermi = np.linspace(ymin, ymax, 2)
                         axs[projection].plot(dx_alpha, doss.doss[:, projection+1, 0], color=color,
                                              linestyle='-', linewidth=linewidth, label='Alpha')
                         axs[projection].plot(dx_beta, -doss.doss[:, projection+1, 1], color=color,
                                              linestyle='--', linewidth=linewidth, label='Beta')
-                        axs[projection].plot(
-                            xfermi, yfermi, color=fermi, linewidth=1.5)
+                        axs[projection].plot(xfermi, yfermi, color=fermi, linewidth=1.5)
                         if dos_range is not None:
                             ymin = dos_range[0]
                             ymax = dos_range[1]
                         axs[projection].set_ylim(ymin, ymax)
                     elif beta == accepted_beta[1]:
                         ymin = -np.amax(doss.doss[:, projection+1, :])
                         ymax = np.amax(doss.doss[:, projection+1, :])
                         yfermi = np.linspace(ymin, ymax, 2)
                         axs[projection].plot(dx_alpha, doss.doss[:, projection+1, 0], color=color,
                                              linestyle='-', linewidth=linewidth, label='Alpha')
                         axs[projection].plot(dx_beta, doss.doss[:, projection+1, 1], color=color,
                                              linestyle='--', linewidth=linewidth, label='Beta')
                         axs[projection].plot(x_zero, y_zero, linewidth=0.4)
-                        axs[projection].plot(
-                            xfermi, yfermi, color=fermi, linewidth=2.5)
+                        axs[projection].plot(xfermi, yfermi, color=fermi, linewidth=2.5)
                         if dos_range is not None:
                             ymin = dos_range[0]
                             ymax = dos_range[1]
                         axs[projection].set_ylim(ymin, ymax)
 
         # Plot for selected projections
         else:
             for index, projection in enumerate(prj):
                 if doss.spin == 1:
                     ymin = 0
                     ymax = np.amax(doss.doss[:, projection])
-                    yfermi = np.linspace(ymin, ymax, 2)
+                    yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
                     axs[index].plot(dx, doss.doss[:, projection],
                                     color=color, linestyle=linestl, linewidth=linewidth)
-                    axs[index].plot(
-                        xfermi, yfermi, color=fermi, linewidth=1.5)
+                    axs[index].plot(xfermi, yfermi, color=fermi, linewidth=1.5)
                     if dos_range is not None:
                         ymin = dos_range[0]
                         ymax = dos_range[1]
                     axs[index].set_ylim(ymin, ymax)
                 elif doss.spin == 2:
                     if beta == accepted_beta[0]:
                         ymin = 0
                         ymax = np.amax(doss.doss[:, projection, :])
-                        yfermi = np.linspace(ymin, ymax, 2)
+                        yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
                         axs[index].plot(dx_alpha, doss.doss[:, projection, 0], color=color,
                                         linestyle='-', linewidth=linewidth, label='Alpha')
                         axs[index].plot(dx_beta, -doss.doss[:, projection, 1], color=color,
                                         linestyle='--', linewidth=linewidth, label='Beta')
                         axs[index].plot(
                             xfermi, yfermi, color=fermi, linewidth=1.5)
                         if dos_range is not None:
                             ymin = dos_range[0]
                             ymax = dos_range[1]
                         axs[index].set_ylim(ymin, ymax)
                     elif beta == accepted_beta[1]:
                         ymin = -np.amax(doss.doss[:, projection, :])
                         ymax = np.amax(doss.doss[:, projection, :])
-                        yfermi = np.linspace(ymin, ymax, 2)
+                        yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
                         axs[index].plot(dx_alpha, doss.doss[:, projection, 0], color=color,
                                         linestyle='-', linewidth=linewidth, label='Alpha')
                         axs[index].plot(dx_beta, doss.doss[:, projection, 1], color=color,
                                         linestyle='--', linewidth=linewidth, label='Beta')
                         axs[index].plot(x_zero, y_zero, linewidth=0.4)
                         axs[index].plot(
                             xfermi, yfermi, color=fermi, linewidth=1.5)
@@ -1225,111 +1539,308 @@
                             ymin = dos_range[0]
                             ymax = dos_range[1]
                         axs[index].set_ylim(ymin, ymax)
 
         if (doss.spin == 2) and (beta == accepted_beta[1]):
             plt.legend()
 
-        fig.text(0.06, 0.5, 'DOS (a.u.)', ha='center',
-                 va='center', rotation='vertical')
-
     if energy_range is not None:
         xmin = energy_range[0]
         xmax = energy_range[1]
     plt.xlim(xmin, xmax)
 
-    plt.xlabel('Energy (eV)')
+    if title is not None:
+        fig.suptitle(title)
+    if labels is not None:
+        plt.legend()
+
+    return fig
+
+
+def plot_electron_banddos(bands, doss, unit='eV', k_labels=None, dos_beta='down',
+                          dos_prj=None, energy_range=None, dos_max_range=None,
+                          color_band='blue', color_dos='blue', labels=None, linestl_band='-',
+                          linestl_dos=None, linewidth=1, fermi='forestgreen',
+                          title=None, figsize=None, save_to_file=None):
+    """
+    A wrapper of plot_cry_es for electron band structure + dos. For spin-polarized cases, beta state.
+
+    Args:
+        bands (BandsBASE|list): Bands object generated by CRYSTALpytools.crystal_io.Properties_output.read_bands
+            or a list of BandsBASE objects.
+        doss (DOSBASE): DOS object generated by CRYSTALpytools.crystal_io.Properties_output.read_doss
+            or a list of DOSBASE objects.
+        unit (str): Unit of energy. Valid options are 'eV' or 'Hartree'.
+        k_labels (list): A list of high-symmetric k point labels. Greek alphabets should be
+            represented as strings, for example, 'Gamma'.
+        dos_beta (str): Spin state to plot. Valid options are 'Up' or 'down'. If 'down', the beta
+            state will be plotted on the same side as the alpha state, otherwise on the other side.
+        dos_prj (list): Index of selected projection. Consistent with the index of the 2nd dimension
+            of doss.doss.
+        energy_range (list): A list of two values representing the energy range to be plotted.
+        dos_max_range (float): Maximum DOS range for the y-axis.
+        color_band (str): Color of the electron bands in the plot.
+        color_dos (str): Color of the density of states (DOS) in the plot.
+        labels (list): A list of labels for the plot legend.
+        linestl_band (str): Linestyle of the electron bands.
+        linestl_dos (str): Linestyle of the density of states (DOS).
+        linewidth (float): Width of the lines in the plot.
+        fermi (str): Color of the Fermi level line.
+        title (str): Title of the plot.
+        figsize (list[float]): Size of the figure in inches (width, height).
+        save_to_file (str): File name to save the plot.
 
-    if save_to_file != False:
-        folder = path.split(save_to_file)[0]
-        if path.exists(folder) == True:
-            plt.savefig('%s.png' % save_to_file)
+    Returns:
+        None
+
+    Raises:
+        ValueError: If the unit parameter is unknown.
+
+    """
+    import matplotlib.pyplot as plt
+    from CRYSTALpytools.units import H_to_eV, eV_to_H
+    import re
+
+    if re.match(r'^ev$', unit, re.IGNORECASE):
+        unit = 'eV'
+        is_ev = True
+    elif re.match(r'^hartree$', unit, re.IGNORECASE):
+        unit = 'Hartree'
+        is_ev = False
+    else:
+        raise ValueError('Unknown unit.')
+
+    if unit != doss.unit:
+        if unit == 'eV':
+            doss.doss[:, 0, :] = H_to_eV(doss.doss[:, 0, :])
+            doss.doss[:, 1:, :] = eV_to_H(doss.doss[:, 1:, :])
+        else:
+            doss.doss[:, 0, :] = eV_to_H(doss.doss[:, 0, :])
+            doss.doss[:, 1:, :] = H_to_eV(doss.doss[:, 1:, :])
+        doss.unit = unit
+    if unit != bands.unit:
+        if unit == 'eV':
+            bands.bands[:, :, :] = H_to_eV(bands.bands[:, :, :])
         else:
-            print('Error: folder %s does not exist' % save_to_file)
-            sys.exit(1)
+            bands.bands[:, :, :] = eV_to_H(bands.bands[:, :, :])
+        bands.unit = unit
 
-    if save_to_file != False:
+    fig = plot_cry_es(bands=bands, doss=doss, k_labels=k_labels, color_bd=color_band,
+                      color_doss=color_dos, fermi=fermi, energy_range=energy_range,
+                      linestl_bd=linestl_band, linestl_doss=linestl_dos,
+                      linewidth=linewidth, prj=dos_prj, figsize=figsize, labels=labels,
+                      dos_max_range=dos_max_range, title=title, dos_beta=dos_beta)
+    if is_ev == True:
+        fig.supylabel('Energy (eV)')
+    else:
+        fig.supylabel('Energy (Hartree)')
+
+    if save_to_file != None:
         save_plot(save_to_file)
 
     plt.show()
 
 
-def plot_cry_es(bands, doss, k_labels: list = None, save_to_file=False, color_bd='blue', color_doss='blue', fermi='forestgreen', energy_range: list = None, linestl_bd='-',
-                linestl_doss=None, linewidth=1, prj: list = None, figsize=None, labels: list = None, dos_max_range: float = None):
+def plot_phonon_banddos(bands, doss, unit='cm-1', k_labels=None, dos_prj=None,
+                        freq_range=None, dos_max_range=None, color_band='blue',
+                        color_dos='blue', labels=None, linestl_band='-',
+                        linestl_dos=None, linewidth=1, freq0_line=None,
+                        title=None, figsize=None, save_to_file=None):
+    """
+    A wrapper of plot_cry_es for phonon band structure + dos. Only one pair is permitted.
+
+    Args:
+        bands (BandsBASE|list): Bands object generated by CRYSTALpytools.crystal_io.Properties_output.read_bands
+            or a list of BandsBASE objects.
+        doss (DOSBASE): DOS object generated by CRYSTALpytools.crystal_io.Properties_output.read_doss
+            or a list of DOSBASE objects.
+        unit (str): Unit of frequency. Valid options are 'cm-1' or 'THz'.
+        k_labels (list): A list of high-symmetric k point labels. Greek alphabets should be
+            represented as strings, for example, 'Gamma'.
+        dos_prj (list): Index of selected projection. Consistent with the index of the 2nd dimension
+            of doss.doss.
+        freq_range (list): A list of two values representing the frequency range to be plotted.
+        dos_max_range (float): Maximum DOS range for the y-axis.
+        color_band (str): Color of the phonon bands in the plot.
+        color_dos (str): Color of the density of states (DOS) in the plot.
+        labels (list): A list of labels for the plot legend.
+        linestl_band (str): Linestyle of the phonon bands.
+        linestl_dos (str): Linestyle of the density of states (DOS).
+        linewidth (float): Width of the lines in the plot.
+        freq0_line (str): Color of the frequency=0 line.
+        title (str): Title of the plot.
+        figsize (list[float]): Size of the figure in inches (width, height).
+        save_to_file (str): File name to save the plot.
+
+    Returns:
+        None
+
+    Raises:
+        ValueError: If the unit parameter is unknown.
+
+    """
+    import matplotlib.pyplot as plt
+    from CRYSTALpytools.units import cm_to_thz, thz_to_cm
+    import re
+
+    if re.match(r'^cm\-1$', unit, re.IGNORECASE):
+        unit = 'cm-1'
+        is_thz = False
+    elif re.match(r'^thz$', unit, re.IGNORECASE):
+        unit = 'THz'
+        is_thz = True
+    else:
+        raise ValueError('Unknown unit.')
+
+    if unit != doss.unit:
+        if unit == 'cm-1':
+            doss.doss[:, 0, :] = thz_to_cm(doss.doss[:, 0, :])
+            doss.doss[:, 1:, :] = cm_to_thz(doss.doss[:, 1:, :])
+        else:
+            doss.doss[:, 0, :] = cm_to_thz(doss.doss[:, 0, :])
+            doss.doss[:, 1:, :] = thz_to_cm(doss.doss[:, 1:, :])
+        doss.unit = unit
+    if unit != bands.unit:
+        if unit == 'cm-1':
+            bands.bands[:, :, :] = thz_to_cm(bands.bands[:, :, :])
+        else:
+            bands.bands[:, :, :] = cm_to_thz(bands.bands[:, :, :])
+        bands.unit = unit
+
+    if line_freq0 == None:
+        line_freq0 = (1., 0., 0., 0.) # Transparent
+
+    fig = plot_cry_es(bands=bands, doss=doss, k_labels=k_labels, color_bd=color_band,
+                      color_doss=color_dos, fermi=line_freq0, energy_range=energy_range,
+                      linestl_bd=linestl_band, linestl_doss=linestl_dos,
+                      linewidth=linewidth, prj=dos_prj, figsize=figsize, labels=labels,
+                      dos_max_range=dos_max_range, title=title, dos_beta='up')
+    if is_thz == True:
+        fig.supylabel('Frequency (THz)')
+    else:
+        fig.supylabel('Frequency (cm$^{-1}$)')
+
+    if save_to_file != None:
+        save_plot(save_to_file)
+
+    plt.show()
 
+
+def plot_cry_es(bands, doss, k_labels, color_bd, color_doss, fermi, energy_range, linestl_bd,
+                linestl_doss, linewidth, prj, figsize, labels, dos_max_range, title, dos_beta):
+    """
+    The base function to plot electron / phonon band structure + DOS
+
+    Args:
+        bands (object): Object containing band structure data
+        doss (object): Object containing density of states data
+        k_labels (list or None): List of labels for high symmetry points along the path
+        color_bd (str): Color for the band structure plot
+        color_doss (str or list or tuple): Color(s) for the density of states plot
+        fermi (str): Color for the Fermi level lines
+        energy_range (list or None): Range of energy values for the y-axis
+        linestl_bd (str): Linestyle for the band structure plot
+        linestl_doss (str or list or tuple or None): Linestyle(s) for the density of states plot
+        linewidth (float): Width of the lines
+        prj (list or None): List of projection indices for plotting specific projections
+        figsize (tuple): Figure size (width, height)
+        labels (str or list or tuple or None): Labels for the density of states plot
+        dos_max_range (float or None): Maximum range of the density of states plot
+        title (str or None): Title of the figure
+        dos_beta (str): Beta state for the density of states plot ('up' or 'down')
+
+    Returns:
+        fig (object): Figure object containing the plotted data
+    """
     import numpy as np
     import matplotlib.pyplot as plt
-    import sys
+    import warnings
     from os import path
 
     # Dictionary of greek letters for the band plot in the electronic structure
     greek = {'Alpha': '\u0391', 'Beta': '\u0392', 'Gamma': '\u0393', 'Delta': '\u0394', 'Epsilon': '\u0395', 'Zeta': '\u0396', 'Eta': '\u0397',
              'Theta': '\u0398', 'Iota': '\u0399', 'Kappa': '\u039A', 'Lambda': '\u039B', 'Mu': '\u039C', 'Nu': '\u039D', 'Csi': '\u039E',
              'Omicron': '\u039F', 'Pi': '\u03A0', 'Rho': '\u03A1', 'Sigma': '\u03A3', 'Tau': '\u03A4', 'Upsilon': '\u03A5', 'Phi': '\u03A6',
              'Chi': '\u03A7', 'Psi': '\u03A8', 'Omega': '\u03A9', 'Sigma_1': '\u03A3\u2081'}
 
-    # Error check on linestl_doss length when the prj kwargs is not used
-    if (prj is None) and (len(linestl_doss) != doss.n_proj):
-        if len(linestl_doss) > doss.n_proj:
-            print(
-                'Warning! You have a number of linestl_doss elements is greater than the number of projection!')
-        else:
-            print(
-                "Error! You don't have enough elements in linestl_doss for the number of projection required")
-            sys.exit(1)
-
-    # Error check on labels length when the prj kwargs is not used
-    if (prj is None) and (len(labels) != doss.n_proj):
-        if len(labels) > doss.n_proj:
-            print(
-                'Warning! You have a number of labels greater than the number of projection!')
-        else:
-            print(
-                "Error! You don't have enough elements in labels for the numeber of projection required")
-            sys.exit(1)
-
-    # Error check on linestl_doss length when the prj kwargs is used
-    if (prj is not None) and (len(linestl_doss) != len(prj)):
-        if len(linestl_doss) > len(prj):
-            print(
-                'Warning! You have a number of linestl_doss element greater than the number of projection required(prj elements)!')
+    if isinstance(color_doss, list) or isinstance(color_doss, tuple):
+        # Error check on linestl_doss length when the prj kwargs is not used
+        if (prj is None) and (len(color_doss) != doss.n_proj):
+            if len(color_doss) > doss.n_proj:
+                warnings.warn('You have a number of linestl_doss elements is greater than the number of projection!',
+                              stacklevel=2)
+            else:
+                raise ValueError("You don't have enough elements in linestl_doss for the number of projection required")
+        # Error check on linestl_doss length when the prj kwargs is used
+        elif (prj is not None) and (len(color_doss) != len(prj)):
+            if len(color_doss) > len(prj):
+                warnings.warn('You have a number of linestl_doss element greater than the number of projection required(prj elements)!',
+                              stacklevel=2)
+            else:
+                raise ValueError("You don't have enough elements in linestl_doss for the number of projection required(prj elements)")
+    else:
+        if prj == None:
+            nprj = doss.n_proj
         else:
-            print(
-                "Error! You don't have enough elements in linestl_doss for the number of projection required(prj elements)")
-            sys.exit(1)
-
-    # Error check on labels length when the prj kwargs is used
-    if (prj is not None) and (len(labels) != len(prj)):
-        if len(labels) > len(prj):
-            print(
-                'Warning! You have a number of linestl_doss element greater than the number of projection required(prj elements)!')
+            nprj = len(prj)
+        if nprj > 1:
+            warnings.warn('Only one color / no color is given. All DOS projections are in the same color.')
+        color_doss = [color_doss for i in range(nprj)]
+
+    if isinstance(labels, list) or isinstance(labels, tuple):
+        # Error check on labels length when the prj kwargs is not used
+        if (prj is None) and (len(labels) != doss.n_proj):
+            if len(labels) > doss.n_proj:
+                warnings.warn('You have a number of labels greater than the number of projection!')
+            else:
+                raise ValueError("You don't have enough elements in labels for the numeber of projection required")
+        # Error check on labels length when the prj kwargs is used
+        elif (prj is not None) and (len(labels) != len(prj)):
+            if len(labels) > len(prj):
+                warnings.warn('You have a number of linestl_doss element greater than the number of projection required(prj elements)!',
+                              stacklevel=2)
+            else:
+                raise ValueError("You don't have enough elements in linestl_doss for the number of projection required(prj elements)")
+    else:
+        if prj == None:
+            nprj = doss.n_proj
         else:
-            print(
-                "Error! You don't have enough elements in linestl_doss for the number of projection required(prj elements)")
-            sys.exit(1)
+            nprj = len(prj)
+        if nprj > 1:
+            warnings.warn('Label not given. No label is available for DOS.')
+        labels = [None for i in range(nprj)]
+
+    # DOS beta state
+    if dos_beta == 'up':
+        spin_idx = -1 # DOS in crystal output is distinguished by +/- sign already
+        line_0 = False
+    elif dos_beta == 'down':
+        spin_idx = 1
+        line_0 = True
+    else:
+        raise ValueError("'dos_beta' should be either 'up' or 'down'.")
+    if doss.doss.shape[2] == 2:
+        doss.doss[:, :, 1] = doss.doss[:, :, 1] * spin_idx
 
     # Definition and creation of the figure and the axes
-    fig, axs = plt.subplots(nrows=1, ncols=2,
-                            gridspec_kw={'width_ratios': [2, 1]},
-                            sharex=False, sharey=True, figsize=figsize,
-                            )
+    fig, axs = plt.subplots(nrows=1, ncols=2, gridspec_kw={'width_ratios': [2, 1]},
+                            sharex=False, sharey=True, figsize=figsize)
+    if title != None:
+        fig.suptitle(title)
 
     # Definition of the hsp position variables
     hsp = bands.tick_position
 
     # Error check on k_labels lenght against the HSP poisitions
     if k_labels is not None:
         if len(hsp) != len(k_labels):
             if len(hsp) > len(k_labels):
-                print(
-                    'Error!, you have specified a number of label smalle than the number of High Simmetry Point along the path')
+                raise ValueError('You have specified a number of label smaller than the number of High Simmetry Point along the path')
             elif len(hsp) < len(k_labels):
-                print(
-                    'Error!, you have more labels than the High Simmetry point along the path')
-            sys.exit(1)
+                raise ValueError('You have more labels than the High Simmetry point along the path')
 
     # Local variable definition for the band plot
     dx_bd = bands.k_point_plot
     pltband = bands.bands
     no_bands = np.shape(pltband)[0]
     ymin_bd = np.amin(pltband)
     ymax_bd = np.amax(pltband)
@@ -1363,16 +1874,30 @@
         dx_dos = doss.doss[:, 0]
     elif doss.spin == 2:
         dx_dos = doss.doss[:, 0, :]
         dx_alpha = doss.doss[:, 0, 0]
         dx_beta = doss.doss[:, 0, 1]
 
     # Determination of xmin, xmax, ymin, and ymax
-    xmin_dos = np.amin(doss.doss[:, 1:, :])
-    xmax_dos = np.amax(doss.doss[:, 1:, :])
+    if prj != None:
+        argplt = prj
+    else:
+        argplt = range(1, doss.doss.shape[1])
+
+    # Plot a vertical line at 0 DOS. Only for spin polarized cases
+    if line_0 == True and doss.spin == 2:
+        xmin_dos = np.amin(doss.doss[:, argplt, 1])
+        xmax_dos = np.amax(doss.doss[:, argplt, 0])
+        # make the scale symmetric, for comparison
+        xmin_dos = -max([abs(xmin_dos), abs(xmax_dos)])
+        xmax_dos = -xmin_dos
+    else:
+        xmin_dos = 0.
+        xmax_dos = np.amax(doss.doss[:, argplt, :])
+
     ymin_dos = np.amin(dx_dos)
     ymax_dos = np.amax(dx_dos)
 
     # Plot of all projections
     if prj is None:
         for projection in range(1, doss.n_proj+1):
             if doss.spin == 1:
@@ -1384,68 +1909,66 @@
                                     label=labels[projection-1], linewidth=linewidth)
 
                     else:
                         axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[projection-1],
                                     label=labels[projection-1], linestyle=linestl_doss[projection-1], linewidth=linewidth)
 
                 else:
-                    axs[1].plot(doss.doss[:, projection], dx_dos,
-                                color=color_doss, linewidth=linewidth)
+                    axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[0],
+                                linewidth=linewidth)
 
             elif doss.spin == 2:
                 if doss.n_proj > 1:
                     axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[projection-1],
                                 label=labels[projection-1], linestyle='-', linewidth=linewidth)
-                    axs[1].plot(-doss.doss[:, projection, 1], dx_beta, color=color_doss[projection-1],
+                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[projection-1],
                                 label=labels[projection-1], linestyle='--', linewidth=linewidth)
                 else:
-                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss,
+                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[0],
                                 linestyle='-', linewidth=linewidth)
-                    axs[1].plot(-doss.doss[:, projection, 1], dx_beta, color=color_doss,
+                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[0],
                                 linestyle='--', linewidth=linewidth)
 
     # Plot of a selected number of projections
     else:
         for index, projection in enumerate(prj):
             if doss.spin == 1:
                 if doss.n_proj > 1:
                     if linestl_doss is None:
                         axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[index],
                                     label=labels[index], linewidth=linewidth)
                     else:
                         axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[index],
                                     label=labels[index], linestyle=linestl_doss[index], linewidth=linewidth)
                 else:
-                    axs[1].plot(doss.doss[:, projection], dx_dos,
-                                color=color_doss, linewidth=linewidth)
+                    axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[0],
+                                linewidth=linewidth)
             elif doss.spin == 2:
                 if doss.n_proj > 1:
                     axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[index],
                                 label=labels[index], linestyle='-', linewidth=linewidth)
-                    axs[1].plot(-doss.doss[:, projection, 1], dx_beta, color=color_doss[index],
+                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[index],
                                 label=labels[index], linestyle='--', linewidth=linewidth)
                 else:
-                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss,
+                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[0],
                                 linestyle='-', linewidth=linewidth)
-                    axs[1].plot(-doss.doss[:, projection, 1], dx_beta, color=color_doss,
+                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[0],
                                 linestyle='--', linewidth=linewidth)
 
     if ymin_bd > ymin_dos:
         ymin = ymin_dos
     elif ymin_bd <= ymin_dos:
         ymin = ymin_bd
 
     if ymax_bd >= ymax_dos:
         ymax = ymax_bd
     elif ymax_bd < ymax_dos:
         ymax = ymax_dos
 
     xmax_bd = hsp[len(hsp)-1]
-    xmin_dos = 0
-
     # Plot of HSP lines
     yhsp = np.linspace(ymin-5, ymax+5, 2)
     for j in hsp:
         xhsp = np.ones(2)*j
         axs[0].plot(xhsp, yhsp, color='black', linewidth=0.5)
 
     # Creation if HSP label ticks
@@ -1459,50 +1982,66 @@
                 hsp_label.append(n)
 
     axs[0].set_xticks(hsp)
     if k_labels is not None:
         axs[0].set_xticklabels(hsp_label)
 
     xfermi_bd = np.linspace(xmin_bd, xmax_bd, 2)
-    xfermi_dos = np.linspace(xmin_dos, xmax_dos, 2)
+    xfermi_dos = np.linspace(xmin_dos*1.05, xmax_dos*1.05, 2)
     yfermi = np.zeros(2)
 
     # Plot of fermi level lines both in the band and the doss plot
     axs[0].plot(xfermi_bd, yfermi, color=fermi, linewidth=1.5)
     axs[1].plot(xfermi_dos, yfermi, color=fermi, linewidth=1.5)
 
     axs[0].set_xlim(xmin_bd, xmax_bd)
 
     if dos_max_range is not None:
         xmax_dos = dos_max_range
 
     # if (prj is None) and (doss.n_proj not in prj):
     #    xmax_dos = np.amax(doss.doss[:, 1:doss.n_proj-1, :])
 
-    axs[1].set_xlim(xmin_dos, xmax_dos+5)
+    if line_0 == True:
+        axs[1].plot(np.zeros([2,]), [ymin, ymax], color='black', linewidth=0.5)
+    axs[1].set_xlim(xmin_dos*1.05, xmax_dos*1.05)
 
     if energy_range is not None:
         ymin = energy_range[0]
         ymax = energy_range[1]
 
     plt.ylim(ymin, ymax)
-
-    fig.text(.06, 0.5, '$E-E_F$ (eV)', ha='center',
-             va='center', rotation='vertical')
-
     plt.legend()
 
-    if save_to_file != False:
-        save_plot(save_to_file)
-
-    plt.show()
+    return fig
 
 
 def plot_cry_contour(contour_obj, save_to_file=False):
+    """
+    Plot a contour plot.
+
+    Args:
+        contour_obj (object): Contour object representing the contour plot.
+        save_to_file (bool, optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Plots a contour plot based on the data in the contour object.
+        - Retrieves the data from the contour object and converts it to a 2D list.
+        - Sets the figure size based on x_graph_param and y_graph_param attributes of the contour object.
+        - Sets the x-axis and y-axis labels.
+        - Creates a meshgrid using the x_points and y_points attributes of the contour object.
+        - Defines contour levels, colors, linestyles, and fmt.
+        - Plots the contour plot.
+        - Saves the plot to a file named 'figure_TIPO_YYYY-MM-DD_HHMMSS.jpg' in the current directory.
+        - If save_to_file is True, saves the plot to a file specified by save_to_file parameter.
 
+    """
     import matplotlib.pyplot as plt
     import os
     import numpy as np
     import time
 
     df = contour_obj.df
     n_punti_x = contour_obj.npx
@@ -1552,15 +2091,38 @@
     if save_to_file != False:
         save_plot(save_to_file)
 
     plt.show()
 
 
 def plot_cry_contour_differences(contour_obj, contour_obj_ref, save_to_file=False):
+    """
+    Plot the differences between two contour plots.
+
+    Args:
+        contour_obj (object): Contour object representing the original contour plot.
+        contour_obj_ref (object): Contour object representing the reference contour plot.
+        save_to_file (bool, optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Plots the differences between two contour plots.
+        - Requires the contour objects to have a tipo attribute with values 'SURFLAPP', 'SURFLAPM', 'SURFRHOO', or 'SURFELFB'.
+        - Calculates the difference between the dataframes of the two contour objects.
+        - Sets the figure size based on x_graph_param and y_graph_param attributes of the contour object.
+        - Sets the x-axis and y-axis labels.
+        - Creates a meshgrid using the x_points and y_points attributes of the contour object.
+        - Defines contour levels, colors, and linestyles.
+        - Plots the contour differences.
+        - Saves the plot to a file named 'figure_diff_TIPO_YYYY-MM-DD_HHMMSS.jpg' in the current directory.
+        - If save_to_file is True, saves the plot to a file specified by save_to_file parameter.
 
+    """
     import matplotlib.pyplot as plt
     import os
     import numpy as np
     import time
     import sys
 
     if (contour_obj.tipo == 'SURFLAPP') or (contour_obj.tipo == 'SURFLAPM') or (contour_obj.tipo == 'SURFRHOO') or (contour_obj.tipo == 'SURFELFB'):
@@ -1630,15 +2192,32 @@
     if save_to_file != False:
         save_plot(save_to_file)
 
     plt.show()
 
 
 def plot_cry_xrd(xrd_obj, save_to_file=False):
+    """
+    Plot the X-ray diffraction pattern.
 
+    Args:
+        xrd_obj (object): XRD object containing the data for the X-ray diffraction pattern.
+        save_to_file (bool, optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Plots the X-ray diffraction pattern.
+        - Sets the figure size to [16, 9].
+        - Sets the x-axis limit to (0, 30).
+        - Saves the plot to a file named 'figure_XRD_YYYY-MM-DD_HHMMSS.jpg' in the current directory.
+        - If save_to_file is True, saves the plot to a file specified by save_to_file parameter.
+
+    """
     import matplotlib.pyplot as plt
     import os
     import time
 
     plt.rcParams["figure.figsize"] = [16, 9]
 
     plt.plot(xrd_obj.x, xrd_obj.y)
@@ -1653,15 +2232,31 @@
     if save_to_file != False:
         save_plot(save_to_file)
 
     plt.show()
 
 
 def plot_cry_rholine(rholine_obj, save_to_file=False):
+    """
+    Plot the resistivity as a function of distance.
+
+    Args:
+        rholine_obj (object): Rholine object containing the data for the resistivity.
+        save_to_file (bool, optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Plots the resistivity as a function of distance.
+        - Sets the x-axis label as 'd  [$\AA$]' and the y-axis label as r'$\rho$  [$\frac{e}{\AA^3}$]'.
+        - Saves the plot to a file named 'figure_rholine_YYYY-MM-DD_HHMMSS.jpg' in the current directory.
+        - If save_to_file is True, saves the plot to a file specified by save_to_file parameter.
 
+    """
     import matplotlib.pyplot as plt
     import os
     import time
 
     plt.plot(rholine_obj.x, rholine_obj.y)
 
     plt.xlabel('d  [$\AA$]', fontsize=14)
@@ -1675,15 +2270,31 @@
     if save_to_file != False:
         save_plot(save_to_file)
 
     plt.show()
 
 
 def plot_cry_seebeck_potential(seebeck_obj, save_to_file=False):
+    """
+    Plot the Seebeck coefficient as a function of chemical potential.
 
+    Args:
+        seebeck_obj (object): Seebeck object containing the data for the Seebeck coefficient.
+        save_to_file (bool, optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to choose the direction to plot among S_xx, S_xy, S_xz, S_yx, S_yy, S_yz, S_yz, S_zx, S_zy, S_zz.
+        - Plots the Seebeck coefficient as a function of chemical potential for each temperature.
+        - Distinguishes between n-type and p-type conduction with dashed and solid lines, respectively.
+        - If save_to_file is True, saves the plot to a file named 'seebeck_potential_at_T_K___YYYY-MM-DD_HHMMSS.jpg' for each temperature, and 'seebeck_potential_different_T_YYYY-MM-DD_HHMMSS.jpg' for all temperatures combined.
+
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     case = input(
         'Please, choose the direction you want to plot. \nYou can choose among S_xx, S_xy, S_xz, S_yx, S_yy, S_yz, S_yz, S_zx, S_zy, S_zz\n')
@@ -1801,15 +2412,31 @@
                 '.jpg', format='jpg', dpi=100, bbox_inches='tight')
     plt.show()
     if save_to_file != False:
         save_plot(save_to_file)
 
 
 def plot_cry_sigma_potential(sigma_obj, save_to_file=False):
+    """
+    Plot the electrical conductivity as a function of chemical potential.
+
+    Args:
+        sigma_obj (object): Sigma object containing the data for electrical conductivity.
+        save_to_file (bool, optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to choose the direction to plot among S_xx, S_xy, S_xz, S_yy, S_yz, S_zz.
+        - Plots the electrical conductivity as a function of chemical potential for each temperature.
+        - Distinguishes between n-type and p-type conduction with dashed and solid lines, respectively.
+        - If save_to_file is True, saves the plot to a file named 'sigma_potential_at_T_K___YYYY-MM-DD_HHMMSS.jpg' for each temperature, and 'sigma_potential_different_T_YYYY-MM-DD_HHMMSS.jpg' for all temperatures combined.
 
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     case = input(
         'Please, choose the direction you want to plot. \nYou can choose among S_xx, S_xy, S_xz, S_yy, S_yz, S_zz\n')
@@ -1919,15 +2546,29 @@
                 '.jpg', format='jpg', dpi=100, bbox_inches='tight')
 
     if save_to_file != False:
         save_plot(save_to_file)
 
 
 def plot_cry_seebeck_carrier(seebeck_obj, save_to_file=False):
+    """
+    Plot the Seebeck coefficient as a function of charge carrier concentration.
 
+    Args:
+        seebeck_obj: Seebeck object containing the data for the Seebeck coefficient.
+        save_to_file (optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to choose the direction to plot among S_xx, S_xy, S_xz, S_yx, S_yy, S_yz, S_yz, S_zx, S_zy, S_zz.
+        - Plots the Seebeck coefficient as a function of charge carrier concentration for each temperature, distinguishing between n-type and p-type conduction.
+        - If save_to_file is True, saves the plot to a file named 'seebeck_carrier_at_T_K___YYYY-MM-DD_HHMMSS.jpg' for each temperature, and 'seebeck_carrier_different_T_YYYY-MM-DD_HHMMSS.jpg' for all temperatures combined.
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     case = input(
         'Please, choose the direction you want to plot. \nYou can choose among S_xx, S_xy, S_xz, S_yx, S_yy, S_yz, S_yz, S_zx, S_zy, S_zz\n')
@@ -2041,15 +2682,29 @@
     plt.show()
 
     if save_to_file != False:
         save_plot(save_to_file)
 
 
 def plot_cry_sigma_carrier(sigma_obj, save_to_file=False):
+    """
+    Plot the electrical conductivity as a function of charge carrier concentration.
 
+    Args:
+        sigma_obj: Sigma object containing the data for the electrical conductivity.
+        save_to_file (optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to choose the direction to plot among S_xx, S_xy, S_xz, S_yy, S_yz, S_zz.
+        - Plots the electrical conductivity as a function of charge carrier concentration for each temperature, distinguishing between n-type and p-type conduction.
+        - If save_to_file is True, saves the plot to a file named 'sigma_carrier_at_T_K___YYYY-MM-DD_HHMMSS.jpg' for each temperature, and 'sigma_carrier_different_T_YYYY-MM-DD_HHMMSS.jpg' for all temperatures combined.
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     case = input(
         'Please, choose the direction you want to plot. \nYou can choose among S_xx, S_xy, S_xz, S_yy, S_yz, S_zz\n')
@@ -2155,15 +2810,31 @@
                 '.jpg', format='jpg', dpi=100, bbox_inches='tight')
 
     if save_to_file != False:
         save_plot(save_to_file)
 
 
 def plot_cry_powerfactor_potential(seebeck_obj, sigma_obj, save_to_file=False):
+    """
+    Plot the power factor for different potentials.
 
+    Args:
+        seebeck_obj: Seebeck object containing the data for the Seebeck coefficient.
+        sigma_obj: Sigma object containing the data for the electrical conductivity.
+        save_to_file (optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to choose the direction to plot among PF_xx, PF_xy, PF_xz, PF_yx, PF_yy, PF_yz, PF_yz, PF_zx, PF_zy, PF_zz.
+        - Calculates the power factor using the Seebeck coefficient and electrical conductivity data for each temperature.
+        - Plots the power factor for each temperature as a function of the chemical potential, distinguishing between n-type and p-type conduction.
+        - If save_to_file is True, saves the plot to a file named 'powerfactor_potential_at_T_K___YYYY-MM-DD_HHMMSS.jpg' for each temperature, and 'powerfactor_potential_different_T_YYYY-MM-DD_HHMMSS.jpg' for all temperatures combined.
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     case = input(
         'Please, choose the direction you want to plot. \nYou can choose among PF_xx, PF_xy, PF_xz, PF_yx, PF_yy, PF_yz, PF_yz, PF_zx, PF_zy, PF_zz\n')
@@ -2348,15 +3019,31 @@
     plt.savefig('powerfactor_potential_different_T_' + time.strftime(
         "%Y-%m-%d_%H%M%S") + '.jpg', format='jpg', dpi=100, bbox_inches='tight')
     if save_to_file != False:
         save_plot(save_to_file)
 
 
 def plot_cry_powerfactor_carrier(seebeck_obj, sigma_obj, save_to_file=False):
+    """
+    Plot the power factor for different charge carrier concentrations.
 
+    Args:
+        seebeck_obj: Seebeck object containing the data for the Seebeck coefficient.
+        sigma_obj: Sigma object containing the data for the electrical conductivity.
+        save_to_file (optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to choose the direction to plot among PF_xx, PF_xy, PF_xz, PF_yx, PF_yy, PF_yz, PF_yz, PF_zx, PF_zy, PF_zz.
+        - Calculates the power factor using the Seebeck coefficient and electrical conductivity data for each temperature.
+        - Plots the power factor for each temperature as a function of the charge carrier concentration, distinguishing between n-type and p-type conduction.
+        - If save_to_file is True, saves the plot to a file named 'powerfactor_carrier_at_T_K___YYYY-MM-DD_HHMMSS.jpg' for each temperature, and 'powerfactor_carrier_different_T_YYYY-MM-DD_HHMMSS.jpg' for all temperatures combined.
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     case = input(
         'Please, choose the direction you want to plot. \nYou can choose among PF_xx, PF_xy, PF_xz, PF_yx, PF_yy, PF_yz, PF_yz, PF_zx, PF_zy, PF_zz\n')
@@ -2549,15 +3236,32 @@
     # plt.show()
 
     if save_to_file != False:
         save_plot(save_to_file)
 
 
 def plot_cry_zt(seebeck_obj, sigma_obj, save_to_file=False):
+    """
+    Plot the ZT value for different temperatures.
 
+    Args:
+        seebeck_obj: Seebeck object containing the data for the Seebeck coefficient.
+        sigma_obj: Sigma object containing the data for the electrical conductivity.
+        save_to_file (optional): If True, saves the plot to a file. Default is False.
+
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to input the value of ktot in W-1K-1m-1.
+        - Prompts the user to choose the direction to plot among ZT_xx, ZT_xy, ZT_xz, ZT_yx, ZT_yy, ZT_yz, ZT_yz, ZT_zx, ZT_zy, ZT_zz.
+        - Calculates the ZT value using the Seebeck coefficient and electrical conductivity data.
+        - Plots the ZT value for each temperature as a function of the chemical potential.
+        - If save_to_file is True, saves the plot to a file named 'zt_at_T_K___YYYY-MM-DD_HHMMSS.jpg' for each temperature, and 'zt_different_T_YYYY-MM-DD_HHMMSS.jpg' for all temperatures combined.
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     ktot = float(input(
         'Please insert the value of ktot in W-1K-1m-1'))
@@ -2662,15 +3366,31 @@
     plt.savefig('zt_different_T_' + time.strftime("%Y-%m-%d_%H%M%S") +
                 '.jpg', format='jpg', dpi=100, bbox_inches='tight')
     if save_to_file != False:
         save_plot(save_to_file)
 
 
 def plot_cry_multiseebeck(*seebeck):
+    """
+    Plot the seebeck coefficients from different files as a function of chemical potential.
+
+    Args:
+        *seebeck: Variable number of seebeck objects containing the data for the Seebeck coefficient.
 
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to input the index of the temperature to plot.
+        - Prompts the user to input the lower and higher values of chemical potential to plot in eV.
+        - Prompts the user to choose the direction to plot among S_xx, S_xy, S_xz, S_yx, S_yy, S_yz, S_yz, S_zx, S_zy, S_zz.
+        - Plots the seebeck coefficient for each seebeck object.
+        - Differentiates transport coefficients due to n-type or p-type conduction using dashed and solid lines.
+        - Saves the plot to a file named 'multiseebeckYYYY-MM-DD_HHMMSS.jpg', where YYYY-MM-DD_HHMMSS represents the current date and time.
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     k = int(input(
         'Insert the index of temperature you want to plot \n(i.e. if your temperature are [T1, T2, T3] indexes are [0, 1, 2])'))
@@ -2777,15 +3497,31 @@
         i = 1+i
     plt.title('MultiSeebeck ' + str(n.temp[k]) + ' K')
     plt.savefig('multiseebeck' + time.strftime("%Y-%m-%d_%H%M%S") +
                 '.jpg', format='jpg', dpi=100, bbox_inches='tight')
 
 
 def plot_cry_multisigma(*sigma):
+    """
+    Plot the electrical conductivities from different files as a function of the chemical potential.
+
+    Args:
+        *sigma: Variable number of sigma objects containing the data for the conductivity.
 
+    Returns:
+        None
+
+    Notes:
+        - Prompts the user to input the index of the temperature to plot.
+        - Prompts the user to input the lower and higher values of chemical potential to plot in eV.
+        - Prompts the user to choose the direction to plot among S_xx, S_xy, S_xz, S_yy, S_yz, S_zz.
+        - Plots the electrical conductivity for each sigma object.
+        - Differentiates transport coefficients due to n-type or p-type conduction using dashed and solid lines.
+        - Saves the plot to a file named 'multisigmaYYYY-MM-DD_HHMMSS.jpg', where YYYY-MM-DD_HHMMSS represents the current date and time.
+    """
     import sys
     import matplotlib.pyplot as plt
     import numpy as np
     import time
 
     k = int(input(
         'Insert the index of temperature you want to plot \n(i.e. if your temperature are [T1, T2, T3] indexes are [0, 1, 2])'))
@@ -2885,15 +3621,32 @@
         i = 1+i
     plt.title('MultiSigma ' + str(sigma[0].temp[k]) + ' K')
     plt.savefig('multisigma' + time.strftime("%Y-%m-%d_%H%M%S") +
                 '.jpg', format='jpg', dpi=100, bbox_inches='tight')
 
 
 def plot_cry_lapl_profile(lapl_obj, save_to_file=False):
+    """
+    Plot the Laplacian profile of a crystal.
 
+    Args:
+        lapl_obj (object): Laplacian object containing the data for the Laplacian profile.
+        save_to_file (bool, optional): Indicates whether to save the plot to a file. Defaults to False.
+
+    Returns:
+        None
+
+    Notes:
+        - Plots the Laplacian profile using the data from the Laplacian object.
+        - The x-axis represents the distance in angstroms.
+        - The y-axis represents the Laplacian in electrons per cubic angstrom to the fifth power (e/A^5).
+        - The area under the curve where the Laplacian is negative is filled with a light blue color.
+        - The area under the curve where the Laplacian is positive is filled with a light coral color.
+        - If save_to_file is set to a file path, the plot is saved to that file.
+    """
     import matplotlib.pyplot as plt
     import time
 
     plt.plot(lapl_obj.datax, lapl_obj.datay)
 
     plt.fill_between(lapl_obj.datax, lapl_obj.datay, where=(
         lapl_obj.datay < 0), color='lightblue', interpolate=True)
@@ -2909,15 +3662,30 @@
     if save_to_file != False:
         save_plot(save_to_file)
 
     plt.show()
 
 
 def plot_cry_density_profile(lapl_obj, save_to_file=False):
+    """
+    Plot the density profile of a crystal.
 
+    Args:
+        lapl_obj (object): Laplacian object containing the data for the density profile.
+        save_to_file (bool, optional): Indicates whether to save the plot to a file. Defaults to False.
+
+    Returns:
+        None
+
+    Notes:
+        - Plots the density profile using the data from the Laplacian object.
+        - The x-axis represents the distance in angstroms.
+        - The y-axis represents the density in electrons per cubic angstrom (e/A^3).
+        - If save_to_file is set to a file path, the plot is saved to that file.
+    """
     import matplotlib.pyplot as plt
     import time
 
     plt.plot(lapl_obj.datax, lapl_obj.datay)
 
     plt.xlabel('Distance [A]')
     plt.ylabel('Density [e/A^3]')
@@ -2925,15 +3693,29 @@
     if save_to_file != False:
         save_plot(save_to_file)
 
     plt.show()
 
 
 def plot_cry_young(theta, phi, S):
-
+    """
+    Compute Young's modulus for each direction of the space (i.e., each pair
+    of theta and phi angles).
+
+    Args:
+        theta (float): Theta value.
+        phi (float): Phi value.
+        S (numpy.ndarray): Compliance matrix.
+
+    Returns:
+        float: Young's modulus values.
+
+    Notes:
+        - This function is intended to be called by cry_ela_plot
+    """
     import numpy as np
 
     # C2V = Matrix to refer the Cartesian into Voigt's notation
     # Observe that the matrix should be written as is shown below
     # C2V = np.array([[1,6,5],[6,2,4],[5,4,3]])
     # Since python start counting from zero all numbers must be subtracted by 1
     C2V = np.array(
@@ -2975,15 +3757,29 @@
                     rtmp = a[i] * a[j] * a[k] * a[l] * (S[v, u] / rf)
                     e = e + rtmp
     E_tmp = 1 / e  # is the Young Modulus of each cycle
     return E_tmp
 
 
 def plot_cry_comp(theta, phi, S):
-
+    """
+    Compute linear compressibility for each direction of the space (i.e., each
+    pair of theta and phi angles).
+
+    Args:
+        theta (float): Theta value.
+        phi (float): Phi value.
+        S (numpy.ndarray): Compliance matrix.
+
+    Returns:
+        float: Linear compressibility values.
+
+    Notes:
+        - This function is intended to be called by cry_ela_plot
+    """
     import numpy as np
 
     C2V = np.array(
         [
             [0, 5, 4],
             [5, 1, 3],
             [4, 3, 2]
@@ -3014,15 +3810,32 @@
 
                 rtmp = a[i] * a[j] * (S[v, u] / rf)
                 B = B + rtmp
     return B
 
 
 def plot_cry_shear(theta_1D, phi_1D, S, ndeg, shear_choice):
-
+    """
+    For each direction of the space (i.e., for each pair
+    of theta and phi angles) the shear modulus is computed for the third angle
+    chi and the average, maximum and minimum values are stored.
+
+    Args:
+        theta_1D (numpy.ndarray): One-dimensional array of theta values.
+        phi_1D (numpy.ndarray): One-dimensional array of phi values.
+        S (numpy.ndarray): Compliance matrix.
+        ndeg (int): Number of degrees for discretization.
+        shear_choice (str): Type of shear property to plot. Options: "avg", "min", "max".
+
+    Returns:
+        numpy.ndarray: Shear property array.
+
+    Notes:
+        - This function is intended to be called by cry_ela_plot
+    """
     import numpy as np
 
     C2V = np.array(
         [
             [0, 5, 4],
             [5, 1, 3],
             [4, 3, 2],
@@ -3083,15 +3896,32 @@
     if shear_choice == "min":
         return shear_min
     if shear_choice == "max":
         return shear_max
 
 
 def plot_cry_poisson(theta_1D, phi_1D, S, ndeg, poisson_choice):
-
+    """
+    For each direction of the space (i.e., for each pair
+    of theta and phi angles) the Poisson ratio is computed for the third angle
+    chi and the average, maximum and minimum values are stored.
+
+    Args:
+        theta_1D (numpy.ndarray): One-dimensional array of theta values.
+        phi_1D (numpy.ndarray): One-dimensional array of phi values.
+        S (numpy.ndarray): Compliance matrix.
+        ndeg (int): Number of degrees for discretization.
+        poisson_choice (str): Type of Poisson's ratio to plot. Options: "avg", "min", "max".
+
+    Returns:
+        numpy.ndarray: Poisson's ratio array.
+
+    Notes:
+        - This function is intended to be called by cry_ela_plot
+    """
     import numpy as np
 
     C2V = np.array(
         [
             [0, 5, 4],
             [5, 1, 3],
             [4, 3, 2],
@@ -3155,15 +3985,32 @@
         return poisson_min
     if poisson_choice == "max":
         return poisson_max
 
 
 def plot_cry_ela(choose, ndeg, *args, dpi=200, filetype=".png",
                  transparency=False):
-
+    """
+    Plot crystal elastic properties on the basis of the elastic tensor. A
+    variable number of elastic tensors can be provided in order to get
+    multiple plots in one shot, establishing a fixed color scale among them.
+
+    Args:
+        choose (str): Property to plot. Options: "young", "comp", "shear avg",
+            "shear min", "shear max", "poisson avg", "poisson min", "poisson max".
+        ndeg (int): Number of degrees for discretization.
+        *args: Variable number of elastic tensors.
+        dpi (int, optional): Dots per inch for saving the plot. Default is 200.
+        filetype (str, optional): File format of the output plot. Default is ".png".
+        transparency (bool, optional): Flag indicating whether to make the plot
+            background transparent. Default is False.
+
+    Returns:
+        None
+    """
     import numpy as np
     import matplotlib.pyplot as plt
     import math
     import time
     import sys
     from mpl_toolkits.mplot3d import axes3d, Axes3D
     from matplotlib import cm, colors, animation
@@ -3261,19 +4108,43 @@
         plt.show()
         fig.savefig(choose + time.strftime("%Y-%m-%d_%H%M%S") +
                     filetype, dpi=dpi, transparent=transparency)
 
         # <--
 
 
-def save_plot(path_to_file):
-
+def save_plot(path_to_file, format='png'):
+    """
+    Save the plot as a file.
+
+    Args:
+        path_to_file (str): Path to the output file.
+        format (str, optional): File format of the output plot. Default is 'png'.
+
+    Raises:
+        FileNotFoundError: If the specified folder does not exist.
+
+    Returns:
+        None
+    """
     from os import path
-    import sys
+    import warnings
     import matplotlib.pyplot as plt
 
     folder = path.split(path_to_file)[0]
+    file = path.split(path_to_file)[1]
+    extension = path.splitext(file)[-1]
+    extension_list = ['.png', '.jpg', '.jpeg', '.tif','.pdf', '.svg', '.eps']
+
+    if folder == '':
+        folder = '.'
+    if extension != '':
+        if extension in extension_list:
+            format = extension[1:]
+        else:
+            warnings.warn('Unrecognized file format. PNG format is used.',
+                          stacklevel=2)
+
     if path.exists(folder) == True:
-        plt.savefig('%s.png' % path_to_file)
+        plt.savefig('%s/%s.%s' % (folder, file, format))
     else:
-        print('Error: folder %s does not exist' % path_to_file)
-        sys.exit(1)
+        raise FileNotFoundError('Folder %s does not exist' % path_to_file)
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/unit_test.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/unit_test.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/units.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/units.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,7 +25,14 @@
 
 def au_to_angstrom(length):
     return length*(constants.physical_constants['atomic unit of length'][0] * 1e10)
 
 def angstrom_to_au(length):
     return length/(constants.physical_constants['atomic unit of length'][0] * 1e10)
 
+def cm_to_thz(freq):
+    # Conversion from cm^-1 to THz
+    return freq*(constants.physical_constants['speed of light in vacuum'][0] * 1e-10)
+
+def thz_to_cm(freq):
+    # Conversion from cm^-1 to THz
+    return freq/(constants.physical_constants['speed of light in vacuum'][0] * 1e-10)
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools/utils.py` & `CRYSTALpytools-2023.7.6/CRYSTALpytools/utils.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/PKG-INFO` & `CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.6.7
+Version: 2023.7.6
 Summary: Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.
 Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com
 Project-URL: Bug Tracker, https://github.com/crystal-code-tools/CRYSTALpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.7 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.7.6 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.6.7/CRYSTALpytools.egg-info/SOURCES.txt` & `CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 CRYSTALpytools.egg-info/SOURCES.txt
 CRYSTALpytools.egg-info/dependency_links.txt
 CRYSTALpytools.egg-info/requires.txt
 CRYSTALpytools.egg-info/top_level.txt
 CRYSTALpytools/base/__init__.py
 CRYSTALpytools/base/basisset.py
 CRYSTALpytools/base/crysd12.py
-CRYSTALpytools/base/inputbase.py
+CRYSTALpytools/base/crysout.py
+CRYSTALpytools/base/inputbase.py
+CRYSTALpytools/base/propout.py
```

### Comparing `CRYSTALpytools-2023.6.7/LICENSE.txt` & `CRYSTALpytools-2023.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.6.7/PKG-INFO` & `CRYSTALpytools-2023.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.6.7
+Version: 2023.7.6
 Summary: Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.
 Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com
 Project-URL: Bug Tracker, https://github.com/crystal-code-tools/CRYSTALpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.6.7 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.7.6 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.6.7/README.md` & `CRYSTALpytools-2023.7.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # CRYSTALpytools
 This repository contains functions that allow the user to access the <a href="https://www.crystal.unito.it/index.php">CRYSTAL code</a>, input, output and execution from a python infrastructure, such as Jupyter Notebooks. Although they can achieve this goal on their own, they achieve their full potential when used together with <a href="https://pymatgen.org/index.html">pymatgen</a>. In this latter scenario, the CRYSTALpytools could be seen as
 a layer between CRYSTAL and pymatgen.
 
 In January 2022 the first stable version (v2022.1.10) was released.
 
+## Documentation
+The [documentation site](https://crystal-code-tools.github.io/CRYSTALpytools/) of CRYSTALpytoosl explains the usage of submodules and classes. The latest released version of CRYSTALpytools is available via [PyPI](https://pypi.org/project/CRYSTALpytools/#history).
+
 ## Installation
 
 ### Create a conda/anaconda environment
 This step is not mandatory, but it makes using CRYSTALpytools very smooth. It is, therefore, very recommended. If you are new to anaconda, please follow <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html">these steps</a> to install it on your computer.
 
 Create a new conda environment:
 ``` console
```

#### html2text {}

```diff
@@ -1,41 +1,45 @@
 # CRYSTALpytools This repository contains functions that allow the user to
 access the CRYSTAL_code, input, output and execution from a python
 infrastructure, such as Jupyter Notebooks. Although they can achieve this goal
 on their own, they achieve their full potential when used together with
 pymatgen. In this latter scenario, the CRYSTALpytools could be seen as a layer
 between CRYSTAL and pymatgen. In January 2022 the first stable version
-(v2022.1.10) was released. ## Installation ### Create a conda/anaconda
-environment This step is not mandatory, but it makes using CRYSTALpytools very
-smooth. It is, therefore, very recommended. If you are new to anaconda, please
-follow these_steps to install it on your computer. Create a new conda
-environment: ``` console conda create --name crystal python=3.9 ``` In the line
-above, âcrystalâ is the name of the environment and can be set to any you
-like. The âpython=3.9â ensures that the suitable python distribution is
-installed. Activate the conda environment: ``` console conda activate crystal
-``` ### Install CRYSTALpytools The CRYSTALpytools package can be installed from
-pip. Pip is a package-management system written in Python and is used to
-install and manage software packages (called modules in python). ``` console
-pip install --upgrade CRYSTALpytools ``` Windows users might need to install
-windows-curses. This can be done by using: ``` console pip install windows-
-curses ``` To check that CRYSTALpytools was install please type ``` console
-conda list ``` This will return a list of all the modules installed in the
-environment. Here there should be crystalpytools. If this was not the case,
-something went wrong during the installation. Please check the location of the
-environment that is being displayed. This appears at the beginning of the
-âconda listâ command. The most common mistake at this stage is that the
-environment was not activated as described above. Please note that pip will
-only install the functions and not the example notebooks. This decision was
-taken in order to reduce the volume of data transferred when installing. If you
-are interested in the example notebooks please read the section below. ### Set
-the path to runcry and runprop If you intend to run CRYSTAL on the machine
-where you are running the CRYSTALpytools, the path to your local runcry amd
-runprop needs to be specified. To do so, please run the set_runcry_path and
-set_runprop_path functions: ``` console python 3 from CRYSTALpytools.execute
-import set_runcry_path, set_runprop_path set_runcry_path('path_to_your_runcry')
+(v2022.1.10) was released. ## Documentation The [documentation site](https://
+crystal-code-tools.github.io/CRYSTALpytools/) of CRYSTALpytoosl explains the
+usage of submodules and classes. The latest released version of CRYSTALpytools
+is available via [PyPI](https://pypi.org/project/CRYSTALpytools/#history). ##
+Installation ### Create a conda/anaconda environment This step is not
+mandatory, but it makes using CRYSTALpytools very smooth. It is, therefore,
+very recommended. If you are new to anaconda, please follow these_steps to
+install it on your computer. Create a new conda environment: ``` console conda
+create --name crystal python=3.9 ``` In the line above, âcrystalâ is the
+name of the environment and can be set to any you like. The âpython=3.9â
+ensures that the suitable python distribution is installed. Activate the conda
+environment: ``` console conda activate crystal ``` ### Install CRYSTALpytools
+The CRYSTALpytools package can be installed from pip. Pip is a package-
+management system written in Python and is used to install and manage software
+packages (called modules in python). ``` console pip install --upgrade
+CRYSTALpytools ``` Windows users might need to install windows-curses. This can
+be done by using: ``` console pip install windows-curses ``` To check that
+CRYSTALpytools was install please type ``` console conda list ``` This will
+return a list of all the modules installed in the environment. Here there
+should be crystalpytools. If this was not the case, something went wrong during
+the installation. Please check the location of the environment that is being
+displayed. This appears at the beginning of the âconda listâ command. The
+most common mistake at this stage is that the environment was not activated as
+described above. Please note that pip will only install the functions and not
+the example notebooks. This decision was taken in order to reduce the volume of
+data transferred when installing. If you are interested in the example
+notebooks please read the section below. ### Set the path to runcry and runprop
+If you intend to run CRYSTAL on the machine where you are running the
+CRYSTALpytools, the path to your local runcry amd runprop needs to be
+specified. To do so, please run the set_runcry_path and set_runprop_path
+functions: ``` console python 3 from CRYSTALpytools.execute import
+set_runcry_path, set_runprop_path set_runcry_path('path_to_your_runcry')
 set_runprop_path('path_to_your_runcry') ``` ## Examples Each function is
 documented in Jupyter Notebooks that can be found in the [example folder]
 (examples/). There is one notebook per function file (e.g. the functions
 contained in crystal_io.py are explained in the example/crystal_io.ipynb
 notebook). ## Tutorials Tutorials can be found in the [tutorial folder]
 (tutorial/) ## Usage The CRYSTALpytools module aims at providing the user a
 python interface to the CRYSTAL code. The central data structure, called
```

### Comparing `CRYSTALpytools-2023.6.7/setup.py` & `CRYSTALpytools-2023.7.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 long_description = 'Python tools for the <a href="https://www.crystal.unito.it/index.php">CRYSTAL code</a> developed and mantained by the CRYSTAL code developers'
 
 setuptools.setup(
     name="CRYSTALpytools",        
-    version="2023.06.07",
+    version="2023.07.06",
     author_email="crystalcodetools@gmail.com",
     description="Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/crystal-code-tools/CRYSTALpytools",
     project_urls={
         "Bug Tracker": "https://github.com/crystal-code-tools/CRYSTALpytools/issues",
@@ -17,12 +17,20 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(include=['CRYSTALpytools', 'CRYSTALpytools.*']),
     #python_requires=">=3.8",
     install_requires=[
-    "pymatgen",
-    "mendeleev",
-    "ase"
+	"numpy",
+	"sympy",
+	"scipy",
+	"matplotlib",
+	"pandas",
+	"PyYAML",
+	"mendeleev>=0.14.0",
+    "pymatgen>=2022.7.25",
+	"pymatgen<2023.6.28",
+    "ase>=3.22.1",
+    "basis_set_exchange>=0.9.1"
     ]
 )
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 import setuptools long_description = 'Python tools for the CRYSTAL_code
 developed and mantained by the CRYSTAL code developers' setuptools.setup
-( name="CRYSTALpytools", version="2023.06.07",
+( name="CRYSTALpytools", version="2023.07.06",
 author_email="crystalcodetools@gmail.com", description="Python tools for the
 CRYSTAL code developed and mantained by the CRYSTAL code developers.",
 long_description=long_description, long_description_content_type="text/
 markdown", url="https://github.com/crystal-code-tools/CRYSTALpytools",
 project_urls={ "Bug Tracker": "https://github.com/crystal-code-tools/
 CRYSTALpytools/issues", }, classifiers=[ "Programming Language :: Python :: 3",
 "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",
 ], packages=setuptools.find_packages(include=['CRYSTALpytools',
-'CRYSTALpytools.*']), #python_requires=">=3.8", install_requires=[ "pymatgen",
-"mendeleev", "ase" ] )
+'CRYSTALpytools.*']), #python_requires=">=3.8", install_requires=[ "numpy",
+"sympy", "scipy", "matplotlib", "pandas", "PyYAML", "mendeleev>=0.14.0",
+"pymatgen>=2022.7.25", "pymatgen<2023.6.28", "ase>=3.22.1",
+"basis_set_exchange>=0.9.1" ] )
```

