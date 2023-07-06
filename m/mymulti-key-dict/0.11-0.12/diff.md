# Comparing `tmp/mymulti_key_dict-0.11.tar.gz` & `tmp/mymulti_key_dict-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mymulti_key_dict-0.11.tar", last modified: Thu Jul  6 02:43:28 2023, max compression
+gzip compressed data, was "mymulti_key_dict-0.12.tar", last modified: Thu Jul  6 17:03:23 2023, max compression
```

## Comparing `mymulti_key_dict-0.11.tar` & `mymulti_key_dict-0.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:43:28.728219 mymulti_key_dict-0.11/
--rw-rw-rw-   0        0        0     1148 2023-07-06 02:43:20.000000 mymulti_key_dict-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      119 2023-07-06 02:43:18.000000 mymulti_key_dict-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     4641 2023-07-06 02:43:28.728219 mymulti_key_dict-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 02:43:28.725228 mymulti_key_dict-0.11/mymulti_key_dict/
--rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.11/mymulti_key_dict/README.MD
--rw-rw-rw-   0        0        0     5962 2023-07-06 02:43:01.000000 mymulti_key_dict-0.11/mymulti_key_dict/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-06 02:43:24.000000 mymulti_key_dict-0.11/mymulti_key_dict/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 02:43:24.000000 mymulti_key_dict-0.11/mymulti_key_dict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-06 02:43:28.728219 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/
--rw-rw-rw-   0        0        0     4641 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-06 02:43:28.000000 mymulti_key_dict-0.11/mymulti_key_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-06 02:43:28.729217 mymulti_key_dict-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1325 2023-07-06 02:43:24.000000 mymulti_key_dict-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:03:23.309709 mymulti_key_dict-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-07-06 17:03:19.000000 mymulti_key_dict-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      119 2023-07-06 17:03:17.000000 mymulti_key_dict-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     4641 2023-07-06 17:03:23.309709 mymulti_key_dict-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 17:03:23.306718 mymulti_key_dict-0.12/mymulti_key_dict/
+-rw-rw-rw-   0        0        0     3952 2023-07-06 02:38:17.000000 mymulti_key_dict-0.12/mymulti_key_dict/README.MD
+-rw-rw-rw-   0        0        0     5890 2023-07-06 17:01:44.000000 mymulti_key_dict-0.12/mymulti_key_dict/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-06 17:03:22.000000 mymulti_key_dict-0.12/mymulti_key_dict/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 17:03:22.000000 mymulti_key_dict-0.12/mymulti_key_dict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-06 17:03:23.309709 mymulti_key_dict-0.12/mymulti_key_dict.egg-info/
+-rw-rw-rw-   0        0        0     4641 2023-07-06 17:03:23.000000 mymulti_key_dict-0.12/mymulti_key_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-07-06 17:03:23.000000 mymulti_key_dict-0.12/mymulti_key_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 17:03:23.000000 mymulti_key_dict-0.12/mymulti_key_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-06 17:03:23.000000 mymulti_key_dict-0.12/mymulti_key_dict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-06 17:03:23.311709 mymulti_key_dict-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-07-06 17:03:22.000000 mymulti_key_dict-0.12/setup.py
```

### Comparing `mymulti_key_dict-0.11/LICENSE.rst` & `mymulti_key_dict-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mymulti_key_dict-0.11/PKG-INFO` & `mymulti_key_dict-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymulti_key_dict
-Version: 0.11
+Version: 0.12
 Summary: Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements
 Home-page: https://github.com/hansalemaos/mymulti_key_dict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,dicts
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mymulti_key_dict-0.11/README.md` & `mymulti_key_dict-0.12/README.md`

 * *Files identical despite different names*

### Comparing `mymulti_key_dict-0.11/mymulti_key_dict/README.MD` & `mymulti_key_dict-0.12/mymulti_key_dict/README.MD`

 * *Files identical despite different names*

### Comparing `mymulti_key_dict-0.11/mymulti_key_dict/__init__.py` & `mymulti_key_dict-0.12/mymulti_key_dict/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,19 +80,16 @@
         clear(self):
             Clears all the elements from the nested dictionary.
 
         reversed(self):
             Returns a reversed iterator of the keys in the nested dictionary.
     """
 
-    def __init__(self, /, initialdata=None, **kwargs):
-        super().__init__(**kwargs)
-
-        if initialdata:
-            self.data.update(initialdata)
+    def __init__(self, dict=None, /, **kwargs):
+        super().__init__(dict,**kwargs)
         self.data = convert_to_default_dict(self.data)
 
     def __getitem__(self, key, /):
         if isinstance(key, list):
             v = self._get_from_original_iter(keys=key)
             if isinstance(v, defaultdict):
                 return convert_to_normal_dict_simple(v)
```

### Comparing `mymulti_key_dict-0.11/mymulti_key_dict.egg-info/PKG-INFO` & `mymulti_key_dict-0.12/mymulti_key_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymulti-key-dict
-Version: 0.11
+Version: 0.12
 Summary: Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements
 Home-page: https://github.com/hansalemaos/mymulti_key_dict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,dicts
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mymulti_key_dict-0.11/setup.py` & `mymulti_key_dict-0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements'''
 
 # Setting up
 setup(
     name="mymulti_key_dict",
     version=VERSION,
     license='MIT',
```

