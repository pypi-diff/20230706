# Comparing `tmp/spark_datax_tools-0.4.tar.gz` & `tmp/spark_datax_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_datax_tools-0.4.tar", last modified: Tue Jun 27 12:07:24 2023, max compression
+gzip compressed data, was "spark_datax_tools-0.5.0.tar", last modified: Thu Jul  6 03:36:05 2023, max compression
```

## Comparing `spark_datax_tools-0.4.tar` & `spark_datax_tools-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.4/LICENSE
--rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4264 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.4/README.md
--rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1162 2023-06-27 12:07:00.000000 spark_datax_tools-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.744099 spark_datax_tools-0.4/spark_datax_tools/
--rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.4/spark_datax_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.759726 spark_datax_tools-0.4/spark_datax_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.4/spark_datax_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    43876 2023-06-27 12:06:38.000000 spark_datax_tools-0.4/spark_datax_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.775353 spark_datax_tools-0.4/spark_datax_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.4/spark_datax_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.4/spark_datax_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.790978 spark_datax_tools-0.4/spark_datax_tools/utils/files/
--rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_datax_tools-0.4/spark_datax_tools/utils/files/ns.csv
--rw-rw-rw-   0        0        0     3472 2023-06-05 07:39:00.000000 spark_datax_tools-0.4/spark_datax_tools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:07:24.759726 spark_datax_tools-0.4/spark_datax_tools.egg-info/
--rw-rw-rw-   0        0        0     4264 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-27 12:07:24.000000 spark_datax_tools-0.4/spark_datax_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:05.500365 spark_datax_tools-0.5.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4266 2023-07-06 03:36:05.500365 spark_datax_tools-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.5.0/README.md
+-rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-06 03:36:05.505368 spark_datax_tools-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-06 03:33:14.000000 spark_datax_tools-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:05.465357 spark_datax_tools-0.5.0/spark_datax_tools/
+-rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.5.0/spark_datax_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:05.491362 spark_datax_tools-0.5.0/spark_datax_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.5.0/spark_datax_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    43876 2023-06-27 12:06:38.000000 spark_datax_tools-0.5.0/spark_datax_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:05.494364 spark_datax_tools-0.5.0/spark_datax_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.5.0/spark_datax_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.5.0/spark_datax_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:05.500365 spark_datax_tools-0.5.0/spark_datax_tools/utils/files/
+-rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_datax_tools-0.5.0/spark_datax_tools/utils/files/ns.csv
+-rw-rw-rw-   0        0        0     3950 2023-07-06 03:31:36.000000 spark_datax_tools-0.5.0/spark_datax_tools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:05.483362 spark_datax_tools-0.5.0/spark_datax_tools.egg-info/
+-rw-rw-rw-   0        0        0     4266 2023-07-06 03:36:05.000000 spark_datax_tools-0.5.0/spark_datax_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-07-06 03:36:05.000000 spark_datax_tools-0.5.0/spark_datax_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:36:05.000000 spark_datax_tools-0.5.0/spark_datax_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-07-06 03:36:05.000000 spark_datax_tools-0.5.0/spark_datax_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-06 03:36:05.000000 spark_datax_tools-0.5.0/spark_datax_tools.egg-info/top_level.txt
```

### Comparing `spark_datax_tools-0.4/LICENSE` & `spark_datax_tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.4/PKG-INFO` & `spark_datax_tools-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_datax_tools
-Version: 0.4
+Version: 0.5.0
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.4/README.md` & `spark_datax_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.4/pyproject.toml` & `spark_datax_tools-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.4/setup.py` & `spark_datax_tools-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_datax_tools',
     packages=find_packages(),
-    version='0.4',
+    version='0.5.0',
     description='spark_datax_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_datax_tools/',
     download_url='https://github.com/jonaqp/spark_datax_tools/archive/main.zip',
```

### Comparing `spark_datax_tools-0.4/spark_datax_tools/__init__.py` & `spark_datax_tools-0.5.0/spark_datax_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.4/spark_datax_tools/functions/generator.py` & `spark_datax_tools-0.5.0/spark_datax_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.4/spark_datax_tools/utils/files/ns.csv` & `spark_datax_tools-0.5.0/spark_datax_tools/utils/files/ns.csv`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.4/spark_datax_tools/utils/utils.py` & `spark_datax_tools-0.5.0/spark_datax_tools/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,14 +63,26 @@
         _type = types.StructField(columns, types.IntegerType())
         if convert_string:
             _mask = ""
             _format = "ALPHANUMERIC"
             _locale = ""
             _schema_type = "['string', 'null']"
             _type = types.StructField(columns, types.StringType())
+    elif str(_format).upper() in ("NUMERIC BIG", "NUMERIC LARGE"):
+        _mask = ""
+        _format = format
+        _locale = ""
+        _schema_type = "['null', 'int64']"
+        _type = types.StructField(columns, types.IntegerType())
+        if convert_string:
+            _mask = ""
+            _format = "ALPHANUMERIC"
+            _locale = ""
+            _schema_type = "['string', 'null']"
+            _type = types.StructField(columns, types.StringType())
     elif str(_format).upper().startswith("DECIMAL"):
         _parentheses = extract_only_parenthesis(format)
         _parentheses_split = str(_parentheses).split(",")
         if len(_parentheses_split) <= 1:
             _decimal_left = int(_parentheses_split[0])
             _decimal_right = 0
         else:
```

### Comparing `spark_datax_tools-0.4/spark_datax_tools.egg-info/PKG-INFO` & `spark_datax_tools-0.5.0/spark_datax_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-datax-tools
-Version: 0.4
+Version: 0.5.0
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.4/spark_datax_tools.egg-info/SOURCES.txt` & `spark_datax_tools-0.5.0/spark_datax_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

