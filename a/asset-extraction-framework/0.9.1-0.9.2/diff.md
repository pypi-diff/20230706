# Comparing `tmp/asset_extraction_framework-0.9.1.tar.gz` & `tmp/asset_extraction_framework-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_extraction_framework-0.9.1.tar", last modified: Tue Jun 20 21:49:45 2023, max compression
+gzip compressed data, was "asset_extraction_framework-0.9.2.tar", last modified: Thu Jul  6 21:32:02 2023, max compression
```

## Comparing `asset_extraction_framework-0.9.1.tar` & `asset_extraction_framework-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.443320 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asserts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/assets/Asset/
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Sound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/CommandLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/File.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:32:02.508064 asset_extraction_framework-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-06 21:32:02.508064 asset_extraction_framework-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:32:02.504064 asset_extraction_framework-0.9.2/asset_extraction_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asserts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:32:02.508064 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/CommandLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/asset_extraction_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:32:02.508064 asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-06 21:32:02.000000 asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-06 21:32:02.000000 asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:32:02.000000 asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 21:32:02.000000 asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 21:32:02.000000 asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:32:02.508064 asset_extraction_framework-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:31:48.000000 asset_extraction_framework-0.9.2/setup.py
```

### Comparing `asset_extraction_framework-0.9.1/LICENSE` & `asset_extraction_framework-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/PKG-INFO` & `asset_extraction_framework-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_extraction_framework
-Version: 0.9.1
+Version: 0.9.2
 Summary: Extract multimedia assets from legacy software
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `asset_extraction_framework-0.9.1/README.md` & `asset_extraction_framework-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/PKG-INFO` & `asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset-extraction-framework
-Version: 0.9.1
+Version: 0.9.2
 Summary: Extract multimedia assets from legacy software
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/SOURCES.txt` & `asset_extraction_framework-0.9.2/asset_extraction_framework.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+asset_extraction_framework/Application.py
+asset_extraction_framework/Asserts.py
+asset_extraction_framework/CommandLine.py
+asset_extraction_framework/File.py
+asset_extraction_framework/__init__.py
 asset_extraction_framework.egg-info/PKG-INFO
 asset_extraction_framework.egg-info/SOURCES.txt
 asset_extraction_framework.egg-info/dependency_links.txt
 asset_extraction_framework.egg-info/requires.txt
 asset_extraction_framework.egg-info/top_level.txt
-assets/Application.py
-assets/Asserts.py
-assets/CommandLine.py
-assets/File.py
-assets/__init__.py
-assets/Asset/Animation.py
-assets/Asset/Asset.py
-assets/Asset/BoundingBox.py
-assets/Asset/Image.py
-assets/Asset/Palette.py
-assets/Asset/Sound.py
-assets/Asset/__init__.py
+asset_extraction_framework/Asset/Animation.py
+asset_extraction_framework/Asset/Asset.py
+asset_extraction_framework/Asset/BoundingBox.py
+asset_extraction_framework/Asset/Image.py
+asset_extraction_framework/Asset/Palette.py
+asset_extraction_framework/Asset/Sound.py
+asset_extraction_framework/Asset/__init__.py
```

### Comparing `asset_extraction_framework-0.9.1/assets/Application.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/Application.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 ## Represents an application whose assets we wish to export.
 ## An application contains a collection of files, which each
 ## contain a collection of assets.
 class Application:
     def __init__(self, application_name: str):
         # CREATE A PLACE TO STORE THE FILES.
         self.files: List[File] = []
-
         self.application_name = application_name
 
     ## Parses the files matching the detection entries for this application.
     ## The files are guaranteed to be parsed in the order the file detection entries
     ## are provided.
     ## \param[in]  paths - The paths to be searched for matching files.
     ##             Recurses into directories to find matching files.
@@ -128,22 +127,20 @@
         # TODO: DOcument why this is necessary.
         jsons.suppress_warnings(True)
 
         # EXPORT THE ASSETS IN THE APPLICATION.
         # First, we want to create a directory to hold all the exported files
         # from this application.
         application_export_subdirectory: str = os.path.join(command_line_arguments.export, self.application_name)
-        # logging.debug(f'Exporting to {application_export_subdirectory}')
         for index, file in enumerate(self.files):
             # EXPORT THE FILE.
             # This method creates a directory for the file.
             print(f'Exporting assets in {file.filepath}')
             file.export(application_export_subdirectory, command_line_arguments)
 
         # EXPORT THE JSON FOR THE APPLICATION.
-        #print(f'Exporting JSON for whole application')
-        #json_export_filename = f'{self.application_name}.json'
-        #json_export_filepath = os.path.join(application_export_subdirectory, json_export_filename)
-        #with open(json_export_filepath, 'w') as json_file:
-        #    asset_tree = jsons.dump(self.files, strip_privates = True)
-        #    # TODO: Ensure this JSON is pretty printed.
-        #    json.dump(asset_tree, json_file)
+        print(f'Exporting JSON for whole application')
+        json_export_filename = f'{self.application_name}.json'
+        json_export_filepath = os.path.join(application_export_subdirectory, json_export_filename)
+        with open(json_export_filepath, 'w') as json_file:
+            asset_tree = jsons.dump(self.files, strip_privates = True)
+            json.dump(asset_tree, json_file, indent = 2)
```

### Comparing `asset_extraction_framework-0.9.1/assets/Asserts.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/Asserts.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/assets/Asset/Animation.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Animation.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/assets/Asset/BoundingBox.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/assets/Asset/Image.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Image.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/assets/Asset/Palette.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Palette.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/assets/Asset/Sound.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/Asset/Sound.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/assets/CommandLine.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/CommandLine.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.1/assets/File.py` & `asset_extraction_framework-0.9.2/asset_extraction_framework/File.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from dataclasses import dataclass
 import mmap
 import os
 from pathlib import Path
 
-from assets.Asserts import assert_equal
+from .Asserts import assert_equal
 
 ## Models a file (whether actually on the filesystem, or logically from an in-memory archive)
 ## that holds one or more assets.
 class File:
     ## \param[in] - filepath: The filepath of the file, if it exists on the filesystem.
     ##                        Defaults to None if not provided.
     ## \param[in] - stream: A BytesIO-like object that holds the file data, if the file does
@@ -54,15 +54,19 @@
     ## \return The subdirectory named after this file created in the provided root.
     def export(self, root_directory_path: str, command_line_arguments) -> str:
         # CREATE THE DIRECTORY FOR THIS FILE.
         directory_path = os.path.join(root_directory_path, self.filename)
         Path(directory_path).mkdir(parents = True, exist_ok = True)
 
         # EXPORT THE ASSETS INTO THIS FILE'S DIRECTORY.
-        for index, asset in enumerate(self.assets):
+        if isinstance(self.assets, dict):
+            assets_list = self.assets.values()
+        else:
+            assets_list = self.assets
+        for index, asset in enumerate(assets_list):
             # SET THE ASSET NAME IF IT IS NOT ALREADY SET.
             # This ensures every asset has a unique name within this file.
             if asset.name is None:
                 asset.name = f'{index}'
 
             # EXPORT THE ASSET.
             asset.export(directory_path, command_line_arguments)
```

### Comparing `asset_extraction_framework-0.9.1/pyproject.toml` & `asset_extraction_framework-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_extraction_framework"
-version = "0.9.1"
+version = "0.9.2"
 description = "Extract multimedia assets from legacy software"
 readme = "README.md"
 authors = [{ name = "npjg" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["struct", "reverse-engineering", "self-document"]
 requires-python = ">=3.9"
-
 dependencies = [
     "Pillow>=9.2.0",
     "numpy>=1.23.0",
     "jsons>=1.6.2"
 ]
 
 [project.urls]
```

