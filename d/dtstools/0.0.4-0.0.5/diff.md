# Comparing `tmp/dtstools-0.0.4.tar.gz` & `tmp/dtstools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtstools-0.0.4.tar", last modified: Sun Jun 18 12:54:24 2023, max compression
+gzip compressed data, was "dtstools-0.0.5.tar", last modified: Thu Jul  6 10:27:19 2023, max compression
```

## Comparing `dtstools-0.0.4.tar` & `dtstools-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 12:54:24.465613 dtstools-0.0.4/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.4/LICENSE
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11056 2023-06-18 12:54:24.465007 dtstools-0.0.4/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     9067 2023-06-18 12:52:46.000000 dtstools-0.0.4/README.md
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      865 2023-06-18 12:51:31.000000 dtstools-0.0.4/pyproject.toml
--rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-06-18 12:54:24.465762 dtstools-0.0.4/setup.cfg
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 12:54:24.458545 dtstools-0.0.4/src/
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 12:54:24.460939 dtstools-0.0.4/src/dtstools/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.4/src/dtstools/__init__.py
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     7956 2023-06-18 12:52:28.000000 dtstools-0.0.4/src/dtstools/dtsTable.py
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 12:54:24.463805 dtstools-0.0.4/src/dtstools.egg-info/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11056 2023-06-18 12:54:24.000000 dtstools-0.0.4/src/dtstools.egg-info/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-06-18 12:54:24.000000 dtstools-0.0.4/src/dtstools.egg-info/SOURCES.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-06-18 12:54:24.000000 dtstools-0.0.4/src/dtstools.egg-info/dependency_links.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-06-18 12:54:24.000000 dtstools-0.0.4/src/dtstools.egg-info/top_level.txt
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 10:27:19.980324 dtstools-0.0.5/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.5/LICENSE
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11321 2023-07-06 10:27:19.979683 dtstools-0.0.5/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     9332 2023-07-05 11:10:06.000000 dtstools-0.0.5/README.md
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      865 2023-07-05 11:10:11.000000 dtstools-0.0.5/pyproject.toml
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-07-06 10:27:19.980533 dtstools-0.0.5/setup.cfg
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 10:27:19.973399 dtstools-0.0.5/src/
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 10:27:19.976004 dtstools-0.0.5/src/dtstools/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.5/src/dtstools/__init__.py
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    10490 2023-07-05 11:09:44.000000 dtstools-0.0.5/src/dtstools/dtsTable.py
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 10:27:19.978889 dtstools-0.0.5/src/dtstools.egg-info/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11321 2023-07-06 10:27:19.000000 dtstools-0.0.5/src/dtstools.egg-info/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-07-06 10:27:19.000000 dtstools-0.0.5/src/dtstools.egg-info/SOURCES.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-07-06 10:27:19.000000 dtstools-0.0.5/src/dtstools.egg-info/dependency_links.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-07-06 10:27:19.000000 dtstools-0.0.5/src/dtstools.egg-info/top_level.txt
```

### Comparing `dtstools-0.0.4/LICENSE` & `dtstools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dtstools-0.0.4/PKG-INFO` & `dtstools-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package aims to provide features for working with Delta Lake.
 Author-email: Reginaldo Silva <reginaldo.silva@dataside.com.br>
 License: MIT License
         
         Copyright (c) 2023 Reginaldo Silva
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,16 @@
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.4" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.4" src="https://img.shields.io/badge/version-0.0.4-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.5" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.5" src="https://img.shields.io/badge/version-0.0.5-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
@@ -84,26 +84,28 @@
 
 ## Table of Contents
 
 - [Introduction](#introducion)
 - [How to use dtstools](#how-to-use-dtstools)
 - [How to use tableSize](#how-to-use-tableSize)
 - [How to use tableMaintenance](#how-to-use-tableMaintenance)
+- [How to use LastMaintenance](#last-maintenance)
 - [Future implementations](#future-implementations)
 - [Notes](#notes)
 - [References](#references)
 
 
+
 <a href="#introducion" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 ## Introduction
 
 | version | date | description |
 |-----------|-------|----------|
-| `v0.0.4` | 2023-06-17 | Basic features |
+| `v0.0.5` | 2023-06-17 | Basic features |
 
 > This package aims to provide functionality to work with Delta Lake.
 >
 > Facilitating the visualization of the actual size (Storage) of your Delta tables and their maintenance (Vacuum and Optimize)
 
 > Below are the steps performed in order of execution:
 1. Executed a **describe detail** to get the current location and size
@@ -190,14 +192,24 @@
 
 **Apply maintenance to all tables for YOUR database**
 ```
 for tb in spark.sql(f"show tables from db_demo").collect():
   dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
 
+<a id="last-maintenance"></a>
+### Last Maintenance
+
+**Use the function dtsTable.LastMaintenance() to see summary vacuum result and optimize operations.**
+
+```
+dtsTable.LastMaintenance('database','tableName')
+```
+
+
 <a href="#future-implementations" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="future-implementations"></a>
 ## Future implementations
 
 > 1. Use Unity Catalog<br>
 > 2. Run for all databases<br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.4 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.5 Summary: This package aims
 to provide features for working with Delta Lake. Author-email: Reginaldo Silva
 silva@dataside.com.br> License: MIT License Copyright (c) 2023 Reginaldo Silva
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -19,57 +19,57 @@
 reginaldosilva27/dtstools Project-URL: README, https://www.datainaction.dev/
 blog Project-URL: Dataside, https://www.dataside.com.br Keywords:
 tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.4] [License:_MIT] [GitLab]
+                   [Version:_0.0.5] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
 ##### ## ##### ## ### ### ####### ##### ``` [https://static.wixstatic.com/
 media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Table of Contents -
 [Introduction](#introducion) - [How to use dtstools](#how-to-use-dtstools) -
 [How to use tableSize](#how-to-use-tableSize) - [How to use tableMaintenance]
-(#how-to-use-tableMaintenance) - [Future implementations](#future-
-implementations) - [Notes](#notes) - [References](#references) [https://
-static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ##
-Introduction | version | date | description | |-----------|-------|----------
-| | `v0.0.4` | 2023-06-17 | Basic features | > This package aims to provide
-functionality to work with Delta Lake. > > Facilitating the visualization of
-the actual size (Storage) of your Delta tables and their maintenance (Vacuum
-and Optimize) > Below are the steps performed in order of execution: 1.
-Executed a **describe detail** to get the current location and size 2. A scan
-(dbutils.fs.ls) is performed on the Storage folders recursively to calculate
-the space used in the Storage, excluding the _delta_logs, with this we can
-calculate an average of how much can be released with Vacuum 3. Returns a
-Dataframet [https://static.wixstatic.com/media/
-a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use dtstools
-**First install the package via PyPi** ``` pip install --upgrade dtstools ```
-**Import the dtsTable module into your context** ``` from dtstools import
-dtsTable ``` **Use the function dtsTable.Help() to see examples of function
-usage and a summary of each function.** ``` dtsTable.Help() ``` [https://
+(#how-to-use-tableMaintenance) - [How to use LastMaintenance](#last-
+maintenance) - [Future implementations](#future-implementations) - [Notes]
+(#notes) - [References](#references) [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Introduction | version |
+date | description | |-----------|-------|----------| | `v0.0.5` | 2023-06-17 |
+Basic features | > This package aims to provide functionality to work with
+Delta Lake. > > Facilitating the visualization of the actual size (Storage) of
+your Delta tables and their maintenance (Vacuum and Optimize) > Below are the
+steps performed in order of execution: 1. Executed a **describe detail** to get
+the current location and size 2. A scan (dbutils.fs.ls) is performed on the
+Storage folders recursively to calculate the space used in the Storage,
+excluding the _delta_logs, with this we can calculate an average of how much
+can be released with Vacuum 3. Returns a Dataframet [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
-### How to use tableSize > Find out the true size of your table Call the
-tableSize function passing the database and table name, use display() to see
-the results. **This function returns a Dataframe.** ``` dtsTable.tableSize
-(databaseName,tableName).display() ``` **Save the result in a Delta Table for
-monitoring and baseline** ``` dtsTable.tableSize(databaseName,tableName) \
-.write.format('delta') \ .mode('append') \ .saveAsTable
-("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/
-bronze/tableSize') ``` **Get the size of all tables in your database** ``` for
-tb in spark.sql(f"show tables from db_demo").collect(): try: print(">>
-Collecting data... Table:",tb.tableName) dtsTable.tableSize
-(tb.database,tb.tableName) \ .write.format('delta') \ .mode('append') \
-.saveAsTable("db_demo.tableSize",path='abfss://
+### How to use dtstools **First install the package via PyPi** ``` pip install
+--upgrade dtstools ``` **Import the dtsTable module into your context** ```
+from dtstools import dtsTable ``` **Use the function dtsTable.Help() to see
+examples of function usage and a summary of each function.** ``` dtsTable.Help
+() ``` [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize >
+Find out the true size of your table Call the tableSize function passing the
+database and table name, use display() to see the results. **This function
+returns a Dataframe.** ``` dtsTable.tableSize(databaseName,tableName).display()
+``` **Save the result in a Delta Table for monitoring and baseline** ```
+dtsTable.tableSize(databaseName,tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') ``` **Get the size of
+all tables in your database** ``` for tb in spark.sql(f"show tables from
+db_demo").collect(): try: print(">> Collecting data... Table:",tb.tableName)
+dtsTable.tableSize(tb.database,tb.tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
 container@storage.dfs.core.windows.net/bronze/tableSize') except Exception as
 e: print (f"###### Error to load tableName {tb.tableName} - {e}######") ```
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use
 tableMaintenance Apply maintenance to a table, Optimize and Vacuum. | Parameter
 | Description | Type | ------------- | ------------- | ------------- | |
 schemaName | Name of the database where the table is created | string | |
@@ -81,17 +81,20 @@
 to hold after vacuum runs | whole | | Debug | Just print the result on screen |
 bool | **Apply in a single table.** ``` dtsTable.tableMaintenance
 (schemaName="Database", tableName="tableName", zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` **Apply
 maintenance to all tables for YOUR database** ``` for tb in spark.sql(f"show
 tables from db_demo").collect(): dtsTable.tableMaintenance
 (schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
-vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` [https://
-static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
-Future implementations > 1. Use Unity Catalog
+vacuumRetention=168, vacuum=True, optimize=True, debug=False) ```  ### Last
+Maintenance **Use the function dtsTable.LastMaintenance() to see summary vacuum
+result and optimize operations.** ``` dtsTable.LastMaintenance
+('database','tableName') ``` [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Future implementations >
+1. Use Unity Catalog
 > 2. Run for all databases
 > 3. Minimize costs with dbutils.fs.ls by looking directly into the transaction
 log
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Notes > - For partitioned
 tables with many partitions, the execution time can take longer, so monitor the
 first executions well, the use is at your responsibility, despite not having
```

### Comparing `dtstools-0.0.4/README.md` & `dtstools-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.4" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.4" src="https://img.shields.io/badge/version-0.0.4-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.5" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.5" src="https://img.shields.io/badge/version-0.0.5-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
@@ -45,26 +45,28 @@
 
 ## Table of Contents
 
 - [Introduction](#introducion)
 - [How to use dtstools](#how-to-use-dtstools)
 - [How to use tableSize](#how-to-use-tableSize)
 - [How to use tableMaintenance](#how-to-use-tableMaintenance)
+- [How to use LastMaintenance](#last-maintenance)
 - [Future implementations](#future-implementations)
 - [Notes](#notes)
 - [References](#references)
 
 
+
 <a href="#introducion" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 ## Introduction
 
 | version | date | description |
 |-----------|-------|----------|
-| `v0.0.4` | 2023-06-17 | Basic features |
+| `v0.0.5` | 2023-06-17 | Basic features |
 
 > This package aims to provide functionality to work with Delta Lake.
 >
 > Facilitating the visualization of the actual size (Storage) of your Delta tables and their maintenance (Vacuum and Optimize)
 
 > Below are the steps performed in order of execution:
 1. Executed a **describe detail** to get the current location and size
@@ -151,14 +153,24 @@
 
 **Apply maintenance to all tables for YOUR database**
 ```
 for tb in spark.sql(f"show tables from db_demo").collect():
   dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
 
+<a id="last-maintenance"></a>
+### Last Maintenance
+
+**Use the function dtsTable.LastMaintenance() to see summary vacuum result and optimize operations.**
+
+```
+dtsTable.LastMaintenance('database','tableName')
+```
+
+
 <a href="#future-implementations" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="future-implementations"></a>
 ## Future implementations
 
 > 1. Use Unity Catalog<br>
 > 2. Run for all databases<br>
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.4] [License:_MIT] [GitLab]
+                   [Version:_0.0.5] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
 ##### ## ##### ## ### ### ####### ##### ``` [https://static.wixstatic.com/
 media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Table of Contents -
 [Introduction](#introducion) - [How to use dtstools](#how-to-use-dtstools) -
 [How to use tableSize](#how-to-use-tableSize) - [How to use tableMaintenance]
-(#how-to-use-tableMaintenance) - [Future implementations](#future-
-implementations) - [Notes](#notes) - [References](#references) [https://
-static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ##
-Introduction | version | date | description | |-----------|-------|----------
-| | `v0.0.4` | 2023-06-17 | Basic features | > This package aims to provide
-functionality to work with Delta Lake. > > Facilitating the visualization of
-the actual size (Storage) of your Delta tables and their maintenance (Vacuum
-and Optimize) > Below are the steps performed in order of execution: 1.
-Executed a **describe detail** to get the current location and size 2. A scan
-(dbutils.fs.ls) is performed on the Storage folders recursively to calculate
-the space used in the Storage, excluding the _delta_logs, with this we can
-calculate an average of how much can be released with Vacuum 3. Returns a
-Dataframet [https://static.wixstatic.com/media/
-a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use dtstools
-**First install the package via PyPi** ``` pip install --upgrade dtstools ```
-**Import the dtsTable module into your context** ``` from dtstools import
-dtsTable ``` **Use the function dtsTable.Help() to see examples of function
-usage and a summary of each function.** ``` dtsTable.Help() ``` [https://
+(#how-to-use-tableMaintenance) - [How to use LastMaintenance](#last-
+maintenance) - [Future implementations](#future-implementations) - [Notes]
+(#notes) - [References](#references) [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Introduction | version |
+date | description | |-----------|-------|----------| | `v0.0.5` | 2023-06-17 |
+Basic features | > This package aims to provide functionality to work with
+Delta Lake. > > Facilitating the visualization of the actual size (Storage) of
+your Delta tables and their maintenance (Vacuum and Optimize) > Below are the
+steps performed in order of execution: 1. Executed a **describe detail** to get
+the current location and size 2. A scan (dbutils.fs.ls) is performed on the
+Storage folders recursively to calculate the space used in the Storage,
+excluding the _delta_logs, with this we can calculate an average of how much
+can be released with Vacuum 3. Returns a Dataframet [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
-### How to use tableSize > Find out the true size of your table Call the
-tableSize function passing the database and table name, use display() to see
-the results. **This function returns a Dataframe.** ``` dtsTable.tableSize
-(databaseName,tableName).display() ``` **Save the result in a Delta Table for
-monitoring and baseline** ``` dtsTable.tableSize(databaseName,tableName) \
-.write.format('delta') \ .mode('append') \ .saveAsTable
-("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/
-bronze/tableSize') ``` **Get the size of all tables in your database** ``` for
-tb in spark.sql(f"show tables from db_demo").collect(): try: print(">>
-Collecting data... Table:",tb.tableName) dtsTable.tableSize
-(tb.database,tb.tableName) \ .write.format('delta') \ .mode('append') \
-.saveAsTable("db_demo.tableSize",path='abfss://
+### How to use dtstools **First install the package via PyPi** ``` pip install
+--upgrade dtstools ``` **Import the dtsTable module into your context** ```
+from dtstools import dtsTable ``` **Use the function dtsTable.Help() to see
+examples of function usage and a summary of each function.** ``` dtsTable.Help
+() ``` [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize >
+Find out the true size of your table Call the tableSize function passing the
+database and table name, use display() to see the results. **This function
+returns a Dataframe.** ``` dtsTable.tableSize(databaseName,tableName).display()
+``` **Save the result in a Delta Table for monitoring and baseline** ```
+dtsTable.tableSize(databaseName,tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') ``` **Get the size of
+all tables in your database** ``` for tb in spark.sql(f"show tables from
+db_demo").collect(): try: print(">> Collecting data... Table:",tb.tableName)
+dtsTable.tableSize(tb.database,tb.tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
 container@storage.dfs.core.windows.net/bronze/tableSize') except Exception as
 e: print (f"###### Error to load tableName {tb.tableName} - {e}######") ```
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use
 tableMaintenance Apply maintenance to a table, Optimize and Vacuum. | Parameter
 | Description | Type | ------------- | ------------- | ------------- | |
 schemaName | Name of the database where the table is created | string | |
@@ -57,17 +57,20 @@
 to hold after vacuum runs | whole | | Debug | Just print the result on screen |
 bool | **Apply in a single table.** ``` dtsTable.tableMaintenance
 (schemaName="Database", tableName="tableName", zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` **Apply
 maintenance to all tables for YOUR database** ``` for tb in spark.sql(f"show
 tables from db_demo").collect(): dtsTable.tableMaintenance
 (schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
-vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` [https://
-static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
-Future implementations > 1. Use Unity Catalog
+vacuumRetention=168, vacuum=True, optimize=True, debug=False) ```  ### Last
+Maintenance **Use the function dtsTable.LastMaintenance() to see summary vacuum
+result and optimize operations.** ``` dtsTable.LastMaintenance
+('database','tableName') ``` [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Future implementations >
+1. Use Unity Catalog
 > 2. Run for all databases
 > 3. Minimize costs with dbutils.fs.ls by looking directly into the transaction
 log
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Notes > - For partitioned
 tables with many partitions, the execution time can take longer, so monitor the
 first executions well, the use is at your responsibility, despite not having
```

### Comparing `dtstools-0.0.4/pyproject.toml` & `dtstools-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtstools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Reginaldo Silva", email="reginaldo.silva@dataside.com.br" },
 ]
 description = "This package aims to provide features for working with Delta Lake."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `dtstools-0.0.4/src/dtstools.egg-info/PKG-INFO` & `dtstools-0.0.5/src/dtstools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package aims to provide features for working with Delta Lake.
 Author-email: Reginaldo Silva <reginaldo.silva@dataside.com.br>
 License: MIT License
         
         Copyright (c) 2023 Reginaldo Silva
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,16 @@
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.4" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.4" src="https://img.shields.io/badge/version-0.0.4-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.5" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.5" src="https://img.shields.io/badge/version-0.0.5-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
@@ -84,26 +84,28 @@
 
 ## Table of Contents
 
 - [Introduction](#introducion)
 - [How to use dtstools](#how-to-use-dtstools)
 - [How to use tableSize](#how-to-use-tableSize)
 - [How to use tableMaintenance](#how-to-use-tableMaintenance)
+- [How to use LastMaintenance](#last-maintenance)
 - [Future implementations](#future-implementations)
 - [Notes](#notes)
 - [References](#references)
 
 
+
 <a href="#introducion" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 ## Introduction
 
 | version | date | description |
 |-----------|-------|----------|
-| `v0.0.4` | 2023-06-17 | Basic features |
+| `v0.0.5` | 2023-06-17 | Basic features |
 
 > This package aims to provide functionality to work with Delta Lake.
 >
 > Facilitating the visualization of the actual size (Storage) of your Delta tables and their maintenance (Vacuum and Optimize)
 
 > Below are the steps performed in order of execution:
 1. Executed a **describe detail** to get the current location and size
@@ -190,14 +192,24 @@
 
 **Apply maintenance to all tables for YOUR database**
 ```
 for tb in spark.sql(f"show tables from db_demo").collect():
   dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
 
+<a id="last-maintenance"></a>
+### Last Maintenance
+
+**Use the function dtsTable.LastMaintenance() to see summary vacuum result and optimize operations.**
+
+```
+dtsTable.LastMaintenance('database','tableName')
+```
+
+
 <a href="#future-implementations" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="future-implementations"></a>
 ## Future implementations
 
 > 1. Use Unity Catalog<br>
 > 2. Run for all databases<br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.4 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.5 Summary: This package aims
 to provide features for working with Delta Lake. Author-email: Reginaldo Silva
 silva@dataside.com.br> License: MIT License Copyright (c) 2023 Reginaldo Silva
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -19,57 +19,57 @@
 reginaldosilva27/dtstools Project-URL: README, https://www.datainaction.dev/
 blog Project-URL: Dataside, https://www.dataside.com.br Keywords:
 tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.4] [License:_MIT] [GitLab]
+                   [Version:_0.0.5] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
 ##### ## ##### ## ### ### ####### ##### ``` [https://static.wixstatic.com/
 media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Table of Contents -
 [Introduction](#introducion) - [How to use dtstools](#how-to-use-dtstools) -
 [How to use tableSize](#how-to-use-tableSize) - [How to use tableMaintenance]
-(#how-to-use-tableMaintenance) - [Future implementations](#future-
-implementations) - [Notes](#notes) - [References](#references) [https://
-static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ##
-Introduction | version | date | description | |-----------|-------|----------
-| | `v0.0.4` | 2023-06-17 | Basic features | > This package aims to provide
-functionality to work with Delta Lake. > > Facilitating the visualization of
-the actual size (Storage) of your Delta tables and their maintenance (Vacuum
-and Optimize) > Below are the steps performed in order of execution: 1.
-Executed a **describe detail** to get the current location and size 2. A scan
-(dbutils.fs.ls) is performed on the Storage folders recursively to calculate
-the space used in the Storage, excluding the _delta_logs, with this we can
-calculate an average of how much can be released with Vacuum 3. Returns a
-Dataframet [https://static.wixstatic.com/media/
-a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use dtstools
-**First install the package via PyPi** ``` pip install --upgrade dtstools ```
-**Import the dtsTable module into your context** ``` from dtstools import
-dtsTable ``` **Use the function dtsTable.Help() to see examples of function
-usage and a summary of each function.** ``` dtsTable.Help() ``` [https://
+(#how-to-use-tableMaintenance) - [How to use LastMaintenance](#last-
+maintenance) - [Future implementations](#future-implementations) - [Notes]
+(#notes) - [References](#references) [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Introduction | version |
+date | description | |-----------|-------|----------| | `v0.0.5` | 2023-06-17 |
+Basic features | > This package aims to provide functionality to work with
+Delta Lake. > > Facilitating the visualization of the actual size (Storage) of
+your Delta tables and their maintenance (Vacuum and Optimize) > Below are the
+steps performed in order of execution: 1. Executed a **describe detail** to get
+the current location and size 2. A scan (dbutils.fs.ls) is performed on the
+Storage folders recursively to calculate the space used in the Storage,
+excluding the _delta_logs, with this we can calculate an average of how much
+can be released with Vacuum 3. Returns a Dataframet [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
-### How to use tableSize > Find out the true size of your table Call the
-tableSize function passing the database and table name, use display() to see
-the results. **This function returns a Dataframe.** ``` dtsTable.tableSize
-(databaseName,tableName).display() ``` **Save the result in a Delta Table for
-monitoring and baseline** ``` dtsTable.tableSize(databaseName,tableName) \
-.write.format('delta') \ .mode('append') \ .saveAsTable
-("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/
-bronze/tableSize') ``` **Get the size of all tables in your database** ``` for
-tb in spark.sql(f"show tables from db_demo").collect(): try: print(">>
-Collecting data... Table:",tb.tableName) dtsTable.tableSize
-(tb.database,tb.tableName) \ .write.format('delta') \ .mode('append') \
-.saveAsTable("db_demo.tableSize",path='abfss://
+### How to use dtstools **First install the package via PyPi** ``` pip install
+--upgrade dtstools ``` **Import the dtsTable module into your context** ```
+from dtstools import dtsTable ``` **Use the function dtsTable.Help() to see
+examples of function usage and a summary of each function.** ``` dtsTable.Help
+() ``` [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize >
+Find out the true size of your table Call the tableSize function passing the
+database and table name, use display() to see the results. **This function
+returns a Dataframe.** ``` dtsTable.tableSize(databaseName,tableName).display()
+``` **Save the result in a Delta Table for monitoring and baseline** ```
+dtsTable.tableSize(databaseName,tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') ``` **Get the size of
+all tables in your database** ``` for tb in spark.sql(f"show tables from
+db_demo").collect(): try: print(">> Collecting data... Table:",tb.tableName)
+dtsTable.tableSize(tb.database,tb.tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
 container@storage.dfs.core.windows.net/bronze/tableSize') except Exception as
 e: print (f"###### Error to load tableName {tb.tableName} - {e}######") ```
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use
 tableMaintenance Apply maintenance to a table, Optimize and Vacuum. | Parameter
 | Description | Type | ------------- | ------------- | ------------- | |
 schemaName | Name of the database where the table is created | string | |
@@ -81,17 +81,20 @@
 to hold after vacuum runs | whole | | Debug | Just print the result on screen |
 bool | **Apply in a single table.** ``` dtsTable.tableMaintenance
 (schemaName="Database", tableName="tableName", zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` **Apply
 maintenance to all tables for YOUR database** ``` for tb in spark.sql(f"show
 tables from db_demo").collect(): dtsTable.tableMaintenance
 (schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
-vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` [https://
-static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
-Future implementations > 1. Use Unity Catalog
+vacuumRetention=168, vacuum=True, optimize=True, debug=False) ```  ### Last
+Maintenance **Use the function dtsTable.LastMaintenance() to see summary vacuum
+result and optimize operations.** ``` dtsTable.LastMaintenance
+('database','tableName') ``` [https://static.wixstatic.com/media/
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Future implementations >
+1. Use Unity Catalog
 > 2. Run for all databases
 > 3. Minimize costs with dbutils.fs.ls by looking directly into the transaction
 log
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Notes > - For partitioned
 tables with many partitions, the execution time can take longer, so monitor the
 first executions well, the use is at your responsibility, despite not having
```

