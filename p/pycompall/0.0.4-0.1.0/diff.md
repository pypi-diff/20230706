# Comparing `tmp/pycompall-0.0.4.tar.gz` & `tmp/pycompall-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.0.4.tar", last modified: Thu Jul  6 06:13:51 2023, max compression
+gzip compressed data, was "pycompall-0.1.0.tar", last modified: Thu Jul  6 06:20:34 2023, max compression
```

## Comparing `pycompall-0.0.4.tar` & `pycompall-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.117416 pycompall-0.0.4/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.0.4/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.0.4/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:13:51.117416 pycompall-0.0.4/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.0.4/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.113416 pycompall-0.0.4/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.0.4/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.0.4/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     3672 2023-07-06 06:12:57.000000 pycompall-0.0.4/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.117416 pycompall-0.0.4/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      849 2023-07-06 05:48:15.000000 pycompall-0.0.4/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 06:13:51.117416 pycompall-0.0.4/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 06:13:35.000000 pycompall-0.0.4/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.117416 pycompall-0.0.4/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     5985 2023-07-06 06:12:00.000000 pycompall-0.0.4/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.0/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.0/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:20:34.822658 pycompall-0.1.0/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.0/README.md
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.0/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.0/app/__main__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     3627 2023-07-06 06:19:39.000000 pycompall-0.1.0/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      874 2023-07-06 06:19:34.000000 pycompall-0.1.0/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 06:20:34.822658 pycompall-0.1.0/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 06:20:25.000000 pycompall-0.1.0/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     5985 2023-07-06 06:12:00.000000 pycompall-0.1.0/test/test_compile.py
```

### Comparing `pycompall-0.0.4/app/application.py` & `pycompall-0.1.0/app/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from pathlib import Path
 from typing import Optional
 
 import click
 
 
 def compile_command(path: Path, recursive: bool = True, in_place: bool = False, create_empty_init: bool = False):
-    click.echo(click.format_filename(path))
-
     if (create_empty_init and not path.is_dir()):
         raise ValueError(
             '--create-empty-init flag can only be used when path supplied is a directory.')
 
     path = Path(path)
     _clear_pycache_dir(path, missing_ok=True)
     compileall(path, recursive)
```

### Comparing `pycompall-0.0.4/pycompall.py` & `pycompall-0.1.0/pycompall.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     pass
 
 
 @cli.command()
 @click.option('-recursive', '-r', is_flag=True, default=True, help='Recurse through subdirectories.')
 @click.option('--in-place', is_flag=True, default=False, help='Remove .py and replace them with compiled .pyc files.')
 @click.option('--create-empty-init', is_flag=True, default=False, help='Create an empty __init__.py file in the path specified after compilation. Useful for interacting with tools such as colcon.')
-@click.argument('path', type=click.Path(exists=True))
-def compile(path, recursive, in_place, create_empty_init):
-    click.echo(create_empty_init)
-    compile_command(
-        Path(path),
-        recursive=recursive,
-        in_place=in_place,
-        create_empty_init=create_empty_init
-    )
+@click.argument('paths', type=click.Path(exists=True), nargs=-1)
+def compile(paths, recursive, in_place, create_empty_init):
+    for path in paths:
+        compile_command(
+            Path(path),
+            recursive=recursive,
+            in_place=in_place,
+            create_empty_init=create_empty_init
+        )
```

### Comparing `pycompall-0.0.4/setup.py` & `pycompall-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='pycompall',
-    version='0.0.4',
+    version='0.1.0',
     author='Kim Yongbeom',
     author_email='yongbeom.kim@u.nus.edu',
     license='<the license you chose>',
     description='Wrapper around the python compileall utility.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Yongbeom-Kim/py-compiler',
```

### Comparing `pycompall-0.0.4/test/test_compile.py` & `pycompall-0.1.0/test/test_compile.py`

 * *Files identical despite different names*

