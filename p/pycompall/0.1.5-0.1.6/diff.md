# Comparing `tmp/pycompall-0.1.5.tar.gz` & `tmp/pycompall-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.1.5.tar", last modified: Thu Jul  6 09:28:07 2023, max compression
+gzip compressed data, was "pycompall-0.1.6.tar", last modified: Thu Jul  6 09:29:16 2023, max compression
```

## Comparing `pycompall-0.1.5.tar` & `pycompall-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:28:07.183791 pycompall-0.1.5/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.5/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.5/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:28:07.183791 pycompall-0.1.5/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.5/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:28:07.183791 pycompall-0.1.5/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.5/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.5/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4904 2023-07-06 09:27:49.000000 pycompall-0.1.5/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:28:07.183791 pycompall-0.1.5/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:28:07.000000 pycompall-0.1.5/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 09:28:07.000000 pycompall-0.1.5/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 09:28:07.000000 pycompall-0.1.5/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 09:28:07.000000 pycompall-0.1.5/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 09:28:07.000000 pycompall-0.1.5/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 09:28:07.000000 pycompall-0.1.5/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.5/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 09:28:07.183791 pycompall-0.1.5/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 09:27:55.000000 pycompall-0.1.5/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:28:07.183791 pycompall-0.1.5/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 09:22:05.000000 pycompall-0.1.5/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:29:16.739531 pycompall-0.1.6/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.6/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.6/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:29:16.739531 pycompall-0.1.6/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.6/README.md
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:29:16.739531 pycompall-0.1.6/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.6/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.6/app/__main__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4790 2023-07-06 09:29:10.000000 pycompall-0.1.6/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:29:16.739531 pycompall-0.1.6/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 09:29:16.000000 pycompall-0.1.6/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 09:29:16.000000 pycompall-0.1.6/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 09:29:16.000000 pycompall-0.1.6/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 09:29:16.000000 pycompall-0.1.6/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 09:29:16.000000 pycompall-0.1.6/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 09:29:16.000000 pycompall-0.1.6/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.6/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 09:29:16.739531 pycompall-0.1.6/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 09:29:15.000000 pycompall-0.1.6/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 09:29:16.739531 pycompall-0.1.6/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 09:22:05.000000 pycompall-0.1.6/test/test_compile.py
```

### Comparing `pycompall-0.1.5/app/application.py` & `pycompall-0.1.6/app/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 from pathlib import Path
 from typing import Optional, Tuple
 
 import click
 
 
 def compile_command(path: Path, recursive: bool = False, in_place: bool = False, create_empty_init: bool = False, exclude_patterns: Tuple[str] = tuple()):
-    click.echo(exclude_patterns)
-    click.echo(path)
-    click.echo(patterns_match_path(exclude_patterns, path))
     if patterns_match_path(exclude_patterns, path):
         click.echo(f'Skipping file \'{path}\'')
         return
 
     if (create_empty_init and not path.is_dir()):
         raise ValueError(
             f'--create-empty-init flag can only be used when path supplied is a directory, but got {path}.')
```

### Comparing `pycompall-0.1.5/pycompall.py` & `pycompall-0.1.6/pycompall.py`

 * *Files identical despite different names*

### Comparing `pycompall-0.1.5/setup.py` & `pycompall-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='pycompall',
-    version='0.1.5',
+    version='0.1.6',
     author='Kim Yongbeom',
     author_email='yongbeom.kim@u.nus.edu',
     license='<the license you chose>',
     description='Wrapper around the python compileall utility.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Yongbeom-Kim/py-compiler',
```

### Comparing `pycompall-0.1.5/test/test_compile.py` & `pycompall-0.1.6/test/test_compile.py`

 * *Files identical despite different names*

