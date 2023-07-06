# Comparing `tmp/ForgeHg-0.5.1.tar.gz` & `tmp/ForgeHg-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ForgeHg-0.5.1.tar", last modified: Mon Jun 13 15:37:30 2022, max compression
+gzip compressed data, was "ForgeHg-0.5.2.tar", last modified: Thu Jul  6 15:31:22 2023, max compression
```

## Comparing `ForgeHg-0.5.1.tar` & `ForgeHg-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/
--rw-r--r--   0 brondsem   (502) staff       (20)      977 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/PKG-INFO
--rw-r--r--   0 brondsem   (502) staff       (20)      462 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/SOURCES.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/dependency_links.txt
--rw-r--r--   0 brondsem   (502) staff       (20)      242 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/entry_points.txt
--rw-r--r--   0 brondsem   (502) staff       (20)       24 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/requires.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        8 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/top_level.txt
--rw-r--r--   0 brondsem   (502) staff       (20)        1 2020-11-03 21:41:30.000000 ForgeHg-0.5.1/ForgeHg.egg-info/zip-safe
--rw-r--r--   0 brondsem   (502) staff       (20)      247 2013-02-15 23:14:03.000000 ForgeHg-0.5.1/MANIFEST.in
--rw-r--r--   0 brondsem   (502) staff       (20)      977 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/PKG-INFO
--rw-r--r--   0 brondsem   (502) staff       (20)     5628 2022-06-13 15:35:18.000000 ForgeHg-0.5.1/README.rst
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/forgehg/
--rw-r--r--   0 brondsem   (502) staff       (20)     2878 2022-04-15 20:49:21.000000 ForgeHg-0.5.1/forgehg/__init__.py
--rw-r--r--   0 brondsem   (502) staff       (20)      665 2022-04-15 20:49:21.000000 ForgeHg-0.5.1/forgehg/controllers.py
--rw-r--r--   0 brondsem   (502) staff       (20)     3774 2022-04-15 20:49:21.000000 ForgeHg-0.5.1/forgehg/hg_main.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/forgehg/model/
--rw-r--r--   0 brondsem   (502) staff       (20)       27 2022-04-15 20:49:21.000000 ForgeHg-0.5.1/forgehg/model/__init__.py
--rw-r--r--   0 brondsem   (502) staff       (20)    27846 2022-06-13 13:56:11.000000 ForgeHg-0.5.1/forgehg/model/hg.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/forgehg/nf/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/forgehg/nf/hg/
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/forgehg/nf/hg/images/
--rw-r--r--   0 brondsem   (502) staff       (20)     4688 2013-02-15 23:14:03.000000 ForgeHg-0.5.1/forgehg/nf/hg/images/hg.png
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/forgehg/templates/
--rw-r--r--   0 brondsem   (502) staff       (20)        0 2013-02-15 23:14:03.000000 ForgeHg-0.5.1/forgehg/templates/__init__.py
-drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/forgehg/templates/hg/
--rw-r--r--   0 brondsem   (502) staff       (20)     3102 2022-06-13 13:56:25.000000 ForgeHg-0.5.1/forgehg/templates/hg/index.html
--rw-r--r--   0 brondsem   (502) staff       (20)       80 2022-06-13 15:35:18.000000 ForgeHg-0.5.1/forgehg/version.py
--rw-r--r--   0 brondsem   (502) staff       (20)       38 2022-06-13 15:37:30.000000 ForgeHg-0.5.1/setup.cfg
--rw-r--r--   0 brondsem   (502) staff       (20)     2816 2022-06-13 15:35:18.000000 ForgeHg-0.5.1/setup.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.066315 ForgeHg-0.5.2/
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:21.991742 ForgeHg-0.5.2/ForgeHg.egg-info/
+-rw-r--r--   0 brondsem   (502) staff       (20)      944 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/PKG-INFO
+-rw-r--r--   0 brondsem   (502) staff       (20)      470 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/SOURCES.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        1 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/dependency_links.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)      130 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/entry_points.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)       24 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/requires.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        8 2023-07-06 15:31:21.000000 ForgeHg-0.5.2/ForgeHg.egg-info/top_level.txt
+-rw-r--r--   0 brondsem   (502) staff       (20)        1 2020-11-03 21:41:30.000000 ForgeHg-0.5.2/ForgeHg.egg-info/zip-safe
+-rw-r--r--   0 brondsem   (502) staff       (20)    18093 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/LICENSE
+-rw-r--r--   0 brondsem   (502) staff       (20)      247 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/MANIFEST.in
+-rw-r--r--   0 brondsem   (502) staff       (20)      944 2023-07-06 15:31:22.065813 ForgeHg-0.5.2/PKG-INFO
+-rw-r--r--   0 brondsem   (502) staff       (20)     5393 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/README.rst
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.059753 ForgeHg-0.5.2/forgehg/
+-rw-r--r--   0 brondsem   (502) staff       (20)        0 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/forgehg/__init__.py
+-rw-r--r--   0 brondsem   (502) staff       (20)      665 2022-04-15 20:49:21.000000 ForgeHg-0.5.2/forgehg/controllers.py
+-rw-r--r--   0 brondsem   (502) staff       (20)     3774 2023-07-06 15:08:14.000000 ForgeHg-0.5.2/forgehg/hg_main.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.061305 ForgeHg-0.5.2/forgehg/model/
+-rw-r--r--   0 brondsem   (502) staff       (20)       27 2022-06-28 21:31:29.000000 ForgeHg-0.5.2/forgehg/model/__init__.py
+-rw-r--r--   0 brondsem   (502) staff       (20)    27843 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/forgehg/model/hg.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:21.984171 ForgeHg-0.5.2/forgehg/nf/
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:21.984308 ForgeHg-0.5.2/forgehg/nf/hg/
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.062961 ForgeHg-0.5.2/forgehg/nf/hg/images/
+-rw-r--r--   0 brondsem   (502) staff       (20)     4688 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/forgehg/nf/hg/images/hg.png
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.064271 ForgeHg-0.5.2/forgehg/templates/
+-rw-r--r--   0 brondsem   (502) staff       (20)        0 2013-02-15 23:14:03.000000 ForgeHg-0.5.2/forgehg/templates/__init__.py
+drwxr-xr-x   0 brondsem   (502) staff       (20)        0 2023-07-06 15:31:22.064888 ForgeHg-0.5.2/forgehg/templates/hg/
+-rw-r--r--   0 brondsem   (502) staff       (20)     3102 2022-06-13 13:56:25.000000 ForgeHg-0.5.2/forgehg/templates/hg/index.html
+-rw-r--r--   0 brondsem   (502) staff       (20)       80 2023-07-06 15:29:09.000000 ForgeHg-0.5.2/forgehg/version.py
+-rw-r--r--   0 brondsem   (502) staff       (20)       38 2023-07-06 15:31:22.066496 ForgeHg-0.5.2/setup.cfg
+-rw-r--r--   0 brondsem   (502) staff       (20)     2739 2023-01-13 19:44:25.000000 ForgeHg-0.5.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ForgeHg-0.5.1/ForgeHg.egg-info/PKG-INFO` & `ForgeHg-0.5.2/ForgeHg.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ForgeHg
-Version: 0.5.1
+Version: 0.5.2
 Summary: Mercurial (Hg) SCM support for Apache Allura
 Home-page: http://sourceforge.net/p/forgehg
 Author-email: dev@allura.apache.org
 License: GPLv2
-Description: ForgeHg enables an Allura installation to use the Mercurial
-        source code management system. Mercurial (Hg) is an open source distributed
-        version control system (DVCS) similar to git and written in Python.
-        
 Keywords: Allura forge Mercurial Hg scm
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: TurboGears
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Python: >=3.7
+License-File: LICENSE
+
+ForgeHg enables an Allura installation to use the Mercurial
+source code management system. Mercurial (Hg) is an open source distributed
+version control system (DVCS) similar to git and written in Python.
```

### Comparing `ForgeHg-0.5.1/PKG-INFO` & `ForgeHg-0.5.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ForgeHg
-Version: 0.5.1
+Version: 0.5.2
 Summary: Mercurial (Hg) SCM support for Apache Allura
 Home-page: http://sourceforge.net/p/forgehg
 Author-email: dev@allura.apache.org
 License: GPLv2
-Description: ForgeHg enables an Allura installation to use the Mercurial
-        source code management system. Mercurial (Hg) is an open source distributed
-        version control system (DVCS) similar to git and written in Python.
-        
 Keywords: Allura forge Mercurial Hg scm
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: TurboGears
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Python: >=3.7
+License-File: LICENSE
+
+ForgeHg enables an Allura installation to use the Mercurial
+source code management system. Mercurial (Hg) is an open source distributed
+version control system (DVCS) similar to git and written in Python.
```

### Comparing `ForgeHg-0.5.1/README.rst` & `ForgeHg-0.5.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -94,34 +94,30 @@
 
 Testing
 =======
 If you've installed ForgeHg from cloned source code repository, as described in
 the `Installation`_ section above, you are able to execute an enclosed test
 suite. Tests examine ForgeHg's code routines in a controlled, isolated manner,
 ensuring its' flawless operation on your system setup. To make use of tests, you
-must install nose [8]_ extension to standard Python unittest framework.
+must install pytest.
 
 Both ForgeHg and Allura use PasteDeploy [9]_ as a mean to configure application
 at startup. PasteDeploy reads configuration from INI files, and testing
 configuration is by convention stored in ``test.ini`` files. You should find
 it in the same directory as this README. The format should be familiar to you,
 but in case it's not, it is fully documented on PasteDeploy website. What's
 important here is that ForgeHg re-uses some sections from Allura's
 ``test.ini``, so you need to put a valid path to it in place of default. The
 paths can be found at ``use`` keys in sections starting with ``app:``.
 
 Once that's done, make sure ``test.ini`` directory is set as your current
 working directory, and from it execute command::
 
-    nosetests
+    pytest
 
-The test suite will be started, outputting one character for each test case:
-``.`` (dot) for success, ``F`` for failure and ``E`` for error.
-
-.. [8] http://packages.python.org/nose
 .. [9] http://pythonpaste.org/deploy/
 
 Licensing
 =========
 ForgeHg is distributed under the terms of GNU General Public License version 2.
 Full text of the license should be enclosed to your copy in the LICENSE file
 residing in the same directory as this README. If there is no such file, please
```

### Comparing `ForgeHg-0.5.1/forgehg/controllers.py` & `ForgeHg-0.5.2/forgehg/controllers.py`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.1/forgehg/hg_main.py` & `ForgeHg-0.5.2/forgehg/hg_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from ming.utils import LazyProperty
-from ming.orm.ormsession import ThreadLocalORMSession
+from ming.odm.odmsession import ThreadLocalODMSession
 from tg import tmpl_context as c
 from timermiddleware import Timer
 
 # Pyforge-specific imports
 import allura.tasks
 from allura.lib import helpers as h
 from allura import model as M
@@ -63,15 +63,15 @@
         super().install(project)
         from . import model as HM
         repo = HM.Repository(
             name=self.config.options.mount_point,
             tool='hg',
             status='initializing',
             fs_path=self.config.options.get('fs_path'))
-        ThreadLocalORMSession.flush_all()
+        ThreadLocalODMSession.flush_all()
         cloned_from_project_id = self.config.options.get('cloned_from_project_id')
         cloned_from_repo_id = self.config.options.get('cloned_from_repo_id')
         init_from_url = self.config.options.get('init_from_url')
         init_from_path = self.config.options.get('init_from_path')
         if cloned_from_project_id is not None:
             cloned_from = HM.Repository.query.get(_id=cloned_from_repo_id)
             repo.default_branch_name = cloned_from.default_branch_name
```

### Comparing `ForgeHg-0.5.1/forgehg/model/hg.py` & `ForgeHg-0.5.2/forgehg/model/hg.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     def __init__(self, *args, **kwargs):
         stdout = kwargs.pop('stdout', False)
         super().__init__(*args, **kwargs)
         self.setconfig(b'ui', b'report_untrusted', b'off', b'allura')
         self.setconfig(b'progress', b'disable', b'true', b'allura')
         self.setconfig(b'ui', b'nontty', b'true', b'allura')
         if stdout:
-            # for easier debugging (in tests).  nosetests --nocapture kinda works too
+            # for easier debugging (in tests).  Probably not relevant with pytest?
             if six.PY3 and hasattr(sys.stdout, 'buffer'):
                 self.fout = sys.stdout.buffer
             else:
                 self.fout = sys.stdout
             # self.ferr = sys.stdout  # doesn't work and makes error output disappear completely
```

### Comparing `ForgeHg-0.5.1/forgehg/nf/hg/images/hg.png` & `ForgeHg-0.5.2/forgehg/nf/hg/images/hg.png`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.1/forgehg/templates/hg/index.html` & `ForgeHg-0.5.2/forgehg/templates/hg/index.html`

 * *Files identical despite different names*

### Comparing `ForgeHg-0.5.1/setup.py` & `ForgeHg-0.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,12 +54,9 @@
       entry_points="""
       [allura]
       Hg=forgehg.hg_main:ForgeHgApp
 
       [allura.timers]
       hg = forgehg.hg_main:hg_timers
       forgehg = forgehg.hg_main:forgehg_timers
-
-      [nose.plugins]
-      monkeypatch_capture = forgehg:MonkeyPatchCapture
       """,
       )
```

