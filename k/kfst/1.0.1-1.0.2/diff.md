# Comparing `tmp/kfst-1.0.1.tar.gz` & `tmp/kfst-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfst-1.0.1.tar", last modified: Wed Jul  5 23:43:04 2023, max compression
+gzip compressed data, was "kfst-1.0.2.tar", last modified: Wed Jul  5 23:46:04 2023, max compression
```

## Comparing `kfst-1.0.1.tar` & `kfst-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:43:04.613324 kfst-1.0.1/
--rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.0.1/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     1853 2023-07-05 23:43:04.613363 kfst-1.0.1/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1221 2023-07-05 12:46:53.000000 kfst-1.0.1/README.md
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:43:04.612730 kfst-1.0.1/kfst/
--rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.0.1/kfst/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)    11326 2023-07-05 22:38:54.000000 kfst-1.0.1/kfst/transducer.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:43:04.613244 kfst-1.0.1/kfst.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     1853 2023-07-05 23:43:04.000000 kfst-1.0.1/kfst.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)      217 2023-07-05 23:43:04.000000 kfst-1.0.1/kfst.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-05 23:43:04.000000 kfst-1.0.1/kfst.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-05 23:43:04.000000 kfst-1.0.1/kfst.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-05 23:43:04.000000 kfst-1.0.1/kfst.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.0.1/pyproject.toml
--rw-r--r--   0 iikka      (501) staff       (20)      756 2023-07-05 23:43:04.613553 kfst-1.0.1/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:46:04.701924 kfst-1.0.2/
+-rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.0.2/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     1853 2023-07-05 23:46:04.701962 kfst-1.0.2/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1221 2023-07-05 12:46:53.000000 kfst-1.0.2/README.md
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:46:04.701309 kfst-1.0.2/kfst/
+-rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.0.2/kfst/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)    11303 2023-07-05 23:44:27.000000 kfst-1.0.2/kfst/transducer.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-05 23:46:04.701841 kfst-1.0.2/kfst.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     1853 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)      217 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-05 23:46:04.000000 kfst-1.0.2/kfst.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.0.2/pyproject.toml
+-rw-r--r--   0 iikka      (501) staff       (20)      756 2023-07-05 23:46:04.702140 kfst-1.0.2/setup.cfg
```

### Comparing `kfst-1.0.1/LICENSE` & `kfst-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kfst-1.0.1/PKG-INFO` & `kfst-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.0.1
+Version: 1.0.2
 Summary: A pure-python finite state transducer library with support for AT&T files and flag diacritics
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `kfst-1.0.1/README.md` & `kfst-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kfst-1.0.1/kfst/__init__.py` & `kfst-1.0.2/kfst/__init__.py`

 * *Files identical despite different names*

### Comparing `kfst-1.0.1/kfst/transducer.py` & `kfst-1.0.2/kfst/transducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,13 +304,13 @@
     while True:
         try:
             text = input("> ")
 
         except EOFError:
             break
 
-        for os, w in fst.lookup(fst.split_to_symbols(text)):
-            print("".join(os), w)
+        for output, w in fst.lookup(text):
+            print(output, w)
 
 if __name__ == "__main__":
     main()
```

### Comparing `kfst-1.0.1/kfst.egg-info/PKG-INFO` & `kfst-1.0.2/kfst.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.0.1
+Version: 1.0.2
 Summary: A pure-python finite state transducer library with support for AT&T files and flag diacritics
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `kfst-1.0.1/setup.cfg` & `kfst-1.0.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kfst
-version = 1.0.1
+version = 1.0.2
 author = Iikka Hauhio
 author_email = iikka.hauhio@helsinki.fi
 description = A pure-python finite state transducer library with support for AT&T files and flag diacritics
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv3 or later
 license_files =
```

