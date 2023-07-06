# Comparing `tmp/pycompall-0.1.1.tar.gz` & `tmp/pycompall-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.1.1.tar", last modified: Thu Jul  6 07:01:55 2023, max compression
+gzip compressed data, was "pycompall-0.1.2.tar", last modified: Thu Jul  6 09:18:40 2023, max compression
```

## Comparing `pycompall-0.1.1.tar` & `pycompall-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.450188 pycompall-0.1.1/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.1/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.1/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 07:01:55.446188 pycompall-0.1.1/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.1/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.446188 pycompall-0.1.1/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.1/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.1/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4565 2023-07-06 07:01:08.000000 pycompall-0.1.1/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.446188 pycompall-0.1.1/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.1/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 07:01:55.450188 pycompall-0.1.1/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 07:01:46.000000 pycompall-0.1.1/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.446188 pycompall-0.1.1/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 06:59:58.000000 pycompall-0.1.1/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:18:40.004392 pycompall-0.1.2/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.2/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.2/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:18:40.004392 pycompall-0.1.2/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.2/README.md
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:18:40.000392 pycompall-0.1.2/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.2/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.2/app/__main__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4582 2023-07-06 09:18:27.000000 pycompall-0.1.2/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:18:40.004392 pycompall-0.1.2/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:18:39.000000 pycompall-0.1.2/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 09:18:39.000000 pycompall-0.1.2/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 09:18:39.000000 pycompall-0.1.2/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 09:18:39.000000 pycompall-0.1.2/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 09:18:39.000000 pycompall-0.1.2/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 09:18:39.000000 pycompall-0.1.2/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.2/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 09:18:40.004392 pycompall-0.1.2/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 09:18:38.000000 pycompall-0.1.2/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:18:40.004392 pycompall-0.1.2/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 06:59:58.000000 pycompall-0.1.2/test/test_compile.py
```

### Comparing `pycompall-0.1.1/app/application.py` & `pycompall-0.1.2/app/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import click
 
 
 def compile_command(path: Path, recursive: bool = False, in_place: bool = False, create_empty_init: bool = False, exclude_patterns: Tuple[str] = tuple()):
     if (create_empty_init and not path.is_dir()):
         raise ValueError(
-            '--create-empty-init flag can only be used when path supplied is a directory.')
+            f'--create-empty-init flag can only be used when path supplied is a directory, but got {path}.')
 
     path = Path(path)
     _clear_pycache_dir(path, missing_ok=True)
     compileall(path, recursive, exclude_patterns=exclude_patterns)
 
     if (in_place):
         replace_py_with_pyc(path, recursive, exclude_patterns=exclude_patterns)
```

### Comparing `pycompall-0.1.1/pycompall.py` & `pycompall-0.1.2/pycompall.py`

 * *Files identical despite different names*

### Comparing `pycompall-0.1.1/setup.py` & `pycompall-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='pycompall',
-    version='0.1.1',
+    version='0.1.2',
     author='Kim Yongbeom',
     author_email='yongbeom.kim@u.nus.edu',
     license='<the license you chose>',
     description='Wrapper around the python compileall utility.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Yongbeom-Kim/py-compiler',
```

### Comparing `pycompall-0.1.1/test/test_compile.py` & `pycompall-0.1.2/test/test_compile.py`

 * *Files identical despite different names*

