# Comparing `tmp/grimp-2.4.tar.gz` & `tmp/grimp-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimp-2.4.tar", last modified: Fri May  5 15:41:18 2023, max compression
+gzip compressed data, was "grimp-2.5.tar", last modified: Thu Jul  6 16:46:15 2023, max compression
```

## Comparing `grimp-2.4.tar` & `grimp-2.5.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.701981 grimp-2.4/
--rw-r--r--   0 david.seddon   (501) staff       (20)      261 2023-01-05 10:37:10.000000 grimp-2.4/AUTHORS.rst
--rw-r--r--   0 david.seddon   (501) staff       (20)     1315 2022-08-04 16:27:12.000000 grimp-2.4/LICENSE
--rw-r--r--   0 david.seddon   (501) staff       (20)     5257 2023-05-05 15:41:18.702105 grimp-2.4/PKG-INFO
--rw-r--r--   0 david.seddon   (501) staff       (20)     4136 2023-03-03 11:28:02.000000 grimp-2.4/README.rst
--rw-r--r--   0 david.seddon   (501) staff       (20)      138 2023-05-05 15:41:18.702506 grimp-2.4/setup.cfg
--rw-r--r--   0 david.seddon   (501) staff       (20)     2020 2023-05-05 15:40:26.000000 grimp-2.4/setup.py
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.689236 grimp-2.4/src/
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.692417 grimp-2.4/src/grimp/
--rw-r--r--   0 david.seddon   (501) staff       (20)      228 2023-05-05 15:40:47.000000 grimp-2.4/src/grimp/__init__.py
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.696527 grimp-2.4/src/grimp/adaptors/
--rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/adaptors/__init__.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     9691 2023-05-05 14:53:46.000000 grimp-2.4/src/grimp/adaptors/caching.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     1400 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/adaptors/filesystem.py
--rw-r--r--   0 david.seddon   (501) staff       (20)    18709 2023-02-18 10:00:32.000000 grimp-2.4/src/grimp/adaptors/graph.py
--rw-r--r--   0 david.seddon   (501) staff       (20)    16100 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/adaptors/importscanner.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     4000 2023-05-05 15:39:26.000000 grimp-2.4/src/grimp/adaptors/modulefinder.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     2041 2022-08-15 08:26:02.000000 grimp-2.4/src/grimp/adaptors/packagefinder.py
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.697022 grimp-2.4/src/grimp/algorithms/
--rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-09-27 15:23:32.000000 grimp-2.4/src/grimp/algorithms/__init__.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     5069 2022-09-27 15:23:32.000000 grimp-2.4/src/grimp/algorithms/shortest_path.py
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.697919 grimp-2.4/src/grimp/application/
--rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/application/__init__.py
--rw-r--r--   0 david.seddon   (501) staff       (20)      494 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/application/config.py
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.701176 grimp-2.4/src/grimp/application/ports/
--rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/application/ports/__init__.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     1592 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/application/ports/caching.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     2570 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/application/ports/filesystem.py
--rw-r--r--   0 david.seddon   (501) staff       (20)    10385 2023-01-05 10:23:07.000000 grimp-2.4/src/grimp/application/ports/graph.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     1688 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/application/ports/importscanner.py
--rw-r--r--   0 david.seddon   (501) staff       (20)      832 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/application/ports/modulefinder.py
--rw-r--r--   0 david.seddon   (501) staff       (20)      269 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/application/ports/packagefinder.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     5908 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/application/usecases.py
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.701717 grimp-2.4/src/grimp/domain/
--rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/domain/__init__.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     2183 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/domain/valueobjects.py
--rw-r--r--   0 david.seddon   (501) staff       (20)     1579 2022-08-15 08:26:02.000000 grimp-2.4/src/grimp/exceptions.py
--rw-r--r--   0 david.seddon   (501) staff       (20)      194 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/helpers.py
--rw-r--r--   0 david.seddon   (501) staff       (20)      622 2023-03-03 11:08:24.000000 grimp-2.4/src/grimp/main.py
--rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.4/src/grimp/py.typed
-drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-05-05 15:41:18.693784 grimp-2.4/src/grimp.egg-info/
--rw-r--r--   0 david.seddon   (501) staff       (20)     5257 2023-05-05 15:41:18.000000 grimp-2.4/src/grimp.egg-info/PKG-INFO
--rw-r--r--   0 david.seddon   (501) staff       (20)     1103 2023-05-05 15:41:18.000000 grimp-2.4/src/grimp.egg-info/SOURCES.txt
--rw-r--r--   0 david.seddon   (501) staff       (20)        1 2023-05-05 15:41:18.000000 grimp-2.4/src/grimp.egg-info/dependency_links.txt
--rw-r--r--   0 david.seddon   (501) staff       (20)        1 2022-08-04 16:27:28.000000 grimp-2.4/src/grimp.egg-info/not-zip-safe
--rw-r--r--   0 david.seddon   (501) staff       (20)       28 2023-05-05 15:41:18.000000 grimp-2.4/src/grimp.egg-info/requires.txt
--rw-r--r--   0 david.seddon   (501) staff       (20)        6 2023-05-05 15:41:18.000000 grimp-2.4/src/grimp.egg-info/top_level.txt
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.262987 grimp-2.5/
+-rw-r--r--   0 david.seddon   (501) staff       (20)      261 2023-05-14 08:56:45.000000 grimp-2.5/AUTHORS.rst
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1315 2022-08-04 16:27:12.000000 grimp-2.5/LICENSE
+-rw-r--r--   0 david.seddon   (501) staff       (20)     5207 2023-07-06 16:46:15.263103 grimp-2.5/PKG-INFO
+-rw-r--r--   0 david.seddon   (501) staff       (20)     4136 2023-05-14 08:56:45.000000 grimp-2.5/README.rst
+-rw-r--r--   0 david.seddon   (501) staff       (20)      173 2023-07-06 16:46:15.263500 grimp-2.5/setup.cfg
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1971 2023-07-06 16:37:11.000000 grimp-2.5/setup.py
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.250694 grimp-2.5/src/
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.254472 grimp-2.5/src/grimp/
+-rw-r--r--   0 david.seddon   (501) staff       (20)      371 2023-07-06 16:37:11.000000 grimp-2.5/src/grimp/__init__.py
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.258734 grimp-2.5/src/grimp/adaptors/
+-rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/adaptors/__init__.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)    11160 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/adaptors/_layers.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)    10390 2023-07-06 15:11:58.000000 grimp-2.5/src/grimp/adaptors/caching.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1400 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/adaptors/filesystem.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)    19151 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/adaptors/graph.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)    16100 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/adaptors/importscanner.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     4000 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/adaptors/modulefinder.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     2041 2022-08-15 08:26:02.000000 grimp-2.5/src/grimp/adaptors/packagefinder.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)      163 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/adaptors/timing.py
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.259148 grimp-2.5/src/grimp/algorithms/
+-rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-09-27 15:23:32.000000 grimp-2.5/src/grimp/algorithms/__init__.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     5069 2022-09-27 15:23:32.000000 grimp-2.5/src/grimp/algorithms/shortest_path.py
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.260186 grimp-2.5/src/grimp/application/
+-rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/application/__init__.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)      494 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/application/config.py
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.262152 grimp-2.5/src/grimp/application/ports/
+-rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/application/ports/__init__.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1592 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/application/ports/caching.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     2570 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/application/ports/filesystem.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)    12018 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/application/ports/graph.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1688 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/application/ports/importscanner.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)      832 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/application/ports/modulefinder.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)      269 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/application/ports/packagefinder.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1215 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/application/ports/timing.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     5876 2023-07-06 10:23:03.000000 grimp-2.5/src/grimp/application/usecases.py
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.262779 grimp-2.5/src/grimp/domain/
+-rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/domain/__init__.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     2442 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/domain/analysis.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     2183 2023-05-14 08:56:45.000000 grimp-2.5/src/grimp/domain/valueobjects.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1714 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/exceptions.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)      194 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/helpers.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)      698 2023-07-06 16:35:01.000000 grimp-2.5/src/grimp/main.py
+-rw-r--r--   0 david.seddon   (501) staff       (20)        0 2022-08-04 16:27:12.000000 grimp-2.5/src/grimp/py.typed
+drwxr-xr-x   0 david.seddon   (501) staff       (20)        0 2023-07-06 16:46:15.255833 grimp-2.5/src/grimp.egg-info/
+-rw-r--r--   0 david.seddon   (501) staff       (20)     5207 2023-07-06 16:46:15.000000 grimp-2.5/src/grimp.egg-info/PKG-INFO
+-rw-r--r--   0 david.seddon   (501) staff       (20)     1229 2023-07-06 16:46:15.000000 grimp-2.5/src/grimp.egg-info/SOURCES.txt
+-rw-r--r--   0 david.seddon   (501) staff       (20)        1 2023-07-06 16:46:15.000000 grimp-2.5/src/grimp.egg-info/dependency_links.txt
+-rw-r--r--   0 david.seddon   (501) staff       (20)        1 2022-08-04 16:27:28.000000 grimp-2.5/src/grimp.egg-info/not-zip-safe
+-rw-r--r--   0 david.seddon   (501) staff       (20)       28 2023-07-06 16:46:15.000000 grimp-2.5/src/grimp.egg-info/requires.txt
+-rw-r--r--   0 david.seddon   (501) staff       (20)        6 2023-07-06 16:46:15.000000 grimp-2.5/src/grimp.egg-info/top_level.txt
```

### Comparing `grimp-2.4/LICENSE` & `grimp-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grimp-2.4/PKG-INFO` & `grimp-2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: grimp
-Version: 2.4
+Version: 2.5
 Summary: Builds a queryable graph of the imports within one or more Python packages.
 Author: David Seddon
 Author-email: david@seddonym.me
 License: BSD 2-Clause License
 Project-URL: Documentation, https://grimp.readthedocs.io/
 Project-URL: Source code, https://github.com/seddonym/grimp/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =====
 Grimp
 =====
```

### Comparing `grimp-2.4/README.rst` & `grimp-2.5/README.rst`

 * *Files identical despite different names*

### Comparing `grimp-2.4/setup.py` & `grimp-2.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='grimp',
-    version='2.4',
+    version='2.5',
     license='BSD 2-Clause License',
     description="Builds a queryable graph of the imports within one or more Python packages.",
     long_description=read('README.rst'),
     long_description_content_type='text/x-rst',
     author='David Seddon',
     author_email='david@seddonym.me',
     project_urls={
@@ -43,20 +43,19 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: Unix',
         'Operating System :: POSIX',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Utilities',
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "typing-extensions>=3.10.0.0",
     ],
 )
```

### Comparing `grimp-2.4/src/grimp/adaptors/caching.py` & `grimp-2.5/src/grimp/adaptors/caching.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import hashlib
 import json
+import logging
 from typing import Dict, List, Optional, Set, Tuple, Type
 
 from grimp.application.ports.filesystem import AbstractFileSystem
 from grimp.application.ports.modulefinder import FoundPackage, ModuleFile
 from grimp.domain.valueobjects import DirectImport, Module
 
 from ..application.ports.caching import Cache as AbstractCache
 from ..application.ports.caching import CacheMiss
 
+logger = logging.getLogger(__name__)
 PrimitiveFormat = Dict[str, List[Tuple[str, Optional[int], str]]]
 
 
 class CacheFileNamer:
     @classmethod
     def make_meta_file_name(cls, found_package: FoundPackage) -> str:
         return f"{found_package.name}.meta.json"
@@ -25,15 +27,17 @@
             found_packages, include_external_packages
         )
 
         bytes_identifier = identifier.encode()
         # Use a hash algorithm with a limited size to avoid cache filenames that are too long
         # the filesystem, which can happen if there are more than a few root packages
         # being analyzed.
-        safe_unicode_identifier = hashlib.blake2b(bytes_identifier, digest_size=20).hexdigest()
+        safe_unicode_identifier = hashlib.blake2b(
+            bytes_identifier, digest_size=20
+        ).hexdigest()
         return f"{safe_unicode_identifier}.data.json"
 
     @classmethod
     def make_data_file_unique_string(
         cls, found_packages: Set[FoundPackage], include_external_packages: bool
     ) -> str:
         """
@@ -102,15 +106,14 @@
             raise CacheMiss
 
     def write(
         self,
         imports_by_module: Dict[Module, Set[DirectImport]],
     ) -> None:
         self._write_marker_files_if_not_already_there()
-
         # Write data file.
         primitives_map: PrimitiveFormat = {}
         for found_package in self.found_packages:
             primitives_map_for_found_package: PrimitiveFormat = {
                 module_file.module.name: [
                     (
                         direct_import.imported.name,
@@ -128,26 +131,28 @@
             self.cache_dir,
             self._namer.make_data_file_name(
                 found_packages=self.found_packages,
                 include_external_packages=self.include_external_packages,
             ),
         )
         self.file_system.write(data_cache_filename, serialized)
+        logger.info(f"Wrote data cache file {data_cache_filename}.")
 
         # Write meta files.
         for found_package in self.found_packages:
             meta_filename = self.file_system.join(
                 self.cache_dir, self._namer.make_meta_file_name(found_package)
             )
             mtime_map = {
                 module_file.module.name: module_file.mtime
                 for module_file in found_package.module_files
             }
             serialized_meta = json.dumps(mtime_map)
             self.file_system.write(meta_filename, serialized_meta)
+            logger.info(f"Wrote meta cache file {meta_filename}.")
 
     def _build_mtime_map(self) -> None:
         self._mtime_map = self._read_mtime_map_files()
 
     def _read_mtime_map_files(self) -> Dict[str, float]:
         all_mtimes: Dict[str, float] = {}
         for found_package in self.found_packages:
@@ -157,18 +162,22 @@
     def _read_mtime_map_file(self, found_package: FoundPackage) -> Dict[str, float]:
         meta_cache_filename = self.file_system.join(
             self.cache_dir, self._namer.make_meta_file_name(found_package)
         )
         try:
             serialized = self.file_system.read(meta_cache_filename)
         except FileNotFoundError:
+            logger.info(f"No cache file: {meta_cache_filename}.")
             return {}
         try:
-            return json.loads(serialized)
+            deserialized = json.loads(serialized)
+            logger.info(f"Used cache meta file {meta_cache_filename}.")
+            return deserialized
         except json.JSONDecodeError:
+            logger.warning(f"Could not use corrupt cache file {meta_cache_filename}.")
             return {}
 
     def _build_data_map(self) -> None:
         self._data_map = self._read_data_map_file()
 
     def _read_data_map_file(self) -> Dict[Module, Set[DirectImport]]:
         data_cache_filename = self.file_system.join(
@@ -177,20 +186,23 @@
                 found_packages=self.found_packages,
                 include_external_packages=self.include_external_packages,
             ),
         )
         try:
             serialized = self.file_system.read(data_cache_filename)
         except FileNotFoundError:
+            logger.info(f"No cache file: {data_cache_filename}.")
             return {}
 
         # Deserialize to primitives.
         try:
             deserialized_json = json.loads(serialized)
+            logger.info(f"Used cache data file {data_cache_filename}.")
         except json.JSONDecodeError:
+            logger.warning(f"Could not use corrupt cache file {data_cache_filename}.")
             return {}
 
         primitives_map: PrimitiveFormat = self._to_primitives_data_map(
             deserialized_json
         )
 
         return {
```

### Comparing `grimp-2.4/src/grimp/adaptors/filesystem.py` & `grimp-2.5/src/grimp/adaptors/filesystem.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/adaptors/graph.py` & `grimp-2.5/src/grimp/adaptors/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+from __future__ import annotations
+
 from copy import copy
-from typing import Dict, List, Optional, Set, Tuple, cast
+from typing import Dict, List, Optional, Sequence, Set, Tuple, cast
 
 from grimp.algorithms.shortest_path import bidirectional_shortest_path
 from grimp.application.ports import graph
+from grimp.domain.analysis import PackageDependency
 from grimp.domain.valueobjects import Module
 from grimp.exceptions import ModuleNotPresent
 
+from . import _layers
+
 
-class ImportGraph(graph.AbstractImportGraph):
+class ImportGraph(graph.ImportGraph):
     """
     Pure Python implementation of the ImportGraph.
     """
 
     def __init__(self) -> None:
         # Maps all the modules directly imported by each key.
         self._importeds_by_importer: Dict[str, Set[str]] = {}
@@ -368,14 +373,25 @@
         for upstream in upstream_modules:
             for downstream in downstream_modules:
                 if self.chain_exists(imported=upstream, importer=downstream):
                     return True
 
         return False
 
+    # High level analysis
+
+    def find_illegal_dependencies_for_layers(
+        self,
+        layers: Sequence[str],
+        containers: Optional[Set[str]] = None,
+    ) -> set[PackageDependency]:
+        return _layers.find_illegal_dependencies(
+            graph=self, layers=layers, containers=containers or set()
+        )
+
     # Private methods
 
     def _find_ancestor_squashed_module(self, module: str) -> Optional[str]:
         """
         Return the name of a squashed module that is an ancestor of the supplied module, or None
         if no such module exists.
         """
```

### Comparing `grimp-2.4/src/grimp/adaptors/importscanner.py` & `grimp-2.5/src/grimp/adaptors/importscanner.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/adaptors/modulefinder.py` & `grimp-2.5/src/grimp/adaptors/modulefinder.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/adaptors/packagefinder.py` & `grimp-2.5/src/grimp/adaptors/packagefinder.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/algorithms/shortest_path.py` & `grimp-2.5/src/grimp/algorithms/shortest_path.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/application/ports/caching.py` & `grimp-2.5/src/grimp/application/ports/caching.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/application/ports/filesystem.py` & `grimp-2.5/src/grimp/application/ports/filesystem.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/application/ports/graph.py` & `grimp-2.5/src/grimp/application/ports/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from __future__ import annotations
+
 import abc
-from typing import Iterator, List, Optional, Set, Tuple
+from typing import Iterator, List, Optional, Sequence, Set, Tuple
 
 from typing_extensions import TypedDict
 
+from grimp.domain.analysis import PackageDependency
+
 
 class DetailedImport(TypedDict):
     importer: str
     imported: str
     line_number: int
     line_contents: str
 
 
-class AbstractImportGraph(abc.ABC):
+class ImportGraph(abc.ABC):
     """
     A Directed Graph of imports between Python modules.
     """
 
     # Mechanics
     # ---------
 
@@ -217,15 +221,15 @@
                            the subpackage.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def find_shortest_chain(
         self, importer: str, imported: str
-    ) -> Optional[Tuple[str, ...]]:
+    ) -> tuple[str, ...] | None:
         """
         Attempt to find the shortest chain of imports between two modules, in the direction
         of importer to imported.
 
         Returns:
             Tuple of module names, from importer to imported, or None if no chain exists.
         """
@@ -270,14 +274,47 @@
             as_packages: Whether to treat the supplied modules as individual modules,
                          or as packages (including any descendants, if there are any). If
                          treating them as subpackages, all descendants of the supplied modules
                          will be checked too.
         """
         raise NotImplementedError
 
+    # High level analysis
+    # -------------------
+
+    def find_illegal_dependencies_for_layers(
+        self,
+        layers: Sequence[str],
+        containers: Optional[Set[str]] = None,
+    ) -> set[PackageDependency]:
+        """
+        Find dependencies that don't conform to the supplied layered architecture.
+
+        'Layers' is an architectural pattern in which a list of sibling modules/packages
+        have a dependency direction from high to low. In other words, a higher layer would
+        be allowed to import a lower layer, but not the other way around.
+
+        Arguments:
+
+        - layers:     The name of each layer module. If containers are also specified,
+                      then these names must be relative to the container. The order is from
+                      higher to lower level layers. Any layers that don't exist in the graph
+                      will be ignored.
+        - containers: The parent modules of the layers, as absolute names that you could import,
+                      such as "mypackage.foo". (Optional.)
+
+        Returns the illegal dependencies in the form of a set of PackageDependency objects.
+        Each package dependency is for a different permutation of two layers for which there
+        is a violation, and contains information about the illegal chains of imports from the
+        lower layer (the 'upstream') to the higher layer (the 'downstream').
+
+        Raises NoSuchContainer if the container is not a module in the graph.
+        """
+        raise NotImplementedError
+
     def __repr__(self) -> str:
         """
         Display the instance in one of the following ways:
 
             <ImportGraph: empty>
             <ImportGraph: 'one', 'two', 'three', 'four', 'five'>
             <ImportGraph: 'one', 'two', 'three', 'four', 'five', ...>
```

### Comparing `grimp-2.4/src/grimp/application/ports/importscanner.py` & `grimp-2.5/src/grimp/application/ports/importscanner.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/application/ports/modulefinder.py` & `grimp-2.5/src/grimp/application/ports/modulefinder.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/application/usecases.py` & `grimp-2.5/src/grimp/application/usecases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Use cases handle application logic.
 """
 from typing import Dict, Sequence, Set, Type, Union, cast
 
 from ..application.ports import caching
 from ..application.ports.filesystem import AbstractFileSystem
-from ..application.ports.graph import AbstractImportGraph
+from ..application.ports.graph import ImportGraph
 from ..application.ports.importscanner import AbstractImportScanner
 from ..application.ports.modulefinder import AbstractModuleFinder, FoundPackage
 from ..application.ports.packagefinder import AbstractPackageFinder
 from ..domain.valueobjects import DirectImport, Module
 from .config import settings
 
 
@@ -18,15 +18,15 @@
 
 
 def build_graph(
     package_name,
     *additional_package_names,
     include_external_packages: bool = False,
     cache_dir: Union[str, Type[NotSupplied], None] = NotSupplied,
-) -> AbstractImportGraph:
+) -> ImportGraph:
     """
     Build and return an import graph for the supplied package name(s).
 
     Args:
         - package_name: the name of the top level package for which to build the graph.
         - additional_package_names: tuple of the
         - include_external_packages: whether to include any external packages in the graph.
@@ -136,16 +136,16 @@
 
     return imports_by_module
 
 
 def _assemble_graph(
     found_packages: Set[FoundPackage],
     imports_by_module: Dict[Module, Set[DirectImport]],
-) -> AbstractImportGraph:
-    graph: AbstractImportGraph = settings.IMPORT_GRAPH_CLASS()
+) -> ImportGraph:
+    graph: ImportGraph = settings.IMPORT_GRAPH_CLASS()
     for module, direct_imports in imports_by_module.items():
         graph.add_module(module.name)
         for direct_import in direct_imports:
             # Before we add the import, check to see if the imported module is in fact an
             # external module, and if so, tell the graph that it is a squashed module.
             graph.add_module(
                 direct_import.imported.name,
```

### Comparing `grimp-2.4/src/grimp/domain/valueobjects.py` & `grimp-2.5/src/grimp/domain/valueobjects.py`

 * *Files identical despite different names*

### Comparing `grimp-2.4/src/grimp/exceptions.py` & `grimp-2.5/src/grimp/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 class ModuleNotPresent(GrimpException):
     """
     Indicates that a module was not present in a graph.
     """
 
 
+class NoSuchContainer(GrimpException):
+    """
+    Indicates that a passed container was not found as a module in the graph.
+    """
+
+
 class NamespacePackageEncountered(GrimpException):
     """
     Indicates that there was no __init__.py at the top level.
 
     This indicates a namespace package (see PEP 420), which is not currently supported. More
     typically this is just an oversight which can be fixed by adding the __init__.py file.
     """
```

### Comparing `grimp-2.4/src/grimp/main.py` & `grimp-2.5/src/grimp/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 from .adaptors.caching import Cache
 from .adaptors.filesystem import FileSystem
 from .adaptors.graph import ImportGraph
 from .adaptors.importscanner import ImportScanner
 from .adaptors.modulefinder import ModuleFinder
 from .adaptors.packagefinder import ImportLibPackageFinder
+from .adaptors.timing import SystemClockTimer
 from .application.config import settings
 from .application.usecases import build_graph
 
 settings.configure(
     MODULE_FINDER=ModuleFinder(),
     FILE_SYSTEM=FileSystem(),
     IMPORT_SCANNER_CLASS=ImportScanner,
     IMPORT_GRAPH_CLASS=ImportGraph,
     PACKAGE_FINDER=ImportLibPackageFinder(),
     CACHE_CLASS=Cache,
+    TIMER=SystemClockTimer(),
 )
```

### Comparing `grimp-2.4/src/grimp.egg-info/PKG-INFO` & `grimp-2.5/src/grimp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: grimp
-Version: 2.4
+Version: 2.5
 Summary: Builds a queryable graph of the imports within one or more Python packages.
 Author: David Seddon
 Author-email: david@seddonym.me
 License: BSD 2-Clause License
 Project-URL: Documentation, https://grimp.readthedocs.io/
 Project-URL: Source code, https://github.com/seddonym/grimp/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =====
 Grimp
 =====
```

### Comparing `grimp-2.4/src/grimp.egg-info/SOURCES.txt` & `grimp-2.5/src/grimp.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 src/grimp.egg-info/PKG-INFO
 src/grimp.egg-info/SOURCES.txt
 src/grimp.egg-info/dependency_links.txt
 src/grimp.egg-info/not-zip-safe
 src/grimp.egg-info/requires.txt
 src/grimp.egg-info/top_level.txt
 src/grimp/adaptors/__init__.py
+src/grimp/adaptors/_layers.py
 src/grimp/adaptors/caching.py
 src/grimp/adaptors/filesystem.py
 src/grimp/adaptors/graph.py
 src/grimp/adaptors/importscanner.py
 src/grimp/adaptors/modulefinder.py
 src/grimp/adaptors/packagefinder.py
+src/grimp/adaptors/timing.py
 src/grimp/algorithms/__init__.py
 src/grimp/algorithms/shortest_path.py
 src/grimp/application/__init__.py
 src/grimp/application/config.py
 src/grimp/application/usecases.py
 src/grimp/application/ports/__init__.py
 src/grimp/application/ports/caching.py
 src/grimp/application/ports/filesystem.py
 src/grimp/application/ports/graph.py
 src/grimp/application/ports/importscanner.py
 src/grimp/application/ports/modulefinder.py
 src/grimp/application/ports/packagefinder.py
+src/grimp/application/ports/timing.py
 src/grimp/domain/__init__.py
+src/grimp/domain/analysis.py
 src/grimp/domain/valueobjects.py
```

