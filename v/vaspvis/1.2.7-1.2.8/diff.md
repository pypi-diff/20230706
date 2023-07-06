# Comparing `tmp/vaspvis-1.2.7.tar.gz` & `tmp/vaspvis-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaspvis-1.2.7.tar", last modified: Thu Apr  6 19:50:13 2023, max compression
+gzip compressed data, was "vaspvis-1.2.8.tar", last modified: Thu Jul  6 04:01:21 2023, max compression
```

## Comparing `vaspvis-1.2.7.tar` & `vaspvis-1.2.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-04-06 19:50:13.318025 vaspvis-1.2.7/
--rw-rw-r--   0 dd        (1000) dd        (1000)     1056 2023-01-26 14:32:30.000000 vaspvis-1.2.7/LICENSE.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)       72 2023-01-26 14:32:30.000000 vaspvis-1.2.7/MANIFEST.in
--rw-rw-r--   0 dd        (1000) dd        (1000)    11478 2023-04-06 19:50:13.318025 vaspvis-1.2.7/PKG-INFO
--rw-rw-r--   0 dd        (1000) dd        (1000)    11176 2023-01-26 14:32:30.000000 vaspvis-1.2.7/README.md
--rw-rw-r--   0 dd        (1000) dd        (1000)     6277 2023-01-26 14:32:30.000000 vaspvis-1.2.7/example.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-04-06 19:50:13.314025 vaspvis-1.2.7/img/
--rw-rw-r--   0 dd        (1000) dd        (1000)   342587 2023-01-26 14:32:30.000000 vaspvis-1.2.7/img/band_atom_orbitals.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   348428 2023-01-26 14:32:30.000000 vaspvis-1.2.7/img/band_atom_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   308011 2023-01-26 14:32:30.000000 vaspvis-1.2.7/img/band_atoms.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   462542 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_atom_orbitals.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   454083 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_atoms.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   394736 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_element_orbitals.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   439321 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_element_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   450754 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_elements.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   590551 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_orbitals.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   243066 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_plain.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   516200 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_dos_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   278341 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_element_orbital.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   310041 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_element_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   306319 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_elements.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   426076 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_orbital.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   174622 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_plain.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   359336 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/band_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   137295 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_atom_orbitals.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   157059 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_atom_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   163001 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_atoms.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   124882 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_element_orbitals.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   141064 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_element_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   161570 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_elements.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   179699 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_orbitals.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   101917 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_plain.png
--rw-rw-r--   0 dd        (1000) dd        (1000)   170210 2023-01-26 14:32:31.000000 vaspvis-1.2.7/img/dos_spd.png
--rw-rw-r--   0 dd        (1000) dd        (1000)       38 2023-04-06 19:50:13.318025 vaspvis-1.2.7/setup.cfg
--rw-rw-r--   0 dd        (1000) dd        (1000)      788 2023-04-06 19:50:09.000000 vaspvis-1.2.7/setup.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-04-06 19:50:13.314025 vaspvis-1.2.7/vaspvis/
--rw-rw-r--   0 dd        (1000) dd        (1000)      175 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/__init__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)   107676 2023-02-28 20:42:29.000000 vaspvis-1.2.7/vaspvis/band.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     6233 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/charge.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    80193 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/dos.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-04-06 19:50:13.318025 vaspvis-1.2.7/vaspvis/passivator_utils/
--rw-rw-r--   0 dd        (1000) dd        (1000)      136 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/passivator_utils/__init__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    11117 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/passivator_utils/passivator_utils.py
--rw-rw-r--   0 dd        (1000) dd        (1000)   347297 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/standard.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    18075 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/stm.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-04-06 19:50:13.318025 vaspvis-1.2.7/vaspvis/unfold/
--rw-rw-r--   0 dd        (1000) dd        (1000)       22 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/unfold/__init__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     6062 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/unfold/convert.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    19858 2023-04-06 19:48:51.000000 vaspvis-1.2.7/vaspvis/unfold/unfold.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     1774 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/unfold/vasp_constant.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    48732 2023-04-05 15:24:57.000000 vaspvis-1.2.7/vaspvis/unfold/vaspwfc.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    38651 2023-01-26 14:32:31.000000 vaspvis-1.2.7/vaspvis/utils.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-04-06 19:50:13.314025 vaspvis-1.2.7/vaspvis.egg-info/
--rw-rw-r--   0 dd        (1000) dd        (1000)    11478 2023-04-06 19:50:13.000000 vaspvis-1.2.7/vaspvis.egg-info/PKG-INFO
--rw-rw-r--   0 dd        (1000) dd        (1000)     1154 2023-04-06 19:50:13.000000 vaspvis-1.2.7/vaspvis.egg-info/SOURCES.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)        1 2023-04-06 19:50:13.000000 vaspvis-1.2.7/vaspvis.egg-info/dependency_links.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)       82 2023-04-06 19:50:13.000000 vaspvis-1.2.7/vaspvis.egg-info/requires.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)        8 2023-04-06 19:50:13.000000 vaspvis-1.2.7/vaspvis.egg-info/top_level.txt
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-07-06 04:01:21.837327 vaspvis-1.2.8/
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1056 2023-01-26 14:32:30.000000 vaspvis-1.2.8/LICENSE.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)       72 2023-01-26 14:32:30.000000 vaspvis-1.2.8/MANIFEST.in
+-rw-rw-r--   0 dd        (1000) dd        (1000)    11478 2023-07-06 04:01:21.837327 vaspvis-1.2.8/PKG-INFO
+-rw-rw-r--   0 dd        (1000) dd        (1000)    11176 2023-01-26 14:32:30.000000 vaspvis-1.2.8/README.md
+-rw-rw-r--   0 dd        (1000) dd        (1000)     6277 2023-01-26 14:32:30.000000 vaspvis-1.2.8/example.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-07-06 04:01:21.837327 vaspvis-1.2.8/img/
+-rw-rw-r--   0 dd        (1000) dd        (1000)   342587 2023-01-26 14:32:30.000000 vaspvis-1.2.8/img/band_atom_orbitals.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   348428 2023-01-26 14:32:30.000000 vaspvis-1.2.8/img/band_atom_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   308011 2023-01-26 14:32:30.000000 vaspvis-1.2.8/img/band_atoms.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   462542 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_atom_orbitals.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   454083 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_atoms.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   394736 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_element_orbitals.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   439321 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_element_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   450754 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_elements.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   590551 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_orbitals.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   243066 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_plain.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   516200 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_dos_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   278341 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_element_orbital.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   310041 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_element_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   306319 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_elements.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   426076 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_orbital.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   174622 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_plain.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   359336 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/band_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   137295 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_atom_orbitals.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   157059 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_atom_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   163001 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_atoms.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   124882 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_element_orbitals.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   141064 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_element_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   161570 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_elements.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   179699 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_orbitals.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   101917 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_plain.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)   170210 2023-01-26 14:32:31.000000 vaspvis-1.2.8/img/dos_spd.png
+-rw-rw-r--   0 dd        (1000) dd        (1000)       38 2023-07-06 04:01:21.837327 vaspvis-1.2.8/setup.cfg
+-rw-rw-r--   0 dd        (1000) dd        (1000)      788 2023-07-06 03:59:49.000000 vaspvis-1.2.8/setup.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-07-06 04:01:21.837327 vaspvis-1.2.8/vaspvis/
+-rw-rw-r--   0 dd        (1000) dd        (1000)      175 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/__init__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)   107678 2023-07-06 03:51:33.000000 vaspvis-1.2.8/vaspvis/band.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     6233 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/charge.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    87711 2023-07-06 03:58:46.000000 vaspvis-1.2.8/vaspvis/dos.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-07-06 04:01:21.837327 vaspvis-1.2.8/vaspvis/passivator_utils/
+-rw-rw-r--   0 dd        (1000) dd        (1000)      136 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/passivator_utils/__init__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    11117 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/passivator_utils/passivator_utils.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)   351000 2023-04-07 17:29:10.000000 vaspvis-1.2.8/vaspvis/standard.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    18075 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/stm.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-07-06 04:01:21.837327 vaspvis-1.2.8/vaspvis/unfold/
+-rw-rw-r--   0 dd        (1000) dd        (1000)       22 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/unfold/__init__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     6062 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/unfold/convert.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    19858 2023-04-06 19:48:51.000000 vaspvis-1.2.8/vaspvis/unfold/unfold.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1774 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/unfold/vasp_constant.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    48732 2023-04-05 15:24:57.000000 vaspvis-1.2.8/vaspvis/unfold/vaspwfc.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    38651 2023-01-26 14:32:31.000000 vaspvis-1.2.8/vaspvis/utils.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-07-06 04:01:21.837327 vaspvis-1.2.8/vaspvis.egg-info/
+-rw-rw-r--   0 dd        (1000) dd        (1000)    11478 2023-07-06 04:01:21.000000 vaspvis-1.2.8/vaspvis.egg-info/PKG-INFO
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1154 2023-07-06 04:01:21.000000 vaspvis-1.2.8/vaspvis.egg-info/SOURCES.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)        1 2023-07-06 04:01:21.000000 vaspvis-1.2.8/vaspvis.egg-info/dependency_links.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)       82 2023-07-06 04:01:21.000000 vaspvis-1.2.8/vaspvis.egg-info/requires.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)        8 2023-07-06 04:01:21.000000 vaspvis-1.2.8/vaspvis.egg-info/top_level.txt
```

### Comparing `vaspvis-1.2.7/LICENSE.txt` & `vaspvis-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/PKG-INFO` & `vaspvis-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaspvis
-Version: 1.2.7
+Version: 1.2.8
 Summary: A highly flexible and customizable library for visualizing electronic structure data from VASP calculations
 Home-page: https://github.com/DerekDardzinski/vaspvis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # vaspvis
```

### Comparing `vaspvis-1.2.7/README.md` & `vaspvis-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/example.py` & `vaspvis-1.2.8/example.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_atom_orbitals.png` & `vaspvis-1.2.8/img/band_atom_orbitals.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_atom_spd.png` & `vaspvis-1.2.8/img/band_atom_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_atoms.png` & `vaspvis-1.2.8/img/band_atoms.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_atom_orbitals.png` & `vaspvis-1.2.8/img/band_dos_atom_orbitals.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_atoms.png` & `vaspvis-1.2.8/img/band_dos_atoms.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_element_orbitals.png` & `vaspvis-1.2.8/img/band_dos_element_orbitals.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_element_spd.png` & `vaspvis-1.2.8/img/band_dos_element_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_elements.png` & `vaspvis-1.2.8/img/band_dos_elements.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_orbitals.png` & `vaspvis-1.2.8/img/band_dos_orbitals.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_plain.png` & `vaspvis-1.2.8/img/band_dos_plain.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_dos_spd.png` & `vaspvis-1.2.8/img/band_dos_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_element_orbital.png` & `vaspvis-1.2.8/img/band_element_orbital.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_element_spd.png` & `vaspvis-1.2.8/img/band_element_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_elements.png` & `vaspvis-1.2.8/img/band_elements.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_orbital.png` & `vaspvis-1.2.8/img/band_orbital.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_plain.png` & `vaspvis-1.2.8/img/band_plain.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/band_spd.png` & `vaspvis-1.2.8/img/band_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_atom_orbitals.png` & `vaspvis-1.2.8/img/dos_atom_orbitals.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_atom_spd.png` & `vaspvis-1.2.8/img/dos_atom_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_atoms.png` & `vaspvis-1.2.8/img/dos_atoms.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_element_orbitals.png` & `vaspvis-1.2.8/img/dos_element_orbitals.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_element_spd.png` & `vaspvis-1.2.8/img/dos_element_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_elements.png` & `vaspvis-1.2.8/img/dos_elements.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_orbitals.png` & `vaspvis-1.2.8/img/dos_orbitals.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_plain.png` & `vaspvis-1.2.8/img/dos_plain.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/img/dos_spd.png` & `vaspvis-1.2.8/img/dos_spd.png`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/setup.py` & `vaspvis-1.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="vaspvis",
-    version="1.2.7",
+    version="1.2.8",
     description="A highly flexible and customizable library for visualizing electronic structure data from VASP calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "pymatgen",
         "matplotlib",
```

### Comparing `vaspvis-1.2.7/vaspvis/band.py` & `vaspvis-1.2.8/vaspvis/band.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
                 then spin='up' states will be defined by positive values of this spin-component
                 and spin='down' states will be defined by negative values of this spin-component.
                 This will only be used for showing a pseudo-spin-polarized plot for calculations
                 that have SOC enabled.
             stretch_factor (float): Used to scale the eigenvalues by a certain constant. Useful for comparing to ARPES data.
                 Default is scale_factor = 1.0 (i.e. no scaling)
         """
-
         self.interpolate = interpolate
         self.soc_axis = soc_axis
         self.new_n = new_n
         self.stretch_factor = stretch_factor
         # self.bandgap = bandgap
         # self.printbg = printbg
         self.eigenval = Eigenval(os.path.join(folder, "EIGENVAL"))
@@ -1069,15 +1068,15 @@
         kpath = [f"${k}$" if k != "G" else "$\\Gamma$" for k in labels]
 
         for k in kpoints_index:
             ax.axvline(
                 x=wave_vectors[k], color=vlinecolor, alpha=0.7, linewidth=0.5
             )
 
-        plt.xticks([wave_vectors[k] for k in kpoints_index], kpath)
+        ax.set_xticks([wave_vectors[k] for k in kpoints_index], kpath)
 
     def _get_kticks_unfold(self, ax, wave_vectors, vlinecolor):
         if self.custom_kpath is not None:
             kpath = []
             for i, b in zip(self.custom_kpath_inds, self.custom_kpath_flip):
                 if b:
                     seg = list(reversed(self.kpath[i]))
```

### Comparing `vaspvis-1.2.7/vaspvis/charge.py` & `vaspvis-1.2.8/vaspvis/charge.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis/dos.py` & `vaspvis-1.2.8/vaspvis/dos.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,508 +14,584 @@
 from ase.visualize.plot import plot_atoms
 from pymatgen.io.ase import AseAtomsAdaptor
 import copy
 import time
 import os
 
 import matplotlib as mpl
+
 mpl.rcParams.update(mpl.rcParamsDefault)
 
+
 class Dos:
     """
     This class contains all the methods for contructing density of states plots from the outputs of VASP calculations.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files.
         spin (str): Which spin direction to parse ('up' or 'down')
         combination_method (str): If the spin option is 'both', the combination method can either be additive or substractive
             by passing 'add' or 'sub'. It spin is passed as 'up' or 'down' this option is ignored.
     """
 
     def __init__(
-            self,
-            folder,
-            spin='up',
-            soc_axis=None,
-            combination_method="add",
-            sp_method='percentage',
-            shift_efermi=0,
+        self,
+        folder,
+        spin="up",
+        soc_axis=None,
+        combination_method="add",
+        sp_method="percentage",
+        shift_efermi=0,
     ):
         self.folder = folder
         self.spin = spin
         self.soc_axis = soc_axis
         self.combination_method = combination_method
         self.sp_method = sp_method
-        self.incar = Incar.from_file(
-            os.path.join(folder, 'INCAR')
-        )
-        if 'LORBIT' in self.incar:
-            if self.incar['LORBIT'] >= 11:
+        self.incar = Incar.from_file(os.path.join(folder, "INCAR"))
+        if "LORBIT" in self.incar:
+            if self.incar["LORBIT"] >= 11:
                 self.lorbit = True
             else:
                 self.lorbit = False
         else:
             self.lorbit = False
 
         if self.lorbit:
-            if os.path.isfile(os.path.join(folder, 'dos.npy')) and os.path.isfile(os.path.join(folder, 'projected_dos.npy')):
-                with open(os.path.join(folder, 'dos.npy'), 'rb') as dos_file:
+            if os.path.isfile(
+                os.path.join(folder, "dos.npy")
+            ) and os.path.isfile(os.path.join(folder, "projected_dos.npy")):
+                with open(os.path.join(folder, "dos.npy"), "rb") as dos_file:
                     dos = np.load(dos_file)
-                with open(os.path.join(folder, 'projected_dos.npy'), 'rb') as projected_dos_file:
+                with open(
+                    os.path.join(folder, "projected_dos.npy"), "rb"
+                ) as projected_dos_file:
                     projected_dos = np.load(projected_dos_file)
 
                 self.doscar = {
-                    'total': dos,
-                    'projected': projected_dos,
+                    "total": dos,
+                    "projected": projected_dos,
                 }
             else:
                 if self._check_f_error():
                     self._fix_doscar()
 
-                self.doscar = VaspDoscar.parse_doscar(os.path.join(folder, 'DOSCAR'))
-                np.save(os.path.join(folder, 'dos.npy'), self.doscar['total'])
-                np.save(os.path.join(folder, 'projected_dos.npy'), self.doscar['projected'])
+                self.doscar = VaspDoscar.parse_doscar(
+                    os.path.join(folder, "DOSCAR")
+                )
+                np.save(os.path.join(folder, "dos.npy"), self.doscar["total"])
+                np.save(
+                    os.path.join(folder, "projected_dos.npy"),
+                    self.doscar["projected"],
+                )
         else:
-            if os.path.isfile(os.path.join(folder, 'dos.npy')):
-                with open(os.path.join(folder, 'dos.npy'), 'rb') as dos_file:
+            if os.path.isfile(os.path.join(folder, "dos.npy")):
+                with open(os.path.join(folder, "dos.npy"), "rb") as dos_file:
                     dos = np.load(dos_file)
 
                 self.doscar = {
-                    'total': dos,
+                    "total": dos,
                 }
             else:
-                self.doscar = VaspDoscar.parse_doscar(os.path.join(folder, 'DOSCAR'))
-                np.save(os.path.join(folder, 'dos.npy'), self.doscar['total'])
+                self.doscar = VaspDoscar.parse_doscar(
+                    os.path.join(folder, "DOSCAR")
+                )
+                np.save(os.path.join(folder, "dos.npy"), self.doscar["total"])
 
-        self.efermi = float(os.popen(f'grep E-fermi {os.path.join(folder, "OUTCAR")}').read().split()[2]) + shift_efermi
+        self.efermi = (
+            float(
+                os.popen(f'grep E-fermi {os.path.join(folder, "OUTCAR")}')
+                .read()
+                .split()[2]
+            )
+            + shift_efermi
+        )
         self.poscar = Poscar.from_file(
-            os.path.join(folder, 'POSCAR'),
+            os.path.join(folder, "POSCAR"),
             check_for_POTCAR=False,
-            read_velocities=False
+            read_velocities=False,
         )
         self.forbitals = self._check_f_orb()
         self.color_dict = {
-            0: '#FF0000',
-            1: '#0000FF',
-            2: '#008000',
-            3: '#800080',
-            4: '#E09200',
-            5: '#FF5C77',
-            6: '#778392',
-            7: '#07C589',
-            8: '#40BAF2',
-            9: '#FF0000',
-            10: '#0000FF',
-            11: '#008000',
-            12: '#800080',
-            13: '#E09200',
-            14: '#FF5C77',
-            15: '#778392',
+            0: "#FF0000",
+            1: "#0000FF",
+            2: "#008000",
+            3: "#800080",
+            4: "#E09200",
+            5: "#FF5C77",
+            6: "#778392",
+            7: "#07C589",
+            8: "#40BAF2",
+            9: "#FF0000",
+            10: "#0000FF",
+            11: "#008000",
+            12: "#800080",
+            13: "#E09200",
+            14: "#FF5C77",
+            15: "#778392",
         }
         self.orbital_labels = {
-            0: 's',
-            1: 'p_{y}',
-            2: 'p_{x}',
-            3: 'p_{z}',
-            4: 'd_{xy}',
-            5: 'd_{yz}',
-            6: 'd_{z^{2}}',
-            7: 'd_{xz}',
-            8: 'd_{x^{2}-y^{2}}',
-            9: 'f_{y^{3}x^{2}}',
-            10: 'f_{xyz}',
-            11: 'f_{yz^{2}}',
-            12: 'f_{z^{3}}',
-            13: 'f_{xz^{2}}',
-            14: 'f_{zx^{3}}',
-            15: 'f_{x^{3}}',
+            0: "s",
+            1: "p_{y}",
+            2: "p_{x}",
+            3: "p_{z}",
+            4: "d_{xy}",
+            5: "d_{yz}",
+            6: "d_{z^{2}}",
+            7: "d_{xz}",
+            8: "d_{x^{2}-y^{2}}",
+            9: "f_{y^{3}x^{2}}",
+            10: "f_{xyz}",
+            11: "f_{yz^{2}}",
+            12: "f_{z^{3}}",
+            13: "f_{xz^{2}}",
+            14: "f_{zx^{3}}",
+            15: "f_{x^{3}}",
         }
         self.spd_relations = {
-            's': 0,
-            'p': 1,
-            'd': 2,
-            'f': 3,
+            "s": 0,
+            "p": 1,
+            "d": 2,
+            "f": 3,
         }
 
-        if 'LSORBIT' in self.incar:
-            if self.incar['LSORBIT']:
+        if "LSORBIT" in self.incar:
+            if self.incar["LSORBIT"]:
                 self.lsorbit = True
             else:
                 self.lsorbit = False
         else:
             self.lsorbit = False
 
-        if 'ISPIN' in self.incar:
-            if self.incar['ISPIN'] == 2:
+        if "ISPIN" in self.incar:
+            if self.incar["ISPIN"] == 2:
                 self.ispin = True
             else:
                 self.ispin = False
         else:
             self.ispin = False
 
-        self.spin_dict = {'up': Spin.up, 'down': Spin.down}
+        self.spin_dict = {"up": Spin.up, "down": Spin.down}
 
         self.tdos_array = self._load_tdos()
 
         if self.lorbit:
             self.pdos_array = self._load_pdos()
 
             if self.lsorbit and self.soc_axis is not None:
-                if self.spin == 'both':
-                    if self.sp_method == 'absolute':
-                        self.tdos_array[:,1] = self.pdos_array.sum(axis=1).sum(axis=1)
-                    elif self.sp_method == 'percentage':
-                        if self.combination_method == 'add':
-                            raise BaseException("If using combination_method='add' and spin orbit coupling is applied, just set spin='up'")
+                if self.spin == "both":
+                    if self.sp_method == "absolute":
+                        self.tdos_array[:, 1] = self.pdos_array.sum(
+                            axis=1
+                        ).sum(axis=1)
+                    elif self.sp_method == "percentage":
+                        if self.combination_method == "add":
+                            raise BaseException(
+                                "If using combination_method='add' and spin orbit coupling is applied, just set spin='up'"
+                            )
                         else:
-                            self.tdos_array[:,1] = (self.pdos_array[0].sum(axis=1).sum(axis=1) - self.pdos_array[1].sum(axis=1).sum(axis=1)) / (self.pdos_array[0].sum(axis=1).sum(axis=1) + self.pdos_array[1].sum(axis=1).sum(axis=1))
-                elif self.spin == 'up':
-                    self.tdos_array[:,1] = self.pdos_array.sum(axis=1).sum(axis=1)
-                elif self.spin == 'down':
-                    self.tdos_array[:,1] = self.pdos_array.sum(axis=1).sum(axis=1)
-
+                            self.tdos_array[:, 1] = (
+                                self.pdos_array[0].sum(axis=1).sum(axis=1)
+                                - self.pdos_array[1].sum(axis=1).sum(axis=1)
+                            ) / (
+                                self.pdos_array[0].sum(axis=1).sum(axis=1)
+                                + self.pdos_array[1].sum(axis=1).sum(axis=1)
+                            )
+                elif self.spin == "up":
+                    self.tdos_array[:, 1] = self.pdos_array.sum(axis=1).sum(
+                        axis=1
+                    )
+                elif self.spin == "down":
+                    self.tdos_array[:, 1] = self.pdos_array.sum(axis=1).sum(
+                        axis=1
+                    )
 
     def _check_f_orb(self):
         f_elements = [
-            'La',
-            'Ac',
-            'Ce',
-            'Tb',
-            'Th',
-            'Pr',
-            'Dy',
-            'Pa',
-            'Nd',
-            'Ho',
-            'U',
-            'Pm',
-            'Er',
-            'Np',
-            'Sm',
-            'Tm',
-            'Pu',
-            'Eu',
-            'Yb',
-            'Am',
-            'Gd',
-            'Lu',
+            "La",
+            "Ac",
+            "Ce",
+            "Tb",
+            "Th",
+            "Pr",
+            "Dy",
+            "Pa",
+            "Nd",
+            "Ho",
+            "U",
+            "Pm",
+            "Er",
+            "Np",
+            "Sm",
+            "Tm",
+            "Pu",
+            "Eu",
+            "Yb",
+            "Am",
+            "Gd",
+            "Lu",
         ]
         f = False
         for element in self.poscar.site_symbols:
             if element in f_elements:
                 f = True
-        
+
         return f
 
     def _check_f_error(self):
-        with open(os.path.join(self.folder, 'DOSCAR'), 'rb') as f:
+        with open(os.path.join(self.folder, "DOSCAR"), "rb") as f:
             f.seek(-2, os.SEEK_END)
-            while f.read(1) != b'\n':
+            while f.read(1) != b"\n":
                 f.seek(-2, os.SEEK_CUR)
             last_line = f.readline().decode()
 
         last_line_len = len(last_line.split())
 
         if last_line_len == 28:
             return True
         else:
             return False
 
     def _fix_doscar(self):
         doscar = []
-        with open(os.path.join(self.folder, 'DOSCAR')) as f:
+        with open(os.path.join(self.folder, "DOSCAR")) as f:
             for line in f:
                 split_line = line.split()
                 doscar.append(split_line)
 
         num_atoms = int(doscar[0][1])
         nedos = int(doscar[5][2])
         nedos_f = 2 * nedos
         start_inds = nedos + 7
 
         top_file = []
 
-        with open(os.path.join(self.folder, 'DOSCAR')) as f:
+        with open(os.path.join(self.folder, "DOSCAR")) as f:
             count = 0
             for line in f:
                 top_file.append(line)
                 count += 1
                 if count == start_inds:
                     break
 
-        a = np.c_[[np.arange(0,nedos_f-1,2),np.arange(1,nedos_f,2)]].T
+        a = np.c_[[np.arange(0, nedos_f - 1, 2), np.arange(1, nedos_f, 2)]].T
         a = np.c_[[a for _ in range(num_atoms)]]
-        b = np.array([1] + [nedos_f for _ in range(num_atoms-1)])
+        b = np.array([1] + [nedos_f for _ in range(num_atoms - 1)])
         c = np.arange(num_atoms)
         d = np.arange(num_atoms)
         d[0] = 1
-        inds = a + (b*c)[:,None,None] + c[:,None,None]
+        inds = a + (b * c)[:, None, None] + c[:, None, None]
         inds += start_inds
 
         new_list = []
 
         for i, ind in enumerate(inds):
             inbetween_ind = np.max(ind) + 1
             for j in ind:
-                new_list.append('\t' + '  '.join(doscar[j[0]] + doscar[j[1]]))
+                new_list.append("\t" + "  ".join(doscar[j[0]] + doscar[j[1]]))
 
-            if i != inds.shape[0]-1:
-                new_list.append('\t' + '    '.join(doscar[inbetween_ind]))
+            if i != inds.shape[0] - 1:
+                new_list.append("\t" + "    ".join(doscar[inbetween_ind]))
 
-        new_doscar = ''.join([''.join(top_file), '\n'.join(new_list)])
+        new_doscar = "".join(["".join(top_file), "\n".join(new_list)])
 
-        os.rename(os.path.join(self.folder, 'DOSCAR'), os.path.join(self.folder, 'DOSCAR_old'))
+        os.rename(
+            os.path.join(self.folder, "DOSCAR"),
+            os.path.join(self.folder, "DOSCAR_old"),
+        )
 
-        with open(os.path.join(self.folder, 'DOSCAR'), 'w') as x:
+        with open(os.path.join(self.folder, "DOSCAR"), "w") as x:
             x.write(new_doscar)
 
     def _load_tdos(self):
         """
         This function loads the total density of states into a dictionary
 
         Returns:
             tdos_dict (dict[str][np.ndarray]): Dictionary that consists or the
                 energies and densities of the system.
         """
 
-        tdos = self.doscar['total']
-        tdos[:,0] = tdos[:,0] - self.efermi
+        tdos = self.doscar["total"]
+        tdos[:, 0] = tdos[:, 0] - self.efermi
 
-        if self.spin == 'up':
-            tdos = tdos[:,:2]
-        elif self.spin == 'down':
-            tdos = tdos[:,[0,2]]
-            tdos[:,1] = -tdos[:,1]
-        elif self.spin == 'both':
-            tdos_up = tdos[:,1]
-            tdos_down = tdos[:,2]
+        if self.spin == "up":
+            tdos = tdos[:, :2]
+        elif self.spin == "down":
+            tdos = tdos[:, [0, 2]]
+            tdos[:, 1] = -tdos[:, 1]
+        elif self.spin == "both":
+            tdos_up = tdos[:, 1]
+            tdos_down = tdos[:, 2]
             if self.combination_method == "add":
-                tdos = np.c_[tdos[:,0], tdos_up + tdos_down]
+                tdos = np.c_[tdos[:, 0], tdos_up + tdos_down]
             if self.combination_method == "sub":
-                if self.sp_method == 'percentage':
-                    tdos = np.c_[tdos[:,0], (tdos_up - tdos_down) / (tdos_up + tdos_down)]
-                elif self.sp_method == 'absolute':
-                    tdos = np.c_[tdos[:,0], tdos_up - tdos_down]
+                if self.sp_method == "percentage":
+                    tdos = np.c_[
+                        tdos[:, 0],
+                        (tdos_up - tdos_down) / (tdos_up + tdos_down),
+                    ]
+                elif self.sp_method == "absolute":
+                    tdos = np.c_[tdos[:, 0], tdos_up - tdos_down]
 
         return tdos
 
-
     def _load_pdos(self):
         """
         This function loads the projected density of states into a dictionary
         of the form:
         atom index --> orbital projections
 
         Returns:
             pdos_dict (dict[int][pd.DataFrame]): Dictionary that contains a data frame
                 with the orbital weights for each atom index.
         """
 
-        pdos = self.doscar['projected']
-        pdos = np.transpose(pdos, axes=(1,0,2))
+        pdos = self.doscar["projected"]
+        pdos = np.transpose(pdos, axes=(1, 0, 2))
 
-        if self.spin == 'up':
+        if self.spin == "up":
             if not self.forbitals:
                 if self.lsorbit:
                     if self.soc_axis is None:
-                        pdos = pdos[:,:,[(j*4) + 1 for j in range(9)]]
-                    elif self.soc_axis == 'x':
-                        pdos = pdos[:,:,[(j*4) + 2 for j in range(9)]]
-                    elif self.soc_axis == 'y':
-                        pdos = pdos[:,:,[(j*4) + 3 for j in range(9)]]
-                    elif self.soc_axis == 'z':
-                        pdos = pdos[:,:,[(j*4) + 4 for j in range(9)]]
+                        pdos = pdos[:, :, [(j * 4) + 1 for j in range(9)]]
+                    elif self.soc_axis == "x":
+                        pdos = pdos[:, :, [(j * 4) + 2 for j in range(9)]]
+                    elif self.soc_axis == "y":
+                        pdos = pdos[:, :, [(j * 4) + 3 for j in range(9)]]
+                    elif self.soc_axis == "z":
+                        pdos = pdos[:, :, [(j * 4) + 4 for j in range(9)]]
 
                     if self.soc_axis is not None:
                         pdos_up = np.zeros(pdos.shape)
                         pdos_up[np.where(pdos > 0)] = pdos[np.where(pdos > 0)]
                         pdos = pdos_up
 
                 elif self.ispin and not self.lsorbit:
-                    pdos = pdos[:,:,[(j*2) + 1 for j in range(9)]]
+                    pdos = pdos[:, :, [(j * 2) + 1 for j in range(9)]]
                 else:
-                    pdos = pdos[:,:,1:]
+                    pdos = pdos[:, :, 1:]
             else:
                 if self.lsorbit:
                     if self.soc_axis is None:
-                        pdos = pdos[:,:,[(j*4) + 1 for j in range(16)]]
-                    if self.soc_axis == 'x':
-                        pdos = pdos[:,:,[(j*4) + 2 for j in range(16)]]
-                    if self.soc_axis == 'y':
-                        pdos = pdos[:,:,[(j*4) + 3 for j in range(16)]]
-                    if self.soc_axis == 'z':
-                        pdos = pdos[:,:,[(j*4) + 4 for j in range(16)]]
+                        pdos = pdos[:, :, [(j * 4) + 1 for j in range(16)]]
+                    if self.soc_axis == "x":
+                        pdos = pdos[:, :, [(j * 4) + 2 for j in range(16)]]
+                    if self.soc_axis == "y":
+                        pdos = pdos[:, :, [(j * 4) + 3 for j in range(16)]]
+                    if self.soc_axis == "z":
+                        pdos = pdos[:, :, [(j * 4) + 4 for j in range(16)]]
 
                     if self.soc_axis is not None:
                         pdos_up = np.zeros(pdos.shape)
                         pdos_up[np.where(pdos > 0)] = pdos[np.where(pdos > 0)]
                         pdos = pdos_up
 
                 elif self.ispin and not self.lsorbit:
-                    pdos = pdos[:,:,[(j*2) + 1 for j in range(16)]]
+                    pdos = pdos[:, :, [(j * 2) + 1 for j in range(16)]]
                 else:
-                    pdos = pdos[:,:,1:]
-        if self.spin == 'down':
+                    pdos = pdos[:, :, 1:]
+        if self.spin == "down":
             if not self.forbitals:
                 if self.lsorbit:
                     if self.soc_axis is None:
-                        raise("You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work.")
-                    elif self.soc_axis == 'x':
-                        pdos = pdos[:,:,[(j*4) + 2 for j in range(9)]]
-                    elif self.soc_axis == 'y':
-                        pdos = pdos[:,:,[(j*4) + 3 for j in range(9)]]
-                    elif self.soc_axis == 'z':
-                        pdos = pdos[:,:,[(j*4) + 4 for j in range(9)]]
+                        raise (
+                            "You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work."
+                        )
+                    elif self.soc_axis == "x":
+                        pdos = pdos[:, :, [(j * 4) + 2 for j in range(9)]]
+                    elif self.soc_axis == "y":
+                        pdos = pdos[:, :, [(j * 4) + 3 for j in range(9)]]
+                    elif self.soc_axis == "z":
+                        pdos = pdos[:, :, [(j * 4) + 4 for j in range(9)]]
 
                     if self.soc_axis is not None:
                         pdos_down = np.zeros(pdos.shape)
-                        pdos_down[np.where(pdos < 0)] = pdos[np.where(pdos < 0)]
+                        pdos_down[np.where(pdos < 0)] = pdos[
+                            np.where(pdos < 0)
+                        ]
                         pdos = pdos_down
 
                 elif self.ispin and not self.lsorbit:
-                    pdos = -pdos[:,:,[(j*2) + 2 for j in range(9)]]
+                    pdos = -pdos[:, :, [(j * 2) + 2 for j in range(9)]]
             else:
                 if self.lsorbit:
                     if self.soc_axis is None:
-                        raise("You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work.")
-                    if self.soc_axis == 'x':
-                        pdos = pdos[:,:,[(j*4) + 2 for j in range(16)]]
-                    if self.soc_axis == 'y':
-                        pdos = pdos[:,:,[(j*4) + 3 for j in range(16)]]
-                    if self.soc_axis == 'z':
-                        pdos = pdos[:,:,[(j*4) + 4 for j in range(16)]]
+                        raise (
+                            "You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work."
+                        )
+                    if self.soc_axis == "x":
+                        pdos = pdos[:, :, [(j * 4) + 2 for j in range(16)]]
+                    if self.soc_axis == "y":
+                        pdos = pdos[:, :, [(j * 4) + 3 for j in range(16)]]
+                    if self.soc_axis == "z":
+                        pdos = pdos[:, :, [(j * 4) + 4 for j in range(16)]]
 
                     if self.soc_axis is not None:
                         pdos_down = np.zeros(pdos.shape)
-                        pdos_down[np.where(pdos < 0)] = pdos[np.where(pdos < 0)]
+                        pdos_down[np.where(pdos < 0)] = pdos[
+                            np.where(pdos < 0)
+                        ]
                         pdos = pdos_down
 
                 elif self.ispin and not self.lsorbit:
-                    pdos = -pdos[:,:,[(j*2) + 2 for j in range(16)]]
-        if self.spin == 'both':
+                    pdos = -pdos[:, :, [(j * 2) + 2 for j in range(16)]]
+        if self.spin == "both":
             if not self.forbitals:
                 if self.lsorbit:
                     if self.soc_axis is None:
-                        raise("You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work.")
-                    elif self.soc_axis == 'x':
-                        pdos = pdos[:,:,[(j*4) + 2 for j in range(9)]]
-                    elif self.soc_axis == 'y':
-                        pdos = pdos[:,:,[(j*4) + 3 for j in range(9)]]
-                    elif self.soc_axis == 'z':
-                        pdos = pdos[:,:,[(j*4) + 4 for j in range(9)]]
+                        raise (
+                            "You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work."
+                        )
+                    elif self.soc_axis == "x":
+                        pdos = pdos[:, :, [(j * 4) + 2 for j in range(9)]]
+                    elif self.soc_axis == "y":
+                        pdos = pdos[:, :, [(j * 4) + 3 for j in range(9)]]
+                    elif self.soc_axis == "z":
+                        pdos = pdos[:, :, [(j * 4) + 4 for j in range(9)]]
 
                     if self.soc_axis is not None:
                         pdos_up = np.zeros(pdos.shape)
                         pdos_up[np.where(pdos > 0)] = pdos[np.where(pdos > 0)]
                         pdos_down = np.zeros(pdos.shape)
-                        pdos_down[np.where(pdos < 0)] = -pdos[np.where(pdos < 0)]
+                        pdos_down[np.where(pdos < 0)] = -pdos[
+                            np.where(pdos < 0)
+                        ]
 
                 elif self.ispin and not self.lsorbit:
-                    pdos_up = pdos[:,:,[(j*2) + 1 for j in range(9)]]
-                    pdos_down = pdos[:,:,[(j*2) + 2 for j in range(9)]]
+                    pdos_up = pdos[:, :, [(j * 2) + 1 for j in range(9)]]
+                    pdos_down = pdos[:, :, [(j * 2) + 2 for j in range(9)]]
             else:
                 if self.lsorbit:
                     if self.soc_axis is None:
-                        raise("You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work.")
-                    if self.soc_axis == 'x':
-                        pdos = pdos[:,:,[(j*4) + 2 for j in range(16)]]
-                    if self.soc_axis == 'y':
-                        pdos = pdos[:,:,[(j*4) + 3 for j in range(16)]]
-                    if self.soc_axis == 'z':
-                        pdos = pdos[:,:,[(j*4) + 4 for j in range(16)]]
+                        raise (
+                            "You have selected spin='down' for a SOC calculation, but soc_axis has not been selected. Please set soc_axis to 'x', 'y', or 'z' for this function to work."
+                        )
+                    if self.soc_axis == "x":
+                        pdos = pdos[:, :, [(j * 4) + 2 for j in range(16)]]
+                    if self.soc_axis == "y":
+                        pdos = pdos[:, :, [(j * 4) + 3 for j in range(16)]]
+                    if self.soc_axis == "z":
+                        pdos = pdos[:, :, [(j * 4) + 4 for j in range(16)]]
 
                     if self.soc_axis is not None:
                         pdos_up = np.zeros(pdos.shape)
                         pdos_up[np.where(pdos > 0)] = pdos[np.where(pdos > 0)]
                         pdos_down = np.zeros(pdos.shape)
-                        pdos_down[np.where(pdos < 0)] = -pdos[np.where(pdos < 0)]
+                        pdos_down[np.where(pdos < 0)] = -pdos[
+                            np.where(pdos < 0)
+                        ]
 
                 elif self.ispin and not self.lsorbit:
-                    pdos_up = pdos[:,:,[(j*2) + 1 for j in range(16)]]
-                    pdos_down = pdos[:,:,[(j*2) + 2 for j in range(16)]]
+                    pdos_up = pdos[:, :, [(j * 2) + 1 for j in range(16)]]
+                    pdos_down = pdos[:, :, [(j * 2) + 2 for j in range(16)]]
 
-            if self.combination_method == 'add':
+            if self.combination_method == "add":
                 pdos = pdos_up + pdos_down
-            if self.combination_method == 'sub':
-                if self.sp_method == 'percentage':
+            if self.combination_method == "sub":
+                if self.sp_method == "percentage":
                     pdos = np.array([pdos_up, pdos_down])
                     #  pdos = (pdos_up - pdos_down) / (pdos_up + pdos_down)
-                elif self.sp_method == 'absolute':
+                elif self.sp_method == "absolute":
                     pdos = pdos_up - pdos_down
 
         return pdos
 
-
     def _sum_spd(self, spd):
         """
         This function sums the weights of the s, p, and d orbitals for each atom
         and creates a dictionary of the form:
         band index --> s,p,d orbital weights
 
         Returns:
             spd_dict (dict([str][pd.DataFrame])): Dictionary that contains the summed weights for the s, p, and d orbitals for each band
         """
 
         if not self.forbitals:
-            spd_indices = [np.array([False for _ in range(9)]) for i in range(3)]
+            spd_indices = [
+                np.array([False for _ in range(9)]) for i in range(3)
+            ]
             spd_indices[0][0] = True
             spd_indices[1][1:4] = True
             spd_indices[2][4:] = True
         else:
-            spd_indices = [np.array([False for _ in range(16)]) for i in range(4)]
+            spd_indices = [
+                np.array([False for _ in range(16)]) for i in range(4)
+            ]
             spd_indices[0][0] = True
             spd_indices[1][1:4] = True
             spd_indices[2][4:9] = True
             spd_indices[3][9:] = True
 
-
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
             orbital_contributions_up = np.sum(self.pdos_array[0], axis=1)
             orbital_contributions_down = np.sum(self.pdos_array[1], axis=1)
 
             spd_contributions_up = np.transpose(
-                np.array([
-                    np.sum(orbital_contributions_up[:,ind], axis=1) for ind in spd_indices
-                ]), axes=[1,0]
+                np.array(
+                    [
+                        np.sum(orbital_contributions_up[:, ind], axis=1)
+                        for ind in spd_indices
+                    ]
+                ),
+                axes=[1, 0],
             )
             spd_contributions_down = np.transpose(
-                np.array([
-                    np.sum(orbital_contributions_down[:,ind], axis=1) for ind in spd_indices
-                ]), axes=[1,0]
+                np.array(
+                    [
+                        np.sum(orbital_contributions_down[:, ind], axis=1)
+                        for ind in spd_indices
+                    ]
+                ),
+                axes=[1, 0],
             )
 
-            spd_contributions_up = spd_contributions_up[:,[self.spd_relations[orb] for orb in spd]]
-            spd_contributions_down = spd_contributions_down[:,[self.spd_relations[orb] for orb in spd]]
+            spd_contributions_up = spd_contributions_up[
+                :, [self.spd_relations[orb] for orb in spd]
+            ]
+            spd_contributions_down = spd_contributions_down[
+                :, [self.spd_relations[orb] for orb in spd]
+            ]
 
             #  spd_contributions = (spd_contributions_up - spd_contributions_down) / (spd_contributions_up + spd_contributions_down)
-            spd_contributions = np.array([spd_contributions_up, spd_contributions_down])
+            spd_contributions = np.array(
+                [spd_contributions_up, spd_contributions_down]
+            )
 
         else:
             orbital_contributions = np.sum(self.pdos_array, axis=1)
 
             spd_contributions = np.transpose(
-                np.array([
-                    np.sum(orbital_contributions[:,ind], axis=1) for ind in spd_indices
-                ]), axes=[1,0]
+                np.array(
+                    [
+                        np.sum(orbital_contributions[:, ind], axis=1)
+                        for ind in spd_indices
+                    ]
+                ),
+                axes=[1, 0],
             )
 
-            spd_contributions = spd_contributions[:,[self.spd_relations[orb] for orb in spd]]
+            spd_contributions = spd_contributions[
+                :, [self.spd_relations[orb] for orb in spd]
+            ]
 
         return spd_contributions
 
-
-
     def _sum_orbitals(self, orbitals):
         """
         This function finds the weights of desired orbitals for all atoms and
             returns a dictionary of the form:
             band index --> orbital index
 
         Parameters:
-            orbitals (list): List of desired orbitals. 
+            orbitals (list): List of desired orbitals.
                 0 = s
                 1 = py
                 2 = pz
                 3 = px
                 4 = dxy
                 5 = dyz
                 6 = dz2
@@ -528,93 +604,133 @@
                 13 = fxz2
                 14 = fzx3
                 15 = fx3
 
         Returns:
             orbital_dict (dict[str][pd.DataFrame]): Dictionary that contains the projected weights of the selected orbitals.
         """
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
             orbital_contributions_up = self.pdos_array[0].sum(axis=1)
             orbital_contributions_down = self.pdos_array[1].sum(axis=1)
 
-            orbital_contributions_up = orbital_contributions_up[:,orbitals]
-            orbital_contributions_down = orbital_contributions_down[:,orbitals]
+            orbital_contributions_up = orbital_contributions_up[:, orbitals]
+            orbital_contributions_down = orbital_contributions_down[
+                :, orbitals
+            ]
 
             #  orbital_contributions = (orbital_contributions_up - orbital_contributions_down) / (orbital_contributions_up + orbital_contributions_down)
-            orbital_contributions = np.array([orbital_contributions_up, orbital_contributions_down])
+            orbital_contributions = np.array(
+                [orbital_contributions_up, orbital_contributions_down]
+            )
         else:
             orbital_contributions = self.pdos_array.sum(axis=1)
-            orbital_contributions = orbital_contributions[:,orbitals]
+            orbital_contributions = orbital_contributions[:, orbitals]
 
         return orbital_contributions
 
     def _sum_atoms(self, atoms, spd=False):
         """
         This function finds the weights of desired atoms for all orbitals and
             returns a dictionary of the form:
             band index --> atom index
 
         Parameters:
             atoms (list): List of desired atoms where atom 0 is the first atom in
-                the POSCAR file. 
+                the POSCAR file.
 
         Returns:
             atom_dict (dict[str][pd.DataFrame]): Dictionary that contains the projected
                 weights of the selected atoms.
         """
 
         if spd:
             if not self.forbitals:
-                spd_indices = [np.array([False for _ in range(9)]) for i in range(3)]
+                spd_indices = [
+                    np.array([False for _ in range(9)]) for i in range(3)
+                ]
                 spd_indices[0][0] = True
                 spd_indices[1][1:4] = True
                 spd_indices[2][4:] = True
             else:
-                spd_indices = [np.array([False for _ in range(16)]) for i in range(4)]
+                spd_indices = [
+                    np.array([False for _ in range(16)]) for i in range(4)
+                ]
                 spd_indices[0][0] = True
                 spd_indices[1][1:4] = True
                 spd_indices[2][4:9] = True
                 spd_indices[3][9:] = True
 
-            if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+            if (
+                self.spin == "both"
+                and self.combination_method == "sub"
+                and self.sp_method == "percentage"
+            ):
                 atoms_spd_up = self.pdos_array[0]
                 atoms_spd_down = self.pdos_array[1]
-                atoms_spd_up = np.transpose(np.array([
-                    np.sum(atoms_spd_up[:,:,ind], axis=2) for ind in spd_indices
-                ]), axes=(1,2,0))
-                atoms_spd_down = np.transpose(np.array([
-                    np.sum(atoms_spd_down[:,:,ind], axis=2) for ind in spd_indices
-                ]), axes=(1,2,0))
+                atoms_spd_up = np.transpose(
+                    np.array(
+                        [
+                            np.sum(atoms_spd_up[:, :, ind], axis=2)
+                            for ind in spd_indices
+                        ]
+                    ),
+                    axes=(1, 2, 0),
+                )
+                atoms_spd_down = np.transpose(
+                    np.array(
+                        [
+                            np.sum(atoms_spd_down[:, :, ind], axis=2)
+                            for ind in spd_indices
+                        ]
+                    ),
+                    axes=(1, 2, 0),
+                )
                 #  atoms_spd = (atoms_spd_up - atoms_spd_down) / (atoms_spd_up + atoms_spd_down)
                 atoms_spd = np.array([atoms_spd_up, atoms_spd_down])
             else:
-                atoms_spd = np.transpose(np.array([
-                    np.sum(self.pdos_array[:,:,ind], axis=2) for ind in spd_indices
-                ]), axes=(1,2,0))
+                atoms_spd = np.transpose(
+                    np.array(
+                        [
+                            np.sum(self.pdos_array[:, :, ind], axis=2)
+                            for ind in spd_indices
+                        ]
+                    ),
+                    axes=(1, 2, 0),
+                )
 
             return atoms_spd
         else:
-            if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+            if (
+                self.spin == "both"
+                and self.combination_method == "sub"
+                and self.sp_method == "percentage"
+            ):
                 atoms_array_up = self.pdos_array[0].sum(axis=2)
                 atoms_array_down = self.pdos_array[1].sum(axis=2)
                 #  atoms_array = (atoms_array_up - atoms_array_down) / (atoms_array_up + atoms_array_down)
                 if atoms is not None:
                     atoms_array_up = atoms_array_up[:, atoms]
                     atoms_array_down = atoms_array_down[:, atoms]
 
                 atoms_array = np.array([atoms_array_up, atoms_array_down])
             else:
                 atoms_array = self.pdos_array.sum(axis=2)
 
                 if atoms is not None:
-                    atoms_array = atoms_array[:,atoms]
+                    atoms_array = atoms_array[:, atoms]
 
             return atoms_array
 
-    def _sum_elements(self, elements, orbitals=False, spd=False, spd_options=None):
+    def _sum_elements(
+        self, elements, orbitals=False, spd=False, spd_options=None
+    ):
         """
         This function sums the weights of the orbitals of specific elements within the
         calculated structure and returns a dictionary of the form:
         band index --> element label --> orbital weights for orbitals = True
         band index --> element label for orbitals = False
         This is useful for structures with many elements because manually entering indicies is
         not practical for large structures.
@@ -630,128 +746,184 @@
             element_dict (dict([str][str][pd.DataFrame])): Dictionary that contains the summed weights for each orbital for a given element in the structure.
         """
 
         poscar = self.poscar
         natoms = poscar.natoms
         symbols = poscar.site_symbols
 
-
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
             pdos_array_up = self.pdos_array[0]
             pdos_array_down = self.pdos_array[1]
 
             element_list = np.hstack(
-                [[symbols[i] for j in range(natoms[i])] for i in range(len(symbols))]
+                [
+                    [symbols[i] for j in range(natoms[i])]
+                    for i in range(len(symbols))
+                ]
             )
 
-            element_indices = [np.where(np.isin(element_list, element))[0] for element in elements]
+            element_indices = [
+                np.where(np.isin(element_list, element))[0]
+                for element in elements
+            ]
 
             element_orbitals_up = np.transpose(
-                np.array([
-                    np.sum(pdos_array_up[:,ind,:], axis=1) for ind in element_indices
-                ]), axes=(1,0,2)
+                np.array(
+                    [
+                        np.sum(pdos_array_up[:, ind, :], axis=1)
+                        for ind in element_indices
+                    ]
+                ),
+                axes=(1, 0, 2),
             )
             element_orbitals_down = np.transpose(
-                np.array([
-                    np.sum(pdos_array_down[:,ind,:], axis=1) for ind in element_indices
-                ]), axes=(1,0,2)
+                np.array(
+                    [
+                        np.sum(pdos_array_down[:, ind, :], axis=1)
+                        for ind in element_indices
+                    ]
+                ),
+                axes=(1, 0, 2),
             )
 
             if orbitals:
                 #  element_orbitals = (element_orbitals_up - element_orbitals_down) / (element_orbitals_up + element_orbitals_down)
-                element_orbitals = np.array([element_orbitals_up, element_orbitals_down])
+                element_orbitals = np.array(
+                    [element_orbitals_up, element_orbitals_down]
+                )
                 return element_orbitals
             elif spd:
                 if not self.forbitals:
-                    spd_indices = [np.array([False for _ in range(9)]) for i in range(3)]
+                    spd_indices = [
+                        np.array([False for _ in range(9)]) for i in range(3)
+                    ]
                     spd_indices[0][0] = True
                     spd_indices[1][1:4] = True
                     spd_indices[2][4:] = True
                 else:
-                    spd_indices = [np.array([False for _ in range(16)]) for i in range(4)]
+                    spd_indices = [
+                        np.array([False for _ in range(16)]) for i in range(4)
+                    ]
                     spd_indices[0][0] = True
                     spd_indices[1][1:4] = True
                     spd_indices[2][4:9] = True
                     spd_indices[3][9:] = True
 
-                element_spd_up = np.transpose(np.array([
-                    np.sum(element_orbitals_up[:,:,ind], axis=2) for ind in spd_indices
-                ]), axes=(1,2,0))
-
-                element_spd_down = np.transpose(np.array([
-                    np.sum(element_orbitals_down[:,:,ind], axis=2) for ind in spd_indices
-                ]), axes=(1,2,0))
+                element_spd_up = np.transpose(
+                    np.array(
+                        [
+                            np.sum(element_orbitals_up[:, :, ind], axis=2)
+                            for ind in spd_indices
+                        ]
+                    ),
+                    axes=(1, 2, 0),
+                )
+
+                element_spd_down = np.transpose(
+                    np.array(
+                        [
+                            np.sum(element_orbitals_down[:, :, ind], axis=2)
+                            for ind in spd_indices
+                        ]
+                    ),
+                    axes=(1, 2, 0),
+                )
 
                 #  element_spd = (element_spd_up - element_spd_down) / (element_spd_up + element_spd_down)
                 element_spd = np.array([element_spd_up, element_spd_down])
 
                 return element_spd
             else:
                 element_array_up = np.sum(element_orbitals_up, axis=2)
                 element_array_down = np.sum(element_orbitals_down, axis=2)
 
                 #  element_array = (element_array_up - element_array_down) / (element_array_up + element_array_down)
-                element_array = np.array([element_array_up, element_array_down])
+                element_array = np.array(
+                    [element_array_up, element_array_down]
+                )
 
                 return element_array
         else:
             pdos_array = self.pdos_array
 
             element_list = np.hstack(
-                [[symbols[i] for j in range(natoms[i])] for i in range(len(symbols))]
+                [
+                    [symbols[i] for j in range(natoms[i])]
+                    for i in range(len(symbols))
+                ]
             )
 
-            element_indices = [np.where(np.isin(element_list, element))[0] for element in elements]
+            element_indices = [
+                np.where(np.isin(element_list, element))[0]
+                for element in elements
+            ]
 
             element_orbitals = np.transpose(
-                np.array([
-                    np.sum(pdos_array[:,ind,:], axis=1) for ind in element_indices
-                ]), axes=(1,0,2)
+                np.array(
+                    [
+                        np.sum(pdos_array[:, ind, :], axis=1)
+                        for ind in element_indices
+                    ]
+                ),
+                axes=(1, 0, 2),
             )
 
             if orbitals:
                 return element_orbitals
             elif spd:
                 if not self.forbitals:
-                    spd_indices = [np.array([False for _ in range(9)]) for i in range(3)]
+                    spd_indices = [
+                        np.array([False for _ in range(9)]) for i in range(3)
+                    ]
                     spd_indices[0][0] = True
                     spd_indices[1][1:4] = True
                     spd_indices[2][4:] = True
                 else:
-                    spd_indices = [np.array([False for _ in range(16)]) for i in range(4)]
+                    spd_indices = [
+                        np.array([False for _ in range(16)]) for i in range(4)
+                    ]
                     spd_indices[0][0] = True
                     spd_indices[1][1:4] = True
                     spd_indices[2][4:9] = True
                     spd_indices[3][9:] = True
 
-                element_spd = np.transpose(np.array([
-                    np.sum(element_orbitals[:,:,ind], axis=2) for ind in spd_indices
-                ]), axes=(1,2,0))
+                element_spd = np.transpose(
+                    np.array(
+                        [
+                            np.sum(element_orbitals[:, :, ind], axis=2)
+                            for ind in spd_indices
+                        ]
+                    ),
+                    axes=(1, 2, 0),
+                )
 
                 return element_spd
             else:
                 element_array = np.sum(element_orbitals, axis=2)
 
                 return element_array
 
-
     def _smear(self, dos, sigma):
         """
         This function applied a 1D gaussian filter to the density of states
 
         Parameters:
             dos (np.ndarray): Array of densities.
             sigma (float): Standard deviation used in the gaussian filter.
 
 
         Returns:
             _smeared_dos (np.ndarray): Array of _smeared densities.
         """
 
-        diff = np.diff(self.tdos_array[:,0])
+        diff = np.diff(self.tdos_array[:, 0])
         avgdiff = np.mean(diff)
         _smeared_dos = gaussian_filter1d(dos, sigma / avgdiff)
 
         return _smeared_dos
 
     def _set_density_lims(
         self,
@@ -761,115 +933,143 @@
         erange,
         energyaxis,
         spin,
         partial=False,
         is_dict=False,
         idx=None,
         multiple=False,
-        log_scale=False
+        log_scale=False,
     ):
         energy_in_plot_index = np.where(
             (tenergy >= erange[0]) & (tenergy <= erange[1])
         )[0]
 
         tdensity = tdensity[energy_in_plot_index]
 
         if len(np.squeeze(tdensity).shape) == 1:
-           density_in_plot = np.squeeze(tdensity) 
+            density_in_plot = np.squeeze(tdensity)
         else:
-            if spin == 'up' or spin == 'both':
+            if spin == "up" or spin == "both":
                 max_index = np.argmax(np.max(tdensity, axis=0))
-                density_in_plot = tdensity[:,max_index]
+                density_in_plot = tdensity[:, max_index]
             else:
                 min_index = np.argmin(np.min(tdensity, axis=0))
-                density_in_plot = tdensity[:,min_index]
+                density_in_plot = tdensity[:, min_index]
 
         if len(ax.lines) == 0:
-            if energyaxis == 'y':
+            if energyaxis == "y":
                 ax.set_ylim(erange)
-                if spin == 'up' or spin == 'both':
+                if spin == "up" or spin == "both":
                     ax.set_xlim(0, np.max(density_in_plot) * 1.1)
                     if log_scale:
-                         ax.set_xlim(np.min(density_in_plot), np.max(density_in_plot) + np.abs(np.max(density_in_plot) * 0.1))
+                        ax.set_xlim(
+                            np.min(density_in_plot),
+                            np.max(density_in_plot)
+                            + np.abs(np.max(density_in_plot) * 0.1),
+                        )
                     else:
                         ax.set_xlim(0, np.max(density_in_plot) * 1.1)
-                elif spin == 'down':
+                elif spin == "down":
                     ax.set_xlim(np.min(density_in_plot) * 1.1, 0)
-            elif energyaxis == 'x':
+            elif energyaxis == "x":
                 ax.set_xlim(erange)
-                if spin == 'up' or spin == 'both':
+                if spin == "up" or spin == "both":
                     if log_scale:
-                         ax.set_ylim(np.min(density_in_plot), np.max(density_in_plot) + np.abs(np.max(density_in_plot) * 0.1))
+                        ax.set_ylim(
+                            np.min(density_in_plot),
+                            np.max(density_in_plot)
+                            + np.abs(np.max(density_in_plot) * 0.1),
+                        )
                     else:
                         ax.set_ylim(0, np.max(density_in_plot) * 1.1)
-                elif spin == 'down':
+                elif spin == "down":
                     ax.set_ylim(np.min(density_in_plot) * 1.1, 0)
         elif len(ax.lines) > 0:
-            if energyaxis == 'y':
+            if energyaxis == "y":
                 ax.set_ylim(erange)
                 xlims = ax.get_xlim()
                 if xlims[0] == 0:
-                    if spin == 'up' or spin == 'both':
+                    if spin == "up" or spin == "both":
                         ax.set_xlim(0, np.max(density_in_plot) * 1.1)
-                    elif spin == 'down':
+                    elif spin == "down":
                         ax.set_xlim(np.min(density_in_plot) * 1.1, xlims[1])
                 if xlims[1] == 0:
-                    if spin == 'up' or spin == 'both':
+                    if spin == "up" or spin == "both":
                         ax.set_xlim(xlims[0], np.max(density_in_plot) * 1.1)
-                    elif spin == 'down':
+                    elif spin == "down":
                         ax.set_xlim(np.min(density_in_plot) * 1.1, 0)
-            elif energyaxis == 'x':
+            elif energyaxis == "x":
                 ax.set_xlim(erange)
                 ylims = ax.get_ylim()
                 if ylims[0] == 0:
-                    if spin == 'up' or spin == 'both':
+                    if spin == "up" or spin == "both":
                         ax.set_ylim(0, np.max(density_in_plot) * 1.1)
-                    elif spin == 'down':
+                    elif spin == "down":
                         ax.set_ylim(np.min(density_in_plot) * 1.1, ylims[1])
                 if ylims[1] == 0:
-                    if spin == 'up' or spin == 'both':
+                    if spin == "up" or spin == "both":
                         ax.set_ylim(ylims[0], np.max(density_in_plot) * 1.1)
-                    elif spin == 'down':
+                    elif spin == "down":
                         ax.set_ylim(np.min(density_in_plot) * 1.1, 0)
 
     def _sum_layers(self, layers, atol=None, custom_layer_inds=None):
         from vaspvis.utils import group_layers
+
         if custom_layer_inds is None:
             groups, _ = group_layers(self.poscar.structure, atol=atol)
         else:
             groups = custom_layer_inds
         atom_densities = self._sum_atoms(atoms=None)
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
-            densities_up = np.vstack([np.sum(np.vstack(atom_densities[0, :,[group]]), axis=1) for group in groups])
-            densities_down = np.vstack([np.sum(np.vstack(atom_densities[1, :,[group]]), axis=1) for group in groups])
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
+            densities_up = np.vstack(
+                [
+                    np.sum(np.vstack(atom_densities[0, :, [group]]), axis=1)
+                    for group in groups
+                ]
+            )
+            densities_down = np.vstack(
+                [
+                    np.sum(np.vstack(atom_densities[1, :, [group]]), axis=1)
+                    for group in groups
+                ]
+            )
             summed_layers_up = np.sum(densities_up[layers], axis=0)
             summed_layers_down = np.sum(densities_down[layers], axis=0)
             summed_layers = np.array([summed_layers_up, summed_layers_down])
         else:
-            densities = np.vstack([np.sum(np.vstack(atom_densities[:,[group]]), axis=1) for group in groups])
+            densities = np.vstack(
+                [
+                    np.sum(np.vstack(atom_densities[:, [group]]), axis=1)
+                    for group in groups
+                ]
+            )
             summed_layers = np.sum(densities[layers], axis=0)
 
         return summed_layers
 
     def _add_legend(self, ax, names, colors, fontsize=10, markersize=4):
         legend_lines = []
         legend_labels = []
         for name, color in zip(names, colors):
-            legend_lines.append(plt.Line2D(
-                [0],
-                [0],
-                marker='o',
-                markersize=markersize,
-                linestyle='',
-                color=color
-            ))
-            legend_labels.append(
-                f'${name}$'
+            legend_lines.append(
+                plt.Line2D(
+                    [0],
+                    [0],
+                    marker="o",
+                    markersize=markersize,
+                    linestyle="",
+                    color=color,
+                )
             )
+            legend_labels.append(f"${name}$")
 
         leg = ax.get_legend()
 
         if leg is None:
             handles = legend_lines
             labels = legend_labels
         else:
@@ -878,77 +1078,102 @@
             handles.extend(legend_lines)
             labels.extend(legend_labels)
 
         ax.legend(
             handles,
             labels,
             ncol=1,
-            loc='upper left',
+            loc="upper left",
             fontsize=fontsize,
             bbox_to_anchor=(1, 1),
             borderaxespad=0,
             frameon=False,
             handletextpad=0.1,
         )
 
-
-    def _plot_projected_general(self, ax, energy, projected_data, colors, sigma, erange, linewidth, alpha_line, alpha, fill, energyaxis, total):
+    def _plot_projected_general(
+        self,
+        ax,
+        energy,
+        projected_data,
+        colors,
+        sigma,
+        erange,
+        linewidth,
+        alpha_line,
+        alpha,
+        fill,
+        energyaxis,
+        total,
+    ):
         energy_in_plot_index = np.where(
             (energy >= erange[0] - 0.5) & (energy <= erange[1] + 0.5)
         )[0]
         energy = energy[energy_in_plot_index]
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
             projected_data_up = projected_data[0]
             projected_data_down = projected_data[1]
 
             projected_data_up = projected_data_up[energy_in_plot_index]
             projected_data_down = projected_data_down[energy_in_plot_index]
 
             unique_colors = np.unique(colors)
 
             if len(unique_colors) == len(colors):
                 plot_colors = colors
             else:
                 unique_inds = [np.isin(colors, c) for c in unique_colors]
                 projected_data_up = np.c_[
-                    [np.sum(projected_data_up[:,i], axis=1) for i in unique_inds]
+                    [
+                        np.sum(projected_data_up[:, i], axis=1)
+                        for i in unique_inds
+                    ]
                 ].transpose()
                 projected_data_down = np.c_[
-                    [np.sum(projected_data_down[:,i], axis=1) for i in unique_inds]
+                    [
+                        np.sum(projected_data_down[:, i], axis=1)
+                        for i in unique_inds
+                    ]
                 ].transpose()
                 plot_colors = unique_colors
 
-            projected_data = (projected_data_up - projected_data_down) / (projected_data_up + projected_data_down)
+            projected_data = (projected_data_up - projected_data_down) / (
+                projected_data_up + projected_data_down
+            )
             projected_data[np.isnan(projected_data)] = 1e-9
 
             if sigma > 0:
                 for i in range(projected_data.shape[-1]):
-                    projected_data[:,i] = self._smear(
-                        projected_data[:,i],
+                    projected_data[:, i] = self._smear(
+                        projected_data[:, i],
                         sigma=sigma,
                     )
         else:
             projected_data = projected_data[energy_in_plot_index]
 
             unique_colors = np.unique(colors)
 
             if len(unique_colors) == len(colors):
                 plot_colors = colors
             else:
                 unique_inds = [np.isin(colors, c) for c in unique_colors]
                 projected_data = np.c_[
-                    [np.sum(projected_data[:,i], axis=1) for i in unique_inds]
+                    [np.sum(projected_data[:, i], axis=1) for i in unique_inds]
                 ].transpose()
                 plot_colors = unique_colors
 
             if sigma > 0:
                 for i in range(projected_data.shape[-1]):
-                    projected_data[:,i] = self._smear(
-                        projected_data[:,i],
+                    projected_data[:, i] = self._smear(
+                        projected_data[:, i],
                         sigma=sigma,
                     )
 
         if total:
             self.plot_plain(
                 ax=ax,
                 linewidth=linewidth,
@@ -968,63 +1193,62 @@
                 energyaxis=energyaxis,
                 spin=self.spin,
                 partial=True,
             )
 
         for i in range(projected_data.shape[-1]):
 
-            pdensity = projected_data[:,i]
+            pdensity = projected_data[:, i]
 
-            if energyaxis == 'y':
+            if energyaxis == "y":
                 ax.plot(
                     pdensity,
                     energy,
                     color=plot_colors[i],
                     linewidth=linewidth,
-                    alpha=alpha_line
+                    alpha=alpha_line,
                 )
 
                 if fill:
                     ax.fill_betweenx(
                         energy,
                         pdensity,
                         0,
                         color=plot_colors[i],
                         alpha=alpha,
                     )
 
-            if energyaxis == 'x':
+            if energyaxis == "x":
                 ax.plot(
                     energy,
                     pdensity,
                     color=plot_colors[i],
                     linewidth=linewidth,
-                    alpha=alpha_line
+                    alpha=alpha_line,
                 )
 
                 if fill:
                     ax.fill_between(
                         energy,
                         pdensity,
                         0,
                         color=plot_colors[i],
                         alpha=alpha,
                     )
 
-
     def plot_plain(
         self,
         ax,
         linewidth=1.5,
         fill=True,
         alpha=0.3,
         alpha_line=1.0,
         sigma=0.05,
-        energyaxis='y',
-        color='black',
+        energyaxis="y",
+        color="black",
         erange=[-6, 6],
         log_scale=False,
     ):
         """
         This function plots the total density of states
 
         Parameters:
@@ -1037,72 +1261,70 @@
             energyaxis (str): Determines the axis to plot the energy on ('x' or 'y')
             color (str): Color of line
             erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         """
 
         tdos_array = self.tdos_array
         energy_in_plot_index = np.where(
-            (tdos_array[:,0] >= erange[0] - 0.5) & (tdos_array[:,0] <= erange[1] + 0.5)
+            (tdos_array[:, 0] >= erange[0] - 0.5)
+            & (tdos_array[:, 0] <= erange[1] + 0.5)
         )[0]
         tdos_array = tdos_array[energy_in_plot_index]
 
         if sigma > 0:
-            tdensity = self._smear(
-                tdos_array[:,1],
-                sigma=sigma
-            )
+            tdensity = self._smear(tdos_array[:, 1], sigma=sigma)
         else:
-            tdensity = tdos_array[:,1]
+            tdensity = tdos_array[:, 1]
 
         if log_scale:
             tdensity = np.log10(tdensity)
             neg_inf_loc = np.isin(tdensity, -np.inf)
             min_val = np.min(tdensity[np.logical_not(neg_inf_loc)])
             tdensity[neg_inf_loc] = min_val
 
         self._set_density_lims(
             ax=ax,
             tdensity=tdensity,
-            tenergy=tdos_array[:,0],
+            tenergy=tdos_array[:, 0],
             erange=erange,
             energyaxis=energyaxis,
             spin=self.spin,
             log_scale=log_scale,
         )
 
-        if energyaxis == 'y':
+        if energyaxis == "y":
             ax.plot(
                 tdensity,
-                tdos_array[:,0],
+                tdos_array[:, 0],
                 linewidth=linewidth,
                 color=color,
-                alpha=alpha_line
+                alpha=alpha_line,
             )
 
             if fill:
                 ax.fill_betweenx(
-                    tdos_array[:,0],
+                    tdos_array[:, 0],
                     tdensity,
                     0,
                     alpha=alpha,
                     color=color,
                 )
 
-        if energyaxis == 'x':
+        if energyaxis == "x":
             ax.plot(
-                tdos_array[:,0],
+                tdos_array[:, 0],
                 tdensity,
                 linewidth=linewidth,
                 color=color,
-                alpha=alpha_line
+                alpha=alpha_line,
             )
 
             if fill:
                 ax.fill_between(
-                    tdos_array[:,0],
+                    tdos_array[:, 0],
                     tdensity,
                     0,
                     color=color,
                     alpha=alpha,
                 )
 
     def plot_ldos(
@@ -1110,21 +1332,21 @@
         ax,
         layers,
         linewidth=1.5,
         fill=False,
         alpha=0.3,
         alpha_line=1.0,
         sigma=0.05,
-        energyaxis='x',
-        color='black',
+        energyaxis="x",
+        color="black",
         log_scale=False,
         erange=[-6, 6],
         atol=None,
         custom_layer_inds=None,
-        linestyle='-',
+        linestyle="-",
     ):
         """
         This function plots the total density of states
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to append the tick labels
             linewidth (float): Linewidth of lines
@@ -1137,82 +1359,99 @@
             erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         """
 
         #  tdos_array = self._sum_layers(layers=layers)
         tdos_array = self.tdos_array
 
         tdensity = self._sum_layers(
-            layers=layers,
-            atol=atol,
-            custom_layer_inds=custom_layer_inds
+            layers=layers, atol=atol, custom_layer_inds=custom_layer_inds
         )
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
-            tdensity = (tdensity[0] - tdensity[1]) / (tdensity[0] + tdensity[1])
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
+            tdensity = (tdensity[0] - tdensity[1]) / (
+                tdensity[0] + tdensity[1]
+            )
             tdensity[np.isnan(tdensity)] = 1e-9
 
         if sigma > 0:
             tdensity = self._smear(tdensity, sigma=sigma)
 
-
         if log_scale:
             tdensity = np.log10(tdensity)
             neg_inf_loc = np.isin(tdensity, -np.inf)
             min_val = np.min(tdensity[np.logical_not(neg_inf_loc)])
             tdensity[neg_inf_loc] = min_val
 
         self._set_density_lims(
             ax=ax,
             tdensity=tdensity,
-            tenergy=tdos_array[:,0],
+            tenergy=tdos_array[:, 0],
             erange=erange,
             energyaxis=energyaxis,
             spin=self.spin,
             log_scale=log_scale,
         )
 
-        if energyaxis == 'y':
+        if energyaxis == "y":
             ax.plot(
                 tdensity,
-                tdos_array[:,0],
+                tdos_array[:, 0],
                 linewidth=linewidth,
                 color=color,
                 alpha=alpha_line,
                 linestyle=linestyle,
             )
 
             if fill:
                 ax.fill_betweenx(
-                    tdos_array[:,0],
+                    tdos_array[:, 0],
                     tdensity,
                     0,
                     alpha=alpha,
                     color=color,
                 )
 
-        if energyaxis == 'x':
+        if energyaxis == "x":
             ax.plot(
-                tdos_array[:,0],
+                tdos_array[:, 0],
                 tdensity,
                 linewidth=linewidth,
                 color=color,
                 alpha=alpha_line,
                 linestyle=linestyle,
             )
 
             if fill:
                 ax.fill_between(
-                    tdos_array[:,0],
+                    tdos_array[:, 0],
                     tdensity,
                     0,
                     color=color,
                     alpha=alpha,
                 )
 
-    def plot_spd(self, ax, orbitals='spd', fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6]):
+    def plot_spd(
+        self,
+        ax,
+        orbitals="spd",
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+    ):
         """
         This function plots the total density of states with the projected
         density of states for the total projections of the s, p, and d orbitals.
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             order (list): Order to plot the projected bands in. This feature helps to
@@ -1234,25 +1473,23 @@
         projected_data = self._sum_spd(spd=orbitals)
 
         if color_list is None:
             color_list = [
                 self.color_dict[0],
                 self.color_dict[1],
                 self.color_dict[2],
-                self.color_dict[4]
+                self.color_dict[4],
             ]
-            colors = np.array(
-                [color_list[i] for i in range(len(orbitals))]
-            )
+            colors = np.array([color_list[i] for i in range(len(orbitals))])
         else:
             colors = color_list
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
@@ -1260,15 +1497,29 @@
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
             self._add_legend(ax, names=[i for i in orbitals], colors=colors)
 
-    def plot_atom_orbitals(self, ax, atom_orbital_dict, fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6]):
+    def plot_atom_orbitals(
+        self,
+        ax,
+        atom_orbital_dict,
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+    ):
         """
         This function plots the total density of states with the projected
         density of states for the projections or orbitals on individual atoms.
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             atom_orbital_pairs (list[list]): List of atoms orbitals pairs in the form of
@@ -1285,43 +1536,58 @@
             erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         """
 
         atom_indices = list(atom_orbital_dict.keys())
         orbital_indices = list(atom_orbital_dict.values())
         number_orbitals = [len(i) for i in orbital_indices]
         atom_indices = np.repeat(atom_indices, number_orbitals)
-        orbital_symbols_long = np.hstack([
-            [self.orbital_labels[o] for o in  orb] for orb in orbital_indices
-        ])
+        orbital_symbols_long = np.hstack(
+            [[self.orbital_labels[o] for o in orb] for orb in orbital_indices]
+        )
         orbital_indices_long = np.hstack(orbital_indices)
         indices = np.vstack([atom_indices, orbital_indices_long]).T
 
         projected_data = self.pdos_array
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
-            projected_data_up = np.transpose(np.array([
-                projected_data[0,:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
-            projected_data_down = np.transpose(np.array([
-                projected_data[1,:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
+            projected_data_up = np.transpose(
+                np.array(
+                    [projected_data[0, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
+            projected_data_down = np.transpose(
+                np.array(
+                    [projected_data[1, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
             projected_data = np.array([projected_data_up, projected_data_down])
         else:
-            projected_data = np.transpose(np.array([
-                projected_data[:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+            projected_data = np.transpose(
+                np.array(
+                    [projected_data[:, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
 
         if color_list is None:
-            colors = np.array([self.color_dict[i] for i in range(len(orbital_indices_long))])
+            colors = np.array(
+                [self.color_dict[i] for i in range(len(orbital_indices_long))]
+            )
         else:
             colors = color_list
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
@@ -1329,20 +1595,36 @@
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
             self._add_legend(
                 ax,
-                names=[f'{i[0]}({i[1]})' for i in zip(atom_indices, orbital_symbols_long)],
-                colors=colors
+                names=[
+                    f"{i[0]}({i[1]})"
+                    for i in zip(atom_indices, orbital_symbols_long)
+                ],
+                colors=colors,
             )
 
-
-    def plot_orbitals(self, ax, orbitals, fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6]):
+    def plot_orbitals(
+        self,
+        ax,
+        orbitals,
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+    ):
         """
         This function plots the total density of states with the projected
         density of states for the projections onto given orbitals
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             orbitals (list): List of orbitals to project onto
@@ -1364,32 +1646,50 @@
         else:
             colors = color_list
 
         projected_data = self._sum_orbitals(orbitals=orbitals)
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
             fill=fill,
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
-            self._add_legend(ax, names=[self.orbital_labels[i] for i in orbitals], colors=colors)
-
+            self._add_legend(
+                ax,
+                names=[self.orbital_labels[i] for i in orbitals],
+                colors=colors,
+            )
 
-    def plot_atoms(self, ax, atoms, fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6], sum_atoms=False):
+    def plot_atoms(
+        self,
+        ax,
+        atoms,
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+        sum_atoms=False,
+    ):
         """
         This function plots the total density of states with the projected density of states on the given atoms.
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             atoms (list): Index of atoms to plot
             fill (bool): Determines wether or not to fill underneath the plot
@@ -1408,25 +1708,25 @@
             colors = np.array([self.color_dict[i] for i in range(len(atoms))])
         else:
             colors = color_list
 
         projected_data = self._sum_atoms(atoms=atoms)
 
         #  if sum_atoms:
-            #  if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
-                #  projected_data_up = np.sum(projected_data[0], axis=1).reshape(-1,1)
-                #  projected_data_up = np.sum(projected_data[1], axis=1).reshape(-1,1)
-                #  colors = [colors[0]]
-            #  else:
-                #  projected_data = np.sum(projected_data, axis=1).reshape(-1,1)
-                #  colors = [colors[0]]
+        #  if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+        #  projected_data_up = np.sum(projected_data[0], axis=1).reshape(-1,1)
+        #  projected_data_up = np.sum(projected_data[1], axis=1).reshape(-1,1)
+        #  colors = [colors[0]]
+        #  else:
+        #  projected_data = np.sum(projected_data, axis=1).reshape(-1,1)
+        #  colors = [colors[0]]
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
@@ -1434,20 +1734,33 @@
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
             self._add_legend(ax, names=atoms, colors=colors)
 
-
-    def plot_atom_spd(self, ax, atom_spd_dict, fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6]):
+    def plot_atom_spd(
+        self,
+        ax,
+        atom_spd_dict,
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+    ):
         """
         This function plots the total density of states with the projected
-        density of states onto the s, p, and d orbitals of specified atoms. 
-        This is useful for supercells where there are many atoms of the same 
+        density of states onto the s, p, and d orbitals of specified atoms.
+        This is useful for supercells where there are many atoms of the same
         atom and it is inconvienient to manually list each index in the POSCAR.
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             atoms (list): List of atom symbols to project onto
             order (list): Order to plot the projected bands in. This feature helps to
                 avoid situations where one projection completely convers the other.
@@ -1465,41 +1778,60 @@
             erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         """
 
         atom_indices = list(atom_spd_dict.keys())
         orbital_symbols = list(atom_spd_dict.values())
         number_orbitals = [len(i) for i in orbital_symbols]
         atom_indices = np.repeat(atom_indices, number_orbitals)
-        orbital_symbols_long = np.hstack([[o for o in  orb] for orb in orbital_symbols])
-        orbital_indices = np.hstack([[self.spd_relations[o] for o in  orb] for orb in orbital_symbols])
+        orbital_symbols_long = np.hstack(
+            [[o for o in orb] for orb in orbital_symbols]
+        )
+        orbital_indices = np.hstack(
+            [[self.spd_relations[o] for o in orb] for orb in orbital_symbols]
+        )
         indices = np.vstack([atom_indices, orbital_indices]).T
 
         projected_data = self._sum_atoms(atoms=atom_indices, spd=True)
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
-            projected_data_up = np.transpose(np.array([
-                projected_data[0,:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
-            projected_data_down = np.transpose(np.array([
-                projected_data[1,:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
+            projected_data_up = np.transpose(
+                np.array(
+                    [projected_data[0, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
+            projected_data_down = np.transpose(
+                np.array(
+                    [projected_data[1, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
             projected_data = np.array([projected_data_up, projected_data_down])
         else:
-            projected_data = np.transpose(np.array([
-                projected_data[:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+            projected_data = np.transpose(
+                np.array(
+                    [projected_data[:, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
 
         if color_list is None:
-            colors = np.array([self.color_dict[i] for i in range(len(orbital_symbols_long))])
+            colors = np.array(
+                [self.color_dict[i] for i in range(len(orbital_symbols_long))]
+            )
         else:
             colors = color_list
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
@@ -1507,22 +1839,39 @@
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
             self._add_legend(
                 ax,
-                names=[f'{i[0]}({i[1]})' for i in zip(atom_indices, orbital_symbols_long)],
-                colors=colors
+                names=[
+                    f"{i[0]}({i[1]})"
+                    for i in zip(atom_indices, orbital_symbols_long)
+                ],
+                colors=colors,
             )
 
-    def plot_elements(self, ax, elements, fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6]):
+    def plot_elements(
+        self,
+        ax,
+        elements,
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+    ):
         """
         This function plots the total density of states with the projected
-        density of states for the projection onto specified elements. This is 
+        density of states for the projection onto specified elements. This is
         useful for supercells where there are many atoms of the same element and
         it is inconvienient to manually list each index in the POSCAR.
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             elements (list): List of element symbols to project onto
             fill (bool): Determines wether or not to fill underneath the plot
@@ -1534,23 +1883,25 @@
             color_list (list): List of colors that is the same length at the elements list
             legend (bool): Determines whether to draw the legend or not
             total (bool): Determines wheth to draw the total density of states or not
             erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         """
 
         if color_list is None:
-            colors = np.array([self.color_dict[i] for i in range(len(elements))])
+            colors = np.array(
+                [self.color_dict[i] for i in range(len(elements))]
+            )
         else:
             colors = color_list
 
         projected_data = self._sum_elements(elements=elements)
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
@@ -1558,18 +1909,32 @@
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
             self._add_legend(ax, names=elements, colors=colors)
 
-    def plot_element_orbitals(self, ax, element_orbital_dict, fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6]):
+    def plot_element_orbitals(
+        self,
+        ax,
+        element_orbital_dict,
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+    ):
         """
         This function plots the total density of states with the projected
-        density of states onto the chosen orbitals of specified elements. This is 
+        density of states onto the chosen orbitals of specified elements. This is
         useful for supercells where there are many atoms of the same element and
         it is inconvienient to manually list each index in the POSCAR.
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             element_orbital_pairs (list[list]): List of element orbital pairs in the form of
                 [[element symbol, orbital index], [element symbol, orbital index], ..]
@@ -1585,42 +1950,63 @@
             erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         """
 
         element_symbols = list(element_orbital_dict.keys())
         orbital_indices = list(element_orbital_dict.values())
         number_orbitals = [len(i) for i in orbital_indices]
         element_symbols_long = np.repeat(element_symbols, number_orbitals)
-        element_indices = np.repeat(range(len(element_symbols)), number_orbitals)
-        orbital_symbols_long = np.hstack([[self.orbital_labels[o] for o in  orb] for orb in orbital_indices])
+        element_indices = np.repeat(
+            range(len(element_symbols)), number_orbitals
+        )
+        orbital_symbols_long = np.hstack(
+            [[self.orbital_labels[o] for o in orb] for orb in orbital_indices]
+        )
         orbital_indices_long = np.hstack(orbital_indices)
         indices = np.vstack([element_indices, orbital_indices_long]).T
 
-        projected_data = self._sum_elements(elements=element_symbols, orbitals=True)
+        projected_data = self._sum_elements(
+            elements=element_symbols, orbitals=True
+        )
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
-            projected_data_up = np.transpose(np.array([
-                projected_data[0, :,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
-            projected_data_down = np.transpose(np.array([
-                projected_data[1, :,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
+            projected_data_up = np.transpose(
+                np.array(
+                    [projected_data[0, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
+            projected_data_down = np.transpose(
+                np.array(
+                    [projected_data[1, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
             projected_data = np.array([projected_data_up, projected_data_down])
         else:
-            projected_data = np.transpose(np.array([
-                projected_data[:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+            projected_data = np.transpose(
+                np.array(
+                    [projected_data[:, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
 
         if color_list is None:
-            colors = np.array([self.color_dict[i] for i in range(len(orbital_indices_long))])
+            colors = np.array(
+                [self.color_dict[i] for i in range(len(orbital_indices_long))]
+            )
         else:
             colors = color_list
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
@@ -1628,23 +2014,40 @@
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
             self._add_legend(
                 ax,
-                names=[f'{i[0]}({i[1]})' for i in zip(element_symbols_long, orbital_symbols_long)],
-                colors=colors
+                names=[
+                    f"{i[0]}({i[1]})"
+                    for i in zip(element_symbols_long, orbital_symbols_long)
+                ],
+                colors=colors,
             )
 
-    def plot_element_spd(self, ax, element_spd_dict, fill=True, alpha=0.3, alpha_line=1.0, linewidth=1.5, sigma=0.05, energyaxis='y', color_list=None, legend=True, total=True, erange=[-6, 6]):
+    def plot_element_spd(
+        self,
+        ax,
+        element_spd_dict,
+        fill=True,
+        alpha=0.3,
+        alpha_line=1.0,
+        linewidth=1.5,
+        sigma=0.05,
+        energyaxis="y",
+        color_list=None,
+        legend=True,
+        total=True,
+        erange=[-6, 6],
+    ):
         """
         This function plots the total density of states with the projected
-        density of states onto the s, p, and d orbitals of specified elements. 
-        This is useful for supercells where there are many atoms of the same 
+        density of states onto the s, p, and d orbitals of specified elements.
+        This is useful for supercells where there are many atoms of the same
         element and it is inconvienient to manually list each index in the POSCAR.
 
         Parameters:
             ax (matplotlib.pyplot.axis): Axis to plot on
             elements (list): List of element symbols to project onto
             order (list): Order to plot the projected bands in. This feature helps to
                 avoid situations where one projection completely convers the other.
@@ -1661,42 +2064,63 @@
             total (bool): Determines wheth to draw the total density of states or not
             erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         """
         element_symbols = list(element_spd_dict.keys())
         orbital_symbols = list(element_spd_dict.values())
         number_orbitals = [len(i) for i in orbital_symbols]
         element_symbols_long = np.repeat(element_symbols, number_orbitals)
-        element_indices = np.repeat(range(len(element_symbols)), number_orbitals)
-        orbital_symbols_long = np.hstack([[o for o in  orb] for orb in orbital_symbols])
-        orbital_indices = np.hstack([[self.spd_relations[o] for o in  orb] for orb in orbital_symbols])
+        element_indices = np.repeat(
+            range(len(element_symbols)), number_orbitals
+        )
+        orbital_symbols_long = np.hstack(
+            [[o for o in orb] for orb in orbital_symbols]
+        )
+        orbital_indices = np.hstack(
+            [[self.spd_relations[o] for o in orb] for orb in orbital_symbols]
+        )
         indices = np.vstack([element_indices, orbital_indices]).T
 
         projected_data = self._sum_elements(elements=element_symbols, spd=True)
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
-            projected_data_up = np.transpose(np.array([
-                projected_data[0,:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
-            projected_data_down = np.transpose(np.array([
-                projected_data[1,:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
+            projected_data_up = np.transpose(
+                np.array(
+                    [projected_data[0, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
+            projected_data_down = np.transpose(
+                np.array(
+                    [projected_data[1, :, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
             projected_data = np.array([projected_data_up, projected_data_down])
         else:
-            projected_data = np.transpose(np.array([
-                projected_data[:,ind[0],ind[1]] for ind in indices
-            ]), axes=(1,0))
+            projected_data = np.transpose(
+                np.array(
+                    [projected_data[:, ind[0], ind[1]] for ind in indices]
+                ),
+                axes=(1, 0),
+            )
 
         if color_list is None:
-            colors = np.array([self.color_dict[i] for i in range(len(orbital_symbols_long))])
+            colors = np.array(
+                [self.color_dict[i] for i in range(len(orbital_symbols_long))]
+            )
         else:
             colors = color_list
 
         self._plot_projected_general(
             ax=ax,
-            energy=self.tdos_array[:,0],
+            energy=self.tdos_array[:, 0],
             projected_data=projected_data,
             colors=colors,
             sigma=sigma,
             erange=erange,
             linewidth=linewidth,
             alpha_line=alpha_line,
             alpha=alpha,
@@ -1704,43 +2128,46 @@
             energyaxis=energyaxis,
             total=total,
         )
 
         if legend:
             self._add_legend(
                 ax,
-                names=[f'{i[0]}({i[1]})' for i in zip(element_symbols_long, orbital_symbols_long)],
-                colors=colors
+                names=[
+                    f"{i[0]}({i[1]})"
+                    for i in zip(element_symbols_long, orbital_symbols_long)
+                ],
+                colors=colors,
             )
 
     def plot_layers(
         self,
         ax,
-        cmap='magma',
+        cmap="magma",
         sigma_energy=0.05,
         sigma_layers=0.75,
-        energyaxis='y',
+        energyaxis="y",
         erange=[-6, 6],
         lrange=None,
         antialiased=False,
         fontsize=6,
         interface_layer=None,
         show_interface_line=False,
-        interface_line_color='white',
+        interface_line_color="white",
         interface_line_width=2,
-        interface_line_style='--',
+        interface_line_style="--",
         log_scale=False,
         contour=False,
         levels=10,
         min_cutoff=1e-7,
         max_cutoff=None,
         atol=None,
         custom_layer_inds=None,
         custom_cbar_label=None,
-        cbar_orientation='vertical',
+        cbar_orientation="vertical",
         show_bounds=False,
         set_bounds=None,
     ):
         """
         This function plots a layer by layer heat map of the density
         of states.
 
@@ -1757,15 +2184,15 @@
             lrange (list): Upper and lower bounds of the layers included in the plot.
             antialiased (bool): Determines if antialiasing is used or not.
             fontsize (float): Fontsize of all the text in the group.
             interface_layer (float or None): If a value is provided, then the axis labels will be
                 shifted accordingly so that the defined interface layer is zero.
             show_interface_line (bool): If True, then a line will be drawn
                 on the plot to identify the interface layer defined by interface_layer.
-            interface_line_color (str): Color of the line drawn on the plot to mark the 
+            interface_line_color (str): Color of the line drawn on the plot to mark the
                 interface.
             interface_line_width (float): Line with of the line marking the interface.
             interface_line_style (str): Style of the line marking the interface.
             log_scale (bool): Determines if the color map is applied in log scale of not.
                 Recommended in order to accurately view the band gap and smaller features.
             contour (bool): Determines if the color map is plotted as a contour plot instead
                 of a heatmap.
@@ -1779,57 +2206,78 @@
                 atomic positions, sometimes the layer grouping algorithm can behave non-idealy.
                 If this is the case, the user can input a list of list that contain the
                 atomic indices in each layers of the material.
             custom_cbar_label (str or None): Custom label for the colorbar
         """
         from vaspvis.utils import group_layers
         import matplotlib.colors as colors
-        energy = self.tdos_array[:,0]
+
+        energy = self.tdos_array[:, 0]
 
         ind = np.where(
-                (erange[0] - 0.1 <= energy) & (energy <= erange[-1] + 0.1)
+            (erange[0] - 0.1 <= energy) & (energy <= erange[-1] + 0.1)
         )
         if custom_layer_inds is None:
             groups, _ = group_layers(self.poscar.structure, atol=atol)
         else:
             groups = custom_layer_inds
 
         atom_index = range(len(groups))
         energies = energy[ind]
-        
+
         atom_densities = self._sum_atoms(atoms=None)
 
-        if self.spin == 'both' and self.combination_method == 'sub' and self.sp_method == 'percentage':
+        if (
+            self.spin == "both"
+            and self.combination_method == "sub"
+            and self.sp_method == "percentage"
+        ):
             atom_densities_up = atom_densities[0, ind].squeeze()
             atom_densities_down = atom_densities[1, ind].squeeze()
-            densities_up = np.vstack([np.sum(np.vstack(atom_densities_up[:, [group]]), axis=1) for group in groups])
-            densities_down = np.vstack([np.sum(np.vstack(atom_densities_down[:, [group]]), axis=1) for group in groups])
-            densities = (densities_up - densities_down) / (densities_up + densities_down)
+            densities_up = np.vstack(
+                [
+                    np.sum(np.vstack(atom_densities_up[:, [group]]), axis=1)
+                    for group in groups
+                ]
+            )
+            densities_down = np.vstack(
+                [
+                    np.sum(np.vstack(atom_densities_down[:, [group]]), axis=1)
+                    for group in groups
+                ]
+            )
+            densities = (densities_up - densities_down) / (
+                densities_up + densities_down
+            )
             densities[np.isnan(densities)] = 1e-9
         else:
             atom_densities = atom_densities[ind]
-            densities = np.vstack([np.sum(np.vstack(atom_densities[:,[group]]), axis=1) for group in groups])
+            densities = np.vstack(
+                [
+                    np.sum(np.vstack(atom_densities[:, [group]]), axis=1)
+                    for group in groups
+                ]
+            )
 
         densities = np.transpose(densities)
 
         if lrange is not None:
-            atom_index = atom_index[lrange[0]:lrange[1]+1]
-            densities = densities[:, lrange[0]:lrange[1]+1]
+            atom_index = atom_index[lrange[0] : lrange[1] + 1]
+            densities = densities[:, lrange[0] : lrange[1] + 1]
 
         if sigma_energy > 0:
             for i in range(densities.shape[-1]):
-                densities[:,i] = self._smear(
-                    densities[:,i],
+                densities[:, i] = self._smear(
+                    densities[:, i],
                     sigma=sigma_energy,
                 )
         if sigma_layers > 0:
             densities = gaussian_filter(densities, sigma=sigma_layers)
 
-
-        f = interp2d(atom_index, energies, densities, kind='cubic')
+        f = interp2d(atom_index, energies, densities, kind="cubic")
         atom_index = np.arange(np.min(atom_index), np.max(atom_index), 0.1)
         densities = f(atom_index, energies)
 
         if log_scale:
             if np.min(densities) <= 0:
                 neg_zero_loc = np.where(densities <= 0)
                 pos_loc = np.where(densities > 0)
@@ -1845,20 +2293,22 @@
                 if min_val < min_cutoff:
                     min_val = min_cutoff
 
             if max_cutoff is not None:
                 max_val = max_cutoff
             else:
                 max_val = np.max(densities)
-                
+
             norm = colors.LogNorm(vmin=min_val, vmax=max_val)
         else:
             if self.combination_method == "sub" and self.spin == "both":
                 if set_bounds is None:
-                    norm_val = np.max(np.abs([np.min(densities), np.max(densities)]))
+                    norm_val = np.max(
+                        np.abs([np.min(densities), np.max(densities)])
+                    )
                 else:
                     norm_val = set_bounds
 
                 norm = colors.Normalize(vmin=-norm_val, vmax=norm_val)
             else:
                 if max_cutoff is not None:
                     max_val = max_cutoff
@@ -1868,89 +2318,87 @@
                 if min_cutoff is not None:
                     min_val = min_cutoff
                 else:
                     min_val = np.min(densities)
 
                 norm = colors.Normalize(vmin=min_val, vmax=max_val)
 
-
         if log_scale:
             lev_exp = np.arange(
-                np.floor(np.log10(densities.min())-1),
-                np.ceil(np.log10(densities.max())+1),
+                np.floor(np.log10(densities.min()) - 1),
+                np.ceil(np.log10(densities.max()) + 1),
             )
             if len(lev_exp) >= levels:
                 pass
             else:
                 if int(levels / len(lev_exp)) >= 3:
                     lev_exp = np.arange(
-                        np.floor(np.log10(densities.min())-1),
-                        np.ceil(np.log10(densities.max())+1),
+                        np.floor(np.log10(densities.min()) - 1),
+                        np.ceil(np.log10(densities.max()) + 1),
                         0.25,
                     )
                 else:
                     lev_exp = np.arange(
-                        np.floor(np.log10(densities.min())-1),
-                        np.ceil(np.log10(densities.max())+1),
+                        np.floor(np.log10(densities.min()) - 1),
+                        np.ceil(np.log10(densities.max()) + 1),
                         0.5,
                     )
             levels = np.power(10, lev_exp)
 
         if interface_layer is not None:
             atom_index -= int(interface_layer)
 
-        if energyaxis == 'y':
+        if energyaxis == "y":
 
             if contour:
                 im = ax.contourf(
-                    atom_index, 
+                    atom_index,
                     energies,
                     densities,
                     cmap=cmap,
                     levels=levels,
                     norm=norm,
                 )
             else:
                 im = ax.pcolormesh(
                     atom_index,
                     energies,
                     densities,
                     cmap=cmap,
-                    shading='gouraud',
+                    shading="gouraud",
                     norm=norm,
                     antialiased=antialiased,
                 )
             ax.xaxis.set_major_locator(MaxNLocator(integer=True))
 
-
             if interface_layer is not None and show_interface_line:
                 ax.axvline(
                     x=0,
                     color=interface_line_color,
                     linestyle=interface_line_style,
                     linewidth=interface_line_width,
                 )
 
-        if energyaxis == 'x':
+        if energyaxis == "x":
             if contour:
                 im = ax.contourf(
                     energies,
-                    atom_index, 
+                    atom_index,
                     densities,
                     cmap=cmap,
                     levels=levels,
                     norm=norm,
                 )
             else:
                 im = ax.pcolormesh(
                     energies,
                     atom_index,
                     np.transpose(densities),
                     cmap=cmap,
-                    shading='gouraud',
+                    shading="gouraud",
                     norm=norm,
                     antialiased=antialiased,
                 )
             ax.yaxis.set_major_locator(MaxNLocator(integer=True))
 
             if interface_layer is not None and show_interface_line:
                 ax.axhline(
@@ -1961,43 +2409,43 @@
                 )
 
         fig = plt.gcf()
         cbar = fig.colorbar(im, ax=ax, orientation=cbar_orientation)
         cbar.ax.tick_params(labelsize=fontsize)
         if custom_cbar_label is None:
             if self.combination_method == "sub" and self.spin == "both":
-                cbar.set_label('Spin Polarization', fontsize=fontsize)
+                cbar.set_label("Spin Polarization", fontsize=fontsize)
                 min_val = im.norm.vmin
                 max_val = im.norm.vmax
                 cbar.set_ticks([min_val, max_val])
                 if not show_bounds:
-                    cbar.set_ticklabels(['Down', 'Up'])
+                    cbar.set_ticklabels(["Down", "Up"])
             else:
-                cbar.set_label('Density of States', fontsize=fontsize)
+                cbar.set_label("Density of States", fontsize=fontsize)
         else:
             cbar.set_label(custom_cbar_label, fontsize=fontsize)
 
-    def plot_structure(self, ax, rotation=[90,90,90]):
+    def plot_structure(self, ax, rotation=[90, 90, 90]):
         structure = self.poscar.structure
         atoms = AseAtomsAdaptor().get_atoms(structure)
         atoms = plot_atoms(
             atoms,
             ax,
             radii=0.5,
-            rotation=(f'{rotation[0]}x,{rotation[1]}y,{rotation[2]}z'),
-            show_unit_cell=0
+            rotation=(f"{rotation[0]}x,{rotation[1]}y,{rotation[2]}z"),
+            show_unit_cell=0,
         )
 
 
-if __name__ == '__main__':
-    dos = Dos(folder='../../vaspvis_data/dos_InAs')
+if __name__ == "__main__":
+    dos = Dos(folder="../../vaspvis_data/dos_InAs")
     #  dos._sum_layers(layers=[0,1,2,3])
-    fig, ax = plt.subplots(figsize=(4,3), dpi=100)
+    fig, ax = plt.subplots(figsize=(4, 3), dpi=100)
     dos.plot_spd(
         ax=ax,
-        erange=[-6,6],
+        erange=[-6, 6],
         fill=True,
         total=False,
-        energyaxis='x',
+        energyaxis="x",
         #  color_list=['red', 'red', 'green'],
     )
     plt.show()
```

### Comparing `vaspvis-1.2.7/vaspvis/passivator_utils/passivator_utils.py` & `vaspvis-1.2.8/vaspvis/passivator_utils/passivator_utils.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis/standard.py` & `vaspvis-1.2.8/vaspvis/standard.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,124 +11,125 @@
 from matplotlib.ticker import MaxNLocator
 from matplotlib.colors import Normalize, to_rgba, LinearSegmentedColormap
 import numpy as np
 import time
 
 
 def _figure_setup(ax, fontsize=6, ylim=[-6, 6]):
-    ax.set_ylabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
+    ax.set_ylabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
     ax.set_ylim(ylim[0], ylim[1])
     ax.tick_params(labelsize=fontsize, length=2.5)
-    ax.tick_params(axis='x', length=0)
+    ax.tick_params(axis="x", length=0)
 
 
-def _figure_setup_dos(ax, fontsize=6, energyaxis='y', log_scale=False):
+def _figure_setup_dos(ax, fontsize=6, energyaxis="y", log_scale=False):
     ax.tick_params(labelsize=fontsize, length=2.5)
-    if energyaxis == 'y':
-        ax.set_ylabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
+    if energyaxis == "y":
+        ax.set_ylabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
         if log_scale:
-            ax.set_xlabel('log(Density of States)', fontsize=fontsize)
+            ax.set_xlabel("log(Density of States)", fontsize=fontsize)
         else:
-            ax.set_xlabel('Density of States', fontsize=fontsize)
-    if energyaxis == 'x':
-        ax.set_xlabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
+            ax.set_xlabel("Density of States", fontsize=fontsize)
+    if energyaxis == "x":
+        ax.set_xlabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
         if log_scale:
-            ax.set_ylabel('log(Density of States)', fontsize=fontsize)
+            ax.set_ylabel("log(Density of States)", fontsize=fontsize)
         else:
-            ax.set_ylabel('Density of States', fontsize=fontsize)
-
+            ax.set_ylabel("Density of States", fontsize=fontsize)
 
 
 def _figure_setup_band_dos(ax, fontsize, ylim):
     ax1 = ax[0]
     ax2 = ax[1]
-    ax2.tick_params(axis='y', length=0)
-    ax2.tick_params(axis='x', length=0, labelsize=fontsize)
-    ax2.set_xlabel('Density of States', fontsize=fontsize)
+    ax2.tick_params(axis="y", length=0)
+    ax2.tick_params(axis="x", length=0, labelsize=fontsize)
+    ax2.set_xlabel("Density of States", fontsize=fontsize)
     ax1.tick_params(labelsize=fontsize)
-    ax1.tick_params(axis='x', length=0)
-    ax1.set_ylabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
-    ax1.set_xlabel('Wave Vector', fontsize=fontsize)
+    ax1.tick_params(axis="x", length=0)
+    ax1.set_ylabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
+    ax1.set_xlabel("Wave Vector", fontsize=fontsize)
     ax1.set_ylim(ylim[0], ylim[1])
 
     return ax1, ax2
 
 
 def _figure_setup_band_dos_spin_polarized(ax, fontsize, ylim):
     ax_band_up = ax[0, 0]
     ax_dos_up = ax[0, 1]
     ax_band_down = ax[1, 0]
     ax_dos_down = ax[1, 1]
 
-    ax_dos_up.tick_params(axis='y', length=0)
-    ax_dos_up.tick_params(axis='x', length=0,
-                          labelsize=fontsize, labelbottom=False)
+    ax_dos_up.tick_params(axis="y", length=0)
+    ax_dos_up.tick_params(
+        axis="x", length=0, labelsize=fontsize, labelbottom=False
+    )
     ax_band_up.tick_params(labelsize=fontsize)
-    ax_band_up.tick_params(axis='x', length=0, labelbottom=False)
-    ax_band_up.set_ylabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
+    ax_band_up.tick_params(axis="x", length=0, labelbottom=False)
+    ax_band_up.set_ylabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
     ax_band_up.set_ylim(ylim[0], ylim[1])
 
-    ax_dos_down.tick_params(axis='y', length=0)
-    ax_dos_down.tick_params(axis='x', length=0, labelsize=fontsize)
-    ax_dos_down.set_xlabel('Density of States', fontsize=fontsize)
+    ax_dos_down.tick_params(axis="y", length=0)
+    ax_dos_down.tick_params(axis="x", length=0, labelsize=fontsize)
+    ax_dos_down.set_xlabel("Density of States", fontsize=fontsize)
     ax_band_down.tick_params(labelsize=fontsize)
-    ax_band_down.tick_params(axis='x', length=0)
-    ax_band_down.set_ylabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
-    ax_band_down.set_xlabel('Wave Vector', fontsize=fontsize)
+    ax_band_down.tick_params(axis="x", length=0)
+    ax_band_down.set_ylabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
+    ax_band_down.set_xlabel("Wave Vector", fontsize=fontsize)
     ax_band_down.set_ylim(ylim[0], ylim[1])
 
     return ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
-def _figure_setup_layer_dos(ax, fontsize=6, energyaxis='y'):
+def _figure_setup_layer_dos(ax, fontsize=6, energyaxis="y"):
     ax.tick_params(labelsize=fontsize)
-    if energyaxis == 'y':
-        ax.set_ylabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
-        ax.set_xlabel('Layers', fontsize=fontsize)
-    if energyaxis == 'x':
-        ax.set_xlabel('$E - E_{F}$ $(eV)$', fontsize=fontsize)
-        ax.set_ylabel('Layers', fontsize=fontsize)
+    if energyaxis == "y":
+        ax.set_ylabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
+        ax.set_xlabel("Layers", fontsize=fontsize)
+    if energyaxis == "x":
+        ax.set_xlabel("$E - E_{F}$ $(eV)$", fontsize=fontsize)
+        ax.set_ylabel("Layers", fontsize=fontsize)
+
 
 def band_plain(
     folder,
-    output='band_plain.png',
-    spin='up',
-    color='black',
+    output="band_plain.png",
+    spin="up",
+    color="black",
     linewidth=1.25,
-    linestyle='-',
+    linestyle="-",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     scale_factor=5,
     heatmap=False,
     bins=1000,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.7,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     highlight_band=False,
-    highlight_band_color='red',
+    highlight_band_color="red",
     band_index=None,
     soc_axis=None,
     sp_scale_factor=5,
-    sp_color='red',
+    sp_color="red",
 ):
     """
     This function generates a plain band structure
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         output (str): File name of the resulting plot.
@@ -139,82 +140,84 @@
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations. This number should be 
+            This is also only required for unfolded calculations. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         scale_factor (float): Factor to scale scatter points in unfolded plots.
         heatmap (bool): Determines if an unfolded plot is plotted as a heat map. Only valid from unfolded plots.
         bins (int): number of bins included in the histogram. More bin will result in higher resolution.
         sigma (float): Value used to smooth the heatmap.
         cmap (str): Matplotlib colormap for the unfolded heatmap.
         vlinecolor (str): Color of the vertical lines in the band structure
             useful for heatmaps when there is a dark background color.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
         soc_axis=soc_axis,
     )
 
     if heatmap:
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -244,15 +247,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -260,139 +263,141 @@
         plt.savefig(output)
     else:
         return fig, ax
 
 
 def band_spd(
     folder,
-    output='band_spd.png',
-    spin='up',
+    output="band_spd.png",
+    spin="up",
     scale_factor=5,
-    orbitals='spd',
+    orbitals="spd",
     display_order=None,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates a s, p, d projected band structure.
-    
+
     Parameters:
         folder (str): This is the folder that contains the VASP files
         orbitals (str): String that contains the s, p, or d orbitals that to project onto.
-            The default is 'spd', if the user only wanted to project onto the p, and d orbitals 
+            The default is 'spd', if the user only wanted to project onto the p, and d orbitals
             than 'pd' should be passed in
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -419,15 +424,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -436,39 +441,39 @@
     else:
         return fig, ax
 
 
 def band_atom_orbitals(
     folder,
     atom_orbital_dict,
-    output='band_atom_orbitals.png',
-    spin='up',
+    output="band_atom_orbitals.png",
+    spin="up",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
@@ -483,91 +488,93 @@
             of the first atom and the s orbital of the second atom then the dictionary would be {0:[0,1,2,3], 1:[0]}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -594,15 +601,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -611,39 +618,39 @@
     else:
         return fig, ax
 
 
 def band_orbitals(
     folder,
     orbitals,
-    output='band_orbital.png',
-    spin='up',
+    output="band_orbital.png",
+    spin="up",
     scale_factor=5,
     display_order=None,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
@@ -674,91 +681,93 @@
 
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -785,15 +794,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -802,39 +811,39 @@
     else:
         return fig, ax
 
 
 def band_atoms(
     folder,
     atoms,
-    output='band_atoms.png',
-    spin='up',
+    output="band_atoms.png",
+    spin="up",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
@@ -848,90 +857,92 @@
             and the atoms are in the same order as they are in the POSCAR
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -958,154 +969,157 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax
 
+
 def band_atom_spd(
     folder,
     atom_spd_dict,
-    output='band_atom_spd.png',
-    spin='up',
+    output="band_atom_spd.png",
+    spin="up",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates a s, p, d projected band structure on specific atoms.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the
-            orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals corresponding 
+            orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals corresponding
             of the first atom and the p orbitals of the second atom then the dictionary would be {0:'spd', 1:'p'}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -1132,15 +1146,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -1149,39 +1163,39 @@
     else:
         return fig, ax
 
 
 def band_elements(
     folder,
     elements,
-    output='band_elements.png',
-    spin='up',
+    output="band_elements.png",
+    spin="up",
     scale_factor=5,
     display_order=None,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
@@ -1194,91 +1208,93 @@
         elements (list): List of elements to project onto. The list should countain the corresponding element symbols
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -1305,15 +1321,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -1322,138 +1338,140 @@
     else:
         return fig, ax
 
 
 def band_element_orbitals(
     folder,
     element_orbital_dict,
-    output='band_element_orbital.png',
-    spin='up',
+    output="band_element_orbital.png",
+    spin="up",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates a projected band structure on orbitals of specific elements.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding 
+        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of In and the s orbital of As for and InAs structure then the dictionary would be {'In':[0,1,2,3], 'As':[0]}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -1480,15 +1498,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -1497,138 +1515,140 @@
     else:
         return fig, ax
 
 
 def band_element_spd(
     folder,
     element_spd_dict,
-    output='band_element_spd.png',
-    spin='up',
+    output="band_element_spd.png",
+    spin="up",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     heatmap=False,
     bins=800,
     sigma=2,
-    cmap='hot',
-    vlinecolor='black',
+    cmap="hot",
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.5,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates a s, p, d projected band structure on specific elements.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding 
+        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of In and the p orbitals of As for an InAs structure then the dictionary would be {'In':'spd', 'As':'p'}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background.
         band_color (string): Color of the plain band structure.
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
         and axis for further editing.
     """
 
     band = Band(
         folder=folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
 
     if heatmap:
         legend = False
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
@@ -1655,15 +1675,15 @@
     if heatmap:
         if cbar:
             im = ax.collections[0]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['min', 'max'])
+            cbar.set_ticklabels(["min", "max"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -1671,42 +1691,42 @@
         plt.savefig(output)
     else:
         return fig, ax
 
 
 def band_plain_spin_polarized(
     folder,
-    output='band_plain_sp.png',
-    up_color='red',
-    down_color='blue',
-    background_color='black',
+    output="band_plain_sp.png",
+    up_color="red",
+    down_color="blue",
+    background_color="black",
     linewidth=1.25,
-    up_linestyle='-',
-    down_linestyle=':',
+    up_linestyle="-",
+    down_linestyle=":",
     figsize=(4, 3),
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
     scale_factor=5,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     heatmap=False,
     bins=1000,
     sigma=2,
-    vlinecolor='black',
+    vlinecolor="black",
     cbar=True,
-    cbar_orientation='horizontal',
+    cbar_orientation="horizontal",
     powernorm=True,
     gamma=0.7,
     soc_axis=None,
     sp_scale_factor=5,
 ):
     """
     This function generates a plain spin polarized band structure.
@@ -1728,122 +1748,124 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
     )
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         unfold=unfold,
-        high_symm_points=high_symm_points, 
+        high_symm_points=high_symm_points,
         interpolate=interpolate,
         new_n=new_n,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
         shift_efermi=shift_efermi,
         soc_axis=soc_axis,
     )
 
     if heatmap:
         if cbar:
-            if cbar_orientation == 'horizontal':
+            if cbar_orientation == "horizontal":
                 fig, (ax, cax) = plt.subplots(
                     nrows=2,
                     figsize=figsize,
                     gridspec_kw={"height_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
-            elif cbar_orientation == 'vertical':
+            elif cbar_orientation == "vertical":
                 fig, (ax, cax) = plt.subplots(
                     ncols=2,
                     figsize=figsize,
                     gridspec_kw={"width_ratios": [1, 0.05]},
                     dpi=400,
                     constrained_layout=True,
                 )
             else:
-                raise('This is not a valid orientation please choose either horizontal or vertical')
+                raise (
+                    "This is not a valid orientation please choose either horizontal or vertical"
+                )
         else:
             fig = plt.figure(figsize=(figsize), dpi=400)
             ax = fig.add_subplot(111)
     else:
         fig = plt.figure(figsize=(figsize), dpi=400)
         ax = fig.add_subplot(111)
 
     _figure_setup(ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
     if heatmap:
         _, axd = plt.subplots()
         spin_cmap = LinearSegmentedColormap.from_list(
-            'spin',
+            "spin",
             [
                 to_rgba(down_color),
                 to_rgba(down_color),
                 to_rgba(down_color),
-                (1,1,1,0),
+                (1, 1, 1, 0),
                 to_rgba(up_color),
                 to_rgba(up_color),
                 to_rgba(up_color),
             ],
-            N=10000
+            N=10000,
         )
 
         bot_cmap = LinearSegmentedColormap.from_list(
-            'background',
+            "background",
             [
-                (1,1,1,0),
+                (1, 1, 1, 0),
                 to_rgba(background_color),
             ],
-            N=10000
+            N=10000,
         )
         band_up.plot_plain(
             ax=ax,
             erange=erange,
             heatmap=heatmap,
             bins=bins,
             sigma=sigma,
@@ -1885,18 +1907,24 @@
             sigma=sigma,
             vlinecolor=vlinecolor,
             cmap=spin_cmap,
             powernorm=False,
             gamma=gamma,
         )
 
-        ax.collections[1].set_array(ax.collections[1].get_array() - axd.collections[1].get_array())
-        ax.collections[0].set_array(ax.collections[0].get_array() + axd.collections[0].get_array())
+        ax.collections[1].set_array(
+            ax.collections[1].get_array() - axd.collections[1].get_array()
+        )
+        ax.collections[0].set_array(
+            ax.collections[0].get_array() + axd.collections[0].get_array()
+        )
         im = ax.collections[1]
-        sym_val = np.max(np.abs([np.min(im.get_array()), np.max(im.get_array())]))
+        sym_val = np.max(
+            np.abs([np.min(im.get_array()), np.max(im.get_array())])
+        )
         norm = Normalize(
             vmin=-sym_val,
             vmax=sym_val,
         )
         ax.collections[1].set_norm(norm)
     else:
         band_up.plot_plain(
@@ -1935,84 +1963,76 @@
 
         if unfold:
             legend_lines = [
                 plt.Line2D(
                     [0],
                     [0],
                     color=up_color,
-                    linestyle='',
-                    marker='o',
+                    linestyle="",
+                    marker="o",
                     markersize=3,
                 ),
                 plt.Line2D(
                     [0],
                     [0],
                     color=down_color,
-                    linestyle='',
-                    marker='o',
+                    linestyle="",
+                    marker="o",
                     markersize=3,
-                )
+                ),
             ]
         elif soc_axis is not None and band_up.lsorbit:
             legend_lines = [
                 plt.Line2D(
                     [0],
                     [0],
                     color=up_color,
-                    linestyle='',
-                    marker='o',
+                    linestyle="",
+                    marker="o",
                     markersize=3,
                 ),
                 plt.Line2D(
                     [0],
                     [0],
                     color=down_color,
-                    linestyle='',
-                    marker='o',
+                    linestyle="",
+                    marker="o",
                     markersize=3,
-                )
+                ),
             ]
         else:
             legend_lines = [
+                plt.Line2D([0], [0], color=up_color, linestyle=up_linestyle),
                 plt.Line2D(
-                    [0],
-                    [0],
-                    color=up_color,
-                    linestyle=up_linestyle
+                    [0], [0], color=down_color, linestyle=down_linestyle
                 ),
-                plt.Line2D(
-                    [0],
-                    [0],
-                    color=down_color,
-                    linestyle=down_linestyle
-                )
             ]
 
-        legend_labels = ['$\\uparrow$', '$\\downarrow$']
+        legend_labels = ["$\\uparrow$", "$\\downarrow$"]
 
         ax.legend(
             legend_lines,
             legend_labels,
             ncol=1,
-            loc='upper left',
+            loc="upper left",
             fontsize=fontsize,
             bbox_to_anchor=(1, 1),
             borderaxespad=0,
             frameon=False,
             handletextpad=0.1,
         )
 
     if heatmap:
         if cbar:
             im = ax.collections[1]
             min_val = im.norm.vmin
             max_val = im.norm.vmax
             cbar = fig.colorbar(im, cax=cax, orientation=cbar_orientation)
             cbar.set_ticks([min_val, max_val])
-            cbar.set_ticklabels(['down', 'up'])
+            cbar.set_ticklabels(["down", "up"])
 
     if heatmap:
         if not cbar:
             fig.tight_layout(pad=0.4)
     else:
         fig.tight_layout(pad=0.4)
 
@@ -2020,59 +2040,59 @@
         fig.savefig(output)
     else:
         return fig, ax
 
 
 def band_spd_spin_polarized(
     folder,
-    output='band_spd_sp.png',
+    output="band_spd_sp.png",
     scale_factor=5,
-    orbitals='spd',
+    orbitals="spd",
     display_order=None,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     fontsize=12,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.02, 0.98),
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates a spin polarized s, p, d projected band structure. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         orbitals (str): String that contains the s, p, or d orbitals that to project onto.
-            The default is 'spd', if the user only wanted to project onto the p, and d orbitals 
+            The default is 'spd', if the user only wanted to project onto the p, and d orbitals
             than 'pd' should be passed in
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -2084,105 +2104,106 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
     ax1.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
     ax2.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
 
     band_up.plot_spd(
         ax=ax1,
         scale_factor=scale_factor,
@@ -2228,58 +2249,58 @@
     else:
         return fig, ax1, ax2
 
 
 def band_atom_orbitals_spin_polarized(
     folder,
     atom_orbital_dict,
-    output='band_atom_orbitals_sp.png',
+    output="band_atom_orbitals_sp.png",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     fontsize=12,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.02, 0.98),
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates an atom orbital spin polarized band structure. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        atom_orbital_dict (dict[int:list]): A dictionary that contains the individual atoms and the corresponding 
+        atom_orbital_dict (dict[int:list]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of the first atom and the s orbital of the second atom then the dictionary would be {0:[0,1,2,3], 1:[0]}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -2291,105 +2312,106 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
     ax1.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
     ax2.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
 
     band_up.plot_atom_orbitals(
         ax=ax1,
         atom_orbital_dict=atom_orbital_dict,
@@ -2435,42 +2457,42 @@
     else:
         return fig, ax1, ax2
 
 
 def band_orbitals_spin_polarized(
     folder,
     orbitals,
-    output='band_orbitals_sp.png',
+    output="band_orbitals_sp.png",
     scale_factor=5,
     display_order=None,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates an orbital spin polarized band structure. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         orbitals (list): List of orbitals to compare
 
             | 0 = s
@@ -2491,15 +2513,15 @@
             | 15 = fx3
 
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -2511,103 +2533,103 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
     bbox = dict(boxstyle="round", fc="white")
     ax1.annotate(
-        '$\\uparrow$ ',
+        "$\\uparrow$ ",
         xy=(0.02, 0.98),
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
     )
     ax2.annotate(
-        '$\\downarrow$ ',
+        "$\\downarrow$ ",
         xy=(0.02, 0.98),
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
     )
 
     band_up.plot_orbitals(
         ax=ax1,
         orbitals=orbitals,
         scale_factor=scale_factor,
@@ -2652,54 +2674,54 @@
     else:
         return fig, ax1, ax2
 
 
 def band_atoms_spin_polarized(
     folder,
     atoms,
-    output='band_atoms_sp.png',
+    output="band_atoms_sp.png",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates an atom spin polarized band structure. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         atoms (list): List of atoms to project onto. The indices should be zero indexed (first atom is 0)
             and the atoms are in the same order as they are in the POSCAR
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -2711,107 +2733,106 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
     bbox = dict(boxstyle="round", fc="white")
     ax1.annotate(
-        '$\\uparrow$ ',
+        "$\\uparrow$ ",
         xy=(0.02, 0.98),
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
     )
     ax2.annotate(
-        '$\\downarrow$ ',
+        "$\\downarrow$ ",
         xy=(0.02, 0.98),
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
     )
 
-
     band_up.plot_atoms(
         ax=ax1,
         atoms=atoms,
         scale_factor=scale_factor,
         color_list=color_list,
         display_order=display_order,
         legend=legend,
@@ -2849,61 +2870,62 @@
     plt.tight_layout(pad=0.4)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
+
 def band_atom_spd_spin_polarized(
     folder,
     atom_spd_dict,
-    output='band_atoms_spd_sp.png',
+    output="band_atoms_spd_sp.png",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     fontsize=12,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.02, 0.98),
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates a s, p, d spin polarized band structure on specific atoms. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding 
+        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of the first atom and the p orbitals of the second atom then the dictionary would be {0:'spd', 1:'p'}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -2915,105 +2937,106 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
     ax1.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
     ax2.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
 
     band_up.plot_atom_spd(
         ax=ax1,
         atom_spd_dict=atom_spd_dict,
@@ -3059,53 +3082,53 @@
     else:
         return fig, ax1, ax2
 
 
 def band_elements_spin_polarized(
     folder,
     elements,
-    output='band_elements_sp.png',
+    output="band_elements_sp.png",
     scale_factor=5,
     display_order=None,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates an element spin polarized band structure. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         elements (list): List of elements to project onto. The list should countain the corresponding element symbols
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -3117,103 +3140,103 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
     bbox = dict(boxstyle="round", fc="white")
     ax1.annotate(
-        '$\\uparrow$ ',
+        "$\\uparrow$ ",
         xy=(0.02, 0.98),
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
     )
     ax2.annotate(
-        '$\\downarrow$ ',
+        "$\\downarrow$ ",
         xy=(0.02, 0.98),
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
     )
 
     band_up.plot_elements(
         ax=ax1,
         elements=elements,
         scale_factor=scale_factor,
@@ -3258,58 +3281,58 @@
     else:
         return fig, ax1, ax2
 
 
 def band_element_orbital_spin_polarized(
     folder,
     element_orbital_dict,
-    output='band_element_orbital_sp.png',
+    output="band_element_orbital_sp.png",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     fontsize=12,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.02, 0.98),
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates an element orbital spin polarized band structure. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding 
+        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of In and the s orbital of As for and InAs structure then the dictionary would be {'In':[0,1,2,3], 'As':[0]}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -3321,105 +3344,106 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
     ax1.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
     ax2.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
 
     band_up.plot_element_orbitals(
         ax=ax1,
         element_orbital_dict=element_orbital_dict,
@@ -3465,58 +3489,58 @@
     else:
         return fig, ax1, ax2
 
 
 def band_element_spd_spin_polarized(
     folder,
     element_spd_dict,
-    output='band_elements_spd_sp.png',
+    output="band_elements_spd_sp.png",
     display_order=None,
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     fontsize=12,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.02, 0.98),
     figsize=(4, 3),
     erange=[-6, 6],
-    stack='vertical',
+    stack="vertical",
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
 ):
     """
     This function generates a s, p, d spin polarized band structure on specific elements. This will plot two plots
-    stacked on top or eachother or next to eachother. The top or left plot will project on the 
+    stacked on top or eachother or next to eachother. The top or left plot will project on the
     spin up bands and the bottom or right plot will project onto the spin down bands.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding 
+        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of In and the p orbitals of As for an InAs structure then the dictionary would be {'In':'spd', 'As':'p'}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot.
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
@@ -3528,105 +3552,106 @@
         figsize (list / tuple): Desired size of the image in inches. (width, height)
         erange (list / tuple): Range of energy to show in the plot. [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. (fig, ax1, ax2) 
+        and axis for further editing. (fig, ax1, ax2)
     """
 
     band_up = Band(
         folder=folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    if stack == 'vertical':
+    if stack == "vertical":
         fig = plt.figure(figsize=(figsize[0], 2 * figsize[1]), dpi=400)
         ax1 = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
-    elif stack == 'horizontal':
+    elif stack == "horizontal":
         fig = plt.figure(figsize=(2 * figsize[0], figsize[1]), dpi=400)
         ax1 = fig.add_subplot(121)
         ax2 = fig.add_subplot(122)
         _figure_setup(ax=ax1, fontsize=fontsize, ylim=[erange[0], erange[1]])
         _figure_setup(ax=ax2, fontsize=fontsize, ylim=[erange[0], erange[1]])
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
     ax1.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
     ax2.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize,
     )
 
     band_up.plot_element_spd(
         ax=ax1,
         element_spd_dict=element_spd_dict,
@@ -3668,33 +3693,34 @@
     plt.tight_layout(pad=0.4)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
+
 # =============================================================
 # -------------------- Density of States ----------------------
 # =============================================================
 
 
 def dos_plain(
     folder,
-    output='dos_plain.png',
+    output="dos_plain.png",
     linewidth=1.5,
     fill=True,
     alpha=0.3,
     sigma=0.05,
-    energyaxis='x',
-    color='black',
+    energyaxis="x",
+    color="black",
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
     log_scale=False,
 ):
     """
     This function plots the total density of states.
@@ -3710,24 +3736,29 @@
         color (list): Color of plot and fill.
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_plain(
         ax=ax,
@@ -3744,71 +3775,79 @@
     plt.tight_layout(pad=0.4)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax
 
+
 def dos_ldos(
     folder,
     layers,
-    output='dos_ldos.png',
+    output="dos_ldos.png",
     linewidth=1.5,
     fill=True,
     alpha=0.3,
     sigma=0.05,
-    energyaxis='x',
-    color='black',
+    energyaxis="x",
+    color="black",
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
     log_scale=False,
     atol=None,
     custom_layer_inds=None,
-    linestyle='-',
+    linestyle="-",
 ):
     """
-    This function plots the local density of states for atomic layers. Useful for comparing 
+    This function plots the local density of states for atomic layers. Useful for comparing
     to STS measurments.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        layers (list): List of atomic layers to include in the ldos plot. 0 = first layer 
+        layers (list): List of atomic layers to include in the ldos plot. 0 = first layer
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
         energyaxis (str): Determines the axis to plot the energy on ('x' or 'y')
         color (list): Color of plot and fill.
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
-    _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis, log_scale=log_scale)
+    _figure_setup_dos(
+        ax=ax, fontsize=fontsize, energyaxis=energyaxis, log_scale=log_scale
+    )
 
     dos.plot_ldos(
         ax=ax,
         layers=layers,
         linewidth=linewidth,
         fill=fill,
         alpha=alpha,
@@ -3828,40 +3867,40 @@
         plt.savefig(output)
     else:
         return fig, ax
 
 
 def dos_spd(
     folder,
-    output='dos_spd.png',
-    orbitals='spd',
+    output="dos_spd.png",
+    orbitals="spd",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots an s, p, d projected density of states.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         orbitals (str): String that contains the s, p, or d orbitals that to project onto.
-            The default is 'spd', if the user only wanted to project onto the p, and d orbitals 
+            The default is 'spd', if the user only wanted to project onto the p, and d orbitals
             than 'pd' should be passed in
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
         energyaxis (str): Determines the axis to plot the energy on ('x' or 'y')
@@ -3871,24 +3910,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_spd(
         ax=ax,
@@ -3911,38 +3955,38 @@
     else:
         return fig, ax
 
 
 def dos_atom_orbitals(
     folder,
     atom_orbital_dict,
-    output='dos_atom_orbitals.png',
+    output="dos_atom_orbitals.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots the orbital projected density of states on specific atoms.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        atom_orbital_dict (dict[int:list]): A dictionary that contains the individual atoms and the corresponding 
+        atom_orbital_dict (dict[int:list]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of the first atom and the s orbital of the second atom then the dictionary would be {0:[0,1,2,3], 1:[0]}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -3953,24 +3997,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_atom_orbitals(
         ax=ax,
@@ -3993,28 +4042,28 @@
     else:
         return fig, ax
 
 
 def dos_orbitals(
     folder,
     orbitals,
-    output='dos_orbitals.png',
+    output="dos_orbitals.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots the orbital projected density of states.
 
@@ -4051,24 +4100,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_orbitals(
         ax=ax,
@@ -4091,28 +4145,28 @@
     else:
         return fig, ax
 
 
 def dos_atoms(
     folder,
     atoms,
-    output='dos_atoms.png',
+    output="dos_atoms.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots the atom projected density of states.
 
@@ -4132,24 +4186,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_atoms(
         ax=ax,
@@ -4168,41 +4227,42 @@
     plt.tight_layout(pad=0.4)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax
 
+
 def dos_atom_spd(
     folder,
     atom_spd_dict,
-    output='dos_atom_spd.png',
+    output="dos_atom_spd.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots the atom projected density of states of the s, p, and d orbitals.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding 
+        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of the first atom and the p orbitals of the second atom then the dictionary would be {0:'spd', 1:'p'}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -4213,24 +4273,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_atom_spd(
         ax=ax,
@@ -4253,28 +4318,28 @@
     else:
         return fig, ax
 
 
 def dos_elements(
     folder,
     elements,
-    output='dos_elements.png',
+    output="dos_elements.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots the element projected density of states.
 
@@ -4293,24 +4358,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_elements(
         ax=ax,
@@ -4333,38 +4403,38 @@
     else:
         return fig, ax
 
 
 def dos_element_spd(
     folder,
     element_spd_dict,
-    output='dos_element_spd.png',
+    output="dos_element_spd.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots the element projected density of states of the s, p, and d orbitals.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding 
+        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of In and the p orbitals of As for an InAs structure then the dictionary would be {'In':'spd', 'As':'p'}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -4375,24 +4445,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_element_spd(
         ax=ax,
@@ -4415,38 +4490,38 @@
     else:
         return fig, ax
 
 
 def dos_element_orbitals(
     folder,
     element_orbital_dict,
-    output='dos_element_orbitals.png',
+    output="dos_element_orbitals.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
+    energyaxis="x",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots the element projected density of states on specific orbitals.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding 
+        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of In and the s orbital of As for and InAs structure then the dictionary would be {'In':[0,1,2,3], 'As':[0]}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -4457,24 +4532,29 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos = Dos(shift_efermi=shift_efermi, folder=folder, spin=spin, combination_method=combination_method)
+    dos = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin=spin,
+        combination_method=combination_method,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos.plot_element_orbitals(
         ax=ax,
@@ -4496,22 +4576,22 @@
         plt.savefig(output)
     else:
         return fig, ax
 
 
 def dos_plain_spin_polarized(
     folder,
-    output='dos_plain_sp.png',
+    output="dos_plain_sp.png",
     linewidth=1.5,
     fill=True,
     alpha=0.3,
     sigma=0.05,
-    energyaxis='x',
-    soc_axis='z',
-    color='black',
+    energyaxis="x",
+    soc_axis="z",
+    color="black",
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
@@ -4525,25 +4605,32 @@
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
         energyaxis (str): Determines the axis to plot the energy on ('x' or 'y')
         color (str): Color of plot and fill.
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_plain(
         ax=ax,
@@ -4573,22 +4660,22 @@
         plt.savefig(output)
     else:
         return fig, ax
 
 
 def dos_spd_spin_polarized(
     folder,
-    output='dos_spd_sp.png',
-    orbitals='spd',
+    output="dos_spd_sp.png",
+    orbitals="spd",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
-    soc_axis='z',
+    energyaxis="x",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
@@ -4596,40 +4683,47 @@
 ):
     """
     This function plots a spin polarized s, p, d projected density of states.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
         orbitals (str): String that contains the s, p, or d orbitals that to project onto.
-            The default is 'spd', if the user only wanted to project onto the p, and d orbitals 
+            The default is 'spd', if the user only wanted to project onto the p, and d orbitals
             than 'pd' should be passed in
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
         energyaxis (str): Determines the axis to plot the energy on ('x' or 'y')
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines whether to draw the legend or not
         total (bool): Determines wheth to draw the total density of states or not
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_spd(
         ax=ax,
@@ -4666,36 +4760,36 @@
     else:
         return fig, ax
 
 
 def dos_atom_orbitals_spin_polarized(
     folder,
     atom_orbital_dict,
-    output='dos_atom_orbitals_sp.png',
+    output="dos_atom_orbitals_sp.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='y',
-    soc_axis='z',
+    energyaxis="y",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots a spin polarized orbital projected density of states on specific atoms.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        atom_orbital_dict (dict[int:list]): A dictionary that contains the individual atoms and the corresponding 
+        atom_orbital_dict (dict[int:list]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of the first atom and the s orbital of the second atom then the dictionary would be {0:[0,1,2,3], 1:[0]}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -4703,25 +4797,32 @@
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines whether to draw the legend or not
         total (bool): Determines wheth to draw the total density of states or not
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_atom_orbitals(
         ax=ax,
@@ -4758,21 +4859,21 @@
     else:
         return fig, ax
 
 
 def dos_orbitals_spin_polarized(
     folder,
     orbitals,
-    output='dos_orbitals_sp.png',
+    output="dos_orbitals_sp.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='y',
-    soc_axis='z',
+    energyaxis="y",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
@@ -4811,25 +4912,32 @@
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines whether to draw the legend or not
         total (bool): Determines wheth to draw the total density of states or not
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_orbitals(
         ax=ax,
@@ -4866,21 +4974,21 @@
     else:
         return fig, ax
 
 
 def dos_atoms_spin_polarized(
     folder,
     atoms,
-    output='dos_atoms_sp.png',
+    output="dos_atoms_sp.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='y',
-    soc_axis='z',
+    energyaxis="y",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
@@ -4902,25 +5010,32 @@
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines whether to draw the legend or not
         total (bool): Determines wheth to draw the total density of states or not
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_atoms(
         ax=ax,
@@ -4953,39 +5068,40 @@
     plt.tight_layout(pad=0.4)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax
 
+
 def dos_atom_spd_spin_polarized(
     folder,
     atom_spd_dict,
-    output='dos_atom_spd_sp.png',
+    output="dos_atom_spd_sp.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
-    soc_axis='z',
+    energyaxis="x",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots a spin polarized atom projected density of states of the s, p, and d orbitals.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding 
+        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of the first atom and the p orbitals of the second atom then the dictionary would be {0:'spd', 1:'p'}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -4996,25 +5112,32 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_atom_spd(
         ax=ax,
@@ -5051,21 +5174,21 @@
     else:
         return fig, ax
 
 
 def dos_elements_spin_polarized(
     folder,
     elements,
-    output='dos_elements_sp.png',
+    output="dos_elements_sp.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='y',
-    soc_axis='z',
+    energyaxis="y",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
@@ -5089,25 +5212,32 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_elements(
         ax=ax,
@@ -5144,36 +5274,36 @@
     else:
         return fig, ax
 
 
 def dos_element_spd_spin_polarized(
     folder,
     element_spd_dict,
-    output='dos_element_spd_sp.png',
+    output="dos_element_spd_sp.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='x',
-    soc_axis='z',
+    energyaxis="x",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots a spin polarized element projected density of states of the s, p, and d orbitals.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding 
+        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of In and the p orbitals of As for an InAs structure then the dictionary would be {'In':'spd', 'As':'p'}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -5184,25 +5314,32 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_element_spd(
         ax=ax,
@@ -5239,36 +5376,36 @@
     else:
         return fig, ax
 
 
 def dos_element_orbitals_spin_polarized(
     folder,
     element_orbital_dict,
-    output='dos_element_orbitals_sp.png',
+    output="dos_element_orbitals_sp.png",
     fill=True,
     alpha=0.3,
     linewidth=1.5,
     sigma=0.05,
-    energyaxis='y',
-    soc_axis='z',
+    energyaxis="y",
+    soc_axis="z",
     color_list=None,
     legend=True,
     total=True,
     figsize=(4, 3),
     erange=[-6, 6],
     fontsize=12,
     save=True,
     shift_efermi=0,
 ):
     """
     This function plots a spin polarized element projected density of states on specific orbitals.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
-        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding 
+        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of In and the s orbital of As for and InAs structure then the dictionary would be {'In':[0,1,2,3], 'As':[0]}
         output (str): File name of the resulting plot.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         linewidth (float): Linewidth of lines
         sigma (float): Standard deviation for gaussian filter
@@ -5279,25 +5416,32 @@
         total (bool): Determines wheth to draw the total density of states or not
         spin (str): Which spin direction to parse ('up' or 'down')
         figsize (list / tuple): Desired size of the image in inches (width, height)
         erange (list): Energy range for the DOS plot ([lower bound, upper bound])
         combination_method (str): If spin == 'both', this determines if the spin up and spin down
             desnities are added or subtracted. ('add' or 'sub')
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=folder, spin='up', soc_axis=soc_axis)
-    dos_down = Dos(shift_efermi=shift_efermi, folder=folder, spin='down', soc_axis=soc_axis)
+    dos_up = Dos(
+        shift_efermi=shift_efermi, folder=folder, spin="up", soc_axis=soc_axis
+    )
+    dos_down = Dos(
+        shift_efermi=shift_efermi,
+        folder=folder,
+        spin="down",
+        soc_axis=soc_axis,
+    )
 
     fig = plt.figure(figsize=figsize, dpi=400)
     ax = fig.add_subplot(111)
     _figure_setup_dos(ax=ax, fontsize=fontsize, energyaxis=energyaxis)
 
     dos_up.plot_element_orbitals(
         ax=ax,
@@ -5335,28 +5479,29 @@
         return fig, ax
 
 
 # =============================================================
 # ---------------------- Band-Dos Plots -----------------------
 # =============================================================
 
+
 def band_dos_plain(
     band_folder,
     dos_folder,
-    output='band_dos_plain.png',
-    spin='up',
-    color='black',
+    output="band_dos_plain.png",
+    spin="up",
+    color="black",
     linewidth=1.25,
-    linestyle='-',
+    linestyle="-",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
     shift_efermi=0,
@@ -5375,72 +5520,70 @@
         dos_folder (str): This is the folder that contains the VASP files for the density of states calculation
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         color (str): Color of the band structure lines
         linewidth (float): Line width of the band structure lines
         linestyle (str): Line style of the bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations. This number should be 
+            This is also only required for unfolded calculations. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_plain(
         ax=ax1,
         color=color,
@@ -5450,50 +5593,50 @@
 
     dos.plot_plain(
         ax=ax2,
         linewidth=linewidth,
         fill=fill,
         alpha=alpha,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color=color,
         erange=erange,
     )
 
     fig.canvas.draw()
     labels = ax2.get_xticklabels()
-    labels[0] = ''
+    labels[0] = ""
     ax2.set_xticklabels(labels)
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_spd(
     band_folder,
     dos_folder,
-    output='band_dos_spd.png',
-    spin='up',
+    output="band_dos_spd.png",
+    spin="up",
     scale_factor=5,
-    orbitals='spd',
+    orbitals="spd",
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -5503,101 +5646,99 @@
     soc_axis=None,
     fill=True,
     alpha=0.3,
     sigma=0.05,
 ):
     """
     This function plots a s, p, d projected band structure next to and s, p, d projected
-    density of states. 
+    density of states.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
         orbitals (str): String that contains the s, p, or d orbitals that to project onto.
-            The default is 'spd', if the user only wanted to project onto the p, and d orbitals 
+            The default is 'spd', if the user only wanted to project onto the p, and d orbitals
             than 'pd' should be passed in
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_spd(
         ax=ax1,
         scale_factor=scale_factor,
@@ -5613,51 +5754,51 @@
     dos.plot_spd(
         ax=ax2,
         orbitals=orbitals,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_atom_orbitals(
     band_folder,
     dos_folder,
     atom_orbital_dict,
-    output='band_dos_atom_orbitals.png',
-    spin='up',
+    output="band_dos_atom_orbitals.png",
+    spin="up",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -5681,87 +5822,85 @@
             of the first atom and the s orbital of the second atom then the dictionary would be {0:[0,1,2,3], 1:[0]}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_atom_orbitals(
         ax=ax1,
         scale_factor=scale_factor,
@@ -5777,51 +5916,51 @@
     dos.plot_atom_orbitals(
         ax=ax2,
         atom_orbital_dict=atom_orbital_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_orbitals(
     band_folder,
     dos_folder,
     orbitals,
-    output='band_dos_orbitals.png',
-    spin='up',
+    output="band_dos_orbitals.png",
+    spin="up",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -5831,15 +5970,15 @@
     soc_axis=None,
     fill=True,
     alpha=0.3,
     sigma=0.05,
 ):
     """
     This function generates a band structure projected on specific orbitals next to a
-    projected density of states on the same orbitals. 
+    projected density of states on the same orbitals.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
         orbitals (list): List of orbitals to compare
 
             | 0 = s
@@ -5861,87 +6000,85 @@
 
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_orbitals(
         ax=ax1,
         orbitals=orbitals,
@@ -5957,51 +6094,51 @@
     dos.plot_orbitals(
         ax=ax2,
         orbitals=orbitals,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_atoms(
     band_folder,
     dos_folder,
     atoms,
-    output='band_dos_atoms.png',
-    spin='up',
+    output="band_dos_atoms.png",
+    spin="up",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -6010,101 +6147,99 @@
     new_n=200,
     soc_axis=None,
     fill=True,
     alpha=0.3,
     sigma=0.05,
 ):
     """
-    This function generates a projected band structure on specific atoms next to a 
+    This function generates a projected band structure on specific atoms next to a
     projected density of states on the same atoms.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
         atoms (list): List of atoms to project onto. The indices should be zero indexed (first atom is 0)
             and the atoms are in the same order as they are in the POSCAR
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_atoms(
         ax=ax1,
         atoms=atoms,
@@ -6120,50 +6255,51 @@
     dos.plot_atoms(
         ax=ax2,
         atoms=atoms,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
+
 def band_dos_atom_spd(
     band_folder,
     dos_folder,
     atom_spd_dict,
-    output='band_dos_atom_spd.png',
-    spin='up',
+    output="band_dos_atom_spd.png",
+    spin="up",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -6172,102 +6308,100 @@
     new_n=200,
     soc_axis=None,
     fill=True,
     alpha=0.3,
     sigma=0.05,
 ):
     """
-    This function generates a s, p, d projected band structure on specific atoms next to a 
+    This function generates a s, p, d projected band structure on specific atoms next to a
     projected density of states on the s, p, d orbitals for the same atoms.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
-        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding 
+        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of the first atom and the p orbitals of the second atom then the dictionary would be {0:'spd', 1:'p'}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_atom_spd(
         ax=ax1,
         atom_spd_dict=atom_spd_dict,
@@ -6283,50 +6417,51 @@
     dos.plot_atom_spd(
         ax=ax2,
         atom_spd_dict=atom_spd_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
+
 def band_dos_elements(
     band_folder,
     dos_folder,
     elements,
-    output='band_dos_elements.png',
-    spin='up',
+    output="band_dos_elements.png",
+    spin="up",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -6348,87 +6483,85 @@
         elements (list): List of elements to project onto. The list should countain the corresponding element symbols
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_elements(
         ax=ax1,
         elements=elements,
@@ -6444,51 +6577,51 @@
     dos.plot_elements(
         ax=ax2,
         elements=elements,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_element_spd(
     band_folder,
     dos_folder,
     element_spd_dict,
-    output='band_dos_element_spd.png',
-    spin='up',
+    output="band_dos_element_spd.png",
+    spin="up",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -6497,102 +6630,100 @@
     new_n=200,
     soc_axis=None,
     fill=True,
     alpha=0.3,
     sigma=0.05,
 ):
     """
-    This function generates a s, p, d projected band structure on specific elements next to a 
+    This function generates a s, p, d projected band structure on specific elements next to a
     projected density of states on the s, p, d orbitals for the same elements.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
-        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding 
+        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of In and the p orbitals of As for an InAs structure then the dictionary would be {'In':'spd', 'As':'p'}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_element_spd(
         ax=ax1,
         element_spd_dict=element_spd_dict,
@@ -6608,51 +6739,51 @@
     dos.plot_element_spd(
         ax=ax2,
         element_spd_dict=element_spd_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_element_orbitals(
     band_folder,
     dos_folder,
     element_orbital_dict,
-    output='band_dos_element_orbitals.png',
-    spin='up',
+    output="band_dos_element_orbitals.png",
+    spin="up",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
+    band_color="black",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
@@ -6667,96 +6798,94 @@
     """
     This function generates a projected band structure on orbitals of specific elements next to a
     projected density of states on the same orbitals for the same elements.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
-        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding 
+        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of In and the s orbital of As for and InAs structure then the dictionary would be {'In':[0,1,2,3], 'As':[0]}
         output (str): File name of the resulting plot.
         spin (str): Choose which spin direction to parse. ('up' or 'down')
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band = Band(
         folder=band_folder,
         spin=spin,
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     dos = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin=spin)
 
     band.plot_element_orbitals(
         ax=ax1,
         scale_factor=scale_factor,
@@ -6772,49 +6901,49 @@
     dos.plot_element_orbitals(
         ax=ax2,
         element_orbital_dict=element_orbital_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_plain_spin_polarized(
     band_folder,
     dos_folder,
-    output='band_dos_plain_sp.png',
-    up_color='black',
-    down_color='red',
+    output="band_dos_plain_sp.png",
+    up_color="black",
+    down_color="red",
     linewidth=1.25,
-    up_linestyle='-',
-    down_linestyle=':',
+    up_linestyle="-",
+    down_linestyle=":",
     figsize=(6, 3),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=12,
     save=True,
     shift_efermi=0,
@@ -6834,92 +6963,90 @@
         output (str): File name of the resulting plot.
         up_color (str): Color of the spin up band structure lines
         down_color (str): Color of the spin down band structure lines
         linewidth (float): Line width of the band structure lines
         up_linestyle (str): Line style of the spin up bands
         down_linestyle (str): Line style of the spin down bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations. This number should be 
+            This is also only required for unfolded calculations. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         fontsize (float): Font size of the text in the figure.
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
     fig, ax = plt.subplots(
         nrows=1,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
     ax1, ax2 = _figure_setup_band_dos(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
     band_up.plot_plain(
         sp_scale_factor=0,
         ax=ax1,
         color=up_color,
         linewidth=linewidth,
         linestyle=up_linestyle,
@@ -6937,68 +7064,68 @@
 
     dos_up.plot_plain(
         ax=ax2,
         linewidth=linewidth,
         fill=fill,
         alpha=alpha,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color=up_color,
         erange=erange,
     )
 
     dos_down.plot_plain(
         ax=ax2,
         linewidth=linewidth,
         fill=fill,
         alpha=alpha,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color=down_color,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax2.get_xticklabels())
-    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune='lower'))
+    ax2.xaxis.set_major_locator(MaxNLocator(nbins=nbins - 1, prune="lower"))
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax1, ax2
 
 
 def band_dos_spd_spin_polarized(
     band_folder,
     dos_folder,
-    output='band_dos_spd_sp.png',
+    output="band_dos_spd_sp.png",
     scale_factor=5,
-    orbitals='spd',
+    orbitals="spd",
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -7009,141 +7136,145 @@
     This function plots a spin polarized s, p, d projected band structure next to a spin polarized s, p, d projected
     density of states. The top figure highlights the spin up bands and the bottom figure highlights the spin down bands.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
         orbitals (str): String that contains the s, p, or d orbitals that to project onto.
-            The default is 'spd', if the user only wanted to project onto the p, and d orbitals 
+            The default is 'spd', if the user only wanted to project onto the p, and d orbitals
             than 'pd' should be passed in
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_spd(
         ax=ax_band_up,
         scale_factor=scale_factor,
@@ -7167,30 +7298,30 @@
     dos_up.plot_spd(
         ax=ax_dos_up,
         orbitals=orbitals,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_down.plot_spd(
         ax=ax_dos_up,
         orbitals=orbitals,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     band_down.plot_spd(
@@ -7216,75 +7347,76 @@
     dos_down.plot_spd(
         ax=ax_dos_down,
         orbitals=orbitals,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_up.plot_spd(
         ax=ax_dos_down,
         orbitals=orbitals,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
 def band_dos_atom_orbitals_spin_polarized(
     band_folder,
     dos_folder,
     atom_orbital_dict,
-    output='band_dos_atom_orbitals_sp.png',
+    output="band_dos_atom_orbitals_sp.png",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     display_order=None,
     unfold=False,
     M=None,
     high_symm_points=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -7304,134 +7436,138 @@
             corresponding orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of the first atom and the s orbital of the second atom then the dictionary would be {0:[0,1,2,3], 1:[0]}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         unfold=unfold,
-        high_symm_points=high_symm_points, 
-	interpolate=interpolate,
-	new_n=new_n,
+        high_symm_points=high_symm_points,
+        interpolate=interpolate,
+        new_n=new_n,
         soc_axis=soc_axis,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
         M=M,
-	shift_efermi=shift_efermi,
+        shift_efermi=shift_efermi,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_atom_orbitals(
         ax=ax_band_up,
         scale_factor=scale_factor,
@@ -7455,30 +7591,30 @@
     dos_up.plot_atom_orbitals(
         ax=ax_dos_up,
         atom_orbital_dict=atom_orbital_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=total,
         erange=erange,
     )
 
     dos_down.plot_atom_orbitals(
         ax=ax_dos_up,
         atom_orbital_dict=atom_orbital_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=total,
         erange=erange,
     )
 
     band_down.plot_atom_orbitals(
@@ -7504,71 +7640,72 @@
     dos_down.plot_atom_orbitals(
         ax=ax_dos_down,
         atom_orbital_dict=atom_orbital_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=total,
         erange=erange,
     )
 
     dos_up.plot_atom_orbitals(
         ax=ax_dos_down,
         atom_orbital_dict=atom_orbital_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=total,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
 def band_dos_orbitals_spin_polarized(
     band_folder,
     dos_folder,
     orbitals,
-    output='band_dos_orbitals_sp.png',
+    output="band_dos_orbitals_sp.png",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -7603,120 +7740,124 @@
             | 15 = fx3
 
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_orbitals(
         ax=ax_band_up,
         scale_factor=scale_factor,
@@ -7737,30 +7878,30 @@
     dos_up.plot_orbitals(
         ax=ax_dos_up,
         orbitals=orbitals,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_down.plot_orbitals(
         ax=ax_dos_up,
         orbitals=orbitals,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     band_down.plot_orbitals(
@@ -7783,71 +7924,72 @@
     dos_down.plot_orbitals(
         ax=ax_dos_down,
         orbitals=orbitals,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_up.plot_orbitals(
         ax=ax_dos_down,
         orbitals=orbitals,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
 def band_dos_atoms_spin_polarized(
     band_folder,
     dos_folder,
     atoms,
-    output='band_dos_atoms_sp.png',
+    output="band_dos_atoms_sp.png",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -7865,120 +8007,124 @@
         atoms (list): List of atoms to project onto. The indices should be zero indexed (first atom is 0)
             and the atoms are in the same order as they are in the POSCAR
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_atoms(
         ax=ax_band_up,
         scale_factor=scale_factor,
@@ -7999,30 +8145,30 @@
     dos_up.plot_atoms(
         ax=ax_dos_up,
         atoms=atoms,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_down.plot_atoms(
         ax=ax_dos_up,
         atoms=atoms,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     band_down.plot_atoms(
@@ -8045,70 +8191,72 @@
     dos_down.plot_atoms(
         ax=ax_dos_down,
         atoms=atoms,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_up.plot_atoms(
         ax=ax_dos_down,
         atoms=atoms,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
+
 def band_dos_atom_spd_spin_polarized(
     band_folder,
     dos_folder,
     atom_spd_dict,
-    output='band_dos_atom_spd_sp.png',
+    output="band_dos_atom_spd_sp.png",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -8119,128 +8267,132 @@
     This function plots a spin polarized s, p, d projected band structure on a given atom next to a spin polarized
     s, p, d projected density of states on the same atom. The top figure highlights the spin up bands and the bottom
     figure highlights the spin down bands.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
-        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding 
+        atom_spd_dict (dict[int:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of the first atom and the p orbitals of the second atom then the dictionary would be {0:'spd', 1:'p'}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_atom_spd(
         ax=ax_band_up,
         atom_spd_dict=atom_spd_dict,
@@ -8261,30 +8413,30 @@
     dos_up.plot_atom_spd(
         ax=ax_dos_up,
         atom_spd_dict=atom_spd_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_down.plot_atom_spd(
         ax=ax_dos_up,
         atom_spd_dict=atom_spd_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     band_down.plot_atom_spd(
@@ -8307,71 +8459,72 @@
     dos_down.plot_atom_spd(
         ax=ax_dos_down,
         atom_spd_dict=atom_spd_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_up.plot_atom_spd(
         ax=ax_dos_down,
         atom_spd_dict=atom_spd_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
 def band_dos_elements_spin_polarized(
     band_folder,
     dos_folder,
     elements,
-    output='band_dos_elements_sp.png',
+    output="band_dos_elements_sp.png",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -8388,120 +8541,124 @@
         dos_folder (str): This is the folder that contains the VASP files for the density of states
         elements (list): List of elements to project onto. The list should countain the corresponding element symbols
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_elements(
         ax=ax_band_up,
         scale_factor=scale_factor,
@@ -8522,30 +8679,30 @@
     dos_up.plot_elements(
         ax=ax_dos_up,
         elements=elements,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_down.plot_elements(
         ax=ax_dos_up,
         elements=elements,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     band_down.plot_elements(
@@ -8568,71 +8725,72 @@
     dos_down.plot_elements(
         ax=ax_dos_down,
         elements=elements,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_up.plot_elements(
         ax=ax_dos_down,
         elements=elements,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
 def band_dos_element_orbitals_spin_polarized(
     band_folder,
     dos_folder,
     element_orbital_dict,
-    output='band_dos_element_orbitals_sp.png',
+    output="band_dos_element_orbitals_sp.png",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -8643,128 +8801,132 @@
     This function plots a spin polarized band structure projected onto specified [element, orbital] dict next to a spin
     polarized density of states projected onto the same [element, orbital] dict. The top figure highlights the spin up
     bands and the bottom figure highlights the spin down bands.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
-        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding 
+        element_orbital_dict (dict[str:list]): A dictionary that contains the individual elements and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, py, pz, and px orbitals
             of In and the s orbital of As for and InAs structure then the dictionary would be {'In':[0,1,2,3], 'As':[0]}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         kpath=kpath,
-	custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        custom_kpath=custom_kpath,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_element_orbitals(
         ax=ax_band_up,
         scale_factor=scale_factor,
@@ -8785,30 +8947,30 @@
     dos_up.plot_element_orbitals(
         ax=ax_dos_up,
         element_orbital_dict=element_orbital_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_down.plot_element_orbitals(
         ax=ax_dos_up,
         element_orbital_dict=element_orbital_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     band_down.plot_element_orbitals(
@@ -8831,71 +8993,72 @@
     dos_down.plot_element_orbitals(
         ax=ax_dos_down,
         element_orbital_dict=element_orbital_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_up.plot_element_orbitals(
         ax=ax_dos_down,
         element_orbital_dict=element_orbital_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
 def band_dos_element_spd_spin_polarized(
     band_folder,
     dos_folder,
     element_spd_dict,
-    output='band_dos_element_spd_sp.png',
+    output="band_dos_element_spd_sp.png",
     scale_factor=5,
     color_list=None,
     legend=True,
     linewidth=0.75,
-    band_color='black',
-    unprojected_band_color='gray',
+    band_color="black",
+    unprojected_band_color="gray",
     unprojected_linewidth=0.6,
     figsize=(8, 6),
     width_ratios=[7, 3],
     erange=[-6, 6],
     kpath=None,
     custom_kpath=None,
-	stretch_factor=1.0,
+    stretch_factor=1.0,
     n=None,
     fontsize=8,
-    annotations=['$\\uparrow$ ', '$\\downarrow$ '],
+    annotations=["$\\uparrow$ ", "$\\downarrow$ "],
     annotation_xy=(0.0125, 0.98),
     save=True,
     shift_efermi=0,
     interpolate=False,
     new_n=200,
     soc_axis=None,
     fill=True,
@@ -8906,128 +9069,132 @@
     This function plots a spin polarized s, p, d projected band structure on a given element next to a spin polarized
     s, p, d projected density of states on the same element. The top figure highlights the spin up bands and the bottom
     figure highlights the spin down bands.
 
     Parameters:
         band_folder (str): This is the folder that contains the VASP files for the band structure
         dos_folder (str): This is the folder that contains the VASP files for the density of states
-        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding 
+        element_spd_dict (dict[str:str]): A dictionary that contains the individual atoms and the corresponding
             orbitals to project onto. For example, if the user wants to project onto the s, p, d orbitals
             of In and the p orbitals of As for an InAs structure then the dictionary would be {'In':'spd', 'As':'p'}
         output (str): File name of the resulting plot.
         scale_factor (float): Factor to scale weights. This changes the size of the
             points in the scatter plot
         display_order (str / None): If None, the projections will be displayed in the same order
             the user inputs them. If 'all' the projections will be plotted from largest to smallest
-            so every point is visable. If 'dominant' the projections will be plotted from smallest 
+            so every point is visable. If 'dominant' the projections will be plotted from smallest
             to largest so only the dominant projection is shown.
         color_list (list): List of colors that is the same length as the number of projections
             in the plot.
         legend (bool): Determines if the legend should be included or not.
         linewidth (float): Line width of the plain band structure plotted in the background
         band_color (string): Color of the plain band structure
         unprojected_band_color (str): Color of the unprojected band
         unprojected_linewidth (float): Line width of the unprojected bands
         figsize (list / tuple): Desired size of the image in inches (width, height)
-        width_ratios (list / tuple): Width ration of the band plot and dos plot. 
+        width_ratios (list / tuple): Width ration of the band plot and dos plot.
         erange (list / tuple): Range of energy to show in the plot [low, high]
         kpath (list[list]): High symmetry k-point path of band structure calculation
             Due to the nature of the KPOINTS file for unfolded calculations this
             information is a required input for proper labeling of the figure
             for unfolded calculations. This information is extracted from the KPOINTS
             files for non-unfolded calculations. (G is automatically converted to \\Gamma)
-	    (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
-	custom_kpath (list): This gives the option to only plot specific segments of a given band structure
-	    calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
-	    G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
-	    where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
-	    If one of the segements should be flipped it can be done by making its value negative
-	    (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
+            (e.g. For the path X-G-X, kpath=[['X', 'G'], ['G', 'X']])
+        custom_kpath (list): This gives the option to only plot specific segments of a given band structure
+            calculation. For example if the kpath was G-X-W-L then there are three segements to choose from:
+            G-X, X-W, and W-L. In this case the default kpath could be plotted by defining custom_kpath=[1,2,3],
+            where 1 -> G-X, 2 -> X-W, and 3 -> W-L. If only G-X and X-W were desired then custom_kpath=[1,2].
+            If one of the segements should be flipped it can be done by making its value negative
+            (e.g. -1 -> X-G, -2 -> W-X, -3 -> L-W)
         n (int): Number of points between each high symmetry points.
-            This is also only required for unfolded calculations and band unfolding. This number should be 
+            This is also only required for unfolded calculations and band unfolding. This number should be
             known by the user, as it was used to generate the KPOINTS file.
         unfold (bool): Determines if the plotted band structure is from a band unfolding calculation.
         M (list[list]): Transformation matrix from the primitive bulk structure to the slab structure.
             Only required for a band unfolding calculation.
-        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in 
+        high_symm_points (list[list]): List of fractional coordinated for each high symmetry point in
             the band structure path. Only required for a band unfolding calculation.
         fontsize (float): Font size of the text in the figure.
         annotations (list): Annotations to put on the top and bottom (left and right) figures.
             By default it will show the spin up and spin down arrows.
         annotation_xy (list / tuple): Fractional (x, y) coordinated of the annotation location
         fill (bool): Determines wether or not to fill underneath the plot
         alpha (float): Alpha value for the fill
         sigma (float): Standard deviation for gaussian filter
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
 
     fig, ax = plt.subplots(
         nrows=2,
         ncols=2,
         sharey=True,
         figsize=figsize,
         dpi=400,
-        gridspec_kw={'width_ratios': width_ratios}
+        gridspec_kw={"width_ratios": width_ratios},
     )
 
-    ax_band_up, ax_dos_up, ax_band_down, ax_dos_down = _figure_setup_band_dos_spin_polarized(
-        ax=ax,
-        fontsize=fontsize,
-        ylim=[erange[0], erange[1]]
+    (
+        ax_band_up,
+        ax_dos_up,
+        ax_band_down,
+        ax_dos_down,
+    ) = _figure_setup_band_dos_spin_polarized(
+        ax=ax, fontsize=fontsize, ylim=[erange[0], erange[1]]
     )
 
     band_up = Band(
         folder=band_folder,
-        spin='up',
+        spin="up",
         projected=True,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
     band_down = Band(
         folder=band_folder,
-        spin='down',
+        spin="down",
         projected=True,
         kpath=kpath,
         custom_kpath=custom_kpath,
-		stretch_factor=stretch_factor,
+        stretch_factor=stretch_factor,
         n=n,
     )
 
-    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='up')
-    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin='down')
+    dos_up = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="up")
+    dos_down = Dos(shift_efermi=shift_efermi, folder=dos_folder, spin="down")
 
-    bbox = dict(boxstyle='round', fc='white',
-                edgecolor='gray', alpha=0.95, pad=0.3)
+    bbox = dict(
+        boxstyle="round", fc="white", edgecolor="gray", alpha=0.95, pad=0.3
+    )
 
     ax_band_up.annotate(
         annotations[0],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
     ax_band_down.annotate(
         annotations[1],
         xy=annotation_xy,
-        xycoords='axes fraction',
+        xycoords="axes fraction",
         zorder=200,
-        va='top',
-        ha='left',
+        va="top",
+        ha="left",
         bbox=bbox,
         fontsize=fontsize + 1,
     )
 
     band_up.plot_element_spd(
         ax=ax_band_up,
         element_spd_dict=element_spd_dict,
@@ -9048,30 +9215,30 @@
     dos_up.plot_element_spd(
         ax=ax_dos_up,
         element_spd_dict=element_spd_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_down.plot_element_spd(
         ax=ax_dos_up,
         element_spd_dict=element_spd_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     band_down.plot_element_spd(
@@ -9094,90 +9261,91 @@
     dos_down.plot_element_spd(
         ax=ax_dos_down,
         element_spd_dict=element_spd_dict,
         fill=fill,
         alpha=alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=legend,
         total=True,
         erange=erange,
     )
 
     dos_up.plot_element_spd(
         ax=ax_dos_down,
         element_spd_dict=element_spd_dict,
         fill=fill,
         alpha=0.25 * alpha,
         alpha_line=0.25 * alpha,
         linewidth=linewidth,
         sigma=sigma,
-        energyaxis='y',
+        energyaxis="y",
         color_list=color_list,
         legend=False,
         total=True,
         erange=erange,
     )
 
     fig.canvas.draw()
     nbins = len(ax_dos_down.get_xticklabels())
     ax_dos_down.xaxis.set_major_locator(
-        MaxNLocator(nbins=nbins - 1, prune='lower'))
+        MaxNLocator(nbins=nbins - 1, prune="lower")
+    )
 
     plt.tight_layout(pad=0.4)
     plt.subplots_adjust(wspace=0, hspace=0.05)
 
     if save:
         plt.savefig(output)
     else:
         return fig, ax_band_up, ax_dos_up, ax_band_down, ax_dos_down
 
 
 def dos_layers(
     folder,
-    output='dos_layers.png',
-    energyaxis='y',
+    output="dos_layers.png",
+    energyaxis="y",
     figsize=(5, 3),
     erange=[-3, 3],
     lrange=None,
-    spin='up',
+    spin="up",
     soc_axis=None,
-    combination_method='add',
+    combination_method="add",
     fontsize=12,
     save=True,
     shift_efermi=0,
-    cmap='magma',
+    cmap="magma",
     sigma_energy=0.05,
     sigma_layers=0.75,
     antialiased=False,
     show_structure=False,
     interface_layer=None,
     show_interface_line=False,
-    interface_line_color='white',
-    interface_line_style='--',
+    interface_line_color="white",
+    interface_line_style="--",
     interface_line_width=2,
     log_scale=True,
     contour=False,
     levels=10,
     min_cutoff=1e-7,
     max_cutoff=None,
     atol=None,
     custom_layer_inds=None,
     custom_cbar_label=None,
     plot_vbm_cbm=False,
-    vbm_color='white',
-    cbm_color='white',
-    vbm_linestyle=':',
-    cbm_linestyle=':',
-    cbar_orientation='vertical',
+    vbm_color="white",
+    cbm_color="white",
+    vbm_linestyle=":",
+    cbm_linestyle=":",
+    cbar_orientation="vertical",
     show_bounds=False,
     set_bounds=None,
-    sp_method='percentage',
+    sp_method="percentage",
 ):
     """
     This function is used to plot a layer by layer density of states heat map for slab structures. It is useful for
     visualizing band alignment of interfaces.
 
     Parameters:
         folder (str): This is the folder that contains the VASP files
@@ -9200,15 +9368,15 @@
         lrange (list): Upper and lower bounds of the layers included in the plot.
         antialiased (bool): Determines if antialiasing is used or not.
         fontsize (float): Fontsize of all the text in the group.
         interface_layer (float or None): If a value is provided, then the axis labels will be
             shifted accordingly so that the defined interface layer is zero.
         show_interface_line (bool): If True, then a line will be drawn
             on the plot to identify the interface layer defined by interface_layer.
-        interface_line_color (str): Color of the line drawn on the plot to mark the 
+        interface_line_color (str): Color of the line drawn on the plot to mark the
             interface.
         interface_line_width (float): Line with of the line marking the interface.
         interface_line_style (str): Style of the line marking the interface.
         log_scale (bool): Determines if the color map is applied in log scale of not.
             Recommended in order to accurately view the band gap and smaller features.
         contour (bool): Determines if the color map is plotted as a contour plot instead
             of a heatmap.
@@ -9221,71 +9389,73 @@
             This value is automatically calculated if None and is usually on the order of
             1e-3.
         custom_layer_inds (list or None): If the structure being calculated has relaxed
             atomic positions, sometimes the layer grouping algorithm can behave non-idealy.
             If this is the case, the user can input a list of list that contain the
             atomic indices in each layers of the material.
         custom_cbar_label (str or None): Custom label for the colorbar
-        save (bool): Determines whether to automatically save the figure or not. If not 
+        save (bool): Determines whether to automatically save the figure or not. If not
             the figure and axis are return for further manipulation.
         plot_vbm_cbm (bool): Determines if the valence band maximum and conduction band minimum
             are plotted on the graph.
         vbm_color (str): Color of the vbm line.
         cbm_color (str): Color of the cbm line.
         vbm_linestyle (str): Linestyle of the vbm line.
         cbm_linestyle (str): Linestyle of the cbm line.
 
     Returns:
         If save == True, this function will return nothing and directly save the image as
         the output name. If save == False, the function will return the matplotlib figure
-        and axis for further editing. 
+        and axis for further editing.
     """
     if show_structure:
-        if energyaxis == 'x':
+        if energyaxis == "x":
             fig, axs = plt.subplots(
                 nrows=1,
                 ncols=2,
-                gridspec_kw={'width_ratios':[1,6]},
+                gridspec_kw={"width_ratios": [1, 6]},
                 figsize=figsize,
                 dpi=400,
             )
             structure_ax = axs[0]
             dos_ax = axs[1]
-            
-        elif energyaxis == 'y':
+
+        elif energyaxis == "y":
             fig, axs = plt.subplots(
                 nrows=2,
                 ncols=1,
-                gridspec_kw={'height_ratios':[1,6], 'hspace': -0.02},
+                gridspec_kw={"height_ratios": [1, 6], "hspace": -0.02},
                 figsize=figsize,
                 dpi=400,
             )
             structure_ax = axs[0]
             sm = plt.cm.ScalarMappable()
             sm.set_array([])
             fig.colorbar(sm, ax=structure_ax).ax.set_visible(False)
             dos_ax = axs[1]
 
-        structure_ax.spines['left'].set_visible(False)
-        structure_ax.spines['right'].set_visible(False)
-        structure_ax.spines['top'].set_visible(False)
-        structure_ax.spines['bottom'].set_visible(False)
+        structure_ax.spines["left"].set_visible(False)
+        structure_ax.spines["right"].set_visible(False)
+        structure_ax.spines["top"].set_visible(False)
+        structure_ax.spines["bottom"].set_visible(False)
 
         structure_ax.tick_params(
             left=False,
             bottom=False,
             labelleft=False,
             labelbottom=False,
         )
 
     else:
         fig = plt.figure(figsize=figsize, dpi=400)
         dos_ax = fig.add_subplot(111)
-        
-    _figure_setup_layer_dos(ax=dos_ax, fontsize=fontsize, energyaxis=energyaxis)
+
+    _figure_setup_layer_dos(
+        ax=dos_ax, fontsize=fontsize, energyaxis=energyaxis
+    )
 
     dos = Dos(
         shift_efermi=shift_efermi,
         folder=folder,
         spin=spin,
         soc_axis=soc_axis,
         combination_method=combination_method,
@@ -9321,130 +9491,132 @@
 
     if plot_vbm_cbm:
         gap = BandGap(folder=folder)
         vbm = gap.vbm
         cbm = gap.cbm
         # _, vbm, cbm = get_bandgap(folder=folder, printbg=False, return_vbm_cbm=True)
 
-        if energyaxis == 'y':
+        if energyaxis == "y":
             dos_ax.axhline(
                 y=cbm,
                 color=cbm_color,
                 linestyle=cbm_linestyle,
             )
             dos_ax.axhline(
                 y=vbm,
                 color=vbm_color,
                 linestyle=vbm_linestyle,
             )
-        elif energyaxis == 'x':
+        elif energyaxis == "x":
             dos_ax.axvline(
                 x=cbm,
                 color=cbm_color,
                 linestyle=cbm_linestyle,
             )
             dos_ax.axvline(
                 x=vbm,
                 color=vbm_color,
                 linestyle=vbm_linestyle,
             )
 
-    if energyaxis == 'y':
+    if energyaxis == "y":
         dos_ax.set_ylim(erange[0], erange[1])
-    elif energyaxis == 'x':
+    elif energyaxis == "x":
         dos_ax.set_xlim(erange[0], erange[1])
 
     if show_structure:
-        if energyaxis == 'y':
-            dos.plot_structure(ax=structure_ax, rotation=[90,90,90])
-        elif energyaxis == 'x':
-            dos.plot_structure(ax=structure_ax, rotation=[0,90,90])
+        if energyaxis == "y":
+            dos.plot_structure(ax=structure_ax, rotation=[90, 90, 90])
+        elif energyaxis == "x":
+            dos.plot_structure(ax=structure_ax, rotation=[0, 90, 90])
             fig.tight_layout(pad=0.4)
 
     if save:
-        plt.savefig(output, bbox_inches='tight')
+        plt.savefig(output, bbox_inches="tight")
     else:
         if show_structure:
             return fig, dos_ax, structure_ax
         else:
             return fig, dos_ax
 
 
 def _main():
     #  band_plain_spin_polarized(
-        #  folder='../../vaspvis_data/band_Cr2O3',
-        #  figsize=(7,3),
-        #  #  interpolate=True
+    #  folder='../../vaspvis_data/band_Cr2O3',
+    #  figsize=(7,3),
+    #  #  interpolate=True
     #  )
     #  band_spd(
-        #  folder='../../vaspvis_data/band_InAs',
-        #  interpolate=False,
-        #  custom_kpath=[1,2,3,4,5,-5,-4,-3,-2,-1]
+    #  folder='../../vaspvis_data/band_InAs',
+    #  interpolate=False,
+    #  custom_kpath=[1,2,3,4,5,-5,-4,-3,-2,-1]
     #  )
     #  dos_orbitals(
-        #  folder='../../vaspvis_data/Fe-slab/',
-        #  orbitals=[0,1,2,3],
-        #  spin='both',
-        #  combination_method='sub',
-        #  color_list=['red' for _ in range(4)]
-    #  )
-     dos_layers(
-         folder='../../vaspvis_data/Fe-slab',
-         spin='both',
-         combination_method='sub',
-         sp_method='percentage',
-         output='percentage_shift.png',
-         log_scale=False,
-         show_bounds=True,
-         interface_layer=10,
-     )
-    #  dos_layers(
-        #  folder='../../vaspvis_data/Fe-slab',
-        #  spin='both',
-        #  combination_method='sub',
-        #  sp_method='absolute',
-        #  output='absolute.png',
-        #  log_scale=False,
-        #  show_bounds=True,
-    #  )
-    #  band_plain_spin_polarized(
-        #  folder='../../vaspvis_data/Fe-sp/band',
-        #  up_linestyle='-',
-        #  down_linestyle='-',
-        #  output='Fe_sp.png',
-    #  )
-    #  dos_layers(
-        #  folder='../../vaspvis_data/slabdos',
-        #  soc_axis='z',
-        #  spin='both',
-        #  sp_method='absolute',
-        #  combination_method='sub',
-        #  log_scale=False,
+    #  folder='../../vaspvis_data/Fe-slab/',
+    #  orbitals=[0,1,2,3],
+    #  spin='both',
+    #  combination_method='sub',
+    #  color_list=['red' for _ in range(4)]
     #  )
-    # M = [[-0.,  0., -1.],[ 1., -1.,  0.],[-16., -16.,  16.]]
+    dos_layers(
+        folder="../../vaspvis_data/Fe-slab",
+        spin="both",
+        combination_method="sub",
+        sp_method="percentage",
+        output="percentage_shift.png",
+        log_scale=False,
+        show_bounds=True,
+        interface_layer=10,
+    )
 
-    # high_symm_points = [
-    #      [0.5, 0.0, 0.5],     
-    #      [0.0, 0.0, 0.0],          
-    #      [0.5, 0.0, 0.5],
-    # ]
-    #  band_spd(
-    #  band_spd_spin_polarized(
-        #  folder="../../vaspvis_data/band_EuS_slab/band",
-        #  #  atoms=[0,1,3,4],
-        #  #  color_list=['green', 'green', 'orange', 'orange'],
-        #  interpolate=False,
-        #  soc_axis='z',
-        #  unfold=True,
-        #  M=M,
-        #  high_symm_points=high_symm_points,
-        #  n=30,
-        #  new_n=50,
-        #  kpath=[['X', 'G'], ['G', 'X']],
-        #  erange=[-6,3],
-        #  #  sp_scale_factor=3,
-        #  scale_factor=1000,
-    #  )
-    # dos_plain(folder='../../vaspvis_data/dos_InAs', fill=False, log_scale=False)
+
+#  dos_layers(
+#  folder='../../vaspvis_data/Fe-slab',
+#  spin='both',
+#  combination_method='sub',
+#  sp_method='absolute',
+#  output='absolute.png',
+#  log_scale=False,
+#  show_bounds=True,
+#  )
+#  band_plain_spin_polarized(
+#  folder='../../vaspvis_data/Fe-sp/band',
+#  up_linestyle='-',
+#  down_linestyle='-',
+#  output='Fe_sp.png',
+#  )
+#  dos_layers(
+#  folder='../../vaspvis_data/slabdos',
+#  soc_axis='z',
+#  spin='both',
+#  sp_method='absolute',
+#  combination_method='sub',
+#  log_scale=False,
+#  )
+# M = [[-0.,  0., -1.],[ 1., -1.,  0.],[-16., -16.,  16.]]
+
+# high_symm_points = [
+#      [0.5, 0.0, 0.5],
+#      [0.0, 0.0, 0.0],
+#      [0.5, 0.0, 0.5],
+# ]
+#  band_spd(
+#  band_spd_spin_polarized(
+#  folder="../../vaspvis_data/band_EuS_slab/band",
+#  #  atoms=[0,1,3,4],
+#  #  color_list=['green', 'green', 'orange', 'orange'],
+#  interpolate=False,
+#  soc_axis='z',
+#  unfold=True,
+#  M=M,
+#  high_symm_points=high_symm_points,
+#  n=30,
+#  new_n=50,
+#  kpath=[['X', 'G'], ['G', 'X']],
+#  erange=[-6,3],
+#  #  sp_scale_factor=3,
+#  scale_factor=1000,
+#  )
+# dos_plain(folder='../../vaspvis_data/dos_InAs', fill=False, log_scale=False)
 
 if __name__ == "__main__":
     _main()
```

### Comparing `vaspvis-1.2.7/vaspvis/stm.py` & `vaspvis-1.2.8/vaspvis/stm.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis/unfold/convert.py` & `vaspvis-1.2.8/vaspvis/unfold/convert.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis/unfold/unfold.py` & `vaspvis-1.2.8/vaspvis/unfold/unfold.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis/unfold/vasp_constant.py` & `vaspvis-1.2.8/vaspvis/unfold/vasp_constant.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis/unfold/vaspwfc.py` & `vaspvis-1.2.8/vaspvis/unfold/vaspwfc.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis/utils.py` & `vaspvis-1.2.8/vaspvis/utils.py`

 * *Files identical despite different names*

### Comparing `vaspvis-1.2.7/vaspvis.egg-info/PKG-INFO` & `vaspvis-1.2.8/vaspvis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaspvis
-Version: 1.2.7
+Version: 1.2.8
 Summary: A highly flexible and customizable library for visualizing electronic structure data from VASP calculations
 Home-page: https://github.com/DerekDardzinski/vaspvis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # vaspvis
```

### Comparing `vaspvis-1.2.7/vaspvis.egg-info/SOURCES.txt` & `vaspvis-1.2.8/vaspvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

