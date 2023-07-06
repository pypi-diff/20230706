# Comparing `tmp/repleno-0.0.12.tar.gz` & `tmp/repleno-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repleno-0.0.12.tar", last modified: Tue Jul  4 11:52:06 2023, max compression
+gzip compressed data, was "repleno-0.0.13.tar", last modified: Thu Jul  6 16:22:58 2023, max compression
```

## Comparing `repleno-0.0.12.tar` & `repleno-0.0.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 11:52:06.273580 repleno-0.0.12/
--rw-rw-rw-   0        0        0     2608 2023-07-04 11:52:06.273580 repleno-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     2017 2023-06-26 17:07:24.000000 repleno-0.0.12/README.md
--rw-rw-rw-   0        0        0     1009 2023-07-04 11:51:42.000000 repleno-0.0.12/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 11:52:06.276286 repleno-0.0.12/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 11:52:06.220829 repleno-0.0.12/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 11:52:06.249622 repleno-0.0.12/src/repleno/
--rw-rw-rw-   0        0        0    33943 2023-07-04 11:49:11.000000 repleno-0.0.12/src/repleno/SKU.py
--rw-rw-rw-   0        0        0      519 2023-06-25 14:02:32.000000 repleno-0.0.12/src/repleno/__init__.py
--rw-rw-rw-   0        0        0       96 2023-06-25 14:02:32.000000 repleno-0.0.12/src/repleno/__main__.py
--rw-rw-rw-   0        0        0    27226 2023-07-04 11:42:19.000000 repleno-0.0.12/src/repleno/factory.py
--rw-rw-rw-   0        0        0     2310 2023-06-26 18:04:48.000000 repleno-0.0.12/src/repleno/order.py
--rw-rw-rw-   0        0        0     9539 2023-06-23 15:07:08.000000 repleno-0.0.12/src/repleno/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:52:06.265848 repleno-0.0.12/src/repleno.egg-info/
--rw-rw-rw-   0        0        0     2608 2023-07-04 11:52:06.000000 repleno-0.0.12/src/repleno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-04 11:52:06.000000 repleno-0.0.12/src/repleno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 11:52:06.000000 repleno-0.0.12/src/repleno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-04 11:52:06.000000 repleno-0.0.12/src/repleno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 11:52:06.000000 repleno-0.0.12/src/repleno.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.465005 repleno-0.0.13/
+-rw-rw-rw-   0        0        0     2608 2023-07-06 16:22:58.462998 repleno-0.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     2017 2023-06-26 17:07:24.000000 repleno-0.0.13/README.md
+-rw-rw-rw-   0        0        0     1009 2023-07-06 16:22:17.000000 repleno-0.0.13/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 16:22:58.465005 repleno-0.0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.404663 repleno-0.0.13/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.440666 repleno-0.0.13/src/repleno/
+-rw-rw-rw-   0        0        0    33949 2023-07-06 12:59:02.000000 repleno-0.0.13/src/repleno/SKU.py
+-rw-rw-rw-   0        0        0      519 2023-06-25 14:02:32.000000 repleno-0.0.13/src/repleno/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-06-25 14:02:32.000000 repleno-0.0.13/src/repleno/__main__.py
+-rw-rw-rw-   0        0        0    27226 2023-07-04 11:42:19.000000 repleno-0.0.13/src/repleno/factory.py
+-rw-rw-rw-   0        0        0     2310 2023-06-26 18:04:48.000000 repleno-0.0.13/src/repleno/order.py
+-rw-rw-rw-   0        0        0     9575 2023-07-06 16:17:59.000000 repleno-0.0.13/src/repleno/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:22:58.458989 repleno-0.0.13/src/repleno.egg-info/
+-rw-rw-rw-   0        0        0     2608 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 16:22:58.000000 repleno-0.0.13/src/repleno.egg-info/top_level.txt
```

### Comparing `repleno-0.0.12/PKG-INFO` & `repleno-0.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repleno
-Version: 0.0.12
+Version: 0.0.13
 Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
 Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
 Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Manufacturing
```

### Comparing `repleno-0.0.12/README.md` & `repleno-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `repleno-0.0.12/pyproject.toml` & `repleno-0.0.13/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = 'repleno'
-version = '0.0.12'
+version = '0.0.13'
 authors = [
     {'name' = 'Afonso Schulz Albrecht', email = 'a.schulzalbrecht@gmail.com'},
 ]
 description = 'Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)'
 keywords = ['supply chain', 'bill of materials', 'material requirements planning', 'BOM', 'MRP']
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `repleno-0.0.12/src/repleno/SKU.py` & `repleno-0.0.13/src/repleno/SKU.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,15 +907,15 @@
 
         attributes : list[str], optional
             Returns the list of dictionaries including the SKU attributes
             specified here. The attributes here must match the SKU attribute
             names, by default None
             
         max_stack_size : int, optional
-            It throws an error if the amount of collaterals collected exceeds
+            It throws an BufferError if the amount of collaterals collected exceeds
             the stack size, by default None
             
         Returns
         -------
         list
             If skus_only = True, it returns a list with the skus. 
             Otherwise, it returns a list of dictionaries with the following
```

### Comparing `repleno-0.0.12/src/repleno/__init__.py` & `repleno-0.0.13/src/repleno/__init__.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.12/src/repleno/factory.py` & `repleno-0.0.13/src/repleno/factory.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.12/src/repleno/order.py` & `repleno-0.0.13/src/repleno/order.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.12/src/repleno/utils.py` & `repleno-0.0.13/src/repleno/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 def read_and_parse_csv(file, mandatory_mapping, optional_mapping={}) -> List[Dict]:
     # docu: mappings are key-value pairs where the key are the column that
     # should be in the output dictionary and the value is the key used to find
     # the data in the csv
 
     output = []
     try:
-        with open(file, newline="") as file:
+        with open(file, newline="", encoding="utf-8") as file:
             data = csv.DictReader(file)
 
             for row in data:
                 output.append(parse_dict(row, mandatory_mapping, optional_mapping))
 
     except FileNotFoundError:
         print("Error: File not found.")
@@ -188,15 +188,15 @@
 
     if not is_valid_csv(file_path):
         raise AttributeError("Path must have csv extension: ", file_path)
 
     fieldnames = dictionaries[0].keys()
 
     separator = "\t"
-    with open(file_path, "w", newline="") as file:
+    with open(file_path, "w", newline="", encoding="utf-8") as file:
         file.write(f"sep={separator}\n")
 
         writer = csv.DictWriter(file, delimiter=separator, fieldnames=fieldnames)
 
         writer.writeheader()
 
         for row in dictionaries:
```

### Comparing `repleno-0.0.12/src/repleno.egg-info/PKG-INFO` & `repleno-0.0.13/src/repleno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repleno
-Version: 0.0.12
+Version: 0.0.13
 Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
 Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
 Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Manufacturing
```

