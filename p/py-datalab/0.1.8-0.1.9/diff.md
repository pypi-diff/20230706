# Comparing `tmp/py-datalab-0.1.8.tar.gz` & `tmp/py-datalab-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.1.8.tar", last modified: Thu Jul  6 12:18:36 2023, max compression
+gzip compressed data, was "py-datalab-0.1.9.tar", last modified: Thu Jul  6 12:22:59 2023, max compression
```

## Comparing `py-datalab-0.1.8.tar` & `py-datalab-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:18:36.359370 py-datalab-0.1.8/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1006 2023-07-06 12:18:36.359370 py-datalab-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:18:36.340550 py-datalab-0.1.8/datalab/
--rw-rw-rw-   0        0        0    10677 2023-07-06 12:15:38.000000 py-datalab-0.1.8/datalab/Matrix.py
--rw-rw-rw-   0        0        0     7445 2023-07-06 12:18:16.000000 py-datalab-0.1.8/datalab/Vector.py
--rw-rw-rw-   0        0        0       56 2023-07-06 12:16:58.000000 py-datalab-0.1.8/datalab/__init__.py
--rw-rw-rw-   0        0        0     4231 2023-07-06 12:02:49.000000 py-datalab-0.1.8/datalab/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:18:36.357371 py-datalab-0.1.8/py_datalab.egg-info/
--rw-rw-rw-   0        0        0     1006 2023-07-06 12:18:36.000000 py-datalab-0.1.8/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-06 12:18:36.000000 py-datalab-0.1.8/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:18:36.000000 py-datalab-0.1.8/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 12:18:36.000000 py-datalab-0.1.8/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 12:18:36.360371 py-datalab-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-06 12:18:31.000000 py-datalab-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:59.882412 py-datalab-0.1.9/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1006 2023-07-06 12:22:59.881411 py-datalab-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2437 2023-07-03 12:36:33.000000 py-datalab-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:59.867869 py-datalab-0.1.9/datalab/
+-rw-rw-rw-   0        0        0    10355 2023-07-06 12:22:56.000000 py-datalab-0.1.9/datalab/Matrix.py
+-rw-rw-rw-   0        0        0     7061 2023-07-06 12:22:50.000000 py-datalab-0.1.9/datalab/Vector.py
+-rw-rw-rw-   0        0        0       56 2023-07-06 12:16:58.000000 py-datalab-0.1.9/datalab/__init__.py
+-rw-rw-rw-   0        0        0     4231 2023-07-06 12:02:49.000000 py-datalab-0.1.9/datalab/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:59.880414 py-datalab-0.1.9/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0     1006 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 12:22:59.000000 py-datalab-0.1.9/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 12:22:59.882412 py-datalab-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-06 12:21:56.000000 py-datalab-0.1.9/setup.py
```

### Comparing `py-datalab-0.1.8/LICENSE` & `py-datalab-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.8/PKG-INFO` & `py-datalab-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.8
+Version: 0.1.9
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.1.8/README.md` & `py-datalab-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.8/datalab/Matrix.py` & `py-datalab-0.1.9/datalab/Matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,31 +81,21 @@
 
         max_element_lengths = tuple(
             max(len(str(row[i])) for row in buffer) for i in range(len(buffer[0]))
         )
 
         output = ""
 
-        for i, row in enumerate(buffer):
-            if i != 0:
-                output += "│ "
-            elif i == len(buffer) - 1:
-                output += "╵"
-            else:
-                output += "╷"
+        for row in buffer:
+            output += "│ "
 
             for value, max_length in zip(row, max_element_lengths):
                 output += f"{value}{' ' * (max_length - len(value) + 1)}"
 
-            if i != 0:
-                output += "│\n"
-            elif i == len(buffer) - 1:
-                output += "╵"
-            else:
-                output += "╷\n"
+            output += "│\n"
 
         return output
 
     def __setitem__(self, index: int, value: object) -> None:
         if isinstance(index, tuple) and len(index) == 2:
             rows, columns = index
             if self.dtype == int:
```

### Comparing `py-datalab-0.1.8/datalab/Vector.py` & `py-datalab-0.1.9/datalab/Vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,30 +70,16 @@
 
             buffer[i] = formatted_value
 
         max_element_length = max(len(str(item)) for item in buffer)
 
         output = ""
 
-        for i, value in enumerate(buffer):
-            if i != 0:
-                output += "│ "
-            elif i == len(buffer) - 1:
-                output += "╵ "
-            else:
-                output += "╷ "
-
-            output += f"{value}{' ' * (max_element_length - len(value) + 1)}"
-
-            if i != 0:
-                output += " │\n"
-            elif i == len(buffer) - 1:
-                output += " ╵\n"
-            else:
-                output += " ╷\n"
+        for value in buffer:
+            output += f"│ {value}{' ' * (max_element_length - len(value) + 1)} │\n"
 
         return output
 
     def __setitem__(self, index: int, value: object) -> None:
         if self.dtype == int:
             self.__data[index] = int(value)
```

### Comparing `py-datalab-0.1.8/datalab/utils.py` & `py-datalab-0.1.9/datalab/utils.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.1.8/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.1.9/py_datalab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.1.8
+Version: 0.1.9
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-datalab-0.1.8/setup.py` & `py-datalab-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 6):
     sys.exit("Sorry, Python < 3.6 is not supported")
 
 setup(
     name="py-datalab",
-    version="0.1.8",
+    version="0.1.9",
     author="Mateusz Nowak",
     author_email="mateusz.nowak.pol@gmail.com",
     description="This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.",
     url="https://github.com/matuszen/Python-DataLab",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

