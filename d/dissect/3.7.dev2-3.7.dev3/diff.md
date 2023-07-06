# Comparing `tmp/dissect-3.7.dev2.tar.gz` & `tmp/dissect-3.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect-3.7.dev2.tar", last modified: Tue Jun 27 07:49:47 2023, max compression
+gzip compressed data, was "dissect-3.7.dev3.tar", last modified: Thu Jul  6 09:18:08 2023, max compression
```

## Comparing `dissect-3.7.dev2.tar` & `dissect-3.7.dev3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:47.769994 dissect-3.7.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 07:49:30.000000 dissect-3.7.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:49:30.000000 dissect-3.7.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:49:30.000000 dissect-3.7.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-27 07:49:47.765994 dissect-3.7.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-27 07:49:30.000000 dissect-3.7.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:47.765994 dissect-3.7.dev2/dissect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:47.000000 dissect-3.7.dev2/dissect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-27 07:49:35.000000 dissect-3.7.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:47.769994 dissect-3.7.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-27 07:49:30.000000 dissect-3.7.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:18:08.671636 dissect-3.7.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 09:17:48.000000 dissect-3.7.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 09:17:48.000000 dissect-3.7.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 09:17:48.000000 dissect-3.7.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-06 09:18:08.671636 dissect-3.7.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-06 09:17:48.000000 dissect-3.7.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:18:08.671636 dissect-3.7.dev3/dissect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-06 09:18:08.000000 dissect-3.7.dev3/dissect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-06 09:18:08.000000 dissect-3.7.dev3/dissect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:18:08.000000 dissect-3.7.dev3/dissect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-06 09:18:08.000000 dissect-3.7.dev3/dissect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:18:08.000000 dissect-3.7.dev3/dissect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-06 09:17:56.000000 dissect-3.7.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:18:08.671636 dissect-3.7.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-06 09:17:48.000000 dissect-3.7.dev3/tox.ini
```

### Comparing `dissect-3.7.dev2/LICENSE` & `dissect-3.7.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect-3.7.dev2/PKG-INFO` & `dissect-3.7.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.7.dev2
+Version: 3.7.dev3
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect-3.7.dev2/README.md` & `dissect-3.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect-3.7.dev2/dissect.egg-info/PKG-INFO` & `dissect-3.7.dev3/dissect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.7.dev2
+Version: 3.7.dev3
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect-3.7.dev2/pyproject.toml` & `dissect-3.7.dev3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -21,38 +21,38 @@
   "Programming Language :: Python :: 3",
   "Topic :: Internet :: Log Analysis",
   "Topic :: Scientific/Engineering :: Information Analysis",
   "Topic :: Security",
   "Topic :: Utilities",
 ]
 dependencies = [
-    "dissect.cim==3.6",
-    "dissect.clfs==1.5",
-    "dissect.cstruct==3.7",
-    "dissect.esedb==3.7",
-    "dissect.etl==3.5",
-    "dissect.eventlog==3.5",
-    "dissect.evidence==3.5",
-    "dissect.executable==1.3",
-    "dissect.extfs==3.5",
-    "dissect.fat==3.5",
-    "dissect.ffs==3.5",
-    "dissect.hypervisor==3.7",
-    "dissect.ntfs==3.5",
-    "dissect.ole==3.5",
-    "dissect.regf==3.5",
-    "dissect.shellitem==3.5",
-    "dissect.sql==3.5",
-    "dissect.squashfs==1.2",
-    "dissect.target[full]==3.9",
-    "dissect.thumbcache==1.4",
-    "dissect.util==3.8",
-    "dissect.vmfs==3.5",
-    "dissect.volume==3.5",
-    "dissect.xfs==3.5",
+    "dissect.cim==3.7",
+    "dissect.clfs==1.6",
+    "dissect.cstruct==3.8",
+    "dissect.esedb==3.8",
+    "dissect.etl==3.6",
+    "dissect.eventlog==3.6",
+    "dissect.evidence==3.6",
+    "dissect.executable==1.4",
+    "dissect.extfs==3.6",
+    "dissect.fat==3.6",
+    "dissect.ffs==3.6",
+    "dissect.hypervisor==3.8",
+    "dissect.ntfs==3.6",
+    "dissect.ole==3.6",
+    "dissect.regf==3.6",
+    "dissect.shellitem==3.6",
+    "dissect.sql==3.6",
+    "dissect.squashfs==1.3",
+    "dissect.target[full]==3.10",
+    "dissect.thumbcache==1.5",
+    "dissect.util==3.9",
+    "dissect.vmfs==3.6",
+    "dissect.volume==3.6",
+    "dissect.xfs==3.6",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://dissect.tools"
 documentation = "https://docs.dissect.tools"
 repository = "https://github.com/fox-it/dissect"
```

### Comparing `dissect-3.7.dev2/tox.ini` & `dissect-3.7.dev3/tox.ini`

 * *Files identical despite different names*

