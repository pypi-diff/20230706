# Comparing `tmp/tui-menu-0.1.6.tar.gz` & `tmp/tui_menu-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui-menu-0.1.6.tar", last modified: Sat Jul  1 11:20:30 2023, max compression
+gzip compressed data, was "tui_menu-0.1.7.tar", last modified: Thu Jul  6 20:15:25 2023, max compression
```

## Comparing `tui-menu-0.1.6.tar` & `tui_menu-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 11:20:30.458062 tui-menu-0.1.6/
--rw-r--r--   0 avili      (501) staff       (20)    35149 2023-07-01 10:44:37.000000 tui-menu-0.1.6/LICENSE
--rw-r--r--   0 avili      (501) staff       (20)      971 2023-07-01 11:20:30.457922 tui-menu-0.1.6/PKG-INFO
--rw-r--r--   0 avili      (501) staff       (20)       57 2023-07-01 10:44:37.000000 tui-menu-0.1.6/README.md
--rw-r--r--   0 avili      (501) staff       (20)     1275 2023-07-01 10:58:37.000000 tui-menu-0.1.6/pyproject.toml
--rw-r--r--   0 avili      (501) staff       (20)       38 2023-07-01 11:20:30.458109 tui-menu-0.1.6/setup.cfg
--rw-r--r--   0 avili      (501) staff       (20)     1378 2023-07-01 11:03:01.000000 tui-menu-0.1.6/setup.py
-drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 11:20:30.456940 tui-menu-0.1.6/tui-menu/
--rwxr-xr-x   0 avili      (501) staff       (20)     7205 2023-07-01 10:48:57.000000 tui-menu-0.1.6/tui-menu/Menu.py
--rw-r--r--   0 avili      (501) staff       (20)      148 2023-07-01 10:50:01.000000 tui-menu-0.1.6/tui-menu/__init__.py
-drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 11:20:30.457712 tui-menu-0.1.6/tui_menu.egg-info/
--rw-r--r--   0 avili      (501) staff       (20)      971 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/PKG-INFO
--rw-r--r--   0 avili      (501) staff       (20)      238 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/SOURCES.txt
--rw-r--r--   0 avili      (501) staff       (20)        1 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/dependency_links.txt
--rw-r--r--   0 avili      (501) staff       (20)       28 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/requires.txt
--rw-r--r--   0 avili      (501) staff       (20)        9 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/top_level.txt
+drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-06 20:15:25.597210 tui_menu-0.1.7/
+-rw-r--r--   0 avili      (501) staff       (20)    35149 2023-07-01 10:44:37.000000 tui_menu-0.1.7/LICENSE
+-rw-r--r--   0 avili      (501) staff       (20)     2564 2023-07-06 20:15:25.597094 tui_menu-0.1.7/PKG-INFO
+-rw-r--r--   0 avili      (501) staff       (20)     1650 2023-07-05 14:37:14.000000 tui_menu-0.1.7/README.md
+-rw-r--r--   0 avili      (501) staff       (20)     1275 2023-07-04 16:54:10.000000 tui_menu-0.1.7/pyproject.toml
+-rw-r--r--   0 avili      (501) staff       (20)       38 2023-07-06 20:15:25.597247 tui_menu-0.1.7/setup.cfg
+-rw-r--r--   0 avili      (501) staff       (20)     1378 2023-07-04 16:56:06.000000 tui_menu-0.1.7/setup.py
+drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-06 20:15:25.596314 tui_menu-0.1.7/tui_menu/
+-rwxr-xr-x   0 avili      (501) staff       (20)     7205 2023-07-01 10:48:57.000000 tui_menu-0.1.7/tui_menu/Menu.py
+-rw-r--r--   0 avili      (501) staff       (20)      148 2023-07-05 14:37:52.000000 tui_menu-0.1.7/tui_menu/__init__.py
+drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-06 20:15:25.596928 tui_menu-0.1.7/tui_menu.egg-info/
+-rw-r--r--   0 avili      (501) staff       (20)     2564 2023-07-06 20:15:25.000000 tui_menu-0.1.7/tui_menu.egg-info/PKG-INFO
+-rw-r--r--   0 avili      (501) staff       (20)      238 2023-07-06 20:15:25.000000 tui_menu-0.1.7/tui_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 avili      (501) staff       (20)        1 2023-07-06 20:15:25.000000 tui_menu-0.1.7/tui_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 avili      (501) staff       (20)       28 2023-07-06 20:15:25.000000 tui_menu-0.1.7/tui_menu.egg-info/requires.txt
+-rw-r--r--   0 avili      (501) staff       (20)        9 2023-07-06 20:15:25.000000 tui_menu-0.1.7/tui_menu.egg-info/top_level.txt
```

### Comparing `tui-menu-0.1.6/LICENSE` & `tui_menu-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tui-menu-0.1.6/pyproject.toml` & `tui_menu-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools >= 65",
     "wheel >= 0.38",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "tui-menu"
+name = "tui_menu"
 dynamic = ["version"]
 description = "A module for TUI Menu driven application"
 readme = "README.md"
 requires-python = ">=3"
 license = {file = "LICENSE.txt"}
 keywords = ["console", "menu", "tui"]
 authors = [
@@ -34,14 +34,14 @@
 
 dependencies = [
     "console>=0.9907",
     "ezenv>=0.92"
 ]
 
 [tool.setuptools.dynamic]
-version = {attr = "tui-menu.__version__"}
+version = {attr = "tui_menu.__version__"}
 
 [project.urls]
 # Homepage = "https://example.com"
 # Documentation = "https://readthedocs.org"
 Repository = "https://github.com/avili68/tui-menu"
 # Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
```

### Comparing `tui-menu-0.1.6/setup.py` & `tui_menu-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 setup(
-    name="tui-menu",
-    version=get_version("tui-menu/__init__.py"),
+    name="tui_menu",
+    version=get_version("tui_menu/__init__.py"),
     description="A module for TUI Menu driven application",
     url="https://github.com/avili68/tui-menu",
     author="Avi Liani",
     author_email="avi@liani.co.il",
     license="GPL",
-    packages=["tui-menu"],
+    packages=["tui_menu"],
     install_requires=["console>=0.9907", "ezenv>=0.92"],
     python_requires=">=3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `tui-menu-0.1.6/tui-menu/Menu.py` & `tui_menu-0.1.7/tui_menu/Menu.py`

 * *Files identical despite different names*

