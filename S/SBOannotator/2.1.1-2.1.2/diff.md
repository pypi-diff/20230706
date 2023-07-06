# Comparing `tmp/SBOannotator-2.1.1.tar.gz` & `tmp/SBOannotator-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SBOannotator-2.1.1.tar", last modified: Wed Apr 19 10:45:45 2023, max compression
+gzip compressed data, was "dist/SBOannotator-2.1.2.tar", last modified: Thu Jul  6 11:24:56 2023, max compression
```

## Comparing `SBOannotator-2.1.1.tar` & `SBOannotator-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 10:45:45.865418 SBOannotator-2.1.1/
--rw-r--r--   0 leonidou   (501) staff       (20)    35149 2023-01-23 22:12:54.000000 SBOannotator-2.1.1/LICENSE
--rw-r--r--   0 leonidou   (501) staff       (20)     4148 2023-04-19 10:45:45.865050 SBOannotator-2.1.1/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)     3376 2023-04-19 08:25:50.000000 SBOannotator-2.1.1/README.md
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 10:45:45.864349 SBOannotator-2.1.1/SBOannotator.egg-info/
--rw-r--r--   0 leonidou   (501) staff       (20)     4148 2023-04-19 10:45:45.000000 SBOannotator-2.1.1/SBOannotator.egg-info/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)      244 2023-04-19 10:45:45.000000 SBOannotator-2.1.1/SBOannotator.egg-info/SOURCES.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 10:45:45.000000 SBOannotator-2.1.1/SBOannotator.egg-info/dependency_links.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       52 2023-04-19 10:45:45.000000 SBOannotator-2.1.1/SBOannotator.egg-info/requires.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       18 2023-04-19 10:45:45.000000 SBOannotator-2.1.1/SBOannotator.egg-info/top_level.txt
--rw-r--r--   0 leonidou   (501) staff       (20)    20309 2023-02-20 21:46:40.000000 SBOannotator-2.1.1/SBOannotator.py
--rw-r--r--   0 leonidou   (501) staff       (20)     1192 2023-02-20 21:45:02.000000 SBOannotator-2.1.1/main.py
--rw-r--r--   0 leonidou   (501) staff       (20)      104 2023-01-30 09:25:48.000000 SBOannotator-2.1.1/pyproject.toml
--rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 10:45:45.865532 SBOannotator-2.1.1/setup.cfg
--rw-r--r--   0 leonidou   (501) staff       (20)     1245 2023-04-19 10:45:14.000000 SBOannotator-2.1.1/setup.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-07-06 11:24:56.923191 SBOannotator-2.1.2/
+-rw-r--r--   0 leonidou   (501) staff       (20)    35149 2023-01-23 22:12:54.000000 SBOannotator-2.1.2/LICENSE
+-rw-r--r--   0 leonidou   (501) staff       (20)     4147 2023-07-06 11:24:56.922770 SBOannotator-2.1.2/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)     3375 2023-05-02 20:20:24.000000 SBOannotator-2.1.2/README.md
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-07-06 11:24:56.922273 SBOannotator-2.1.2/SBOannotator.egg-info/
+-rw-r--r--   0 leonidou   (501) staff       (20)     4147 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)      259 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/SOURCES.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/dependency_links.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       52 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/requires.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       18 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/top_level.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)    21544 2023-05-23 14:06:51.000000 SBOannotator-2.1.2/SBOannotator.py
+-rw-r--r--   0 leonidou   (501) staff       (20)    13264 2023-01-23 22:12:54.000000 SBOannotator-2.1.2/create_dbs.sql
+-rw-r--r--   0 leonidou   (501) staff       (20)     1261 2023-05-08 09:07:21.000000 SBOannotator-2.1.2/main.py
+-rw-r--r--   0 leonidou   (501) staff       (20)      104 2023-01-30 09:25:48.000000 SBOannotator-2.1.2/pyproject.toml
+-rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-07-06 11:24:56.923323 SBOannotator-2.1.2/setup.cfg
+-rw-r--r--   0 leonidou   (501) staff       (20)     1315 2023-07-06 11:20:45.000000 SBOannotator-2.1.2/setup.py
```

### Comparing `SBOannotator-2.1.1/LICENSE` & `SBOannotator-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SBOannotator-2.1.1/PKG-INFO` & `SBOannotator-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBOannotator
-Version: 2.1.1
+Version: 2.1.2
 Summary: SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms
 Home-page: https://github.com/draeger-lab/SBOannotator
 Author: Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: SBOannotator,SBO Terms,automated tool
 Platform: UNKNOWN
@@ -65,15 +65,15 @@
 * json
 * time
 
 ### Input data
 + `doc`: an SBML document
 + `model_libsbml`: SBML model of interest
 + `modelType`: type of modelling framework (see below)
-+ `model_annotated`: True, if model already includes annotations with EC numbers
++ `modelAnnotated`: True, if model already includes annotations with EC numbers
 + `database_name`: name of imported database, without extension
 + `new_filename`: file name for output model
 
 Types of modelling framework accepted:
 - constraint-based
 - logical
 - continuous
```

### Comparing `SBOannotator-2.1.1/README.md` & `SBOannotator-2.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 * json
 * time
 
 ### Input data
 + `doc`: an SBML document
 + `model_libsbml`: SBML model of interest
 + `modelType`: type of modelling framework (see below)
-+ `model_annotated`: True, if model already includes annotations with EC numbers
++ `modelAnnotated`: True, if model already includes annotations with EC numbers
 + `database_name`: name of imported database, without extension
 + `new_filename`: file name for output model
 
 Types of modelling framework accepted:
 - constraint-based
 - logical
 - continuous
```

### Comparing `SBOannotator-2.1.1/SBOannotator.egg-info/PKG-INFO` & `SBOannotator-2.1.2/SBOannotator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBOannotator
-Version: 2.1.1
+Version: 2.1.2
 Summary: SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms
 Home-page: https://github.com/draeger-lab/SBOannotator
 Author: Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: SBOannotator,SBO Terms,automated tool
 Platform: UNKNOWN
@@ -65,15 +65,15 @@
 * json
 * time
 
 ### Input data
 + `doc`: an SBML document
 + `model_libsbml`: SBML model of interest
 + `modelType`: type of modelling framework (see below)
-+ `model_annotated`: True, if model already includes annotations with EC numbers
++ `modelAnnotated`: True, if model already includes annotations with EC numbers
 + `database_name`: name of imported database, without extension
 + `new_filename`: file name for output model
 
 Types of modelling framework accepted:
 - constraint-based
 - logical
 - continuous
```

### Comparing `SBOannotator-2.1.1/SBOannotator.py` & `SBOannotator-2.1.2/SBOannotator.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import sqlite3
 from libsbml import writeSBMLToFile
 from collections import Counter
 import requests
 import json
 
 # define globals
-DEMAND_IDS = ['_DM_', '_DEMAND_', '_demand_']
-SINK_IDS = ['_SK_', '_SINK_', '_sink_']
-EXCHANGE_IDS = ['_EX_', '_EXCHANGE_', '_exchange_']
-BIOMASS_IDS = ['BIOMASS', 'biomass', 'growth', 'GROWTH']
+DEMAND_IDS = ['_DM_', '_DEMAND_', '_demand_','Demand_']
+SINK_IDS = ['_SK_', '_SINK_', '_sink_', 'Sink_']
+EXCHANGE_IDS = ['_EX_', '_EXCHANGE_', '_exchange_', 'Exchange_']
+BIOMASS_IDS = ['BIOMASS', 'biomass', 'growth', 'GROWTH', 'Growth']
+RXN_BOUND_PARAMETERS = ["cobra_default_lb", "cobra_default_ub", "cobra_0_bound", "minus_inf", "plus_inf"]
 
 
 def getCompartmentlessSpeciesId(speciesReference):
     speciesId = speciesReference.getSpecies()
     species = speciesReference.getModel().getSpecies(speciesId)
     compartment = species.getCompartment()
     wasteStringLen = len(compartment) + 1
@@ -172,17 +173,17 @@
             react.setSBOTerm('SBO:0000376')
         # Lyases
         elif '4' in set(lst):
             react.setSBOTerm('SBO:0000211')
         # Isomerases
         elif '5' in set(lst):
             react.setSBOTerm('SBO:0000377')
-        # Ligases, proper SBO is missing from graph --> use one for modification of covalent bonds
+        # Ligases
         elif '6' in set(lst):
-            react.setSBOTerm('SBO:0000182')
+            react.setSBOTerm('SBO:0000695')
         # Translocases
         elif '7' in set(lst):
             react.setSBOTerm('SBO:0000185')
         # Metabolic reactions
         else:
             react.setSBOTerm('SBO:0000176')
 
@@ -210,14 +211,17 @@
                 ECNums.append(link['id'])
 
             multipleECs(react, ECNums)
 
         except:
             react.setSBOTerm('SBO:0000176')
 
+    # return annotated model
+    return model
+
 
 def splitTransportBiochem(react):
     """" Classify between transport reactions and biochemical reactions """
     if len(getCompartmentList(react)) > 1 and not soleProtonTransported(react):
         react.setSBOTerm('SBO:0000655')
     else:
         react.setSBOTerm('SBO:0000176')
@@ -507,55 +511,83 @@
 
 
 def addSBOforParameters(model):
     for param in model.getListOfParameters():
         # reaction bounds
         if 'R_' in param.getId():
             param.setSBOTerm('SBO:0000625')
-        # default set bounds
-        else:
+        # default values for bounds
+        elif param.getId() in RXN_BOUND_PARAMETERS:
             param.setSBOTerm('SBO:0000626')
+        # length
+        elif 'length' in param.getId() or 'Length' in param.getId():
+            param.setSBOTerm('SBO:0000466')
+        # area
+        elif 'area' in param.getId() or 'Area' in param.getId():
+            param.setSBOTerm('SBO:0000467')
+        # volume
+        elif 'volume' in param.getId() or 'Volume' in param.getId():
+            param.setSBOTerm('SBO:0000468')
+        # any parameter
+        else:
+            param.setSBOTerm('SBO: 0000545')
 
 
 def addSBOforCompartments(model):
     for cmp in model.getListOfCompartments():
         cmp.setSBOTerm('SBO:0000290')
 
 
+def addSBOforRateLaw(model):
+    for r in model.reactions:
+        if r.getKineticLaw():
+            r.getKineticLaw().setSBOTerm('SBO:0000001')
+
+
+def addSBOforEvents(model):
+    if model.getListOfEvents() is not None:
+        for event in model.getListOfEvents():
+            event.setSBOTerm('SBO:0000231')
+            if event.getTrigger() is not None:
+                event.getTrigger().setSBOTerm('SBO:0000171')
+            if event.getDelay() is not None:
+                event.getDelay().setSBOTerm('SBO:0000225')
+
+
 def write_to_file(model, new_filename):
     new_document = model.getSBMLDocument()
     writeSBMLToFile(new_document, new_filename)
 
 
-def sbo_annotator(doc, model_libsbml, modelType, model_annotated, database_name, new_filename):
+def sbo_annotator(doc, model_libsbml, modelType, modelAnnotated, database_name, new_filename):
     """
     Main function to run SBOannotator
 
     Inputs:
         doc: SBML document
         model_libsbml (libsbml-model): input model (unannotated)
         modelType (str): type of modelling framework
-        model_annotated (boolean): True, if model already includes annotations with EC numbers
+        modelAnnotated (boolean): True, if model already includes annotations with EC numbers
         database_name (str): name of imported database, without extension
         new_filename (str): file name for output model
     Output:
         Annotated libsbml model
     """
 
     # connect to database
     con = sqlite3.connect(database_name)
     cur = con.cursor()
 
     with open(database_name + '.sql') as schema:
         cur.executescript(schema.read())
 
     # model is already annotated?
-    if not model_annotated:
+    if not modelAnnotated:
         print('Model is not annotated. Use API call ... ')
-        callForECAnnot(model_libsbml)
+        model_libsbml = callForECAnnot(model_libsbml)
 
     for reaction in model_libsbml.reactions:
         if not addSBOfromDB(reaction, cur):
             # print(reaction.getId())
             reaction.unsetSBOTerm()
 
             # needs to be checked first
@@ -594,14 +626,18 @@
 
     addSBOforGroups(model_libsbml)
 
     addSBOforParameters(model_libsbml)
 
     addSBOforCompartments(model_libsbml)
 
+    addSBOforRateLaw(model_libsbml)
+
+    addSBOforEvents(model_libsbml)
+
     write_to_file(model_libsbml, new_filename)
     print(f'\nModel with SBO Annotations written to {new_filename} ...')
 
     # close database connection
     cur.close()
     con.close()
```

### Comparing `SBOannotator-2.1.1/main.py` & `SBOannotator-2.1.2/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from SBOannotator import *
 from libsbml import *
 import time
 
 start = time.time()
 
-doc = readSBML('models/BiGG_Models/RECON1.xml')
+#doc = readSBML('models/BiGG_Models/RECON1.xml')
+doc = readSBML('/Users/leonidou/Downloads/BIOMD0000000497_url.xml')
 model = doc.getModel()
 
 print('-----------------------------')
 print('SBO before: ')
 print('-----------------------------')
 print(f'Reactions: {printCounts(model)[0]}')
 print(f'\nMetabolites: {printCounts(model)[1]}')
```

### Comparing `SBOannotator-2.1.1/setup.py` & `SBOannotator-2.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SBOannotator',
-    version='2.1.1',
+    version='2.1.2',
     description='SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/draeger-lab/SBOannotator',
     author='Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger',
     author_email='nantia.leonidou@uni-tuebingen.de',
     license=' GPL-3.0',
@@ -17,17 +17,19 @@
     install_requires=['python-libsbml',
                       'python-collection',
                       'requests',
                       'pypi-json'],
     #packages=find_packages(include=['models']),
     py_modules=['SBOannotator', 'main'],
     include_package_data=True,
+    package_data={
+        'create_dbs.sql': ['SBOannotator/'],
+    },
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Version Control :: Git",
         "Operating System :: MacOS",
         "Operating System :: Unix"
-
     ],
 )
```

