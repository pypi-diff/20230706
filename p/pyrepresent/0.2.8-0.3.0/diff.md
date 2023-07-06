# Comparing `tmp/pyrepresent-0.2.8.tar.gz` & `tmp/pyrepresent-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.2.8.tar", last modified: Mon Jul  3 16:05:04 2023, max compression
+gzip compressed data, was "pyrepresent-0.3.0.tar", last modified: Thu Jul  6 13:38:55 2023, max compression
```

## Comparing `pyrepresent-0.2.8.tar` & `pyrepresent-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 16:05:04.342604 pyrepresent-0.2.8/
--rw-rw-rw-   0        0        0      115 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2548 2023-07-03 16:05:04.342604 pyrepresent-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.8/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.8/build.py
--rw-rw-rw-   0        0        0      715 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-03 16:05:04.337603 pyrepresent-0.2.8/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     2548 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 16:05:04.000000 pyrepresent-0.2.8/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 16:05:04.341574 pyrepresent-0.2.8/represent/
--rw-rw-rw-   0        0        0      116 2023-07-03 14:00:08.000000 pyrepresent-0.2.8/represent/__init__.py
--rw-rw-rw-   0        0        0     9089 2023-07-03 16:01:42.000000 pyrepresent-0.2.8/represent/colors.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.8/represent/indentation.py
--rw-rw-rw-   0        0        0    17405 2023-07-03 16:02:23.000000 pyrepresent-0.2.8/represent/object.py
--rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.8/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.8/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 16:05:04.342604 pyrepresent-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-03 16:02:40.000000 pyrepresent-0.2.8/setup.py
--rw-rw-rw-   0        0        0     1363 2023-07-03 13:34:56.000000 pyrepresent-0.2.8/test.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:38:55.648549 pyrepresent-0.3.0/
+-rw-rw-rw-   0        0        0      115 2023-07-06 13:38:55.000000 pyrepresent-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-06 13:38:55.647239 pyrepresent-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.3.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.3.0/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-06 13:38:55.000000 pyrepresent-0.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-06 13:38:55.642033 pyrepresent-0.3.0/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-06 13:38:55.000000 pyrepresent-0.3.0/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-06 13:38:55.000000 pyrepresent-0.3.0/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:38:55.000000 pyrepresent-0.3.0/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-06 13:38:55.000000 pyrepresent-0.3.0/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 13:38:55.000000 pyrepresent-0.3.0/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 13:38:55.647239 pyrepresent-0.3.0/represent/
+-rw-rw-rw-   0        0        0      116 2023-07-03 14:00:08.000000 pyrepresent-0.3.0/represent/__init__.py
+-rw-rw-rw-   0        0        0     9089 2023-07-03 16:01:42.000000 pyrepresent-0.3.0/represent/colors.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.3.0/represent/indentation.py
+-rw-rw-rw-   0        0        0    17393 2023-07-06 13:38:21.000000 pyrepresent-0.3.0/represent/object.py
+-rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.3.0/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.3.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:38:55.648549 pyrepresent-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-06 13:38:47.000000 pyrepresent-0.3.0/setup.py
+-rw-rw-rw-   0        0        0     1363 2023-07-06 13:38:31.000000 pyrepresent-0.3.0/test.py
```

### Comparing `pyrepresent-0.2.8/PKG-INFO` & `pyrepresent-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.8
+Version: 0.3.0
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.8/README.md` & `pyrepresent-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.8/build.py` & `pyrepresent-0.3.0/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.8/pyproject.toml` & `pyrepresent-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.2.8'
+version = '0.3.0'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.2.8/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.3.0/pyrepresent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.8
+Version: 0.3.0
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.8/represent/colors.py` & `pyrepresent-0.3.0/represent/colors.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.8/represent/indentation.py` & `pyrepresent-0.3.0/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.8/represent/object.py` & `pyrepresent-0.3.0/represent/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     :param excluded: The excluded values.
     :param defined: The value to show only defined valid_values.
 
     :return: The validation value.
     """
 
     try:
-        if isinstance(value, int):
+        if value == 0:
             bool_value = True
 
         else:
             bool_value = bool(value)
         # end try
 
     except ValueError:
```

### Comparing `pyrepresent-0.2.8/represent/structures.py` & `pyrepresent-0.3.0/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.8/setup.py` & `pyrepresent-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.2.8',
+        version='0.3.0',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.2.8/test.py` & `pyrepresent-0.3.0/test.py`

 * *Files identical despite different names*

