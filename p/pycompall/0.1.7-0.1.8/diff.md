# Comparing `tmp/pycompall-0.1.7.tar.gz` & `tmp/pycompall-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.1.7.tar", last modified: Thu Jul  6 09:38:01 2023, max compression
+gzip compressed data, was "pycompall-0.1.8.tar", last modified: Thu Jul  6 09:39:33 2023, max compression
```

## Comparing `pycompall-0.1.7.tar` & `pycompall-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:38:01.112957 pycompall-0.1.7/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.7/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.7/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:38:01.112957 pycompall-0.1.7/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.7/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:38:01.108957 pycompall-0.1.7/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.7/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.7/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4799 2023-07-06 09:37:52.000000 pycompall-0.1.7/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:38:01.112957 pycompall-0.1.7/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:38:01.000000 pycompall-0.1.7/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 09:38:01.000000 pycompall-0.1.7/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 09:38:01.000000 pycompall-0.1.7/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 09:38:01.000000 pycompall-0.1.7/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 09:38:01.000000 pycompall-0.1.7/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 09:38:01.000000 pycompall-0.1.7/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.7/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 09:38:01.112957 pycompall-0.1.7/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 09:37:58.000000 pycompall-0.1.7/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:38:01.112957 pycompall-0.1.7/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 09:22:05.000000 pycompall-0.1.7/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.332432 pycompall-0.1.8/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.8/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.8/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:39:33.328432 pycompall-0.1.8/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.8/README.md
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.328432 pycompall-0.1.8/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.8/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.8/app/__main__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4832 2023-07-06 09:39:26.000000 pycompall-0.1.8/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.328432 pycompall-0.1.8/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 09:39:33.000000 pycompall-0.1.8/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.8/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 09:39:33.332432 pycompall-0.1.8/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 09:39:32.000000 pycompall-0.1.8/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:39:33.328432 pycompall-0.1.8/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 09:22:05.000000 pycompall-0.1.8/test/test_compile.py
```

### Comparing `pycompall-0.1.7/app/application.py` & `pycompall-0.1.8/app/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from typing import Optional, Tuple
 
 import click
 
 
 def compile_command(path: Path, recursive: bool = False, in_place: bool = False, create_empty_init: bool = False, exclude_patterns: Tuple[str] = tuple()):
+    click.echo(exclude_patterns)
     if patterns_match_path(exclude_patterns, path):
         click.echo(f'Skipping file \'{path}\'')
         return
 
     if (create_empty_init and not path.is_dir()):
         raise ValueError(
             f'--create-empty-init flag can only be used when path supplied is a directory, but got {path}.')
```

### Comparing `pycompall-0.1.7/pycompall.py` & `pycompall-0.1.8/pycompall.py`

 * *Files identical despite different names*

### Comparing `pycompall-0.1.7/setup.py` & `pycompall-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='pycompall',
-    version='0.1.7',
+    version='0.1.8',
     author='Kim Yongbeom',
     author_email='yongbeom.kim@u.nus.edu',
     license='<the license you chose>',
     description='Wrapper around the python compileall utility.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Yongbeom-Kim/py-compiler',
```

### Comparing `pycompall-0.1.7/test/test_compile.py` & `pycompall-0.1.8/test/test_compile.py`

 * *Files identical despite different names*

