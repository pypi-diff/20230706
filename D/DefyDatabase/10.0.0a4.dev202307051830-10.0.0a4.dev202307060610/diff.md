# Comparing `tmp/DefyDatabase-10.0.0a4.dev202307051830.tar.gz` & `tmp/DefyDatabase-10.0.0a4.dev202307060610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307051830.tar", last modified: Wed Jul  5 10:28:54 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307060610.tar", last modified: Wed Jul  5 22:10:15 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a4.dev202307051830.tar` & `DefyDatabase-10.0.0a4.dev202307060610.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 10:28:54.272289 DefyDatabase-10.0.0a4.dev202307051830/
-drwxrwxrwx   0        0        0        0 2023-07-05 10:28:54.271292 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      567 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-07-05 10:28:54.272289 DefyDatabase-10.0.0a4.dev202307051830/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307051830/README.md
--rw-rw-rw-   0        0        0     2757 2023-07-05 10:28:28.000000 DefyDatabase-10.0.0a4.dev202307051830/defy.py
--rw-rw-rw-   0        0        0       42 2023-07-05 10:28:54.273223 DefyDatabase-10.0.0a4.dev202307051830/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202307051830/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 22:10:15.625861 DefyDatabase-10.0.0a4.dev202307060610/
+drwxrwxrwx   0        0        0        0 2023-07-05 22:10:15.624598 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-07-05 22:10:15.625861 DefyDatabase-10.0.0a4.dev202307060610/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307060610/README.md
+-rw-rw-rw-   0        0        0     2882 2023-07-05 22:09:56.000000 DefyDatabase-10.0.0a4.dev202307060610/defy.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 22:10:15.625861 DefyDatabase-10.0.0a4.dev202307060610/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202307060610/setup.py
```

### Comparing `DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307051830
+Version: 10.0.0a4.dev202307060610
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202307051830/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307060610/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307051830
+Version: 10.0.0a4.dev202307060610
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202307051830/defy.py` & `DefyDatabase-10.0.0a4.dev202307060610/defy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #Rules are meant to break by proudest ones.
 '''
 这是亮天计划的数据库官方API。
 '''
 import sqlite3,sys,os,datetime,io
 
 tor='DefyDatabase'
-version='10.0.0a4.dev202307051830'
+version='10.0.0a4.dev202307060610'
 
 
 
 commands={
     'COUNT_MAIN':'SELECT COUNT(*) FROM LIGHTSKY',
     'CHECK_BIND':'SELECT UID,BIND FROM BIND WHERE UID = "{}"',
     'QUERYUID':'SELECT UID, GRADE, JOB ,ABOUT FROM LIGHTSKY WHERE UID = "{}"',
@@ -85,20 +85,25 @@
         self.__cur=self.__con.cursor()
         a=self.__query(commands['COUNT_MAIN'])
         b=self.__query(commands['COUNT_BIND'])
         if a==0 or b==0:
             for i in tablemaker:
                 self.__atest(i)
 
-    def query(uid):
+    def query(self,uid):
         pass
 
-    def atest(*datas):
+    def atest(self,*datas):
         for i in datas:
             if len(i)==2:
                 pass
             elif len(i)==3:
                 pass
 
+    def close(self):
+        self.__cur.close()
+        self.__con.close()
+        del self.__cur,self.__con
+
 def open(file):
     return __DefyProject(file)
```

### Comparing `DefyDatabase-10.0.0a4.dev202307051830/setup.py` & `DefyDatabase-10.0.0a4.dev202307060610/setup.py`

 * *Files identical despite different names*

