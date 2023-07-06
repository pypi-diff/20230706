# Comparing `tmp/DefyDatabase-10.0.0a4.dev202307060610.tar.gz` & `tmp/DefyDatabase-10.0.0a4.dev202307061815.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307060610.tar", last modified: Wed Jul  5 22:10:15 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307061815.tar", last modified: Thu Jul  6 10:12:44 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a4.dev202307060610.tar` & `DefyDatabase-10.0.0a4.dev202307061815.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 22:10:15.625861 DefyDatabase-10.0.0a4.dev202307060610/
-drwxrwxrwx   0        0        0        0 2023-07-05 22:10:15.624598 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      567 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-05 22:10:15.000000 DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-07-05 22:10:15.625861 DefyDatabase-10.0.0a4.dev202307060610/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307060610/README.md
--rw-rw-rw-   0        0        0     2882 2023-07-05 22:09:56.000000 DefyDatabase-10.0.0a4.dev202307060610/defy.py
--rw-rw-rw-   0        0        0       42 2023-07-05 22:10:15.625861 DefyDatabase-10.0.0a4.dev202307060610/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202307060610/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:12:44.797074 DefyDatabase-10.0.0a4.dev202307061815/
+drwxrwxrwx   0        0        0        0 2023-07-06 10:12:44.791025 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-07-06 10:12:44.796040 DefyDatabase-10.0.0a4.dev202307061815/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307061815/README.md
+-rw-rw-rw-   0        0        0     2578 2023-07-06 10:12:01.000000 DefyDatabase-10.0.0a4.dev202307061815/defy.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 10:12:44.797074 DefyDatabase-10.0.0a4.dev202307061815/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202307061815/setup.py
```

### Comparing `DefyDatabase-10.0.0a4.dev202307060610/DefyDatabase.egg-info/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307060610
+Version: 10.0.0a4.dev202307061815
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202307060610/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307061815/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307060610
+Version: 10.0.0a4.dev202307061815
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202307060610/defy.py` & `DefyDatabase-10.0.0a4.dev202307061815/defy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,49 @@
 #Rules are meant to break by proudest ones.
 '''
 这是亮天计划的数据库官方API。
 '''
 import sqlite3,sys,os,datetime,io
 
 tor='DefyDatabase'
-version='10.0.0a4.dev202307060610'
+version='10.0.0a4.dev202307061815'
 
 
 
 commands={
-    'COUNT_MAIN':'SELECT COUNT(*) FROM LIGHTSKY',
-    'CHECK_BIND':'SELECT UID,BIND FROM BIND WHERE UID = "{}"',
-    'QUERYUID':'SELECT UID, GRADE, JOB ,ABOUT FROM LIGHTSKY WHERE UID = "{}"',
-    'QUERYROW':'SELECT UID, GRADE, JOB ,ABOUT from LIGHTSKY WHERE rowid={}',
-    'COUNT_BIND':'SELECT COUNT(*) FROM BIND',
-    'ATEST_MAIN_2':'UPDATE LIGHTSKY SET GRADE=?,JOB=?,ABOUT=? WHERE UID=?',
-    'ATEST_MAIN_1':'INSERT INTO LIGHTSKY (UID,GRADE,JOB,ABOUT) VALUES (?,?,?,?)',
-    'ATEST_BIND_2':'UPDATE BIND SET BIND=? WHERE UID=?',
-    'ATEST_BIND_1':'INSERT INTO BIND (UID,BIND) VALUES (?,?)',
-    'DEL_MAIN':'DELETE FROM LIGHTSKY WHERE UID=?',
-    'DEL_BIND':'DELETE FROM BIND WHERE UID=?',
+    'COUNT_MAIN':'SELECT COUNT(*) FROM LIGHTSKY1',
+    'CHECK_BIND':'SELECT UID,BIND FROM BIND1 WHERE UID = "{}"',
+    'QUERYUID':'SELECT UID, GRADE, JOB FROM LIGHTSKY1 WHERE UID = "{}"',
+    'QUERYROW':'SELECT UID, GRADE, JOB FROM LIGHTSKY1 WHERE rowid={}',
+    'COUNT_BIND':'SELECT COUNT(*) FROM BIND1',
+    'ATEST_MAIN_1':'INSERT INTO LIGHTSKY1 (UID,GRADE,JOB) VALUES (?,?,?)',
+    'ATEST_MAIN_2':'UPDATE LIGHTSKY1 SET GRADE=?,JOB=? WHERE UID=?',
+    'ATEST_BIND_1':'INSERT INTO BIND1 (UID,BIND) VALUES (?,?)',
+    'ATEST_BIND_2':'UPDATE BIND1 SET BIND=? WHERE UID=?',
+    'DEL_MAIN':'DELETE FROM LIGHTSKY1 WHERE UID=?',
+    'DEL_BIND':'DELETE FROM BIND1 WHERE UID=?',
     'CLEAN':'VACUUM'}
 
 tablemaker=[
     """CREATE TABLE "ACTION" (
 	"ABOUT"	TEXT
 )""",
-    """CREATE TABLE "BIND" (
+    """CREATE TABLE "BIND1" (
 	"UID"	TEXT NOT NULL,
 	"BIND"	TEXT NOT NULL,
 	PRIMARY KEY("UID")
 )""",
     """
-CREATE TABLE "LIGHTSKY" (
+CREATE TABLE "LIGHTSKY1" (
 	"UID"	TEXT NOT NULL,
 	"GRADE"	INTEGER,
 	"JOB"   INTEGER,
-	"ABOUT" TEXT,
 	PRIMARY KEY("UID")
 )"""]
 
-class DefyStatus:
-    def __init__(self,code:int):
-        self.code=code
-    def __repr__(self):
-        return str(self.code)
-    def __eq__(self,value,/):
-        return self.code==value
-    def __int__(self):
-        return self.code
-
-KEEP=DefyStatus(280)
 
 #数据库管理对象。
 class __DefyProject(io.IOBase):   
     def __reset(self):
         self.__con=sqlite3.connect(self.__file)
         self.__cur=self.__con.cursor()
```

### Comparing `DefyDatabase-10.0.0a4.dev202307060610/setup.py` & `DefyDatabase-10.0.0a4.dev202307061815/setup.py`

 * *Files identical despite different names*

