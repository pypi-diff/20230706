# Comparing `tmp/pizazz-1.3.4.tar.gz` & `tmp/pizazz-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizazz-1.3.4.tar", last modified: Thu Jul  6 06:54:23 2023, max compression
+gzip compressed data, was "pizazz-1.3.5.tar", last modified: Thu Jul  6 07:01:06 2023, max compression
```

## Comparing `pizazz-1.3.4.tar` & `pizazz-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.229168 pizazz-1.3.4/
--rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 pizazz-1.3.4/AUTHORS.md
--rw-rw-rw-   0        0        0     1912 2023-07-06 06:54:09.000000 pizazz-1.3.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.4/LICENSE
--rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0    11614 2023-07-06 06:54:23.229168 pizazz-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-07-06 06:52:54.000000 pizazz-1.3.4/README.md
--rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.4/pyproject.toml
--rw-rw-rw-   0        0        0     1473 2023-07-06 06:54:23.235690 pizazz-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      115 2023-04-21 12:33:15.000000 pizazz-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.166666 pizazz-1.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.213536 pizazz-1.3.4/src/pizazz/
--rw-rw-rw-   0        0        0      356 2023-07-06 06:54:10.000000 pizazz-1.3.4/src/pizazz/__init__.py
--rw-rw-rw-   0        0        0     8109 2023-04-21 12:33:15.000000 pizazz-1.3.4/src/pizazz/pizazz.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.229168 pizazz-1.3.4/src/pizazz.egg-info/
--rw-rw-rw-   0        0        0    11614 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 07:01:06.117352 pizazz-1.3.5/
+-rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 pizazz-1.3.5/AUTHORS.md
+-rw-rw-rw-   0        0        0     2069 2023-07-06 07:00:54.000000 pizazz-1.3.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    11614 2023-07-06 07:01:06.117352 pizazz-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-07-06 06:52:54.000000 pizazz-1.3.5/README.md
+-rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1473 2023-07-06 07:01:06.117352 pizazz-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      115 2023-04-21 12:33:15.000000 pizazz-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:01:06.070559 pizazz-1.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 07:01:06.101824 pizazz-1.3.5/src/pizazz/
+-rw-rw-rw-   0        0        0      356 2023-07-06 07:00:54.000000 pizazz-1.3.5/src/pizazz/__init__.py
+-rw-rw-rw-   0        0        0     8109 2023-04-21 12:33:15.000000 pizazz-1.3.5/src/pizazz/pizazz.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:01:06.101824 pizazz-1.3.5/src/pizazz.egg-info/
+-rw-rw-rw-   0        0        0    11614 2023-07-06 07:01:06.000000 pizazz-1.3.5/src/pizazz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-07-06 07:01:06.000000 pizazz-1.3.5/src/pizazz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:01:06.000000 pizazz-1.3.5/src/pizazz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-06 07:01:06.000000 pizazz-1.3.5/src/pizazz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 07:01:06.000000 pizazz-1.3.5/src/pizazz.egg-info/top_level.txt
```

### Comparing `pizazz-1.3.4/CHANGELOG.md` & `pizazz-1.3.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.5 (2023-07-06)
+### Fix
+* Citation file ([`2d3afbb`](https://github.com/Stephen-RA-King/pizazz/commit/2d3afbbd69f16a205206fab81144df6635bbcf7e))
+
 ## v1.3.4 (2023-07-06)
 ### Fix
 * Corrupted files ([`f97229a`](https://github.com/Stephen-RA-King/pizazz/commit/f97229ab6b1630ae4c6fdbf8fdba78bb4292553e))
 
 ## v1.3.3 (2023-07-06)
 ### Documentation
 * Add citation ([`4d52948`](https://github.com/Stephen-RA-King/pizazz/commit/4d529489fe3fbf05472390c1cedcbd05f7f5d432))
```

### Comparing `pizazz-1.3.4/LICENSE` & `pizazz-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.4/PKG-INFO` & `pizazz-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizazz
-Version: 1.3.4
+Version: 1.3.5
 Summary: Easy configuration and control of 74HC595 Shift Registers on a Raspberry Pi
 Home-page: https://github.com/stephen-ra-king/pizazz
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pizazz-1.3.4/README.md` & `pizazz-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.4/pyproject.toml` & `pizazz-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.4/setup.cfg` & `pizazz-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.4/src/pizazz/pizazz.py` & `pizazz-1.3.5/src/pizazz/pizazz.py`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.4/src/pizazz.egg-info/PKG-INFO` & `pizazz-1.3.5/src/pizazz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizazz
-Version: 1.3.4
+Version: 1.3.5
 Summary: Easy configuration and control of 74HC595 Shift Registers on a Raspberry Pi
 Home-page: https://github.com/stephen-ra-king/pizazz
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

