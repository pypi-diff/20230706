# Comparing `tmp/pyappbundler-0.1.1.tar.gz` & `tmp/pyappbundler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappbundler-0.1.1.tar", last modified: Thu Jul  6 13:07:49 2023, max compression
+gzip compressed data, was "pyappbundler-0.1.2.tar", last modified: Thu Jul  6 15:32:58 2023, max compression
```

## Comparing `pyappbundler-0.1.1.tar` & `pyappbundler-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.282609 pyappbundler-0.1.1/
--rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      730 2023-07-06 13:07:49.281609 pyappbundler-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.277608 pyappbundler-0.1.1/pyappbundler/
--rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.1/pyappbundler/__init__.py
--rw-rw-rw-   0        0        0     2553 2023-07-06 07:59:09.000000 pyappbundler-0.1.1/pyappbundler/__main__.py
--rw-rw-rw-   0        0        0       22 2023-07-06 12:57:54.000000 pyappbundler-0.1.1/pyappbundler/_version.py
--rw-rw-rw-   0        0        0     3572 2023-07-06 12:57:31.000000 pyappbundler-0.1.1/pyappbundler/pyappbundler.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.281609 pyappbundler-0.1.1/pyappbundler/templates/
--rw-rw-rw-   0        0        0     1537 2023-07-05 15:18:33.000000 pyappbundler-0.1.1/pyappbundler/templates/iss.tmpl
-drwxrwxrwx   0        0        0        0 2023-07-06 13:07:49.280608 pyappbundler-0.1.1/pyappbundler.egg-info/
--rw-rw-rw-   0        0        0      730 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 13:07:49.000000 pyappbundler-0.1.1/pyappbundler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 13:07:49.282609 pyappbundler-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.926449 pyappbundler-0.1.2/
+-rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      730 2023-07-06 15:32:58.926449 pyappbundler-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.920447 pyappbundler-0.1.2/pyappbundler/
+-rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.2/pyappbundler/__init__.py
+-rw-rw-rw-   0        0        0     2544 2023-07-06 15:29:57.000000 pyappbundler-0.1.2/pyappbundler/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-07-06 15:07:54.000000 pyappbundler-0.1.2/pyappbundler/_version.py
+-rw-rw-rw-   0        0        0     4879 2023-07-06 15:06:52.000000 pyappbundler-0.1.2/pyappbundler/pyappbundler.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.925448 pyappbundler-0.1.2/pyappbundler/templates/
+-rw-rw-rw-   0        0        0     1537 2023-07-05 15:18:33.000000 pyappbundler-0.1.2/pyappbundler/templates/iss.tmpl
+drwxrwxrwx   0        0        0        0 2023-07-06 15:32:58.924448 pyappbundler-0.1.2/pyappbundler.egg-info/
+-rw-rw-rw-   0        0        0      730 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 15:32:58.000000 pyappbundler-0.1.2/pyappbundler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:32:58.926449 pyappbundler-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.2/setup.py
```

### Comparing `pyappbundler-0.1.1/LICENSE` & `pyappbundler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.1/PKG-INFO` & `pyappbundler-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.1
+Version: 0.1.2
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.1/pyappbundler/__main__.py` & `pyappbundler-0.1.2/pyappbundler/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,21 +11,25 @@
         (https://pyinstaller.org/en/stable). And then (for Windows), put it all into
         a setup file with Inno Setup (https://jrsoftware.org/isdl.php#stable).""",
 )
 
 parser.add_argument(
     '-t', '--target', required=True, help='target python script')
 parser.add_argument(
-    '-a', '--app-name', required=True, help='application name')
+    '-a', '--app-name', default='',
+    help="""Application name.
+        If not specified, then it calculates from "target" value.""")
 parser.add_argument(
     '-i', '--icon', required=True, help='application icon')
 parser.add_argument(
-    '-g', '--app-guid', required=True, help='application GUID')
+    '-g', '--app-guid', default='',
+    help='Application GUID. Required for setup building!')
 parser.add_argument(
-    '-v', '--app-ver', required=True, help='application version')
+    '-v', '--app-ver', default='',
+    help='Application version. Required for setup building!')
 
 parser.add_argument(
     '-r', '--res-dir', action="extend", nargs=1,
     help="""Directory with additional files to be added to the executable.
         Multiple definitions are allowed.""")
 parser.add_argument(
     '-f', '--pyinst-flag', action="extend", nargs=1,
@@ -52,24 +56,21 @@
 #
 logging.basicConfig(
     format='%(levelname)s: %(message)s',
     level=logging.INFO,
 )
 
 #
+bundler_args = {
+    'target': args.target, 'app_name': args.app_name, 'icon': args.icon,
+    'dist': args.dist_dir, 'build': args.build_dir,
+    'res_dirs': args.res_dir, 'pyinst_flags': args.pyinst_flag,
+    'no_clean_dist': args.no_clean_dist,
+}
+
 if args.no_setup:
-    exe(
-        args.target,
-        app_name=args.app_name, icon=args.icon,
-        dist=args.dist_dir, build=args.build_dir,
-        res_dirs=args.res_dir, pyinst_flags=args.pyinst_flag,
-        no_clean_dist=args.no_clean_dist,
-    )
+    exe(**bundler_args)
 else:
-    exe_and_setup(
-        args.target,
-        app_name=args.app_name, icon=args.icon,
-        app_guid=args.app_guid, app_ver=args.app_ver,
-        dist=args.dist_dir, build=args.build_dir,
-        res_dirs=args.res_dir, pyinst_flags=args.pyinst_flag,
-        no_clean_dist=args.no_clean_dist,
-    )
+    bundler_args['app_guid'] = args.app_guid
+    bundler_args['app_ver'] = args.app_ver
+
+    exe_and_setup(**bundler_args)
```

### Comparing `pyappbundler-0.1.1/pyappbundler/templates/iss.tmpl` & `pyappbundler-0.1.2/pyappbundler/templates/iss.tmpl`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.1/pyappbundler.egg-info/PKG-INFO` & `pyappbundler-0.1.2/pyappbundler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.1
+Version: 0.1.2
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.1/pyproject.toml` & `pyappbundler-0.1.2/pyproject.toml`

 * *Files identical despite different names*

