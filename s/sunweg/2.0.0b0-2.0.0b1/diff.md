# Comparing `tmp/sunweg-2.0.0b0.tar.gz` & `tmp/sunweg-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunweg-2.0.0b0.tar", last modified: Thu Jul  6 10:36:08 2023, max compression
+gzip compressed data, was "sunweg-2.0.0b1.tar", last modified: Thu Jul  6 13:53:29 2023, max compression
```

## Comparing `sunweg-2.0.0b0.tar` & `sunweg-2.0.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/sunweg/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/plant.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/sunweg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:29.870240 sunweg-2.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 13:53:29.870240 sunweg-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:53:29.870240 sunweg-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:29.866240 sunweg-2.0.0b1/sunweg/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/sunweg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/sunweg/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/sunweg/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/sunweg/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/sunweg/plant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/sunweg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:29.870240 sunweg-2.0.0b1/sunweg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 13:53:29.000000 sunweg-2.0.0b1/sunweg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 13:53:29.000000 sunweg-2.0.0b1/sunweg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:53:29.000000 sunweg-2.0.0b1/sunweg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 13:53:29.000000 sunweg-2.0.0b1/sunweg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:53:29.000000 sunweg-2.0.0b1/sunweg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:29.870240 sunweg-2.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-06 13:53:15.000000 sunweg-2.0.0b1/tests/test_api.py
```

### Comparing `sunweg-2.0.0b0/LICENSE` & `sunweg-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b0/PKG-INFO` & `sunweg-2.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sunweg-2.0.0b0/README.md` & `sunweg-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b0/setup.py` & `sunweg-2.0.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 requires = [
     "requests",
 ]
 
 setuptools.setup(
     name="sunweg",
-    version="2.0.0b",
+    version="2.0.0b1",
     author="rokam",
     author_email="lucas@mindello.com.br",
     description="A library to retrieve data from sunweg.net",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rokam/sunweg",
```

### Comparing `sunweg-2.0.0b0/sunweg/api.py` & `sunweg-2.0.0b1/sunweg/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             )
             inverter.total_energy_metric = (result["energiaAcumulada"].split(" ")[1],)
             inverter.today_energy = float(
                 result["energiaDoDia"].split(" ")[0].replace(",", ".")
             )
             inverter.today_energy_metric = (result["energiaDoDia"].split(" ")[1],)
             inverter.power_factor = float(result["fatorpotencia"].replace(",", "."))
-            inverter.frequency = result["frequencia"]
+            inverter.frequency = float(result["frequencia"].replace(",", "."))
             inverter.power = float(
                 result["potenciaativa"].split(" ")[0].replace(",", ".")
             )
             inverter.power_metric = (result["potenciaativa"].split(" ")[1],)
 
             self._populate_MPPT(result=result, inverter=inverter)
         except LoginError:
```

### Comparing `sunweg-2.0.0b0/sunweg/const.py` & `sunweg-2.0.0b1/sunweg/const.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b0/sunweg/device.py` & `sunweg-2.0.0b1/sunweg/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,16 +228,16 @@
         :type temperature: int
         :param total_energy: total generated energy
         :type total_energy: float
         :param total_energy_metric: total generated energy metric
         :type total_energy_metric: str
         :param today_energy: total generated energy today
         :type today_energy: float
-        :param today_energy: total generated energy today metric
-        :type today_energy: str
+        :param today_energy_metric: total generated energy today metric
+        :type today_energy_metric: str
         :param power_factor: inverter power factor
         :type power_factor: float
         :param frequency: inverter output frequency in Hz
         :type frequency: float
         :param power: inverter output power
         :type power: float
         :param power: inverter output power metric
```

### Comparing `sunweg-2.0.0b0/sunweg/plant.py` & `sunweg-2.0.0b1/sunweg/plant.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b0/sunweg.egg-info/PKG-INFO` & `sunweg-2.0.0b1/sunweg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sunweg-2.0.0b0/tests/common.py` & `sunweg-2.0.0b1/tests/common.py`

 * *Files identical despite different names*

### Comparing `sunweg-2.0.0b0/tests/test_api.py` & `sunweg-2.0.0b1/tests/test_api.py`

 * *Files identical despite different names*

