# Comparing `tmp/zope.lifecycleevent-4.4.tar.gz` & `tmp/zope.lifecycleevent-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.lifecycleevent-4.4.tar", last modified: Mon May  9 11:53:58 2022, max compression
+gzip compressed data, was "zope.lifecycleevent-5.0.tar", last modified: Thu Jul  6 07:39:42 2023, max compression
```

## Comparing `zope.lifecycleevent-4.4.tar` & `zope.lifecycleevent-5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-05-09 11:53:58.058646 zope.lifecycleevent-4.4/
--rw-r--r--   0 mac        (513) staff       (20)     2658 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      343 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     5624 2022-05-09 11:53:58.058777 zope.lifecycleevent-4.4/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1645 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      108 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)       87 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-05-09 11:53:58.053127 zope.lifecycleevent-4.4/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7610 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      174 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)    10935 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)       53 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/handling.rst
--rw-r--r--   0 mac        (513) staff       (20)      596 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)       51 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/manual.rst
--rw-r--r--   0 mac        (513) staff       (20)       51 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/docs/quickstart.rst
--rw-r--r--   0 mac        (513) staff       (20)      446 2022-05-09 11:53:58.059427 zope.lifecycleevent-4.4/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3297 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-05-09 11:53:58.045535 zope.lifecycleevent-4.4/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-05-09 11:53:58.053473 zope.lifecycleevent-4.4/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-05-09 11:53:58.058368 zope.lifecycleevent-4.4/src/zope/lifecycleevent/
--rw-r--r--   0 mac        (513) staff       (20)     9796 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/src/zope/lifecycleevent/README.rst
--rw-r--r--   0 mac        (513) staff       (20)     5326 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/src/zope/lifecycleevent/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     9957 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/src/zope/lifecycleevent/handling.rst
--rw-r--r--   0 mac        (513) staff       (20)     5188 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/src/zope/lifecycleevent/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     2647 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/src/zope/lifecycleevent/manual.rst
--rw-r--r--   0 mac        (513) staff       (20)     9345 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/src/zope/lifecycleevent/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-05-09 11:53:58.056011 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     5624 2022-05-09 11:53:57.000000 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      848 2022-05-09 11:53:57.000000 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-05-09 11:53:57.000000 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-05-09 11:53:57.000000 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-05-09 11:53:57.000000 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      161 2022-05-09 11:53:57.000000 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-05-09 11:53:57.000000 zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1605 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/tox.ini
--rw-r--r--   0 mac        (513) staff       (20)        4 2022-05-09 11:53:56.000000 zope.lifecycleevent-4.4/version.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:39:42.639069 zope.lifecycleevent-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2768 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      343 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5590 2023-07-06 07:39:42.639149 zope.lifecycleevent-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1645 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      108 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)       87 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:39:42.636424 zope.lifecycleevent-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7610 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      174 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10935 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/handling.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      596 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/manual.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/docs/quickstart.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      447 2023-07-06 07:39:42.639442 zope.lifecycleevent-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3130 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:39:42.632663 zope.lifecycleevent-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:39:42.636570 zope.lifecycleevent-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:39:42.638900 zope.lifecycleevent-5.0/src/zope/lifecycleevent/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9796 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope/lifecycleevent/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5262 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope/lifecycleevent/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9957 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope/lifecycleevent/handling.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5188 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope/lifecycleevent/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2647 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope/lifecycleevent/manual.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9102 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope/lifecycleevent/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:39:42.637814 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5590 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      848 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      161 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1581 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/tox.ini
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-06 07:39:42.000000 zope.lifecycleevent-5.0/version.txt
```

### Comparing `zope.lifecycleevent-4.4/CHANGES.rst` & `zope.lifecycleevent-5.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-05-09)
 ================
 
 - Add support for Python 3.8, 3,9, 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.lifecycleevent-4.4/CONTRIBUTING.md` & `zope.lifecycleevent-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/LICENSE.txt` & `zope.lifecycleevent-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/PKG-INFO` & `zope.lifecycleevent-5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: zope.lifecycleevent
-Version: 4.4
+Version: 5.0
 Summary: Object life-cycle events
 Home-page: http://github.com/zopefoundation/zope.lifecycleevent
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: event lifecycle zope component interface flexible
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =========================
  ``zope.lifecycleevent``
 =========================
@@ -67,14 +64,22 @@
 Documentation is hosted at https://zopelifecycleevent.readthedocs.io
 
 
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-05-09)
 ================
 
 - Add support for Python 3.8, 3,9, 3.10.
 
 - Drop support for Python 3.4.
 
@@ -188,9 +193,7 @@
 
 - Use ``zope.container`` instead of ``zope.app.container``.
 
 3.4.0 (2007-09-01)
 ==================
 
 Initial release as an independent package
-
-
```

### Comparing `zope.lifecycleevent-4.4/README.rst` & `zope.lifecycleevent-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/docs/Makefile` & `zope.lifecycleevent-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/docs/conf.py` & `zope.lifecycleevent-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/docs/index.rst` & `zope.lifecycleevent-5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/setup.py` & `zope.lifecycleevent-5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.lifecycleevent package
 """
 import os
 
@@ -30,30 +30,27 @@
 
 
 setup(
     name='zope.lifecycleevent',
     version=read('version.txt').strip(),
     url='http://github.com/zopefoundation/zope.lifecycleevent',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     license='ZPL 2.1',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development',
     ],
     description='Object life-cycle events',
@@ -62,14 +59,15 @@
         + '\n\n' +
         read('CHANGES.rst')),
     keywords="event lifecycle zope component interface flexible",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
     include_package_data=True,
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.interface',
         'zope.event'
     ],
     extras_require={
         'test': [
@@ -81,10 +79,9 @@
             'zope.testrunner',
         ],
         'docs': [
             'repoze.sphinx.autointerface',
             'sphinx_rtd_theme',
         ]
     },
-    test_suite='zope.lifecycleevent.tests.test_suite',
     zip_safe=False,
 )
```

### Comparing `zope.lifecycleevent-4.4/src/zope/lifecycleevent/README.rst` & `zope.lifecycleevent-5.0/src/zope/lifecycleevent/README.rst`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/src/zope/lifecycleevent/__init__.py` & `zope.lifecycleevent-5.0/src/zope/lifecycleevent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,52 +44,52 @@
 
 def created(object):
     "See :meth:`.IZopeLifecycleEvent.created`"
     notify(ObjectCreatedEvent(object))
 
 
 @implementer(IAttributes)
-class Attributes(object):
+class Attributes:
     """Describes modified attributes of an interface."""
 
     def __init__(self, interface, *attributes):
         self.interface = interface
         self.attributes = attributes
 
 
 @implementer(ISequence)
-class Sequence(object):
+class Sequence:
     """Describes modified keys of an interface."""
 
     def __init__(self, interface, *keys):
         self.interface = interface
         self.keys = keys
 
 
 @implementer(IObjectModifiedEvent)
 class ObjectModifiedEvent(ObjectEvent):
     """An object has been modified"""
 
     def __init__(self, object, *descriptions):
         """Init with a list of modification descriptions."""
-        super(ObjectModifiedEvent, self).__init__(object)
+        super().__init__(object)
         self.descriptions = descriptions
 
 
 def modified(object, *descriptions):
     "See :meth:`.IZopeLifecycleEvent.modified`"
     notify(ObjectModifiedEvent(object, *descriptions))
 
 
 @implementer(IObjectCopiedEvent)
 class ObjectCopiedEvent(ObjectCreatedEvent):
     """An object has been copied"""
 
     def __init__(self, object, original):
-        super(ObjectCopiedEvent, self).__init__(object)
+        super().__init__(object)
         self.original = original
 
 
 def copied(object, original):
     "See :meth:`.IZopeLifecycleEvent.copied`"
     notify(ObjectCopiedEvent(object, original))
```

### Comparing `zope.lifecycleevent-4.4/src/zope/lifecycleevent/handling.rst` & `zope.lifecycleevent-5.0/src/zope/lifecycleevent/handling.rst`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/src/zope/lifecycleevent/interfaces.py` & `zope.lifecycleevent-5.0/src/zope/lifecycleevent/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/src/zope/lifecycleevent/manual.rst` & `zope.lifecycleevent-5.0/src/zope/lifecycleevent/manual.rst`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/src/zope/lifecycleevent/tests.py` & `zope.lifecycleevent-5.0/src/zope/lifecycleevent/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,31 +34,31 @@
 from zope.lifecycleevent import copied
 from zope.lifecycleevent import created
 from zope.lifecycleevent import modified
 from zope.lifecycleevent import moved
 from zope.lifecycleevent import removed
 
 
-class Context(object):
+class Context:
     pass
 
 
-class _AbstractListenerCase(object):
+class _AbstractListenerCase:
 
     def setUp(self):
-        super(_AbstractListenerCase, self).setUp()
+        super().setUp()
         from zope.event import subscribers
         self._old_subscribers = subscribers[:]
         self.listener = []
         subscribers[:] = [self.listener.append]
 
     def tearDown(self):
         from zope.event import subscribers
         subscribers[:] = self._old_subscribers
-        super(_AbstractListenerCase, self).tearDown()
+        super().tearDown()
 
 
 class _AbstractEventCase(_AbstractListenerCase):
 
     klass = None
     object = object()
     notifier = None
@@ -69,15 +69,15 @@
     def _getInitArgs(self):
         return (self.object,)
 
     def _makeOne(self):
         return self._getTargetClass()(*self._getInitArgs())
 
     def setUp(self):
-        super(_AbstractEventCase, self).setUp()
+        super().setUp()
         self.event = self._makeOne()
 
     def testGetObject(self):
         self.assertEqual(self.event.object, self.object)
 
     def test_verifyObject(self):
         iface = list(interface.providedBy(self.event).flattened())[0]
@@ -85,18 +85,14 @@
 
     def test_verifyClass(self):
         iface = list(interface.implementedBy(type(self.event)).flattened())[0]
         verifyClass(iface, self._getTargetClass())
 
     def test_notify(self):
         notifier = type(self).notifier
-        try:
-            notifier = notifier.__func__
-        except AttributeError:
-            pass  # Python 3
         notifier(*self._getInitArgs())
         self.assertEqual(len(self.listener), 1)
         self.assertEqual(self.listener[-1].object, self.object)
         return self.listener[-1]
 
 
 class TestSequence(unittest.TestCase):
@@ -143,15 +139,15 @@
         from zope.interface import Interface
         from zope.interface import implementer
 
         class ISample(Interface):
             field = Attribute("A test field")
 
         @implementer(ISample)
-        class Sample(object):
+        class Sample:
             pass
         obj = Sample()
         obj.field = 42
         attrs = Attributes(ISample, "field")
 
         modified(obj, attrs)
         self.assertEqual(self.listener[-1].object, obj)
@@ -165,15 +161,15 @@
     original = object()
     notifier = copied
 
     def _getInitArgs(self):
         return (self.object, self.original)
 
     def test_notify(self):
-        delivered = super(TestObjectCopiedEvent, self).test_notify()
+        delivered = super().test_notify()
         self.assertEqual(delivered.original, self.original)
 
 
 class TestObjectMovedEvent(_AbstractEventCase,
                            unittest.TestCase):
 
     klass = ObjectMovedEvent
```

### Comparing `zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/PKG-INFO` & `zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: zope.lifecycleevent
-Version: 4.4
+Version: 5.0
 Summary: Object life-cycle events
 Home-page: http://github.com/zopefoundation/zope.lifecycleevent
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: event lifecycle zope component interface flexible
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 =========================
  ``zope.lifecycleevent``
 =========================
@@ -67,14 +64,22 @@
 Documentation is hosted at https://zopelifecycleevent.readthedocs.io
 
 
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-05-09)
 ================
 
 - Add support for Python 3.8, 3,9, 3.10.
 
 - Drop support for Python 3.4.
 
@@ -188,9 +193,7 @@
 
 - Use ``zope.container`` instead of ``zope.app.container``.
 
 3.4.0 (2007-09-01)
 ==================
 
 Initial release as an independent package
-
-
```

### Comparing `zope.lifecycleevent-4.4/src/zope.lifecycleevent.egg-info/SOURCES.txt` & `zope.lifecycleevent-5.0/src/zope.lifecycleevent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.lifecycleevent-4.4/tox.ini` & `zope.lifecycleevent-5.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
@@ -37,14 +34,15 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
@@ -58,24 +56,22 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=100
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.lifecycleevent
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

