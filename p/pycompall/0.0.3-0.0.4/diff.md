# Comparing `tmp/pycompall-0.0.3.tar.gz` & `tmp/pycompall-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.0.3.tar", last modified: Thu Jul  6 06:03:57 2023, max compression
+gzip compressed data, was "pycompall-0.0.4.tar", last modified: Thu Jul  6 06:13:51 2023, max compression
```

## Comparing `pycompall-0.0.3.tar` & `pycompall-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:03:57.529137 pycompall-0.0.3/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.0.3/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.0.3/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:03:57.529137 pycompall-0.0.3/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.0.3/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:03:57.529137 pycompall-0.0.3/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.0.3/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.0.3/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     3642 2023-07-06 05:40:34.000000 pycompall-0.0.3/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:03:57.529137 pycompall-0.0.3/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:03:57.000000 pycompall-0.0.3/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      340 2023-07-06 06:03:57.000000 pycompall-0.0.3/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 06:03:57.000000 pycompall-0.0.3/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 06:03:57.000000 pycompall-0.0.3/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 06:03:57.000000 pycompall-0.0.3/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       19 2023-07-06 06:03:57.000000 pycompall-0.0.3/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      849 2023-07-06 05:48:15.000000 pycompall-0.0.3/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 06:03:57.529137 pycompall-0.0.3/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 06:03:53.000000 pycompall-0.0.3/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:03:57.529137 pycompall-0.0.3/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:43:46.000000 pycompall-0.0.3/test/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     5985 2023-07-06 05:43:50.000000 pycompall-0.0.3/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.117416 pycompall-0.0.4/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.0.4/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.0.4/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:13:51.117416 pycompall-0.0.4/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.0.4/README.md
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.113416 pycompall-0.0.4/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.0.4/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.0.4/app/__main__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     3672 2023-07-06 06:12:57.000000 pycompall-0.0.4/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.117416 pycompall-0.0.4/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 06:13:51.000000 pycompall-0.0.4/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      849 2023-07-06 05:48:15.000000 pycompall-0.0.4/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 06:13:51.117416 pycompall-0.0.4/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 06:13:35.000000 pycompall-0.0.4/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:13:51.117416 pycompall-0.0.4/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     5985 2023-07-06 06:12:00.000000 pycompall-0.0.4/test/test_compile.py
```

### Comparing `pycompall-0.0.3/app/application.py` & `pycompall-0.0.4/app/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from compileall import compile_dir, compile_file
 from pathlib import Path
+from typing import Optional
 
 import click
 
 
 def compile_command(path: Path, recursive: bool = True, in_place: bool = False, create_empty_init: bool = False):
     click.echo(click.format_filename(path))
 
@@ -44,15 +45,15 @@
 
     if (path.is_dir()):
         _replace_py_with_pyc_dir(path, is_recursive)
     elif (path.is_file()):
         assert (path.suffix == '.py')
         _replace_py_with_pyc_file(path)
 
-    _clear_pycache_dir(path, missing_ok=False)
+    _clear_pycache_dir(path, missing_ok=True)
 
 
 def _replace_py_with_pyc_dir(path: Path, is_recursive: bool):
     for child in path.iterdir():
         if (child.is_dir() and is_recursive):
             _replace_py_with_pyc_dir(child, is_recursive)
             continue
@@ -69,15 +70,15 @@
     if (compiled_file is None):
         raise FileNotFoundError(
             f'.pyc file does not exist for the file {python_file_path.as_posix()}')
     python_file_path.unlink()
     compiled_file.rename(python_file_path.with_suffix('.pyc'))
 
 
-def _get_pycache_pyc_from_py(python_file_path: Path) -> Path | None:
+def _get_pycache_pyc_from_py(python_file_path: Path) -> Optional[Path]:
     """For a given .py file, get its corresponding .pyc file path in the __pycache__ directory."""
     assert (python_file_path.is_file() and python_file_path.suffix == '.py')
     pycache_dir = python_file_path.parent / '__pycache__'
     query = list(pycache_dir.glob(python_file_path.stem + '.cpython-*.pyc'))
     if (len(query) == 0):
         return None
     assert (len(query) == 1)
@@ -90,15 +91,15 @@
     """For a given directory, create an empty __init__.py file and return the resulting file as a Path object."""
     assert dir.is_dir()
     file = (dir / '__init__.py')
     file.touch()
     return file
 
 
-def _clear_pycache_dir(path: Path, missing_ok: bool) -> Path:
+def _clear_pycache_dir(path: Path, missing_ok: bool) -> None:
     """Given a directory or file, delete the __pycache__ folder."""
     if (path.is_file()):
         path = path.parent
 
     rmtree(path / '__pycache__', missing_ok=missing_ok)
```

### Comparing `pycompall-0.0.3/pycompall.py` & `pycompall-0.0.4/pycompall.py`

 * *Files identical despite different names*

### Comparing `pycompall-0.0.3/setup.py` & `pycompall-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='pycompall',
-    version='0.0.3',
+    version='0.0.4',
     author='Kim Yongbeom',
     author_email='yongbeom.kim@u.nus.edu',
     license='<the license you chose>',
     description='Wrapper around the python compileall utility.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Yongbeom-Kim/py-compiler',
```

### Comparing `pycompall-0.0.3/test/test_compile.py` & `pycompall-0.0.4/test/test_compile.py`

 * *Files identical despite different names*

