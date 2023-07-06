# Comparing `tmp/mdrpaLibrary-1.9.tar.gz` & `tmp/mdrpaLibrary-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-1.9.tar", last modified: Thu Jul  6 11:48:53 2023, max compression
+gzip compressed data, was "mdrpaLibrary-2.0.tar", last modified: Thu Jul  6 12:10:08 2023, max compression
```

## Comparing `mdrpaLibrary-1.9.tar` & `mdrpaLibrary-2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.974649 mdrpaLibrary-1.9/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 11:48:53.974463 mdrpaLibrary-1.9/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.972991 mdrpaLibrary-1.9/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-1.9/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-1.9/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 17:39:47.000000 mdrpaLibrary-1.9/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-1.9/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1871 2023-07-06 11:47:58.000000 mdrpaLibrary-1.9/mdrpaLibrary/modelDrivenRpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-1.9/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-1.9/mdrpaLibrary/selectFromDropdownModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-06 11:20:30.000000 mdrpaLibrary-1.9/mdrpaLibrary/sendReportModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.974145 mdrpaLibrary-1.9/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.9/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.9/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.973772 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-06 11:48:53.974700 mdrpaLibrary-1.9/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-06 11:48:22.000000 mdrpaLibrary-1.9/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.702796 mdrpaLibrary-2.0/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 12:10:08.702628 mdrpaLibrary-2.0/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.701269 mdrpaLibrary-2.0/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-2.0/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-2.0/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 17:39:47.000000 mdrpaLibrary-2.0/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-2.0/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1982 2023-07-06 12:07:38.000000 mdrpaLibrary-2.0/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-2.0/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-2.0/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-06 11:20:30.000000 mdrpaLibrary-2.0/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.702304 mdrpaLibrary-2.0/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-2.0/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-2.0/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.702006 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-06 12:10:08.702848 mdrpaLibrary-2.0/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-06 12:07:51.000000 mdrpaLibrary-2.0/setup.py
```

### Comparing `mdrpaLibrary-1.9/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-2.0/mdrpaLibrary/clickButtonModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.9/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-2.0/mdrpaLibrary/inputFieldModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.9/mdrpaLibrary/modelDrivenRpa.py` & `mdrpaLibrary-2.0/mdrpaLibrary/modelDrivenRpa.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
             'selectFromDropdownModel.robot',
             'getUiModels.robot',
             'sendReportModel.robot'
         ]  
 
     def import_resource_file(self, resource_file):
         file_path = os.path.join(self.resource_dir, resource_file)
-        file_path = os.path.normpath(file_path)
+        if os.name == 'nt':  # Check if the platform is Windows
+          file_path = file_path.replace('/', '\\')  # Use backslash for Windows path separator
         self.builtin.import_resource(file_path)
 
 
 
     @keyword
     def click_button_model(self, *args):
         self.import_resource_file(self.resource_files[0])
```

### Comparing `mdrpaLibrary-1.9/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-2.0/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.9/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-2.0/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.9/mdrpaLibrary/sendReportModel.robot` & `mdrpaLibrary-2.0/mdrpaLibrary/sendReportModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.9/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-2.0/mdrpaLibrary/utils/utils.robot`

 * *Files identical despite different names*

