# Comparing `tmp/sicdeploy-0.1.6-py3-none-any.whl.zip` & `tmp/sicdeploy-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 1659 bytes, number of entries: 7
+Zip file size: 4185 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 08:36 sicdeploy/__init__.py
 -rw-r--r--  2.0 unx       94 b- defN 23-Jul-06 08:03 sicdeploy/run.py
--rw-r--r--  2.0 unx      162 b- defN 23-Jul-06 08:46 sicdeploy-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 08:46 sicdeploy-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jul-06 08:46 sicdeploy-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-06 08:46 sicdeploy-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      548 b- defN 23-Jul-06 08:46 sicdeploy-0.1.6.dist-info/RECORD
-7 files, 954 bytes uncompressed, 675 bytes compressed:  29.2%
+-rw-r--r--  2.0 unx     5014 b- defN 23-Jul-06 07:31 sicdeploy/commands/build.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-05 18:43 sicdeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      284 b- defN 23-Jul-06 08:42 sicdeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-06 08:47 sicdeploy-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 08:47 sicdeploy-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-06 08:47 sicdeploy-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-06 08:47 sicdeploy-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      811 b- defN 23-Jul-06 08:47 sicdeploy-0.1.7.dist-info/RECORD
+10 files, 6903 bytes uncompressed, 2785 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
 Filename: sicdeploy/__init__.py
 Comment: 
 
 Filename: sicdeploy/run.py
 Comment: 
 
-Filename: sicdeploy-0.1.6.dist-info/METADATA
+Filename: sicdeploy/commands/build.py
 Comment: 
 
-Filename: sicdeploy-0.1.6.dist-info/WHEEL
+Filename: sicdeploy/templates/meta.yaml.dist
 Comment: 
 
-Filename: sicdeploy-0.1.6.dist-info/entry_points.txt
+Filename: sicdeploy/templates/setup.py.dist
 Comment: 
 
-Filename: sicdeploy-0.1.6.dist-info/top_level.txt
+Filename: sicdeploy-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: sicdeploy-0.1.6.dist-info/RECORD
+Filename: sicdeploy-0.1.7.dist-info/WHEEL
+Comment: 
+
+Filename: sicdeploy-0.1.7.dist-info/entry_points.txt
+Comment: 
+
+Filename: sicdeploy-0.1.7.dist-info/top_level.txt
+Comment: 
+
+Filename: sicdeploy-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

