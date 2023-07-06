# Comparing `tmp/spark_dummy_tools-0.4.0.tar.gz` & `tmp/spark_dummy_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dummy_tools-0.4.0.tar", last modified: Sun Jul  2 20:55:53 2023, max compression
+gzip compressed data, was "spark_dummy_tools-0.5.0.tar", last modified: Thu Jul  6 03:36:01 2023, max compression
```

## Comparing `spark_dummy_tools-0.4.0.tar` & `spark_dummy_tools-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 20:55:53.691036 spark_dummy_tools-0.4.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_dummy_tools-0.4.0/LICENSE
--rw-rw-rw-   0        0        0        4 2023-06-26 03:19:39.000000 spark_dummy_tools-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4254 2023-07-02 20:55:53.691036 spark_dummy_tools-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3495 2023-06-28 06:31:22.000000 spark_dummy_tools-0.4.0/README.md
--rw-rw-rw-   0        0        0      636 2023-06-26 03:37:00.000000 spark_dummy_tools-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-02 20:55:53.692035 spark_dummy_tools-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-07-02 20:55:28.000000 spark_dummy_tools-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 20:55:53.673030 spark_dummy_tools-0.4.0/spark_dummy_tools/
--rw-rw-rw-   0        0        0      485 2023-07-02 20:48:09.000000 spark_dummy_tools-0.4.0/spark_dummy_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 20:55:53.689033 spark_dummy_tools-0.4.0/spark_dummy_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_dummy_tools-0.4.0/spark_dummy_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     9556 2023-06-28 07:01:11.000000 spark_dummy_tools-0.4.0/spark_dummy_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-02 20:55:53.690033 spark_dummy_tools-0.4.0/spark_dummy_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_dummy_tools-0.4.0/spark_dummy_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_dummy_tools-0.4.0/spark_dummy_tools/utils/color.py
--rw-rw-rw-   0        0        0     6996 2023-07-02 20:55:28.000000 spark_dummy_tools-0.4.0/spark_dummy_tools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-02 20:55:53.688033 spark_dummy_tools-0.4.0/spark_dummy_tools.egg-info/
--rw-rw-rw-   0        0        0     4254 2023-07-02 20:55:53.000000 spark_dummy_tools-0.4.0/spark_dummy_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-07-02 20:55:53.000000 spark_dummy_tools-0.4.0/spark_dummy_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 20:55:53.000000 spark_dummy_tools-0.4.0/spark_dummy_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2023-07-02 20:55:53.000000 spark_dummy_tools-0.4.0/spark_dummy_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-02 20:55:53.000000 spark_dummy_tools-0.4.0/spark_dummy_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:01.329807 spark_dummy_tools-0.5.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_dummy_tools-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0        4 2023-06-26 03:19:39.000000 spark_dummy_tools-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4254 2023-07-06 03:36:01.329807 spark_dummy_tools-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3495 2023-06-28 06:31:22.000000 spark_dummy_tools-0.5.0/README.md
+-rw-rw-rw-   0        0        0      636 2023-06-26 03:37:00.000000 spark_dummy_tools-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-06 03:36:01.330807 spark_dummy_tools-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-06 03:35:44.000000 spark_dummy_tools-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:01.294798 spark_dummy_tools-0.5.0/spark_dummy_tools/
+-rw-rw-rw-   0        0        0      485 2023-07-02 20:48:09.000000 spark_dummy_tools-0.5.0/spark_dummy_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:01.322805 spark_dummy_tools-0.5.0/spark_dummy_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_dummy_tools-0.5.0/spark_dummy_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     9556 2023-06-28 07:01:11.000000 spark_dummy_tools-0.5.0/spark_dummy_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:01.329807 spark_dummy_tools-0.5.0/spark_dummy_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_dummy_tools-0.5.0/spark_dummy_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_dummy_tools-0.5.0/spark_dummy_tools/utils/color.py
+-rw-rw-rw-   0        0        0     7524 2023-07-06 03:35:33.000000 spark_dummy_tools-0.5.0/spark_dummy_tools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:36:01.314803 spark_dummy_tools-0.5.0/spark_dummy_tools.egg-info/
+-rw-rw-rw-   0        0        0     4254 2023-07-06 03:36:01.000000 spark_dummy_tools-0.5.0/spark_dummy_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-07-06 03:36:01.000000 spark_dummy_tools-0.5.0/spark_dummy_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:36:01.000000 spark_dummy_tools-0.5.0/spark_dummy_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2023-07-06 03:36:01.000000 spark_dummy_tools-0.5.0/spark_dummy_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-06 03:36:01.000000 spark_dummy_tools-0.5.0/spark_dummy_tools.egg-info/top_level.txt
```

### Comparing `spark_dummy_tools-0.4.0/LICENSE` & `spark_dummy_tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dummy_tools-0.4.0/PKG-INFO` & `spark_dummy_tools-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dummy_tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: spark_dummy_tools
 Home-page: https://github.com/jonaqp/spark_dummy_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dummy_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_dummy_tools-0.4.0/README.md` & `spark_dummy_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_dummy_tools-0.4.0/pyproject.toml` & `spark_dummy_tools-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_dummy_tools-0.4.0/setup.py` & `spark_dummy_tools-0.5.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dummy_tools',
     packages=find_packages(),
-    version='0.4.0',
+    version='0.5.0',
     description='spark_dummy_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dummy_tools/',
     download_url='https://github.com/jonaqp/spark_dummy_tools/archive/main.zip',
```

### Comparing `spark_dummy_tools-0.4.0/spark_dummy_tools/functions/generator.py` & `spark_dummy_tools-0.5.0/spark_dummy_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_dummy_tools-0.4.0/spark_dummy_tools/utils/utils.py` & `spark_dummy_tools-0.5.0/spark_dummy_tools/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,26 @@
         _type = types.StructField(columns, types.IntegerType())
         _type_string = types.StructField(columns, types.StringType())
         if convert_string:
             _mask = ""
             _format = "ALPHANUMERIC"
             _locale = ""
             _schema_type = "['string', 'null']"
-
+    elif str(_format).upper() in ("NUMERIC BIG", "NUMERIC LARGE"):
+        _mask = ""
+        _format = format
+        _locale = ""
+        _schema_type = "['null', 'int64']"
+        _type = types.StructField(columns, types.IntegerType())
+        _type_string = types.StructField(columns, types.StringType())
+        if convert_string:
+            _mask = ""
+            _format = "ALPHANUMERIC"
+            _locale = ""
+            _schema_type = "['string', 'null']"
     elif str(_format).upper().startswith("DECIMAL"):
         _parentheses = extract_only_parenthesis(format)
         _parentheses_split = str(_parentheses).split(",")
         if len(_parentheses_split) <= 1:
             _decimal_left = int(_parentheses_split[0])
             _decimal_right = 0
         else:
@@ -128,15 +139,15 @@
     from datetime import datetime
     from dateutil.relativedelta import relativedelta
 
     fake = Faker()
     _fake = None
     format = str(format).upper()
 
-    if format.startswith(("INTEGER", "NUMERIC")):
+    if format.startswith(("INTEGER", "NUMERIC", "NUMERIC SHORT", "NUMERIC BIG", "NUMERIC LARGE")):
         _fake = fake.pyint(min_value=0, max_value=9999)
         if naming in list(columns_integer_default.keys()):
             new_int = int(columns_integer_default[naming])
             _fake = fake.pyint(min_value=new_int, max_value=new_int)
 
     elif format.startswith("TIMESTAMP"):
         d2 = datetime.now()
```

### Comparing `spark_dummy_tools-0.4.0/spark_dummy_tools.egg-info/PKG-INFO` & `spark_dummy_tools-0.5.0/spark_dummy_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dummy-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: spark_dummy_tools
 Home-page: https://github.com/jonaqp/spark_dummy_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dummy_tools/archive/main.zip
 Keywords: spark,datax,schema
```

