# Comparing `tmp/batcave-42.1.0.tar.gz` & `tmp/batcave-42.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batcave-42.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "batcave-42.1.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `batcave-42.1.0.tar` & `batcave-42.1.0rc0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     4792 2023-07-05 22:46:39.766550 batcave-42.1.0/.gitignore
--rw-r--r--   0        0        0     3569 2023-07-05 22:46:39.766550 batcave-42.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0       23 2023-07-05 22:46:39.766550 batcave-42.1.0/.p4cfg
--rw-r--r--   0        0        0     5043 2023-07-05 22:46:39.766550 batcave-42.1.0/.p4ignore
--rw-r--r--   0        0        0      158 2023-07-05 22:46:39.766550 batcave-42.1.0/.pypirc
--rw-r--r--   0        0        0       39 2023-07-05 22:46:39.766550 batcave-42.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     4034 2023-07-05 22:46:39.766550 batcave-42.1.0/.vscode/.ropeproject/config.py
--rw-r--r--   0        0        0      592 2023-07-05 22:46:39.766550 batcave-42.1.0/.vscode/.ropeproject/objectdb
--rw-r--r--   0        0        0     5757 2023-07-05 22:46:39.766550 batcave-42.1.0/.vscode/launch.json
--rw-r--r--   0        0        0      468 2023-07-05 22:46:39.766550 batcave-42.1.0/.vscode/tasks.json
--rw-r--r--   0        0        0    38715 2023-07-05 22:46:39.766550 batcave-42.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       86 2023-07-05 22:46:39.766550 batcave-42.1.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2023-07-05 22:46:39.766550 batcave-42.1.0/LICENSE
--rw-r--r--   0        0        0       93 2023-07-05 22:46:39.766550 batcave-42.1.0/MANIFEST.in
--rw-r--r--   0        0        0     1017 2023-07-05 22:46:39.766550 batcave-42.1.0/README.md
--rw-r--r--   0        0        0     1832 2023-07-05 22:47:06.296996 batcave-42.1.0/batcave/__init__.py
--rw-r--r--   0        0        0     5483 2023-07-05 22:46:39.767550 batcave-42.1.0/batcave/automation.py
--rw-r--r--   0        0        0    14410 2023-07-05 22:46:39.767550 batcave-42.1.0/batcave/cloudmgr.py
--rw-r--r--   0        0        0    74524 2023-07-05 22:46:39.767550 batcave-42.1.0/batcave/cms.py
--rw-r--r--   0        0        0     8590 2023-07-05 22:46:39.767550 batcave-42.1.0/batcave/commander.py
--rw-r--r--   0        0        0     9592 2023-07-05 22:46:39.767550 batcave-42.1.0/batcave/configmgr.py
--rw-r--r--   0        0        0    27694 2023-07-05 22:46:39.767550 batcave-42.1.0/batcave/data.py
--rw-r--r--   0        0        0    31760 2023-07-05 22:46:39.767550 batcave-42.1.0/batcave/expander.py
--rw-r--r--   0        0        0     8908 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/fileutil.py
--rw-r--r--   0        0        0    10747 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/gui.py
--rw-r--r--   0        0        0    28879 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/iispy.py
--rw-r--r--   0        0        0    17890 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/k8s.py
--rw-r--r--   0        0        0    10608 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/lang.py
--rw-r--r--   0        0        0     3035 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/menu.py
--rw-r--r--   0        0        0     2378 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/netutil.py
--rw-r--r--   0        0        0     3842 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/platarch.py
--rw-r--r--   0        0        0        0 2023-07-05 22:46:39.793551 batcave-42.1.0/batcave/py.typed
--rw-r--r--   0        0        0    13106 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/qbpy.py
--rw-r--r--   0        0        0    28247 2023-07-05 22:46:39.768550 batcave-42.1.0/batcave/reporter.py
--rw-r--r--   0        0        0    52861 2023-07-05 22:46:39.769550 batcave-42.1.0/batcave/servermgr.py
--rw-r--r--   0        0        0    11200 2023-07-05 22:46:39.769550 batcave-42.1.0/batcave/serverpath.py
--rw-r--r--   0        0        0     7801 2023-07-05 22:46:39.769550 batcave-42.1.0/batcave/statemachine.py
--rw-r--r--   0        0        0    23468 2023-07-05 22:46:39.769550 batcave-42.1.0/batcave/sysutil.py
--rw-r--r--   0        0        0     5429 2023-07-05 22:46:39.769550 batcave-42.1.0/batcave/tcpy.py
--rw-r--r--   0        0        0     3342 2023-07-05 22:46:39.769550 batcave-42.1.0/batcave/time.py
--rw-r--r--   0        0        0     3340 2023-07-05 22:46:39.769550 batcave-42.1.0/batcave/version.py
--rw-r--r--   0        0        0      634 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/Makefile
--rw-r--r--   0        0        0     3747 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/batcave.rst
--rw-r--r--   0        0        0     9167 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2109 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/conf.py
--rw-r--r--   0        0        0      469 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/make.bat
--rw-r--r--   0        0        0       65 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2023-07-05 22:46:39.769550 batcave-42.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     2826 2023-07-05 22:47:06.296996 batcave-42.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-05 22:46:39.769550 batcave-42.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1253 2023-07-05 22:46:39.770550 batcave-42.1.0/tests/test_lang.py
--rw-r--r--   0        0        0     2744 2023-07-05 22:46:39.770550 batcave-42.1.0/tests/test_statemachine.py
--rw-r--r--   0        0        0     3062 2023-07-05 22:46:39.770550 batcave-42.1.0/tests/test_sysutil.py
--rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 batcave-42.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4792 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.gitignore
+-rw-r--r--   0        0        0     3569 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.gitlab-ci.yml
+-rw-r--r--   0        0        0       23 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.p4cfg
+-rw-r--r--   0        0        0     5043 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.p4ignore
+-rw-r--r--   0        0        0      158 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.pypirc
+-rw-r--r--   0        0        0       39 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.readthedocs.yml
+-rw-r--r--   0        0        0     4034 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.vscode/.ropeproject/config.py
+-rw-r--r--   0        0        0      592 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.vscode/.ropeproject/objectdb
+-rw-r--r--   0        0        0     5757 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.vscode/launch.json
+-rw-r--r--   0        0        0      468 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/.vscode/tasks.json
+-rw-r--r--   0        0        0    38715 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0       86 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/LICENSE
+-rw-r--r--   0        0        0       93 2023-07-05 22:29:39.492618 batcave-42.1.0rc0/MANIFEST.in
+-rw-r--r--   0        0        0     1017 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/README.md
+-rw-r--r--   0        0        0     1892 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/batcave/__init__.py
+-rw-r--r--   0        0        0     5483 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/batcave/automation.py
+-rw-r--r--   0        0        0    14410 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/batcave/cloudmgr.py
+-rw-r--r--   0        0        0    74524 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/batcave/cms.py
+-rw-r--r--   0        0        0     8590 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/batcave/commander.py
+-rw-r--r--   0        0        0     9592 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/batcave/configmgr.py
+-rw-r--r--   0        0        0    27694 2023-07-05 22:29:39.493618 batcave-42.1.0rc0/batcave/data.py
+-rw-r--r--   0        0        0    31760 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/expander.py
+-rw-r--r--   0        0        0     8908 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/fileutil.py
+-rw-r--r--   0        0        0    10747 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/gui.py
+-rw-r--r--   0        0        0    28879 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/iispy.py
+-rw-r--r--   0        0        0    17890 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/k8s.py
+-rw-r--r--   0        0        0    10608 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/lang.py
+-rw-r--r--   0        0        0     3035 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/menu.py
+-rw-r--r--   0        0        0     2378 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/netutil.py
+-rw-r--r--   0        0        0     3842 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/platarch.py
+-rw-r--r--   0        0        0        0 2023-07-05 22:29:39.519617 batcave-42.1.0rc0/batcave/py.typed
+-rw-r--r--   0        0        0    13106 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/qbpy.py
+-rw-r--r--   0        0        0    28247 2023-07-05 22:29:39.494618 batcave-42.1.0rc0/batcave/reporter.py
+-rw-r--r--   0        0        0    52861 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/batcave/servermgr.py
+-rw-r--r--   0        0        0    11200 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/batcave/serverpath.py
+-rw-r--r--   0        0        0     7801 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/batcave/statemachine.py
+-rw-r--r--   0        0        0    23468 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/batcave/sysutil.py
+-rw-r--r--   0        0        0     5429 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/batcave/tcpy.py
+-rw-r--r--   0        0        0     3342 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/batcave/time.py
+-rw-r--r--   0        0        0     3340 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/batcave/version.py
+-rw-r--r--   0        0        0      634 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/Makefile
+-rw-r--r--   0        0        0     3747 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/batcave.rst
+-rw-r--r--   0        0        0     9167 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2109 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/conf.py
+-rw-r--r--   0        0        0      469 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/make.bat
+-rw-r--r--   0        0        0       65 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/docs/requirements.txt
+-rw-r--r--   0        0        0     2942 2023-07-05 22:29:39.495617 batcave-42.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-05 22:29:39.496618 batcave-42.1.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0     1253 2023-07-05 22:29:39.496618 batcave-42.1.0rc0/tests/test_lang.py
+-rw-r--r--   0        0        0     2744 2023-07-05 22:29:39.496618 batcave-42.1.0rc0/tests/test_statemachine.py
+-rw-r--r--   0        0        0     3062 2023-07-05 22:29:39.496618 batcave-42.1.0rc0/tests/test_sysutil.py
+-rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 batcave-42.1.0rc0/PKG-INFO
```

### Comparing `batcave-42.1.0/.gitignore` & `batcave-42.1.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/.gitlab-ci.yml` & `batcave-42.1.0rc0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/.p4ignore` & `batcave-42.1.0rc0/.p4ignore`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/.vscode/.ropeproject/config.py` & `batcave-42.1.0rc0/.vscode/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/.vscode/.ropeproject/objectdb` & `batcave-42.1.0rc0/.vscode/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/.vscode/launch.json` & `batcave-42.1.0rc0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/CHANGELOG.md` & `batcave-42.1.0rc0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/LICENSE` & `batcave-42.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/README.md` & `batcave-42.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/__init__.py` & `batcave-42.1.0rc0/batcave/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-"""BatCave Utilities module.
-
-This module provides utilities for making it easier to write Python programs.
-
-The exported modules fall into several categories:
-
-Modules that provide simplified interfaces to standard modules:
-    * commander - argparse
-    * platarch - platform
-
-Modules that provide simplified interfaces to third-party modules:
-    * gui - PyQt5
-    * k8s - kubernetes
-
-Modules that provide Pythonic interfaces to external systems:
-    * cloudmgr - cloud resources
-    * cms - code management systems
-    * data - data sources
-    * iispy - Internet Information Server
-    * netutil - network services
-    * qbpy - QuickBuild
-    * servermgr - OS-independent servers
-    * sysutil - system utilities
-    * tcpy - TeamCity
-
-Modules that provide utilities for accomplishing specific programming tasks:
-    * automation - building automation
-    * configmgr - managing configurations
-    * expander - working with string expansion
-    * fileutil - working with files
-    * lang - Python language utilities
-    * menu - creating command line menus
-    * statemachine - a simple state machine
-    * reporter - creating reports
-    * version - reporting version information
-"""
-
-__all__ = ('__title__', '__summary__', '__uri__',
-           '__version__', '__build_name__', '__build_date__',
-           '__author__', '__email__',
-           '__license__', '__copyright__')
-
-__title__ = 'BatCave'
-__summary__ = 'Python Programming Toolkit'
-__uri__ = 'https://gitlab.com/arisilon/batcave/'
-
-__version__ = '42.1.0'
-__build_name__ = '{var:build_name}'
-__build_date__ = '{var:build_date}'
-
-__author__ = 'Jeffery G. Smith'
-__email__ = 'web@pobox.com'
-
-__license__ = 'MIT'
-__copyright__ = 'Copyright (c) 2023 Jeffery G. Smith'
-
-# cSpell:ignore iispy netutil qbpy tcpy platarch cloudmgr servermgr configmgr fileutil statemachine
+"""BatCave Utilities module.
+
+This module provides utilities for making it easier to write Python programs.
+
+The exported modules fall into several categories:
+
+Modules that provide simplified interfaces to standard modules:
+    * commander - argparse
+    * platarch - platform
+
+Modules that provide simplified interfaces to third-party modules:
+    * gui - PyQt5
+    * k8s - kubernetes
+
+Modules that provide Pythonic interfaces to external systems:
+    * cloudmgr - cloud resources
+    * cms - code management systems
+    * data - data sources
+    * iispy - Internet Information Server
+    * netutil - network services
+    * qbpy - QuickBuild
+    * servermgr - OS-independent servers
+    * sysutil - system utilities
+    * tcpy - TeamCity
+
+Modules that provide utilities for accomplishing specific programming tasks:
+    * automation - building automation
+    * configmgr - managing configurations
+    * expander - working with string expansion
+    * fileutil - working with files
+    * lang - Python language utilities
+    * menu - creating command line menus
+    * statemachine - a simple state machine
+    * reporter - creating reports
+    * version - reporting version information
+"""
+
+__all__ = ('__title__', '__summary__', '__uri__',
+           '__version__', '__build_name__', '__build_date__',
+           '__author__', '__email__',
+           '__license__', '__copyright__')
+
+__title__ = 'BatCave'
+__summary__ = 'Python Programming Toolkit'
+__uri__ = 'https://gitlab.com/arisilon/batcave/'
+
+__version__ = '42.1.0rc0'
+__build_name__ = '{var:build_name}'
+__build_date__ = '{var:build_date}'
+
+__author__ = 'Jeffery G. Smith'
+__email__ = 'web@pobox.com'
+
+__license__ = 'MIT'
+__copyright__ = 'Copyright (c) 2023 Jeffery G. Smith'
+
+# cSpell:ignore iispy netutil qbpy tcpy platarch cloudmgr servermgr configmgr fileutil statemachine
```

### Comparing `batcave-42.1.0/batcave/automation.py` & `batcave-42.1.0rc0/batcave/automation.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/cloudmgr.py` & `batcave-42.1.0rc0/batcave/cloudmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/cms.py` & `batcave-42.1.0rc0/batcave/cms.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/commander.py` & `batcave-42.1.0rc0/batcave/commander.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/configmgr.py` & `batcave-42.1.0rc0/batcave/configmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/data.py` & `batcave-42.1.0rc0/batcave/data.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/expander.py` & `batcave-42.1.0rc0/batcave/expander.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/fileutil.py` & `batcave-42.1.0rc0/batcave/fileutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/gui.py` & `batcave-42.1.0rc0/batcave/gui.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/iispy.py` & `batcave-42.1.0rc0/batcave/iispy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/k8s.py` & `batcave-42.1.0rc0/batcave/k8s.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/lang.py` & `batcave-42.1.0rc0/batcave/lang.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/menu.py` & `batcave-42.1.0rc0/batcave/menu.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/netutil.py` & `batcave-42.1.0rc0/batcave/netutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/platarch.py` & `batcave-42.1.0rc0/batcave/platarch.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/qbpy.py` & `batcave-42.1.0rc0/batcave/qbpy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/reporter.py` & `batcave-42.1.0rc0/batcave/reporter.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/servermgr.py` & `batcave-42.1.0rc0/batcave/servermgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/serverpath.py` & `batcave-42.1.0rc0/batcave/serverpath.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/statemachine.py` & `batcave-42.1.0rc0/batcave/statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/sysutil.py` & `batcave-42.1.0rc0/batcave/sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/tcpy.py` & `batcave-42.1.0rc0/batcave/tcpy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/time.py` & `batcave-42.1.0rc0/batcave/time.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/batcave/version.py` & `batcave-42.1.0rc0/batcave/version.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/docs/Makefile` & `batcave-42.1.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/docs/batcave.rst` & `batcave-42.1.0rc0/docs/batcave.rst`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/docs/coding_standards.py` & `batcave-42.1.0rc0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/docs/conf.py` & `batcave-42.1.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/docs/make.bat` & `batcave-42.1.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/pyproject.toml` & `batcave-42.1.0rc0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "batcave"
-authors = [{name = "Jeffery G. Smith", email = "web@pobox.com"}]
-readme = "DOCUMENTATION.md"
-license = {file = "LICENSE"}
-dynamic = ["version", "description"]
-
-requires-python = "~=3.10"
-keywords = ["python", "programming", "utilities"]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "License :: OSI Approved :: MIT License",
-
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.10",
-
-    "Intended Audience :: Developers",
-    "Topic :: Software Development",
-    "Natural Language :: English",
-]
-
-dependencies = [
-    "docker ~= 6.1",
-    "DotMap ~= 1.3",
-    "GitPython ~= 3.1",
-    "google-api-core",
-    "kubernetes ~= 26.1",
-    "requests ~= 2.30",
-    "PyYAML ~= 6.0",
-    "pywin32-stubs; sys_platform == 'win32'",
-    "WMI ~= 1.5; sys_platform == 'win32'",
-    "psutil ~= 5.9; platform_machine not in 'arm arm64 armv6l armv7l armv8b armv8l'",
-    "PyQt5 ~= 5.15; platform_machine not in 'aarch64 aarch64_be arm arm64 armv6l armv7l armv8b armv8l'"
-]
-
-[project.optional-dependencies]
-dev = ["flit", "twine", "bumpver"]
-test = [
-    "flake8",
-    "flake8-annotations",
-    "flake8-pyproject",
-    "mypy",
-    "pylint",
-    "PyQt5-stubs",
-    "types-python-dateutil",
-    "types-PyYAML",
-    "types-psutil",
-    "types-requests",
-    "types-pywin32; sys_platform == 'win32'",
-    "unittest-xml-reporting"
-]
-# doc = []
-
-[project_urls]
-homepage = "https://gitlab.com/arisilon/batcave/"  # batcave.__uri__,
-documentation = "https://batcave.readthedocs.io"
-repository = "https://gitlab.com/arisilon/batcave/"
-changelog = "https://gitlab.com/arisilon/batcave/-/blob/master/CHANGELOG.md"
-
-[tool.flake8]
-max-line-length = 200
-ignore = ["ANN002", "ANN003", "ANN101", "ANN204", "ANN401"]
-[tool.pylint.format]
-max-line-length = 200
-
-[tool.pylint.design]
-max-attributes = 10
-
-[tool.pylint.messages_control]
-disable = ["duplicate-code" , "fixme"]
-
-[[tool.mypy.overrides]]
-module = "docker.*"
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "dotmap.*"
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "kubernetes.*"
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "P4.*"
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "pywintypes.*"
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "win32typing.*"
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = "wmi.*"
-ignore_missing_imports = true
-
-[tool.bumpver]
-current_version = "42.1.0"
-version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
-commit_message = "bump version {old_version} -> {new_version} [skip-ci]"
-commit = true
-tag = false
-push = false
-
-[tool.bumpver.file_patterns]
-"batcave/__init__.py" = ["__version__ = '{version}'"]
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "batcave"
+authors = [{name = "Jeffery G. Smith", email = "web@pobox.com"}]
+readme = "DOCUMENTATION.md"
+license = {file = "LICENSE"}
+dynamic = ["version", "description"]
+
+requires-python = "~=3.10"
+keywords = ["python", "programming", "utilities"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: MIT License",
+
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.10",
+
+    "Intended Audience :: Developers",
+    "Topic :: Software Development",
+    "Natural Language :: English",
+]
+
+dependencies = [
+    "docker ~= 6.1",
+    "DotMap ~= 1.3",
+    "GitPython ~= 3.1",
+    "google-api-core",
+    "kubernetes ~= 26.1",
+    "requests ~= 2.30",
+    "PyYAML ~= 6.0",
+    "pywin32-stubs; sys_platform == 'win32'",
+    "WMI ~= 1.5; sys_platform == 'win32'",
+    "psutil ~= 5.9; platform_machine not in 'arm arm64 armv6l armv7l armv8b armv8l'",
+    "PyQt5 ~= 5.15; platform_machine not in 'aarch64 aarch64_be arm arm64 armv6l armv7l armv8b armv8l'"
+]
+
+[project.optional-dependencies]
+dev = ["flit", "twine", "bumpver"]
+test = [
+    "flake8",
+    "flake8-annotations",
+    "flake8-pyproject",
+    "mypy",
+    "pylint",
+    "PyQt5-stubs",
+    "types-python-dateutil",
+    "types-PyYAML",
+    "types-psutil",
+    "types-requests",
+    "types-pywin32; sys_platform == 'win32'",
+    "unittest-xml-reporting"
+]
+# doc = []
+
+[project_urls]
+homepage = "https://gitlab.com/arisilon/batcave/"  # batcave.__uri__,
+documentation = "https://batcave.readthedocs.io"
+repository = "https://gitlab.com/arisilon/batcave/"
+changelog = "https://gitlab.com/arisilon/batcave/-/blob/master/CHANGELOG.md"
+
+[tool.flake8]
+max-line-length = 200
+ignore = ["ANN002", "ANN003", "ANN101", "ANN204", "ANN401"]
+[tool.pylint.format]
+max-line-length = 200
+
+[tool.pylint.design]
+max-attributes = 10
+
+[tool.pylint.messages_control]
+disable = ["duplicate-code" , "fixme"]
+
+[[tool.mypy.overrides]]
+module = "docker.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "dotmap.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "kubernetes.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "P4.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "pywintypes.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "win32typing.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "wmi.*"
+ignore_missing_imports = true
+
+[tool.bumpver]
+current_version = "42.1.0rc0"
+version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
+commit_message = "bump version {old_version} -> {new_version} [skip-ci]"
+commit = true
+tag = false
+push = false
+
+[tool.bumpver.file_patterns]
+"batcave/__init__.py" = ["__version__ = '{version}'"]
```

### Comparing `batcave-42.1.0/tests/test_lang.py` & `batcave-42.1.0rc0/tests/test_lang.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/tests/test_statemachine.py` & `batcave-42.1.0rc0/tests/test_statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/tests/test_sysutil.py` & `batcave-42.1.0rc0/tests/test_sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.1.0/PKG-INFO` & `batcave-42.1.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batcave
-Version: 42.1.0
+Version: 42.1.0rc0
 Summary: BatCave Utilities module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

