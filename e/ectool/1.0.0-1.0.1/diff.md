# Comparing `tmp/ectool-1.0.0.tar.gz` & `tmp/ectool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.0.0.tar", last modified: Thu Jul  6 14:56:39 2023, max compression
+gzip compressed data, was "ectool-1.0.1.tar", last modified: Thu Jul  6 15:02:55 2023, max compression
```

## Comparing `ectool-1.0.0.tar` & `ectool-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 14:56:39.158983 ectool-1.0.0/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1209 2023-07-06 14:56:39.159980 ectool-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-07-06 14:20:41.000000 ectool-1.0.0/README.md
--rw-rw-rw-   0        0        0      113 2023-07-06 14:56:39.160982 ectool-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     7872 2023-07-06 14:56:29.000000 ectool-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 14:56:39.140981 ectool-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 14:56:39.151981 ectool-1.0.0/src/ectool/
--rw-rw-rw-   0        0        0      112 2023-07-06 14:56:04.000000 ectool-1.0.0/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    15134 2023-07-06 14:56:04.000000 ectool-1.0.0/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0     2233 2023-07-06 14:56:04.000000 ectool-1.0.0/src/ectool/ecburn.py
--rw-rw-rw-   0        0        0     1249 2023-07-06 14:41:48.000000 ectool-1.0.0/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.0.0/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     1811 2023-07-04 13:47:02.000000 ectool-1.0.0/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-06 14:56:39.157981 ectool-1.0.0/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     1209 2023-07-06 14:56:39.000000 ectool-1.0.0/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-06 14:56:39.000000 ectool-1.0.0/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 14:56:39.000000 ectool-1.0.0/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 14:56:39.000000 ectool-1.0.0/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-06 14:56:39.000000 ectool-1.0.0/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 14:56:39.000000 ectool-1.0.0/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 15:02:55.558506 ectool-1.0.1/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1209 2023-07-06 15:02:55.558506 ectool-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-07-06 14:20:41.000000 ectool-1.0.1/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-06 15:02:55.559506 ectool-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     7872 2023-07-06 15:01:55.000000 ectool-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:02:55.540508 ectool-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 15:02:55.550506 ectool-1.0.1/src/ectool/
+-rw-rw-rw-   0        0        0      112 2023-07-06 14:56:04.000000 ectool-1.0.1/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    15134 2023-07-06 14:56:04.000000 ectool-1.0.1/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0     2527 2023-07-06 15:00:58.000000 ectool-1.0.1/src/ectool/ecburn.py
+-rw-rw-rw-   0        0        0     1249 2023-07-06 14:41:48.000000 ectool-1.0.1/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.0.1/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     1811 2023-07-04 13:47:02.000000 ectool-1.0.1/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:02:55.557506 ectool-1.0.1/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     1209 2023-07-06 15:02:55.000000 ectool-1.0.1/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-06 15:02:55.000000 ectool-1.0.1/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:02:55.000000 ectool-1.0.1/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:02:55.000000 ectool-1.0.1/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-06 15:02:55.000000 ectool-1.0.1/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 15:02:55.000000 ectool-1.0.1/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.0.0/LICENSE` & `ectool-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.0.0/PKG-INFO` & `ectool-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectools2py
 Author: Wendal Chen
 Author-email: vt400@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/openLuat/ectools2py/issues
 Project-URL: Source, https://github.com/openLuat/ectools2py/
```

### Comparing `ectool-1.0.0/setup.py` & `ectool-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     name="ectool",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.0",  # Required
+    version="1.0.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ectool-1.0.0/src/ectool/ecaction.py` & `ectool-1.0.1/src/ectool/ecaction.py`

 * *Files identical despite different names*

### Comparing `ectool-1.0.0/src/ectool/ecburn.py` & `ectool-1.0.1/src/ectool/ecburn.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,10 +70,23 @@
 
 def main() :
     if len(sys.argv) > 1 :
         ecburn(sys.argv[1])
     else:
         ecburn_test()
 
+def print_help():
+    print("""
+Usage:
+    ectool <action> [options] [args]
+
+example:
+    ectool burn example.binpkg
+    ectool burn --port COM46 example.binpkg
+    ectool unpack --outdir tmp example.binpkg 
+    """)
 
 if __name__ == "__main__":
-    main()
+    if len(sys.argv) == 1 :
+        print_help()
+    else :
+        main()
```

### Comparing `ectool-1.0.0/src/ectool/ecconst.py` & `ectool-1.0.1/src/ectool/ecconst.py`

 * *Files identical despite different names*

### Comparing `ectool-1.0.0/src/ectool/ecstruct.py` & `ectool-1.0.1/src/ectool/ecstruct.py`

 * *Files identical despite different names*

### Comparing `ectool-1.0.0/src/ectool/unpkg.py` & `ectool-1.0.1/src/ectool/unpkg.py`

 * *Files identical despite different names*

### Comparing `ectool-1.0.0/src/ectool.egg-info/PKG-INFO` & `ectool-1.0.1/src/ectool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectools2py
 Author: Wendal Chen
 Author-email: vt400@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/openLuat/ectools2py/issues
 Project-URL: Source, https://github.com/openLuat/ectools2py/
```

