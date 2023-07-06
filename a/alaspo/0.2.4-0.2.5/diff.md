# Comparing `tmp/alaspo-0.2.4.tar.gz` & `tmp/alaspo-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alaspo-0.2.4.tar", last modified: Thu Mar 16 09:31:49 2023, max compression
+gzip compressed data, was "alaspo-0.2.5.tar", last modified: Thu Jul  6 10:50:11 2023, max compression
```

## Comparing `alaspo-0.2.4.tar` & `alaspo-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-03-16 09:31:49.750508 alaspo-0.2.4/
--rw-r--r--   0 tgeibing   (501) staff       (20)     1047 2023-02-06 12:44:36.000000 alaspo-0.2.4/LICENSE
--rw-r--r--   0 tgeibing   (501) staff       (20)     1381 2023-03-16 09:31:49.750374 alaspo-0.2.4/PKG-INFO
--rw-r--r--   0 tgeibing   (501) staff       (20)      988 2023-02-09 23:05:59.000000 alaspo-0.2.4/README.md
--rw-r--r--   0 tgeibing   (501) staff       (20)      615 2023-02-09 23:05:59.000000 alaspo-0.2.4/READMEPyPi.md
--rw-r--r--   0 tgeibing   (501) staff       (20)     1170 2023-02-24 15:58:56.000000 alaspo-0.2.4/pyproject.toml
--rw-r--r--   0 tgeibing   (501) staff       (20)       38 2023-03-16 09:31:49.750543 alaspo-0.2.4/setup.cfg
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-03-16 09:31:49.747038 alaspo-0.2.4/src/
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-03-16 09:31:49.749510 alaspo-0.2.4/src/alaspo/
--rw-r--r--   0 tgeibing   (501) staff       (20)       53 2023-02-06 12:44:36.000000 alaspo-0.2.4/src/alaspo/__init__.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     9044 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/__main__.py
--rw-r--r--   0 tgeibing   (501) staff       (20)       24 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/__version__.py
--rw-r--r--   0 tgeibing   (501) staff       (20)       51 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/config.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     2051 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/initial.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     1817 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/json_config.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     5450 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/lns.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     7612 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/relax.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     3958 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/search.py
--rw-r--r--   0 tgeibing   (501) staff       (20)    17627 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/solver.py
--rw-r--r--   0 tgeibing   (501) staff       (20)    11401 2023-03-16 09:31:25.000000 alaspo-0.2.4/src/alaspo/strategy.py
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-03-16 09:31:49.750224 alaspo-0.2.4/src/alaspo.egg-info/
--rw-r--r--   0 tgeibing   (501) staff       (20)     1381 2023-03-16 09:31:49.000000 alaspo-0.2.4/src/alaspo.egg-info/PKG-INFO
--rw-r--r--   0 tgeibing   (501) staff       (20)      496 2023-03-16 09:31:49.000000 alaspo-0.2.4/src/alaspo.egg-info/SOURCES.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)        1 2023-03-16 09:31:49.000000 alaspo-0.2.4/src/alaspo.egg-info/dependency_links.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)       48 2023-03-16 09:31:49.000000 alaspo-0.2.4/src/alaspo.egg-info/entry_points.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)       52 2023-03-16 09:31:49.000000 alaspo-0.2.4/src/alaspo.egg-info/requires.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)        7 2023-03-16 09:31:49.000000 alaspo-0.2.4/src/alaspo.egg-info/top_level.txt
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.288180 alaspo-0.2.5/
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1047 2023-02-06 12:44:36.000000 alaspo-0.2.5/LICENSE
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1381 2023-07-06 10:50:11.288056 alaspo-0.2.5/PKG-INFO
+-rw-r--r--   0 tgeibing   (501) staff       (20)      988 2023-02-09 23:05:59.000000 alaspo-0.2.5/README.md
+-rw-r--r--   0 tgeibing   (501) staff       (20)      615 2023-02-09 23:05:59.000000 alaspo-0.2.5/READMEPyPi.md
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1170 2023-02-24 15:58:56.000000 alaspo-0.2.5/pyproject.toml
+-rw-r--r--   0 tgeibing   (501) staff       (20)       38 2023-07-06 10:50:11.288222 alaspo-0.2.5/setup.cfg
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.284202 alaspo-0.2.5/src/
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.287155 alaspo-0.2.5/src/alaspo/
+-rw-r--r--   0 tgeibing   (501) staff       (20)       53 2023-02-06 12:44:36.000000 alaspo-0.2.5/src/alaspo/__init__.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     9044 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/__main__.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)       24 2023-07-06 10:49:02.000000 alaspo-0.2.5/src/alaspo/__version__.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)       51 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/config.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     2051 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/initial.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1817 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/json_config.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     5450 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/lns.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     7612 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/relax.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     3958 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/search.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)    17548 2023-07-06 10:49:02.000000 alaspo-0.2.5/src/alaspo/solver.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)    11401 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/strategy.py
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.287871 alaspo-0.2.5/src/alaspo.egg-info/
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1381 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/PKG-INFO
+-rw-r--r--   0 tgeibing   (501) staff       (20)      496 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/SOURCES.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)        1 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/dependency_links.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)       48 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/entry_points.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)       52 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/requires.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)        7 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/top_level.txt
```

### Comparing `alaspo-0.2.4/LICENSE` & `alaspo-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/PKG-INFO` & `alaspo-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alaspo
-Version: 0.2.4
+Version: 0.2.5
 Summary: ALASPO: ASP + Large-Neighborhood Search
 Author-email: Tobias Geibinger <tobias.geibinger@tuwien.ac.at>, Thomas Eiter <thomas.eiter@tuwien.ac.at>, Johannes Oetsch <johannes.oetsch@tuwien.ac.at>, Nelson Higuera Ruiz <nelson.ruiz@tuwien.ac.at>, Nysret Musliu <nysret.musliu@tuwien.ac.at>, Daria Stepanova <daria.stepanova@de.bosch.com>
 Project-URL: Homepage, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo
 Project-URL: Bug Tracker, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alaspo-0.2.4/README.md` & `alaspo-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/READMEPyPi.md` & `alaspo-0.2.5/READMEPyPi.md`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/pyproject.toml` & `alaspo-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo/__main__.py` & `alaspo-0.2.5/src/alaspo/__main__.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo/initial.py` & `alaspo-0.2.5/src/alaspo/initial.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo/json_config.py` & `alaspo-0.2.5/src/alaspo/json_config.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo/lns.py` & `alaspo-0.2.5/src/alaspo/lns.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo/relax.py` & `alaspo-0.2.5/src/alaspo/relax.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo/search.py` & `alaspo-0.2.5/src/alaspo/search.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo/solver.py` & `alaspo-0.2.5/src/alaspo/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,16 @@
                 None ... no answer set was found
                 Model ... the found answer set
         """
         sol = argparse.Namespace()
         sol.sat = result.satisfiable if result else None
         sol.cost = self._read_cost(model) if model else None
         sol.model = model
-        if sol.cost == None:
-            sol.exhausted = True
-        else:
-            sol.exhausted = result.exhausted if result else None
+        sol.exhausted = result.exhausted if result else None
+
         return sol
 
     def _ast_visitor(self, ast, pb):
         """
         called on the addition of a new ast node to the program
         """
         pass
```

### Comparing `alaspo-0.2.4/src/alaspo/strategy.py` & `alaspo-0.2.5/src/alaspo/strategy.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.4/src/alaspo.egg-info/PKG-INFO` & `alaspo-0.2.5/src/alaspo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alaspo
-Version: 0.2.4
+Version: 0.2.5
 Summary: ALASPO: ASP + Large-Neighborhood Search
 Author-email: Tobias Geibinger <tobias.geibinger@tuwien.ac.at>, Thomas Eiter <thomas.eiter@tuwien.ac.at>, Johannes Oetsch <johannes.oetsch@tuwien.ac.at>, Nelson Higuera Ruiz <nelson.ruiz@tuwien.ac.at>, Nysret Musliu <nysret.musliu@tuwien.ac.at>, Daria Stepanova <daria.stepanova@de.bosch.com>
 Project-URL: Homepage, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo
 Project-URL: Bug Tracker, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

