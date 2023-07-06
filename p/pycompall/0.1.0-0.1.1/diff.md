# Comparing `tmp/pycompall-0.1.0.tar.gz` & `tmp/pycompall-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.1.0.tar", last modified: Thu Jul  6 06:20:34 2023, max compression
+gzip compressed data, was "pycompall-0.1.1.tar", last modified: Thu Jul  6 07:01:55 2023, max compression
```

## Comparing `pycompall-0.1.0.tar` & `pycompall-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.0/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.0/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:20:34.822658 pycompall-0.1.0/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.0/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.0/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.0/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     3627 2023-07-06 06:19:39.000000 pycompall-0.1.0/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 06:20:34.000000 pycompall-0.1.0/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      874 2023-07-06 06:19:34.000000 pycompall-0.1.0/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 06:20:34.822658 pycompall-0.1.0/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 06:20:25.000000 pycompall-0.1.0/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 06:20:34.822658 pycompall-0.1.0/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     5985 2023-07-06 06:12:00.000000 pycompall-0.1.0/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.450188 pycompall-0.1.1/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.1/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.1/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 07:01:55.446188 pycompall-0.1.1/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.1/README.md
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.446188 pycompall-0.1.1/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.1/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.1/app/__main__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     4565 2023-07-06 07:01:08.000000 pycompall-0.1.1/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.446188 pycompall-0.1.1/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-06 07:01:55.000000 pycompall-0.1.1/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1073 2023-07-06 06:57:49.000000 pycompall-0.1.1/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-06 07:01:55.450188 pycompall-0.1.1/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-06 07:01:46.000000 pycompall-0.1.1/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 07:01:55.446188 pycompall-0.1.1/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     7083 2023-07-06 06:59:58.000000 pycompall-0.1.1/test/test_compile.py
```

### Comparing `pycompall-0.1.0/app/application.py` & `pycompall-0.1.1/app/application.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,90 @@
-from compileall import compile_dir, compile_file
+from compileall import compile_file
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Tuple
 
 import click
 
 
-def compile_command(path: Path, recursive: bool = True, in_place: bool = False, create_empty_init: bool = False):
+def compile_command(path: Path, recursive: bool = False, in_place: bool = False, create_empty_init: bool = False, exclude_patterns: Tuple[str] = tuple()):
     if (create_empty_init and not path.is_dir()):
         raise ValueError(
             '--create-empty-init flag can only be used when path supplied is a directory.')
 
     path = Path(path)
     _clear_pycache_dir(path, missing_ok=True)
-    compileall(path, recursive)
+    compileall(path, recursive, exclude_patterns=exclude_patterns)
 
     if (in_place):
-        replace_py_with_pyc(path, recursive)
+        replace_py_with_pyc(path, recursive, exclude_patterns=exclude_patterns)
 
     if (create_empty_init):
         _create_init_file(dir=path)
 
 
-def compileall(path: Path, is_recursive: bool):
+def compileall(path: Path, is_recursive: bool, exclude_patterns: Tuple[str]):
     """
     Simple wrapper around python compileall package to compile .py to .pyc files.
 
     Note that created .pyc files are under the __pycache__ directory.
     """
     assert (path.exists())
-
     if (path.is_dir()):
-        max_recursion_levels = None if is_recursive else 0
-        compile_dir(path, maxlevels=max_recursion_levels)
-    elif (path.is_file()):
-        assert (path.suffix == '.py')
+        if (not is_recursive):
+            for file in path.glob('*.py'):
+                compileall(file, is_recursive=is_recursive,
+                           exclude_patterns=exclude_patterns)
+            return
+
+        for file in path.iterdir():
+            compileall(file, is_recursive=is_recursive,
+                       exclude_patterns=exclude_patterns)
+
+    elif (path.is_file() and path.suffix == '.py'):
+        for pattern in exclude_patterns:
+            if (path.match(pattern)):
+                click.echo(f'Skipping file \'{path}\'')
+                return
+        click.echo(f'Compiling file \'{path}\'')
         compile_file(path)
 
 
-def replace_py_with_pyc(path: Path, is_recursive: bool):
+def replace_py_with_pyc(path: Path, is_recursive: bool, exclude_patterns: Tuple[str]):
     """Replace .py with .pyc files """
     assert (path.exists())
 
     if (path.is_dir()):
-        _replace_py_with_pyc_dir(path, is_recursive)
+        _replace_py_with_pyc_dir(
+            path, is_recursive, exclude_patterns=exclude_patterns)
     elif (path.is_file()):
         assert (path.suffix == '.py')
-        _replace_py_with_pyc_file(path)
+        _replace_py_with_pyc_file(path, exclude_patterns=exclude_patterns)
 
     _clear_pycache_dir(path, missing_ok=True)
 
 
-def _replace_py_with_pyc_dir(path: Path, is_recursive: bool):
+def _replace_py_with_pyc_dir(path: Path, is_recursive: bool, exclude_patterns: Tuple[str]):
     for child in path.iterdir():
         if (child.is_dir() and is_recursive):
-            _replace_py_with_pyc_dir(child, is_recursive)
+            _replace_py_with_pyc_dir(
+                child, is_recursive, exclude_patterns=exclude_patterns)
             continue
 
         if (child.is_file() and child.suffix == '.py'):
-            _replace_py_with_pyc_file(child)
+            _replace_py_with_pyc_file(child, exclude_patterns=exclude_patterns)
             continue
 
 
-def _replace_py_with_pyc_file(python_file_path: Path):
+def _replace_py_with_pyc_file(python_file_path: Path, exclude_patterns: Tuple[str]):
     """Replace a .py file with its corresponding .pyc file in the __pycache__ directory."""
     assert (python_file_path.is_file() and python_file_path.suffix == '.py')
+    for pattern in exclude_patterns:
+        if python_file_path.match(pattern):
+            return
+
     compiled_file = _get_pycache_pyc_from_py(python_file_path)
     if (compiled_file is None):
         raise FileNotFoundError(
             f'.pyc file does not exist for the file {python_file_path.as_posix()}')
     python_file_path.unlink()
     compiled_file.rename(python_file_path.with_suffix('.pyc'))
 
@@ -99,15 +116,14 @@
         path = path.parent
 
     rmtree(path / '__pycache__', missing_ok=missing_ok)
 
 
 # UTILITY
 
-
 def rmtree(root: Path, missing_ok: bool):
     if (missing_ok and not root.exists()):
         return
     for p in root.iterdir():
         if p.is_dir():
             rmtree(p, missing_ok=missing_ok)
         else:
```

### Comparing `pycompall-0.1.0/setup.py` & `pycompall-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='pycompall',
-    version='0.1.0',
+    version='0.1.1',
     author='Kim Yongbeom',
     author_email='yongbeom.kim@u.nus.edu',
     license='<the license you chose>',
     description='Wrapper around the python compileall utility.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Yongbeom-Kim/py-compiler',
```

### Comparing `pycompall-0.1.0/test/test_compile.py` & `pycompall-0.1.1/test/test_compile.py`

 * *Files 16% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
     def test_compile_nested_by_dir_non_recursive(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (non-recursive), without replacing it."""
         dir, files = nested_py_file
         compile_command(dir, recursive=False, in_place=False)
         expected_pycache_files = [_get_pycache_pyc_from_py(
             file) for file in dir.glob('*.py')]
-
         for file in files:
             assert file.exists()
         for file in expected_pycache_files:
             assert file.exists()
 
     def test_compile_nested_by_dir_recursive(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (recursive), without replacing it."""
@@ -147,7 +146,35 @@
     def test_create_empty_init(self, one_py_file: Tuple[Path, Path]):
         dir, file = one_py_file
         compile_command(dir, create_empty_init=True)
 
         assert file.exists()
         assert _get_pycache_pyc_from_py(file).exists()
         assert (dir / '__init__.py').exists()
+
+
+class TestExcludePattern:
+    def test_exclude_all_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
+        dir, files = nested_py_file
+        pattern = '*.py'
+        compile_command(dir, recursive=True, in_place=True,
+                        exclude_patterns=(pattern,))
+        for file in files:
+            if (file.match(pattern)):
+                assert file.exists()
+                assert not file.with_suffix('.pyc').exists()
+            else:
+                assert not file.exists()
+                assert file.with_suffix('.pyc').exists()
+
+    def test_exclude_one_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
+        dir, files = nested_py_file
+        pattern = 'one.py'
+        compile_command(dir, recursive=True, in_place=True,
+                        exclude_patterns=(pattern,))
+        for file in files:
+            if (file.match(pattern)):
+                assert file.exists()
+                assert not file.with_suffix('.pyc').exists()
+            else:
+                assert not file.exists()
+                assert file.with_suffix('.pyc').exists()
```

