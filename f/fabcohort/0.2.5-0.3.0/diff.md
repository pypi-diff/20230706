# Comparing `tmp/fabcohort-0.2.5.tar.gz` & `tmp/fabcohort-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabcohort-0.2.5.tar", last modified: Wed Jul  5 13:22:50 2023, max compression
+gzip compressed data, was "fabcohort-0.3.0.tar", last modified: Thu Jul  6 10:25:11 2023, max compression
```

## Comparing `fabcohort-0.2.5.tar` & `fabcohort-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:22:50.043326 fabcohort-0.2.5/
--rw-r--r--   0 linliding   (501) staff       (20)     2569 2023-07-05 13:22:50.043167 fabcohort-0.2.5/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)     1878 2023-07-05 13:22:26.000000 fabcohort-0.2.5/README.md
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:22:50.042252 fabcohort-0.2.5/fab_cohort/
--rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.2.5/fab_cohort/__init__.py
--rw-r--r--   0 linliding   (501) staff       (20)     4953 2023-07-05 13:21:02.000000 fabcohort-0.2.5/fab_cohort/cohort.py
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-05 13:22:50.042972 fabcohort-0.2.5/fabcohort.egg-info/
--rw-r--r--   0 linliding   (501) staff       (20)     2569 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      226 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/SOURCES.txt
--rw-r--r--   0 linliding   (501) staff       (20)        1 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/dependency_links.txt
--rw-r--r--   0 linliding   (501) staff       (20)       13 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/requires.txt
--rw-r--r--   0 linliding   (501) staff       (20)       11 2023-07-05 13:22:50.000000 fabcohort-0.2.5/fabcohort.egg-info/top_level.txt
--rw-r--r--   0 linliding   (501) staff       (20)       38 2023-07-05 13:22:50.043379 fabcohort-0.2.5/setup.cfg
--rw-r--r--   0 linliding   (501) staff       (20)     1293 2023-07-05 13:22:38.000000 fabcohort-0.2.5/setup.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-06 10:25:11.178961 fabcohort-0.3.0/
+-rw-r--r--   0 linliding   (501) staff       (20)     2575 2023-07-06 10:25:11.178783 fabcohort-0.3.0/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)     1884 2023-07-05 13:37:24.000000 fabcohort-0.3.0/README.md
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-06 10:25:11.176688 fabcohort-0.3.0/fab_cohort/
+-rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.3.0/fab_cohort/__init__.py
+-rw-r--r--   0 linliding   (501) staff       (20)     3202 2023-07-06 10:21:55.000000 fabcohort-0.3.0/fab_cohort/cohort.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-07-06 10:25:11.178559 fabcohort-0.3.0/fabcohort.egg-info/
+-rw-r--r--   0 linliding   (501) staff       (20)     2575 2023-07-06 10:25:11.000000 fabcohort-0.3.0/fabcohort.egg-info/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)      226 2023-07-06 10:25:11.000000 fabcohort-0.3.0/fabcohort.egg-info/SOURCES.txt
+-rw-r--r--   0 linliding   (501) staff       (20)        1 2023-07-06 10:25:11.000000 fabcohort-0.3.0/fabcohort.egg-info/dependency_links.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       13 2023-07-06 10:25:11.000000 fabcohort-0.3.0/fabcohort.egg-info/requires.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       11 2023-07-06 10:25:11.000000 fabcohort-0.3.0/fabcohort.egg-info/top_level.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       38 2023-07-06 10:25:11.179017 fabcohort-0.3.0/setup.cfg
+-rw-r--r--   0 linliding   (501) staff       (20)     1293 2023-07-06 10:24:39.000000 fabcohort-0.3.0/setup.py
```

### Comparing `fabcohort-0.2.5/PKG-INFO` & `fabcohort-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.2.5
+Version: 0.3.0
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -47,15 +47,15 @@
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort method, e.g., MS for month start, WS for week start
+# Call the count_cohort method, e.g., MS for month start, W-MON for week start
 result = cohort.count_cohort(df, frequency)
 
 ```
 
 #### **FUNCTION2**:
 
 Cohort analysis by segments
@@ -71,15 +71,15 @@
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort_segments method, e.g., MS for month start, WS for week start
+# Call the count_cohort_segments method, e.g., MS for month start, W-MON for week start
 result = cohort.count_cohort_segments(df, frequency)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
```

### Comparing `fabcohort-0.2.5/README.md` & `fabcohort-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort method, e.g., MS for month start, WS for week start
+# Call the count_cohort method, e.g., MS for month start, W-MON for week start
 result = cohort.count_cohort(df, frequency)
 
 ```
 
 #### **FUNCTION2**:
 
 Cohort analysis by segments
@@ -51,15 +51,15 @@
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort_segments method, e.g., MS for month start, WS for week start
+# Call the count_cohort_segments method, e.g., MS for month start, W-MON for week start
 result = cohort.count_cohort_segments(df, frequency)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
```

### Comparing `fabcohort-0.2.5/fabcohort.egg-info/PKG-INFO` & `fabcohort-0.3.0/fabcohort.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.2.5
+Version: 0.3.0
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -47,15 +47,15 @@
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort method, e.g., MS for month start, WS for week start
+# Call the count_cohort method, e.g., MS for month start, W-MON for week start
 result = cohort.count_cohort(df, frequency)
 
 ```
 
 #### **FUNCTION2**:
 
 Cohort analysis by segments
@@ -71,15 +71,15 @@
 
 ```Python
 from fab_cohort import Cohort
 
 # Instantiate a Cohort object
 cohort = Cohort()
 
-# Call the count_cohort_segments method, e.g., MS for month start, WS for week start
+# Call the count_cohort_segments method, e.g., MS for month start, W-MON for week start
 result = cohort.count_cohort_segments(df, frequency)
 
 # (Optional) if you have multiple segments just parse it
 result[['segment1', 'segment2']] = result['segment'].str.split(',', expand=True)
 result.drop('segment', axis=1, inplace=True)
 
 ```
```

### Comparing `fabcohort-0.2.5/setup.py` & `fabcohort-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="fabcohort",
-    version="0.2.5",
+    version="0.3.0",
     description="for cohort analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/linliD/fabcohort/",
     author="Linli Ding",
     author_email="linli@joinbonnet.com",
     license="MIT",
```

