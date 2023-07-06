# Comparing `tmp/EduStatTests-0.1.3.tar.gz` & `tmp/EduStatTests-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EduStatTests-0.1.3.tar", last modified: Tue Jul  4 20:22:01 2023, max compression
+gzip compressed data, was "EduStatTests-0.1.4.tar", last modified: Thu Jul  6 18:50:21 2023, max compression
```

## Comparing `EduStatTests-0.1.3.tar` & `EduStatTests-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:22:01.206992 EduStatTests-0.1.3/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-02 11:36:16.000000 EduStatTests-0.1.3/LICENSE
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:22:01.202992 EduStatTests-0.1.3/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       67 2023-07-03 20:02:42.000000 EduStatTests-0.1.3/README.md
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-04 20:21:47.000000 EduStatTests-0.1.3/pyproject.toml
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-04 20:22:01.206992 EduStatTests-0.1.3/setup.cfg
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:22:01.202992 EduStatTests-0.1.3/src/
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-04 20:22:01.202992 EduStatTests-0.1.3/src/EduStatTests.egg-info/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-04 20:22:01.000000 EduStatTests-0.1.3/src/EduStatTests.egg-info/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      228 2023-07-04 20:22:01.000000 EduStatTests-0.1.3/src/EduStatTests.egg-info/SOURCES.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-04 20:22:01.000000 EduStatTests-0.1.3/src/EduStatTests.egg-info/dependency_links.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       22 2023-07-04 20:22:01.000000 EduStatTests-0.1.3/src/EduStatTests.egg-info/top_level.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     2997 2023-07-04 20:21:18.000000 EduStatTests-0.1.3/src/EduStatTests.py
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-02 11:47:24.000000 EduStatTests-0.1.3/src/__init__.py
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-06 18:50:21.484356 EduStatTests-0.1.4/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-06 18:41:57.000000 EduStatTests-0.1.4/LICENSE
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-06 18:50:21.484356 EduStatTests-0.1.4/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       67 2023-07-06 18:41:57.000000 EduStatTests-0.1.4/README.md
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-06 18:46:56.000000 EduStatTests-0.1.4/pyproject.toml
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-06 18:50:21.484356 EduStatTests-0.1.4/setup.cfg
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-06 18:50:21.484356 EduStatTests-0.1.4/src/
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-06 18:50:21.484356 EduStatTests-0.1.4/src/EduStatTests.egg-info/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      539 2023-07-06 18:50:21.000000 EduStatTests-0.1.4/src/EduStatTests.egg-info/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      228 2023-07-06 18:50:21.000000 EduStatTests-0.1.4/src/EduStatTests.egg-info/SOURCES.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-06 18:50:21.000000 EduStatTests-0.1.4/src/EduStatTests.egg-info/dependency_links.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       22 2023-07-06 18:50:21.000000 EduStatTests-0.1.4/src/EduStatTests.egg-info/top_level.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     2682 2023-07-06 18:42:44.000000 EduStatTests-0.1.4/src/EduStatTests.py
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-06 18:41:57.000000 EduStatTests-0.1.4/src/__init__.py
```

### Comparing `EduStatTests-0.1.3/LICENSE` & `EduStatTests-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EduStatTests-0.1.3/PKG-INFO` & `EduStatTests-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `EduStatTests-0.1.3/pyproject.toml` & `EduStatTests-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy; python_version>='3.12'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EduStatTests"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Hakan Güldal", email="hguldal@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `EduStatTests-0.1.3/src/EduStatTests.egg-info/PKG-INFO` & `EduStatTests-0.1.4/src/EduStatTests.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `EduStatTests-0.1.3/src/EduStatTests.py` & `EduStatTests-0.1.4/src/EduStatTests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,105 @@
 import pandas as pd
 import numpy as np
 from scipy.stats import *
 
-class Analysis:
+def LoadFromCSV(CSVPath):
+  return pd.read_csv(CSVPath)
 
-  def __init__(self):
-    self.data=None
+def LoadFromDict(dictData):
+  return pd.DataFrame(dictData)
 
-  def LoadFromCSV(self,CSVPath):
-    self.data = pd.read_csv(CSVPath)
-  
-  def LoadFromDict(self,dictData):
-    self.data = pd.DataFrame(dictData)
-
-  def LoadFromExcel(self,ExcelPath):
-    self.data = pd.read_csv(ExcelPath)
-
-  """ Independent T-Test
-  Parameters (Input):
-  ================================================== 
-    self:       Instance of the EduStatTests class
-                
+def LoadFromExcel(ExcelPath):
+    return pd.read_csv(ExcelPath)
 
-    variable1*: string                
-                Independent variable (X) 
+""" Independent T-Test
+Parameters (Input):
+==================================================
+df        : Pandas DataFrame 2xN (Two Columns x N Row)
+
+variable1*: string
+                Independent variable (X)
                 Name of DataFrame column object
 
-    variable2*: string
+variable2*: string
                 Dependent variable (Y)
                 Name of DataFrame column object
-    
-    *: Required Parameter
 
-  Return (Output):
-  ===================================================
-  Type: dictionary
-  Description: T-Test Stats
-  """
-  def IndTTest(self,variable1,variable2):
-    
-    if self.data is None:
-      raise Exception("No data loaded")
-
-    if len(self.data[variable1].value_counts().index)>2:
-      raise Exception("The number of groups cannot be greater than 2")
-    
-    # Create a dictionary object for the store data and etc.
-    dataCollection=dict()
-    
-    # Extract the groups from DataFrame and put into the dataCollection dictionary object
-    for idx in self.data[variable1].value_counts().index:
-      dataCollection[idx]={"data":self.data.query(variable1 + "==" + str(idx))[variable2]}
-
-    # Extract the raw data from dictionary object to pass scipy.stats functions
-    rawData=list()
-    for item in dataCollection:
-      rawData.append(dataCollection[item]["data"])
-
-    data1,data2=rawData[0],rawData[1]
-    
-    # Calculate Indepentend T-Test
-    result1 = ttest_ind(data1, data2)
-    
-    # Calculate Levent Test
-    result2=levene(data1, data2,center='mean')
-
-    # Calculate Indepentend Welch Test
-    result3= ttest_ind(data1, data2,equal_var = False)
-    
-    # Calculate Degree of Freedom score
-    dofF=len(data1)+len(data2)-2
-
-    # Calculate group descriptive statistics
-    groupStats=list()
-    for item in dataCollection:
-      group=dict()
-      group[item]={"N":dataCollection[item]["data"].count(),
+*: Required Parameter
+
+Return (Output):
+===================================================
+Type: dictionary
+Description: T-Test Stats
+"""
+def IndTTest(df,variable1,variable2):
+
+  if df is None:
+    raise Exception("No data loaded")
+
+  if len(df[variable1].value_counts().index)>2:
+    raise Exception("The number of groups cannot be greater than 2")
+
+  # Create a dictionary object for the store data and etc.
+  dataCollection=dict()
+
+  # Extract the groups from DataFrame and put into the dataCollection dictionary object
+  for idx in df[variable1].value_counts().index:
+    dataCollection[idx]={"data":df.query(variable1 + "==" + str(idx))[variable2]}
+
+  # Extract the raw data from dictionary object to pass scipy.stats functions
+  rawData=list()
+  for item in dataCollection:
+    rawData.append(dataCollection[item]["data"])
+
+  data1,data2=rawData[0],rawData[1]
+
+  # Calculate Indepentend T-Test
+  result1 = ttest_ind(data1, data2)
+
+  # Calculate Levent Test
+  result2=levene(data1, data2,center='mean')
+
+  # Calculate Indepentend Welch Test
+  result3= ttest_ind(data1, data2,equal_var = False)
+
+  # Calculate Degree of Freedom score
+  dofF=len(data1)+len(data2)-2
+
+  # Calculate group descriptive statistics
+  groupStats=list()
+  for item in dataCollection:
+    group=dict()
+    group[item]={"N":dataCollection[item]["data"].count(),
                    "Mean":dataCollection[item]["data"].mean(),
                    "StdDev":dataCollection[item]["data"].std()
-      }
-      groupStats.append(group)
-    
-    # Create  dictionary object(dictReturn) to return stats 
-    dictReturn={
+    }
+    groupStats.append(group)
+
+  # Create  dictionary object(dictReturn) to return stats
+  dictReturn={
         # Groups statistics
         "groupStats":groupStats,
-        
+
         # T-Test results
         "TTest":{
             "t":result1[0],
             "df":dofF,
             "sigTwoTailed":result1[1]
         },
 
         # Levene test results
         "LeveneTest":
         {
          "F":result2[0],
          "sigTwoTailed":result2[1]
-            
+
         },
 
         # Welch test results
         "WelchTest":{
             "t":result3[0],
             "sigTwoTailed":result3[1]
         }
-    }
-    
-    return dictReturn
+  }
+
+  return dictReturn
```

