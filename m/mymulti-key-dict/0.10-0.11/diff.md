# Comparing `tmp/mymulti_key_dict-0.10.tar.gz` & `tmp/mymulti_key_dict-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mymulti_key_dict-0.10.tar", last modified: Thu Jul  6 02:39:03 2023, max compression
+gzip compressed data, was "mymulti_key_dict-0.11.tar", last modified: Thu Jul  6 02:43:28 2023, max compression
```

## Comparing `mymulti_key_dict-0.10.tar` & `mymulti_key_dict-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:39:03.440390 mymulti_key_dict-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-06 02:38:57.000000 mymulti_key_dict-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      119 2023-07-06 02:38:49.000000 mymulti_key_dict-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4641 2023-07-06 02:39:03.440390 mymulti_key_dict-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 02:39:03.436403 mymulti_key_dict-0.10/mymulti_key_dict/
--rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.10/mymulti_key_dict/README.MD
--rw-rw-rw-   0        0        0     5972 2023-07-06 02:24:44.000000 mymulti_key_dict-0.10/mymulti_key_dict/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-06 02:39:02.000000 mymulti_key_dict-0.10/mymulti_key_dict/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 02:39:02.000000 mymulti_key_dict-0.10/mymulti_key_dict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-06 02:39:03.439393 mymulti_key_dict-0.10/mymulti_key_dict.egg-info/
--rw-rw-rw-   0        0        0     4641 2023-07-06 02:39:03.000000 mymulti_key_dict-0.10/mymulti_key_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-07-06 02:39:03.000000 mymulti_key_dict-0.10/mymulti_key_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 02:39:03.000000 mymulti_key_dict-0.10/mymulti_key_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-06 02:39:03.000000 mymulti_key_dict-0.10/mymulti_key_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-06 02:39:03.441388 mymulti_key_dict-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1325 2023-07-06 02:39:02.000000 mymulti_key_dict-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:43:28.728219 mymulti_key_dict-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-06 02:43:20.000000 mymulti_key_dict-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      119 2023-07-06 02:43:18.000000 mymulti_key_dict-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4641 2023-07-06 02:43:28.728219 mymulti_key_dict-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 02:43:28.725228 mymulti_key_dict-0.11/mymulti_key_dict/
+-rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.11/mymulti_key_dict/README.MD
+-rw-rw-rw-   0        0        0     5962 2023-07-06 02:43:01.000000 mymulti_key_dict-0.11/mymulti_key_dict/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-06 02:43:24.000000 mymulti_key_dict-0.11/mymulti_key_dict/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 02:43:24.000000 mymulti_key_dict-0.11/mymulti_key_dict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-06 02:43:28.728219 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/
+-rw-rw-rw-   0        0        0     4641 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-06 02:43:28.729217 mymulti_key_dict-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-07-06 02:43:24.000000 mymulti_key_dict-0.11/setup.py
```

### Comparing `mymulti_key_dict-0.10/LICENSE.rst` & `mymulti_key_dict-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mymulti_key_dict-0.10/PKG-INFO` & `mymulti_key_dict-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymulti_key_dict
-Version: 0.10
+Version: 0.11
 Summary: Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements
 Home-page: https://github.com/hansalemaos/mymulti_key_dict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,dicts
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mymulti_key_dict-0.10/README.md` & `mymulti_key_dict-0.11/README.md`

 * *Files identical despite different names*

### Comparing `mymulti_key_dict-0.10/mymulti_key_dict/README.MD` & `mymulti_key_dict-0.11/mymulti_key_dict/README.MD`

 * *Files identical despite different names*

### Comparing `mymulti_key_dict-0.10/mymulti_key_dict/__init__.py` & `mymulti_key_dict-0.11/mymulti_key_dict/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     def setdefault(self, key, default=None):
         raise TypeError("setdefault not allowed!")
 
     def to_dict(self):
         return convert_to_normal_dict_simple(self.data)
 
     def copy(self):
-        return deepcopy(MultiKeyDict(deepcopy(self.data)))
+        return MultiKeyDict(deepcopy(self.data))
 
     def items(self):
         return self.to_dict().items()
 
     def keys(self):
         return self.to_dict().keys()
```

### Comparing `mymulti_key_dict-0.10/mymulti_key_dict.egg-info/PKG-INFO` & `mymulti_key_dict-0.11/mymulti_key_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymulti-key-dict
-Version: 0.10
+Version: 0.11
 Summary: Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements
 Home-page: https://github.com/hansalemaos/mymulti_key_dict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,dicts
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mymulti_key_dict-0.10/setup.py` & `mymulti_key_dict-0.11/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements'''
 
 # Setting up
 setup(
     name="mymulti_key_dict",
     version=VERSION,
     license='MIT',
```

