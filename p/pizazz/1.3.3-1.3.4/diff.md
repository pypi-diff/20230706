# Comparing `tmp/pizazz-1.3.3.tar.gz` & `tmp/pizazz-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizazz-1.3.3.tar", last modified: Thu Jul  6 06:18:23 2023, max compression
+gzip compressed data, was "pizazz-1.3.4.tar", last modified: Thu Jul  6 06:54:23 2023, max compression
```

## Comparing `pizazz-1.3.3.tar` & `pizazz-1.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 06:18:23.784201 pizazz-1.3.3/
--rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 pizazz-1.3.3/AUTHORS.md
--rw-rw-rw-   0        0        0     1753 2023-07-06 06:18:10.000000 pizazz-1.3.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      986 2023-07-06 06:18:23.784201 pizazz-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-06 06:17:09.000000 pizazz-1.3.3/README.md
--rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0     1473 2023-07-06 06:18:23.784201 pizazz-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      115 2023-04-21 12:33:15.000000 pizazz-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:18:23.746870 pizazz-1.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 06:18:23.768560 pizazz-1.3.3/src/pizazz/
--rw-rw-rw-   0        0        0      356 2023-07-06 06:18:11.000000 pizazz-1.3.3/src/pizazz/__init__.py
--rw-rw-rw-   0        0        0     8109 2023-04-21 12:33:15.000000 pizazz-1.3.3/src/pizazz/pizazz.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:18:23.784201 pizazz-1.3.3/src/pizazz.egg-info/
--rw-rw-rw-   0        0        0      986 2023-07-06 06:18:23.000000 pizazz-1.3.3/src/pizazz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-07-06 06:18:23.000000 pizazz-1.3.3/src/pizazz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 06:18:23.000000 pizazz-1.3.3/src/pizazz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-06 06:18:23.000000 pizazz-1.3.3/src/pizazz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 06:18:23.000000 pizazz-1.3.3/src/pizazz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.229168 pizazz-1.3.4/
+-rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 pizazz-1.3.4/AUTHORS.md
+-rw-rw-rw-   0        0        0     1912 2023-07-06 06:54:09.000000 pizazz-1.3.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    11614 2023-07-06 06:54:23.229168 pizazz-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-07-06 06:52:54.000000 pizazz-1.3.4/README.md
+-rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1473 2023-07-06 06:54:23.235690 pizazz-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      115 2023-04-21 12:33:15.000000 pizazz-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.166666 pizazz-1.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.213536 pizazz-1.3.4/src/pizazz/
+-rw-rw-rw-   0        0        0      356 2023-07-06 06:54:10.000000 pizazz-1.3.4/src/pizazz/__init__.py
+-rw-rw-rw-   0        0        0     8109 2023-04-21 12:33:15.000000 pizazz-1.3.4/src/pizazz/pizazz.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:54:23.229168 pizazz-1.3.4/src/pizazz.egg-info/
+-rw-rw-rw-   0        0        0    11614 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 06:54:23.000000 pizazz-1.3.4/src/pizazz.egg-info/top_level.txt
```

### Comparing `pizazz-1.3.3/CHANGELOG.md` & `pizazz-1.3.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.4 (2023-07-06)
+### Fix
+* Corrupted files ([`f97229a`](https://github.com/Stephen-RA-King/pizazz/commit/f97229ab6b1630ae4c6fdbf8fdba78bb4292553e))
+
 ## v1.3.3 (2023-07-06)
 ### Documentation
 * Add citation ([`4d52948`](https://github.com/Stephen-RA-King/pizazz/commit/4d529489fe3fbf05472390c1cedcbd05f7f5d432))
 
 ## v1.3.2 (2023-07-06)
 ### Documentation
 * Update hyperlinks ([`bc1fa76`](https://github.com/Stephen-RA-King/pizazz/commit/bc1fa7627be96cff136eaaa27aa002c26db17aed))
```

### Comparing `pizazz-1.3.3/LICENSE` & `pizazz-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.3/pyproject.toml` & `pizazz-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.3/setup.cfg` & `pizazz-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.3/src/pizazz/pizazz.py` & `pizazz-1.3.4/src/pizazz/pizazz.py`

 * *Files identical despite different names*

