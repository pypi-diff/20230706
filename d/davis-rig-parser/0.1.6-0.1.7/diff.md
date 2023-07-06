# Comparing `tmp/davis_rig_parser-0.1.6.tar.gz` & `tmp/davis_rig_parser-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davis_rig_parser-0.1.6.tar", last modified: Thu Jul  6 14:40:22 2023, max compression
+gzip compressed data, was "davis_rig_parser-0.1.7.tar", last modified: Thu Jul  6 15:44:25 2023, max compression
```

## Comparing `davis_rig_parser-0.1.6.tar` & `davis_rig_parser-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5451 2023-07-03 19:46:06.000000 davis_rig_parser-0.1.6/README.md
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/davis_rig_parser/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.6/davis_rig_parser/__init__.py
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18475 2023-07-06 14:33:58.000000 davis_rig_parser-0.1.6/davis_rig_parser/davis_rig_parser.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/requires.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/top_level.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/setup.cfg
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-06 14:37:03.000000 davis_rig_parser-0.1.6/setup.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/tests/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.1.6/tests/test.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.1.7/README.md
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.540785 davis_rig_parser-0.1.7/davis_rig_parser/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.7/davis_rig_parser/__init__.py
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18459 2023-07-06 15:43:14.000000 davis_rig_parser-0.1.7/davis_rig_parser/davis_rig_parser.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/requires.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-06 15:44:25.000000 davis_rig_parser-0.1.7/davis_rig_parser.egg-info/top_level.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/setup.cfg
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-06 15:43:28.000000 davis_rig_parser-0.1.7/setup.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 15:44:25.544786 davis_rig_parser-0.1.7/tests/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.1.7/tests/test.py
```

### Comparing `davis_rig_parser-0.1.6/README.md` & `davis_rig_parser-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 # Davis Rig Parser
 
-This module is for preprocessing and parsing brief access task data from the Med Associates gustometer, also known as the "Davis Rig." It ajusts the raw inputs for  some artifacts created by the Davis Rig, including false licks. 
+This module is for preprocessing and parsing brief access task data from the Med Associates gustometer, also known as the "Davis Rig." It ajusts the raw inputs for  some artifacts created by the Davis Rig, including false licks (see Changing Parameters). 
 
 ## Installation
 
 The `davis_rig_parser` module can be installed using pip. It's hosted on PyPI, so you can install it directly from there.
 
 First, you need to make sure you have Python installed on your machine. `davis_rig_parser` was written in Python 3.7.6, but it should work with many other versions. However, if you encounter errors, you can check your Python version by running the following command in your command prompt:
```

### Comparing `davis_rig_parser-0.1.6/davis_rig_parser/davis_rig_parser.py` & `davis_rig_parser-0.1.7/davis_rig_parser/davis_rig_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,18 +224,16 @@
         for case in range(detail_row.shape[1]):
             if detail_df.Notes[detail_row[:,case][0]].lower() in \
                 Detail_Dict['FileName'][Detail_Dict['FileName'].rfind('_')+1:].lower()\
                 and detail_df.Animal[detail_row[:,case][0]] in Detail_Dict['Animal']:
                 
                     
                 #Add details to dataframe    
-                df.insert(loc=1, column='Notes', \
-                    value=detail_df.Notes[detail_row[:,case][0]].lower())
-                df.insert(loc=2, column='Condition', \
-                    value=detail_df.Condition[detail_row[:,case][0]].lower())
+				df.insert(loc=1, column='Notes', value=detail_df['Notes'].apply(lambda x: x.lower() if not pd.isnull(x) else x))
+				df.insert(loc=2, column='Condition', value=detail_df['Condition'].apply(lambda x: x.lower() if not pd.isnull(x) else x))
                 break
                 
     if len(file_check) == 0:
         #Add blank columns
         df.insert(loc=1, column='Notes', value='')
         df.insert(loc=2, column='Condition', value='')
```

