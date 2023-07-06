# Comparing `tmp/wwtp-configuration-0.2.3.tar.gz` & `tmp/wwtp-configuration-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwtp-configuration-0.2.3.tar", last modified: Thu May  4 17:23:35 2023, max compression
+gzip compressed data, was "wwtp-configuration-0.3.0.tar", last modified: Thu Jul  6 03:55:22 2023, max compression
```

## Comparing `wwtp-configuration-0.2.3.tar` & `wwtp-configuration-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:23:35.041539 wwtp-configuration-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-04 17:23:35.041539 wwtp-configuration-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:23:35.041539 wwtp-configuration-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/connection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/node.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/parse_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/tag.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/docs/visualize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 17:23:35.041539 wwtp-configuration-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:23:35.041539 wwtp-configuration-0.2.3/wwtp_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:23:35.041539 wwtp-configuration-0.2.3/wwtp_configuration/data/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/data/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/data/unit_definitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)    71197 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    43691 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/parse_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-04 17:23:29.000000 wwtp-configuration-0.2.3/wwtp_configuration/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:23:35.041539 wwtp-configuration-0.2.3/wwtp_configuration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-04 17:23:34.000000 wwtp-configuration-0.2.3/wwtp_configuration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 17:23:34.000000 wwtp-configuration-0.2.3/wwtp_configuration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:23:34.000000 wwtp-configuration-0.2.3/wwtp_configuration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:23:34.000000 wwtp-configuration-0.2.3/wwtp_configuration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 17:23:34.000000 wwtp-configuration-0.2.3/wwtp_configuration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 17:23:34.000000 wwtp-configuration-0.2.3/wwtp_configuration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.491190 wwtp-configuration-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/connection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/node.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/parse_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/tag.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/visualize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-06 03:55:22.499190 wwtp-configuration-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/wwtp_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/wwtp_configuration/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/data/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/data/unit_definitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    71289 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44321 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/parse_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/top_level.txt
```

### Comparing `wwtp-configuration-0.2.3/CONTRIBUTING.rst` & `wwtp-configuration-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/LICENSE` & `wwtp-configuration-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/PKG-INFO` & `wwtp-configuration-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwtp-configuration
-Version: 0.2.3
+Version: 0.3.0
 Summary: Class hierarchy to represent a wastewater treatment plant's configuration.
 Home-page: https://github.com/we3lab/wwtp-configuration
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: wwtp-configuration
 Platform: UNKNOWN
```

### Comparing `wwtp-configuration-0.2.3/README.rst` & `wwtp-configuration-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/docs/Makefile` & `wwtp-configuration-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/docs/conf.py` & `wwtp-configuration-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/docs/index.rst` & `wwtp-configuration-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/docs/make.bat` & `wwtp-configuration-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/setup.py` & `wwtp-configuration-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,10 +63,10 @@
     python_requires=">=3.9",
     install_requires=requirements,
     setup_requires=setup_requirements,
     tests_require=test_requirements,
     extras_require=extra_requirements,
     test_suite="tests",
     url="https://github.com/we3lab/wwtp-configuration",
-    version="0.2.3",
+    version="0.3.0",
     zip_safe=False,
 )
```

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration/connection.py` & `wwtp-configuration-0.3.0/wwtp_configuration/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         """Adds a tag to the node
 
         Parameters
         ----------
         tag : Tag
             Tag object to add to the node
         """
+        if not tag.parent_id:
+            tag.parent_id = self.id
         self.tags[tag.id] = tag
 
     def remove_tag(self, tag_name):
         """Removes a tag from the node
 
         Parameters
         ----------
@@ -427,23 +429,24 @@
             return self.entry_point < self.entry_point
         elif len(self.tags) < len(other.tags):
             return True
         elif len(self.tags) > len(other.tags):
             return False
         elif self.tags == other.tags:
             if self.source != other.source:
-                if isinstance(self.source, type(other.source)):
-                    return self.source < other.source
-                else:
-                    return self.source.id < other.source.id
+                # TODO: uncomment when node comparison are supported
+                # if isinstance(self.source, type(other.source)):
+                #     return self.source < other.source
+                # else:
+                return self.source.id < other.source.id
             elif self.destination != other.destination:
-                if isinstance(self.destination, type(other.destination)):
-                    return self.destination < other.destination
-                else:
-                    return self.destination.id < other.destination.id
+                # if isinstance(self.destination, type(other.destination)):
+                #     return self.destination < other.destination
+                # else:
+                return self.destination.id < other.destination.id
             else:
                 return self.id < other.id
         # case with same number of different tags, so we compare tags in order
         else:
             other_tags = [tag for _, tag in sorted(other.tags.items())]
             for i, tag in enumerate([tag for _, tag in sorted(self.tags.items())]):
                 if tag != other_tags[i]:
@@ -604,23 +607,24 @@
             return self.entry_point < self.entry_point
         elif len(self.tags) < len(other.tags):
             return True
         elif len(self.tags) > len(other.tags):
             return False
         elif self.tags == other.tags:
             if self.source != other.source:
-                if isinstance(self.source, type(other.source)):
-                    return self.source < other.source
-                else:
-                    return self.source.id < other.source.id
+                # TODO: uncomment when node comparison are supported
+                # if isinstance(self.source, type(other.source)):
+                #     return self.source < other.source
+                # else:
+                return self.source.id < other.source.id
             elif self.destination != other.destination:
-                if isinstance(self.destination, type(other.destination)):
-                    return self.destination < other.destination
-                else:
-                    return self.destination.id < other.destination.id
+                # if isinstance(self.destination, type(other.destination)):
+                #     return self.destination < other.destination
+                # else:
+                return self.destination.id < other.destination.id
             else:
                 return self.id < other.id
         # case with same number of different tags, so we compare tags in order
         else:
             other_tags = [tag for _, tag in sorted(other.tags.items())]
             for i, tag in enumerate([tag for _, tag in sorted(self.tags.items())]):
                 if tag != other_tags[i]:
```

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration/data/sample.json` & `wwtp-configuration-0.3.0/wwtp_configuration/data/sample.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944866071428572%*

 * *Differences: {"'CogenToFacility'": "{'virtual_tags': OrderedDict([('ElectricityGeneration_RShift2', "*

 * *                      "OrderedDict([('tags', ['ElectricityGeneration']), ('unary_operations', "*

 * *                      "[['>>', '>>']])])), ('ElectricityGeneration_LShift1', OrderedDict([('tags', "*

 * *                      "['ElectricityGeneration']), ('unary_operations', '<<')])), "*

 * *                      "('ElectricityGenDelta', OrderedDict([('tags', ['ElectricityGeneration']), "*

 * *                      "('unary_operations', […]*

```diff
@@ -79,15 +79,40 @@
             "ElectricityGeneration": {
                 "contents": "Electricity",
                 "totalized": false,
                 "type": "Flow",
                 "units": "kWh"
             }
         },
-        "type": "Wire"
+        "type": "Wire",
+        "virtual_tags": {
+            "ElectricityGenDelta": {
+                "tags": [
+                    "ElectricityGeneration"
+                ],
+                "unary_operations": "delta"
+            },
+            "ElectricityGeneration_LShift1": {
+                "tags": [
+                    "ElectricityGeneration"
+                ],
+                "unary_operations": "<<"
+            },
+            "ElectricityGeneration_RShift2": {
+                "tags": [
+                    "ElectricityGeneration"
+                ],
+                "unary_operations": [
+                    [
+                        ">>",
+                        ">>"
+                    ]
+                ]
+            }
+        }
     },
     "Cogenerator": {
         "generation_capacity": {
             "avg": null,
             "max": null,
             "min": null,
             "units": "kW"
@@ -191,15 +216,14 @@
         "destination": "DesalPlant",
         "flowrate": {
             "avg": null,
             "max": null,
             "min": null,
             "units": "MGD"
         },
-        "pump_type": null,
         "source": "Ocean",
         "tags": {},
         "type": "Pipe"
     },
     "DesalOutlet": {
         "contents": "DrinkingWater",
         "destination": "WaterDistribution",
@@ -378,15 +402,26 @@
             "GasPurchases": {
                 "contents": "NaturalGas",
                 "totalized": false,
                 "type": "Flow",
                 "units": "SCFM"
             }
         },
-        "type": "Pipe"
+        "type": "Pipe",
+        "virtual_tags": {
+            "NoGasPurchases": {
+                "tags": [
+                    "GasPurchases"
+                ],
+                "type": "RunStatus",
+                "unary_operations": [
+                    "~"
+                ]
+            }
+        }
     },
     "GravityThickener": {
         "flowrate": {
             "avg": null,
             "max": null,
             "min": null,
             "units": "MGD"
@@ -671,14 +706,22 @@
     },
     "Ultrafiltration": {
         "contents": "TreatedSewage",
         "flowrate": {
             "avg": null,
             "max": null,
             "min": null,
+            "tags": {
+                "InletTemperature": {
+                    "contents": "SecondaryEffluent",
+                    "totalized": false,
+                    "type": "Temperature",
+                    "units": "C"
+                }
+            },
             "units": "MGD"
         },
         "num_units": null,
         "type": "Filtration",
         "volume (cubic meters)": null
     },
     "VirtualDemand": {
@@ -790,26 +833,27 @@
         "RecycledWaterFacility",
         "PurplePipeSystem",
         "DesalPlant",
         "Ocean"
     ],
     "virtual_tags": {
         "ElectricityProductionByGasVolume": {
-            "operations": [
+            "binary_operations": [
                 "/"
             ],
+            "parent_id": "Cogenerator",
             "tags": [
                 "ElectricityGeneration",
                 "GrossGasProduction"
             ],
             "type": "Efficiency"
         },
         "GrossGasProduction": {
+            "binary_operations": "+",
             "contents": "GasBlend",
-            "operations": "+",
             "tags": [
                 "CombinedDigesterGasFlow",
                 "GasPurchases"
             ]
         }
     }
 }
```

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration/node.py` & `wwtp-configuration-0.3.0/wwtp_configuration/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         """Adds a tag to the node
 
         Parameters
         ----------
         tag : Tag
             Tag object to add to the node
         """
+        if not tag.parent_id:
+            tag.parent_id = self.id
         self.tags[tag.id] = tag
 
     def remove_tag(self, tag_name):
         """Removes a tag from the node
 
         Parameters
         ----------
@@ -360,15 +362,15 @@
             object for which we want the parent object
 
         Returns
         -------
         Node or Connection
             parent object of the Tag
         """
-        if isinstance(tag, VirtualTag):
+        if isinstance(tag, VirtualTag) and tag.parent_id is None:
             if tag.id in self.tags.keys():
                 return self
             else:
                 children = self.get_all_connections(recurse=True) + self.get_all_nodes(
                     recurse=True
                 )
                 for child in children:
```

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration/parse_json.py` & `wwtp-configuration-0.3.0/wwtp_configuration/parse_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,15 +385,17 @@
                         "total" not in tag_source_unit_ids
                         and len(tag_source_unit_ids) > 1
                     ):
                         tag_obj = tags_by_contents[0]
                         tag_id = "_".join(
                             [node_id, tag_obj.contents.name, tag_obj.tag_type.name]
                         )
-                        v_tag = VirtualTag(tag_id, tags_by_contents, "+")
+                        v_tag = VirtualTag(
+                            tag_id, tags_by_contents, binary_operations="+"
+                        )
                         node_obj.add_tag(v_tag)
 
         v_tags = self.config[node_id].get("virtual_tags")
         if v_tags:
             for v_tag_id, v_tag_info in v_tags.items():
                 v_tag = self.parse_virtual_tag(v_tag_id, v_tag_info, node_obj)
                 node_obj.add_tag(v_tag)
@@ -541,15 +543,17 @@
                                     exit_point_id,
                                     connection_obj.get_dest_id(),
                                     entry_point_id,
                                     dest_unit_id,
                                     tag_obj.contents.name,
                                     tag.tag_type.name,
                                 )
-                                v_tag = VirtualTag(tag_id, tag_list, "+")
+                                v_tag = VirtualTag(
+                                    tag_id, tag_list, binary_operations="+"
+                                )
                                 connection_obj.add_tag(v_tag)
 
                         else:
                             tag_list = [
                                 connection_obj.tags[tag_obj.id]
                                 for tag_obj in tags_by_contents
                                 if tag_obj.contents == contents
@@ -559,15 +563,15 @@
                                 connection_obj.get_source_id(),
                                 exit_point_id,
                                 connection_obj.get_dest_id(),
                                 entry_point_id,
                                 tag_obj.contents.name,
                                 tag.tag_type.name,
                             )
-                            v_tag = VirtualTag(tag_id, tag_list, "+")
+                            v_tag = VirtualTag(tag_id, tag_list, binary_operations="+")
                             connection_obj.add_tag(v_tag)
                     if "total" not in tag_dest_unit_ids and len(tag_dest_unit_ids) > 1:
                         tag_obj = tags_by_contents[0]
                         # create a separate virtual total for each source unit.
                         # If none exist then just use total
                         if tag_source_unit_ids:
                             for id in tag_source_unit_ids:
@@ -583,15 +587,17 @@
                                     exit_point_id,
                                     source_unit_id,
                                     connection_obj.get_dest_id(),
                                     entry_point_id,
                                     tag_obj.contents.name,
                                     tag.tag_type.name,
                                 )
-                                v_tag = VirtualTag(tag_id, tag_list, "+")
+                                v_tag = VirtualTag(
+                                    tag_id, tag_list, binary_operations="+"
+                                )
                                 connection_obj.add_tag(v_tag)
                         else:
                             tag_list = [
                                 connection_obj.tags[tag_obj.id]
                                 for tag_obj in tags_by_contents
                                 if tag_obj.contents == contents
                             ]
@@ -600,15 +606,15 @@
                                 connection_obj.get_source_id(),
                                 exit_point_id,
                                 connection_obj.get_dest_id(),
                                 entry_point_id,
                                 tag_obj.contents.name,
                                 tag.tag_type.name,
                             )
-                            v_tag = VirtualTag(tag_id, tag_list, "+")
+                            v_tag = VirtualTag(tag_id, tag_list, binary_operations="+")
                             connection_obj.add_tag(v_tag)
 
         v_tags = self.config[connection_id].get("virtual_tags")
         if v_tags:
             for v_tag_id, v_tag_info in v_tags.items():
                 v_tag = self.parse_virtual_tag(v_tag_id, v_tag_info, connection_obj)
                 connection_obj.add_tag(v_tag)
@@ -667,15 +673,16 @@
         ----------
         tag_id : str
             name of the tag
 
         tag_info : dict
             dictionary of the form {
                 'tags': dict of Tag,
-                'operations': list of str,
+                'unary_operations': list of str,
+                'binary_operations': list of str,
                 'type': TagType,
                 'contents': str
             }
 
         obj : Node or Connection
             parent object that contains all constituent tags,
             which is used to gather the tag list for combining data correctly
@@ -702,15 +709,21 @@
         except KeyError:
             tag_type = None
         try:
             contents_type = utils.ContentsType[tag_info["contents"]]
         except KeyError:
             contents_type = None
         v_tag = VirtualTag(
-            tag_id, tag_list, tag_info["operations"], tag_type, contents_type
+            tag_id,
+            tag_list,
+            unary_operations=tag_info.get("unary_operations"),
+            binary_operations=tag_info.get("binary_operations"),
+            tag_type=tag_type,
+            contents=contents_type,
+            parent_id=tag_info.get("parent_id"),
         )
         return v_tag
 
     @staticmethod
     def parse_tag(tag_id, tag_info, obj):
         """Parse tag ID and dictionary of information into Tag object
 
@@ -890,15 +903,16 @@
         -------
         dict
             `tag_obj` in dictionary form
         """
         tag_dict = {}
         if isinstance(tag_obj, VirtualTag):
             tag_dict["tags"] = [tag.id for tag in tag_obj.tags]
-            tag_dict["operations"] = tag_obj.operations
+            tag_dict["unary_operations"] = tag_obj.unary_operations
+            tag_dict["binary_operations"] = tag_obj.binary_operations
         elif isinstance(tag_obj, Tag):
             tag_dict["units"] = "{!s}".format(tag_obj.units)
             tag_dict["source_unit_id"] = tag_obj.source_unit_id
             tag_dict["dest_unit_id"] = tag_obj.dest_unit_id
             tag_dict["totalized"] = tag_obj.totalized
         else:
             raise TypeError("'tag_obj' must be of type Tag or VirtualTag")
```

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration/units.py` & `wwtp-configuration-0.3.0/wwtp_configuration/units.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration/utils.py` & `wwtp-configuration-0.3.0/wwtp_configuration/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import warnings
+from pandas import Series
 from enum import Enum, auto
+from numpy import ndarray, nan
 from pint import UndefinedUnitError, DimensionalityError
 from .units import u
 
 
 def parse_quantity(value, units):
     """Convert a value and unit string to a Pint quantity
 
@@ -162,14 +164,39 @@
             or clean_units == "meters/s"
             or clean_units == "m/second"
             or clean_units == "meter/second"
             or clean_units == "meters/second"
         ):
             return u.m / u.s
         elif (
+            clean_units == "cubicmeters/day"
+            or clean_units == "cubicmeter/day"
+            or clean_units == "m**3/day"
+            or clean_units == "m^3/day"
+            or clean_units == "m3/day"
+            or clean_units == "meter3/day"
+            or clean_units == "meter**3/day"
+            or clean_units == "meter^3/day"
+            or clean_units == "meters3/day"
+            or clean_units == "meters**3/day"
+            or clean_units == "meters^3/day"
+            or clean_units == "cubicmeters/d"
+            or clean_units == "cubicmeter/d"
+            or clean_units == "m**3/d"
+            or clean_units == "m^3/d"
+            or clean_units == "m3/d"
+            or clean_units == "meter3/d"
+            or clean_units == "meter**3/d"
+            or clean_units == "meter^3/d"
+            or clean_units == "meters3/d"
+            or clean_units == "meters**3/d"
+            or clean_units == "meters^3/d"
+        ):
+            return u.m**3 / u.day
+        elif (
             clean_units == "psi"
             or clean_units == "poundspersquareinch"
             or clean_units == "poundpersquareinch"
             or clean_units == "poundspersquarein"
             or clean_units == "poundpersquarein"
             or clean_units == "poundspersqin"
             or clean_units == "poundpersqin"
@@ -534,29 +561,33 @@
         not hasattr(obj, "tag_type") or obj.tag_type != tag_type
     ):
         return False
 
     return True
 
 
-def operation_helper(operation, unit, prev_unit, totalized_mix=False):
+def binary_helper(operation, unit, prev_unit, totalized_mix=False):
     """Helper for parsing operations and checking units
 
     Parameters
     ----------
     operation : ["+", "-", "*", "/"]
         Function to apply when combining tags.
         Supported functions are "+", "-", "*", and "/".
 
     unit : Unit
         Units for the right side of the operation, represented as a Pint unit.
 
     prev_unit : Unit
         Units for the left side of the operation, represented as a Pint unit.
 
+    totalized_mix : bool
+        Skip unit checking when there is a mix of totalized and detotalized variables.
+        Default is False
+
     Raises
     ------
     ValueError
         When units are incompatible for addition or subtraction.
         When `operation` is unsupported.
 
     UserWarning
@@ -588,7 +619,97 @@
             prev_unit = prev_unit / unit
         else:
             prev_unit = prev_unit * unit
     else:
         raise ValueError("Unsupported operation " + operation)
 
     return prev_unit
+
+
+def unary_helper(data, un_op):
+    """Transform the given data according to the VirtualTag's unary operator
+
+    Parameters
+    ----------
+    data : list, array, or Series
+        a list, numpy array, or pandas Series of data to apply a unary operation to
+
+    un_op : ["noop", "delta", "<<", ">>", "~", "-"]
+        Supported operations are:
+            "noop" : null operator, useful when
+            skipping tags in a list of unary operations.
+
+            "delta" : calculate the difference between
+            the current timestep and previous timestep
+
+            "<<" : shift all data left one timestep,
+            so that the last time step will be NaN
+
+            ">>" : shift all data right one timestep,
+            so that the first time step will be NaN
+
+            "~" : Boolean not
+
+            "-" : unary negation
+
+        Note that "delta", "<<", and ">>" return a timeseries padded
+        with NaN so that it is the same length as input data
+
+    Returns
+    -------
+    list, array, or Series
+        numpy array of dataset trannsformed by unary operation
+    """
+    # allow for multiple unary operations to be performed sequentially
+    if isinstance(un_op, list):
+        result = data.copy()
+        for op in un_op:
+            result = unary_helper(result, op)
+    elif un_op == "noop":
+        result = data.copy()
+    elif un_op == "delta":
+        r_shift = unary_helper(data, ">>")
+        result = data - r_shift
+    elif un_op == "-":
+        if isinstance(data, list):
+            result = [not -x for x in data]
+        elif isinstance(data, (ndarray, Series)):
+            result = -data
+        else:
+            raise TypeError("Data must be either a list, array, or Series")
+    elif un_op == "~":
+        if isinstance(data, list):
+            result = result = [not bool(x) for x in data]
+        elif isinstance(data, (ndarray, Series)):
+            result = data == 0
+        else:
+            raise TypeError("Data must be either a list, array, or Series")
+    else:
+        if isinstance(data, list):
+            result = data.copy()
+            if un_op == "<<":
+                for i in range(len(data) - 1):
+                    result[i] = data[i + 1]
+                result[len(data) - 1] = float("nan")
+            elif un_op == ">>":
+                for i in range(1, len(data)):
+                    result[i] = data[i - 1]
+                result[0] = float("nan")
+        elif isinstance(data, ndarray):
+            result = data.copy().astype("float")
+            if un_op == "<<":
+                for i in range(len(data) - 1):
+                    result[i] = data[i + 1]
+                result[len(data) - 1] = nan
+            elif un_op == ">>":
+                for i in range(1, len(data)):
+                    result[i] = data[i - 1]
+                result[0] = nan
+        elif isinstance(data, Series):
+            if un_op == "<<":
+                result = data.shift(-1)
+            elif un_op == ">>":
+                result = data.shift(1)
+        else:
+            raise TypeError("Data must be either a list, array, or Series")
+
+    return result
```

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration/visualize.py` & `wwtp-configuration-0.3.0/wwtp_configuration/visualize.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration.egg-info/PKG-INFO` & `wwtp-configuration-0.3.0/wwtp_configuration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwtp-configuration
-Version: 0.2.3
+Version: 0.3.0
 Summary: Class hierarchy to represent a wastewater treatment plant's configuration.
 Home-page: https://github.com/we3lab/wwtp-configuration
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: wwtp-configuration
 Platform: UNKNOWN
```

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration.egg-info/SOURCES.txt` & `wwtp-configuration-0.3.0/wwtp_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.3/wwtp_configuration.egg-info/requires.txt` & `wwtp-configuration-0.3.0/wwtp_configuration.egg-info/requires.txt`

 * *Files identical despite different names*

