# Comparing `tmp/sunweg-2.0.0b2.tar.gz` & `tmp/sunweg-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunweg-2.0.0b2.tar", last modified: Thu Jul  6 14:00:45 2023, max compression
+gzip compressed data, was "sunweg-2.0.0b3.tar", last modified: Thu Jul  6 14:30:43 2023, max compression
```

## Comparing `sunweg-2.0.0b2.tar` & `sunweg-2.0.0b3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:00:45.045709 sunweg-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 14:00:45.045709 sunweg-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:00:45.045709 sunweg-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:00:45.041709 sunweg-2.0.0b2/sunweg/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/sunweg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/sunweg/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/sunweg/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/sunweg/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/sunweg/plant.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/sunweg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:00:45.045709 sunweg-2.0.0b2/sunweg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 14:00:45.000000 sunweg-2.0.0b2/sunweg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 14:00:45.000000 sunweg-2.0.0b2/sunweg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:00:45.000000 sunweg-2.0.0b2/sunweg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 14:00:45.000000 sunweg-2.0.0b2/sunweg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 14:00:45.000000 sunweg-2.0.0b2/sunweg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:00:45.045709 sunweg-2.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-07-06 14:00:30.000000 sunweg-2.0.0b2/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:30:43.353629 sunweg-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 14:30:43.353629 sunweg-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:30:43.353629 sunweg-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:30:43.353629 sunweg-2.0.0b3/sunweg/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/sunweg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/sunweg/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/sunweg/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/sunweg/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/sunweg/plant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/sunweg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:30:43.353629 sunweg-2.0.0b3/sunweg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 14:30:43.000000 sunweg-2.0.0b3/sunweg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 14:30:43.000000 sunweg-2.0.0b3/sunweg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:30:43.000000 sunweg-2.0.0b3/sunweg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 14:30:43.000000 sunweg-2.0.0b3/sunweg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 14:30:43.000000 sunweg-2.0.0b3/sunweg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:30:43.353629 sunweg-2.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-07-06 14:30:31.000000 sunweg-2.0.0b3/tests/test_api.py
```

### Comparing `sunweg-2.0.0b2/LICENSE` & `sunweg-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b2/PKG-INFO` & `sunweg-2.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sunweg-2.0.0b2/README.md` & `sunweg-2.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b2/setup.py` & `sunweg-2.0.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 requires = [
     "requests",
 ]
 
 setuptools.setup(
     name="sunweg",
-    version="2.0.0b2",
+    version="2.0.0b3",
     author="rokam",
     author_email="lucas@mindello.com.br",
     description="A library to retrieve data from sunweg.net",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rokam/sunweg",
```

### Comparing `sunweg-2.0.0b2/sunweg/api.py` & `sunweg-2.0.0b3/sunweg/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,25 +203,25 @@
         :type retry: bool
         """
         try:
             result = self._get(SUNWEG_INVERTER_DETAIL_PATH + str(inverter.id))
             inverter.total_energy = float(
                 result["energiaAcumulada"].split(" ")[0].replace(",", ".")
             )
-            inverter.total_energy_metric = (result["energiaAcumulada"].split(" ")[1],)
+            inverter.total_energy_metric = result["energiaAcumulada"].split(" ")[1]
             inverter.today_energy = float(
                 result["energiaDoDia"].split(" ")[0].replace(",", ".")
             )
-            inverter.today_energy_metric = (result["energiaDoDia"].split(" ")[1],)
+            inverter.today_energy_metric = result["energiaDoDia"].split(" ")[1]
             inverter.power_factor = float(result["fatorpotencia"].replace(",", "."))
             inverter.frequency = float(result["frequencia"].replace(",", "."))
             inverter.power = float(
                 result["potenciaativa"].split(" ")[0].replace(",", ".")
             )
-            inverter.power_metric = (result["potenciaativa"].split(" ")[1],)
+            inverter.power_metric = result["potenciaativa"].split(" ")[1]
 
             self._populate_MPPT(result=result, inverter=inverter)
         except LoginError:
             if retry:
                 self.authenticate()
                 self.complete_inverter(inverter, False)
```

### Comparing `sunweg-2.0.0b2/sunweg/const.py` & `sunweg-2.0.0b3/sunweg/const.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b2/sunweg/device.py` & `sunweg-2.0.0b3/sunweg/device.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b2/sunweg/plant.py` & `sunweg-2.0.0b3/sunweg/plant.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b2/sunweg.egg-info/PKG-INFO` & `sunweg-2.0.0b3/sunweg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sunweg-2.0.0b2/tests/common.py` & `sunweg-2.0.0b3/tests/common.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b2/tests/test_api.py` & `sunweg-2.0.0b3/tests/test_api.py`

 * *Files identical despite different names*

