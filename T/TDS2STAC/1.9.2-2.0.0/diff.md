# Comparing `tmp/TDS2STAC-1.9.2.tar.gz` & `tmp/TDS2STAC-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDS2STAC-1.9.2.tar", last modified: Wed Feb  8 06:52:33 2023, max compression
+gzip compressed data, was "TDS2STAC-2.0.0.tar", last modified: Thu Jul  6 11:09:45 2023, max compression
```

## Comparing `TDS2STAC-1.9.2.tar` & `TDS2STAC-2.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-02-08 06:52:33.210288 TDS2STAC-1.9.2/
--rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/AUTHORS.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     3603 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/CONTRIBUTING.rst
--rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/LICENSE
--rw-r--r--   0 hadizadeh-m (15144)      901      389 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/MANIFEST.in
--rw-r--r--   0 hadizadeh-m (15144)      901    10706 2023-02-08 06:52:33.210391 TDS2STAC-1.9.2/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901     9299 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/README.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-02-08 06:52:33.208188 TDS2STAC-1.9.2/TDS2STAC.egg-info/
--rw-r--r--   0 hadizadeh-m (15144)      901    10706 2023-02-08 06:52:33.000000 TDS2STAC-1.9.2/TDS2STAC.egg-info/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901      638 2023-02-08 06:52:33.000000 TDS2STAC-1.9.2/TDS2STAC.egg-info/SOURCES.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-02-08 06:52:33.000000 TDS2STAC-1.9.2/TDS2STAC.egg-info/dependency_links.txt
--rw-r--r--   0 hadizadeh-m (15144)      901      326 2023-02-08 06:52:33.000000 TDS2STAC-1.9.2/TDS2STAC.egg-info/requires.txt
--rw-r--r--   0 hadizadeh-m (15144)      901       15 2023-02-08 06:52:33.000000 TDS2STAC-1.9.2/TDS2STAC.egg-info/top_level.txt
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-02-08 06:52:33.209215 TDS2STAC-1.9.2/docs/
--rw-r--r--   0 hadizadeh-m (15144)      901      609 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/Makefile
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/authors.rst
--rwxr-xr-x   0 hadizadeh-m (15144)      901     4816 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/conf.py
--rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/contributing.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/history.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      296 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/index.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     1174 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/installation.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      806 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/make.bat
--rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/readme.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       71 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/docs/usage.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      181 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/pyproject.toml
--rw-r--r--   0 hadizadeh-m (15144)      901      195 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/requirements_dev.txt
--rw-r--r--   0 hadizadeh-m (15144)      901     1896 2023-02-08 06:52:33.210801 TDS2STAC-1.9.2/setup.cfg
--rw-r--r--   0 hadizadeh-m (15144)      901      299 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/setup.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-02-08 06:52:33.210938 TDS2STAC-1.9.2/tds2stac/
--rw-r--r--   0 hadizadeh-m (15144)      901       99 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/tds2stac/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-02-08 06:52:33.210969 TDS2STAC-1.9.2/tds2stac/_version.py
--rw-r--r--   0 hadizadeh-m (15144)      901      402 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/tds2stac/cli.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1029 2023-02-08 06:36:03.000000 TDS2STAC-1.9.2/tds2stac/config_pgstac.py
--rw-r--r--   0 hadizadeh-m (15144)      901      949 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/tds2stac/constants.py
--rw-r--r--   0 hadizadeh-m (15144)      901     2012 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/tds2stac/funcs.py
--rw-r--r--   0 hadizadeh-m (15144)      901    49129 2023-02-08 06:48:03.000000 TDS2STAC-1.9.2/tds2stac/tds2stac.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-02-08 06:52:33.210196 TDS2STAC-1.9.2/tests/
--rw-r--r--   0 hadizadeh-m (15144)      901       38 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/tests/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      986 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/tests/test_tds2stac.py
--rw-r--r--   0 hadizadeh-m (15144)      901    83607 2023-02-08 06:32:33.000000 TDS2STAC-1.9.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.340764 TDS2STAC-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    13807 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10810 2023-07-06 11:09:45.340764 TDS2STAC-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.338764 TDS2STAC-2.0.0/TDS2STAC.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10810 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.338764 TDS2STAC-2.0.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/authors.rst
+-rwxr-xr-x   0 root         (0) root         (0)     4870 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/history.rst
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/readme.rst
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/usage.rst
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-07-06 11:09:45.341764 TDS2STAC-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.341764 TDS2STAC-2.0.0/tds2stac/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-06 11:09:45.341764 TDS2STAC-2.0.0/tds2stac/_version.py
+-rw-r--r--   0 root         (0) root         (0)    54920 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/app.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/cli.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7868 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/core.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.340764 TDS2STAC-2.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tests/test_tds2stac.py
+-rw-r--r--   0 root         (0) root         (0)    84134 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/versioneer.py
```

### Comparing `TDS2STAC-1.9.2/CONTRIBUTING.rst` & `TDS2STAC-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-1.9.2/LICENSE` & `TDS2STAC-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TDS2STAC-1.9.2/PKG-INFO` & `TDS2STAC-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 1.9.2
+Version: 2.0.0
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
@@ -32,16 +32,21 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 TDS2STAC
 ========
 
+.. image:: https://codebase.helmholtz.cloud/cat4kit/tds2stac/-/raw/main/tds2stac-logo.png
 
 
+
+
+=========
+
 .. image:: https://img.shields.io/pypi/v/tds2stac.svg
         :target: https://pypi.python.org/pypi/tds2stac
 
 .. image:: https://readthedocs.org/projects/tds2stac/badge/?version=latest
         :target: https://tds2stac.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
@@ -159,7 +164,8 @@
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the EUPL-1.2 license for more details.
 
 You should have received a copy of the EUPL-1.2 license along with this
 program. If not, see https://www.eupl.eu/.
 
+
```

### Comparing `TDS2STAC-1.9.2/README.rst` & `TDS2STAC-2.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 ========
 TDS2STAC
 ========
 
+.. image:: https://codebase.helmholtz.cloud/cat4kit/tds2stac/-/raw/main/tds2stac-logo.png
 
 
+
+
+=========
+
 .. image:: https://img.shields.io/pypi/v/tds2stac.svg
         :target: https://pypi.python.org/pypi/tds2stac
 
 .. image:: https://readthedocs.org/projects/tds2stac/badge/?version=latest
         :target: https://tds2stac.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
@@ -123,8 +128,8 @@
 Licensed under the EUPL-1.2-or-later
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the EUPL-1.2 license for more details.
 
 You should have received a copy of the EUPL-1.2 license along with this
-program. If not, see https://www.eupl.eu/.
+program. If not, see https://www.eupl.eu/.
```

### Comparing `TDS2STAC-1.9.2/TDS2STAC.egg-info/PKG-INFO` & `TDS2STAC-2.0.0/TDS2STAC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 1.9.2
+Version: 2.0.0
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
@@ -32,16 +32,21 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 TDS2STAC
 ========
 
+.. image:: https://codebase.helmholtz.cloud/cat4kit/tds2stac/-/raw/main/tds2stac-logo.png
 
 
+
+
+=========
+
 .. image:: https://img.shields.io/pypi/v/tds2stac.svg
         :target: https://pypi.python.org/pypi/tds2stac
 
 .. image:: https://readthedocs.org/projects/tds2stac/badge/?version=latest
         :target: https://tds2stac.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
@@ -159,7 +164,8 @@
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the EUPL-1.2 license for more details.
 
 You should have received a copy of the EUPL-1.2 license along with this
 program. If not, see https://www.eupl.eu/.
 
+
```

### Comparing `TDS2STAC-1.9.2/TDS2STAC.egg-info/SOURCES.txt` & `TDS2STAC-2.0.0/TDS2STAC.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tds2stac/__init__.py
 tds2stac/_version.py
+tds2stac/app.py
 tds2stac/cli.py
-tds2stac/config_pgstac.py
 tds2stac/constants.py
-tds2stac/funcs.py
-tds2stac/tds2stac.py
+tds2stac/core.py
+tds2stac/utils.py
 tests/__init__.py
 tests/test_tds2stac.py
```

### Comparing `TDS2STAC-1.9.2/docs/Makefile` & `TDS2STAC-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TDS2STAC-1.9.2/docs/conf.py` & `TDS2STAC-2.0.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,42 +15,43 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 import tds2stac
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'TDS2STAC'
+project = "TDS2STAC"
 copyright = "2023, Mostafa Hadizadeh"
 author = "Mostafa Hadizadeh"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
@@ -65,98 +66,95 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'tds2stacdoc'
+htmlhelp_basename = "tds2stacdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'tds2stac.tex',
-     'TDS2STAC Documentation',
-     'Mostafa Hadizadeh', 'manual'),
+    (
+        master_doc,
+        "tds2stac.tex",
+        "TDS2STAC Documentation",
+        "Mostafa Hadizadeh",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'tds2stac',
-     'TDS2STAC Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "tds2stac", "TDS2STAC Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'tds2stac',
-     'TDS2STAC Documentation',
-     author,
-     'tds2stac',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "tds2stac",
+        "TDS2STAC Documentation",
+        author,
+        "tds2stac",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
-
-
-
```

### Comparing `TDS2STAC-1.9.2/docs/installation.rst` & `TDS2STAC-2.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-1.9.2/docs/make.bat` & `TDS2STAC-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `TDS2STAC-1.9.2/setup.cfg` & `TDS2STAC-2.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 	autodocsumm
 	sphinxcontrib-django
 
 [mypy]
 ignore_missing_imports = True
 
 [versioneer]
-VCS = git
+vcs = git
 style = pep440
 versionfile_source = tds2stac/_version.py
 versionfile_build = tds2stac/_version.py
 tag_prefix = 
 parentdir_prefix = 
 
 [bdist_wheel]
```

### Comparing `TDS2STAC-1.9.2/versioneer.py` & `TDS2STAC-2.0.0/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -344,33 +343,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(my_path), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -380,29 +383,29 @@
     # the top of versioneer.py for instructions on writing your setup.cfg .
     root = Path(root)
     pyproject_toml = root / "pyproject.toml"
     setup_cfg = root / "setup.cfg"
     section = None
     if pyproject_toml.exists() and have_tomllib:
         try:
-            with open(pyproject_toml, 'rb') as fobj:
+            with open(pyproject_toml, "rb") as fobj:
                 pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
+            section = pp["tool"]["versioneer"]
         except (tomllib.TOMLDecodeError, KeyError):
             pass
     if not section:
         parser = configparser.ConfigParser()
         with open(setup_cfg) as cfg_file:
             parser.read_file(cfg_file)
         parser.get("versioneer", "VCS")  # raise error if missing
 
         section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
+    cfg.VCS = section["VCS"]
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
     if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
@@ -417,23 +420,26 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands, args, cwd=None, verbose=False, hide_stderr=False, env=None
+):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
 
     popen_kwargs = {}
     if sys.platform == "win32":
         # This hides the console window if pythonw.exe is used
@@ -441,18 +447,22 @@
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
         popen_kwargs["startupinfo"] = startupinfo
 
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
+            )
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -467,15 +477,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = r'''
+LONG_VERSION_PY[
+    "git"
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain.
@@ -1183,49 +1195,56 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
-            if not re.match(r'\d', r):
+            if not re.match(r"\d", r):
                 continue
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
@@ -1239,43 +1258,54 @@
     # GIT_DIR can interfere with correct operation of Versioneer.
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
     env.pop("GIT_DIR", None)
     runner = functools.partial(runner, env=env)
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    _, rc = runner(
+        GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose
+    )
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            f"{tag_prefix}[[:digit:]]*",
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
+    branch_name, rc = runner(
+        GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root
+    )
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
     if branch_name == "HEAD":
         # If we aren't exactly on a branch, pick a branch which represents
@@ -1307,52 +1337,57 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = (
+                "unable to parse git-describe output: '%s'" % describe_out
+            )
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
         out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
         pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
+        0
+    ].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
@@ -1403,23 +1438,29 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1440,29 +1481,36 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+        contents,
+        re.M | re.S,
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+            contents,
+            re.M | re.S,
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(
+        versions, sort_keys=True, indent=1, separators=(",", ": ")
+    )
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1486,16 +1534,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
@@ -1516,16 +1563,15 @@
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
         rendered = "0"
         if pieces["branch"] != "master":
             rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
@@ -1542,18 +1588,23 @@
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            tag_version, post_version = pep440_split_post(
+                pieces["closest-tag"]
+            )
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+                rendered += ".post%d.dev%d" % (
+                    post_version + 1,
+                    pieces["distance"],
+                )
             else:
                 rendered += ".post0.dev%d" % (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
@@ -1678,19 +1729,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-branch":
@@ -1706,17 +1759,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1731,16 +1788,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1786,17 +1844,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1841,14 +1903,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1862,16 +1925,16 @@
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
     # pip install -e . and setuptool/editable_wheel will invoke build_py
     # but the build_py command is not expected to copy any files.
 
     # we override different "build_py" commands for both environments
-    if 'build_py' in cmds:
-        _build_py = cmds['build_py']
+    if "build_py" in cmds:
+        _build_py = cmds["build_py"]
     else:
         from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1880,22 +1943,24 @@
             if getattr(self, "editable_mode", False):
                 # During editable installs `.py` and data files are
                 # not copied to build_lib
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(
+                    self.build_lib, cfg.versionfile_build
+                )
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
-    if 'build_ext' in cmds:
-        _build_ext = cmds['build_ext']
+    if "build_ext" in cmds:
+        _build_ext = cmds["build_ext"]
     else:
         from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1907,27 +1972,32 @@
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if not cfg.versionfile_build:
                 return
-            target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
+            target_versionfile = os.path.join(
+                self.build_lib, cfg.versionfile_build
+            )
             if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
                 return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
+
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1940,25 +2010,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
             from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1969,63 +2043,70 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info = cmds['egg_info']
+    if "egg_info" in cmds:
+        _egg_info = cmds["egg_info"]
     else:
         from setuptools.command.egg_info import egg_info as _egg_info
 
     class cmd_egg_info(_egg_info):
         def find_sources(self):
             # egg_info.find_sources builds the manifest list and writes it
             # in one shot
             super().find_sources()
 
             # Modify the filelist and normalize it
             root = get_root()
             cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
+            self.filelist.append("versioneer.py")
             if cfg.versionfile_source:
                 # There are rare cases where versionfile_source might not be
                 # included by default, so we must be explicit
                 self.filelist.append(cfg.versionfile_source)
             self.filelist.sort()
             self.filelist.remove_duplicates()
 
             # The write method is hidden in the manifest_maker instance that
             # generated the filelist and was thrown away
             # We will instead replicate their final normalization (to unicode,
             # and POSIX-style paths)
             from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
 
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
 
-    cmds['egg_info'] = cmd_egg_info
+    cmds["egg_info"] = cmd_egg_info
 
     # we override different "sdist" commands for both environments
-    if 'sdist' in cmds:
-        _sdist = cmds['sdist']
+    if "sdist" in cmds:
+        _sdist = cmds["sdist"]
     else:
         from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
@@ -2039,16 +2120,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -2100,36 +2183,43 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        OSError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print(
+                "Adding sample versioneer config to setup.cfg", file=sys.stderr
+            )
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
```

