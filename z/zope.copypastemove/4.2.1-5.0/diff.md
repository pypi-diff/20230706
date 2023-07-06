# Comparing `tmp/zope.copypastemove-4.2.1.tar.gz` & `tmp/zope.copypastemove-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.copypastemove-4.2.1.tar", last modified: Thu Aug 25 15:22:17 2022, max compression
+gzip compressed data, was "zope.copypastemove-5.0.tar", last modified: Thu Jul  6 12:09:57 2023, max compression
```

## Comparing `zope.copypastemove-4.2.1.tar` & `zope.copypastemove-5.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-25 15:22:17.209264 zope.copypastemove-4.2.1/
--rw-r--r--   0 mac        (513) staff       (20)     2960 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      212 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     5463 2022-08-25 15:22:17.209407 zope.copypastemove-4.2.1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1194 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      112 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      145 2022-08-25 15:22:17.210008 zope.copypastemove-4.2.1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3974 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-25 15:22:17.197126 zope.copypastemove-4.2.1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-25 15:22:17.202082 zope.copypastemove-4.2.1/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-25 15:22:17.206428 zope.copypastemove-4.2.1/src/zope/copypastemove/
--rw-r--r--   0 mac        (513) staff       (20)    19618 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      865 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2961 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/interfaces.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-25 15:22:17.209013 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/
--rw-r--r--   0 mac        (513) staff       (20)       15 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     3492 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_clipboard.py
--rw-r--r--   0 mac        (513) staff       (20)     1693 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_configure.py
--rw-r--r--   0 mac        (513) staff       (20)     3769 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_metadata.py
--rw-r--r--   0 mac        (513) staff       (20)     7252 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_objectcopier.py
--rw-r--r--   0 mac        (513) staff       (20)     7578 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_objectmover.py
--rw-r--r--   0 mac        (513) staff       (20)     4601 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_rename.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-25 15:22:17.204974 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     5463 2022-08-25 15:22:16.000000 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      884 2022-08-25 15:22:17.000000 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-25 15:22:16.000000 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-25 15:22:16.000000 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-25 15:22:16.000000 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      370 2022-08-25 15:22:16.000000 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-25 15:22:16.000000 zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1208 2022-08-25 15:22:15.000000 zope.copypastemove-4.2.1/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 12:09:57.163720 zope.copypastemove-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3127 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5484 2023-07-06 12:09:57.163796 zope.copypastemove-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1194 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      112 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      418 2023-07-06 12:09:57.164088 zope.copypastemove-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3281 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 12:09:57.158698 zope.copypastemove-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 12:09:57.160671 zope.copypastemove-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 12:09:57.162390 zope.copypastemove-5.0/src/zope/copypastemove/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19604 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      865 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2987 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/interfaces.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 12:09:57.163558 zope.copypastemove-5.0/src/zope/copypastemove/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       15 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3484 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/tests/test_clipboard.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1695 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/tests/test_configure.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3745 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/tests/test_metadata.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7021 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/tests/test_objectcopier.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7346 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/tests/test_objectmover.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4564 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/src/zope/copypastemove/tests/test_rename.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 12:09:57.161883 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5484 2023-07-06 12:09:57.000000 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      900 2023-07-06 12:09:57.000000 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 12:09:57.000000 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 12:09:57.000000 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 12:09:57.000000 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      370 2023-07-06 12:09:57.000000 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 12:09:57.000000 zope.copypastemove-5.0/src/zope.copypastemove.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1398 2023-07-06 12:09:56.000000 zope.copypastemove-5.0/tox.ini
```

### Comparing `zope.copypastemove-4.2.1/CHANGES.rst` & `zope.copypastemove-5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop deprecated support for ``python setup.py test``.
+
+
 4.2.1 (2022-08-25)
 ==================
 
 - Fix DeprecationWarnings.
 
 
 4.2.0 (2022-01-24)
```

### Comparing `zope.copypastemove-4.2.1/LICENSE.txt` & `zope.copypastemove-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.copypastemove-4.2.1/PKG-INFO` & `zope.copypastemove-5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: zope.copypastemove
-Version: 4.2.1
+Version: 5.0
 Summary: Copy, Paste and Move support for content components.
 Home-page: http://github.com/zopefoundation/zope.copypastemove
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
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
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: zcml
 License-File: LICENSE.txt
 
 ========================
  ``zope.copypastemove``
 ========================
@@ -64,14 +61,24 @@
 objects as known from the ``zope.container`` package.
 
 
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop deprecated support for ``python setup.py test``.
+
+
 4.2.1 (2022-08-25)
 ==================
 
 - Fix DeprecationWarnings.
 
 
 4.2.0 (2022-01-24)
@@ -183,9 +190,7 @@
 - No further changes since 3.4.0a1.
 
 3.4.0a1 (2007-04-22)
 ====================
 
 - Initial release as a separate project, corresponds to
   ``zope.copypastemove`` from Zope 3.4.0a1
-
-
```

### Comparing `zope.copypastemove-4.2.1/README.rst` & `zope.copypastemove-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.copypastemove-4.2.1/setup.py` & `zope.copypastemove-5.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,37 +13,24 @@
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
 # http://docs.zope.org/zopetoolkit
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
-def alltests():
-    import sys
-    import unittest
-    # use the zope.testrunner machinery to find all the
-    # test suites we've put under ourselves
-    import zope.testrunner.find
-    import zope.testrunner.options
-    here = os.path.abspath(os.path.join(os.path.dirname(__file__), 'src'))
-    args = sys.argv[:]
-    defaults = ["--test-path", here]
-    options = zope.testrunner.options.get_options(args, defaults)
-    suites = list(zope.testrunner.find.find_suites(options))
-    return unittest.TestSuite(suites)
-
-
 long_description = (read('README.rst') + '\n\n' + read('CHANGES.rst'))
 
 ZCML_REQUIRES = [
     'zope.component[zcml]',
     'zope.configuration',
     'zope.security[zcml]',
 ]
@@ -53,45 +40,43 @@
     'zope.principalannotation',
     'zope.testing',
     'zope.testrunner',
     'zope.traversing',
 ]
 
 setup(name='zope.copypastemove',
-      version='4.2.1',
+      version='5.0',
       url='http://github.com/zopefoundation/zope.copypastemove',
       license='ZPL 2.1',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       description="Copy, Paste and Move support for content components.",
       long_description=long_description,
       classifiers=[
           'Environment :: Web Environment',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
           'Programming Language :: Python',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: Implementation :: PyPy',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Topic :: Internet :: WWW/HTTP',
           'Framework :: Zope :: 3',
       ],
       packages=find_packages('src'),
       package_dir={'': 'src'},
-      namespace_packages=['zope', ],
+      namespace_packages=['zope'],
+      python_requires='>=3.7',
       extras_require={
           'test': TESTS_REQUIRE,
           'zcml': ZCML_REQUIRES,
       },
       install_requires=[
           'setuptools',
           'zope.annotation',
@@ -100,12 +85,10 @@
           'zope.copy',
           'zope.event',
           'zope.exceptions',
           'zope.interface',
           'zope.lifecycleevent',
           'zope.location',
       ],
-      tests_require=TESTS_REQUIRE,
-      test_suite='__main__.alltests',
       include_package_data=True,
       zip_safe=False,
       )
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/__init__.py` & `zope.copypastemove-5.0/src/zope/copypastemove/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,50 +12,51 @@
 #
 ##############################################################################
 """Copy, Paste and Move support for content components
 """
 __docformat__ = 'restructuredtext'
 
 import zope.component
-from zope.interface import implementer, Invalid
-from zope.exceptions import DuplicationError
+from zope.annotation.interfaces import IAnnotations
 from zope.component import adapter
+from zope.container.constraints import checkObject
+from zope.container.interfaces import IContainer
+from zope.container.interfaces import INameChooser
+from zope.container.interfaces import IOrderedContainer
+from zope.container.sample import SampleContainer
 from zope.copy import copy
 from zope.event import notify
-from zope.location.interfaces import ISublocations
-from zope.annotation.interfaces import IAnnotations
+from zope.exceptions import DuplicationError
+from zope.interface import Invalid
+from zope.interface import implementer
 from zope.lifecycleevent import ObjectCopiedEvent
+from zope.location.interfaces import IContained
+from zope.location.interfaces import ISublocations
 
-from zope.copypastemove.interfaces import IObjectMover
-from zope.copypastemove.interfaces import IObjectCopier
 from zope.copypastemove.interfaces import IContainerItemRenamer
+from zope.copypastemove.interfaces import IObjectCopier
+from zope.copypastemove.interfaces import IObjectMover
 from zope.copypastemove.interfaces import IPrincipalClipboard
 from zope.copypastemove.interfaces import ItemNotFoundError
 
-from zope.container.sample import SampleContainer
-from zope.container.interfaces import IContainer, IOrderedContainer
-from zope.location.interfaces import IContained
-from zope.container.interfaces import INameChooser
-from zope.container.constraints import checkObject
-
 
 @adapter(IContained)
 @implementer(IObjectMover)
-class ObjectMover(object):
+class ObjectMover:
     """Adapter for moving objects between containers
 
     To use an object mover, pass a contained `object` to the class.
     The contained `object` should implement `IContained`.  It should be
     contained in a container that has an adapter to `INameChooser`.
 
 
     >>> from zope.container.contained import Contained
     >>> ob = Contained()
     >>> container = ExampleContainer()
-    >>> container[u'foo'] = ob
+    >>> container['foo'] = ob
     >>> mover = ObjectMover(ob)
 
     In addition to moving objects, object movers can tell you if the
     object is movable:
 
     >>> mover.moveable()
     True
@@ -72,45 +73,45 @@
     ...
     TypeError: Container is not a valid Zope container.
 
     Of course, once we've decided we can move an object, we can use
     the mover to do so:
 
     >>> mover.moveTo(container2)
-    u'foo'
+    'foo'
     >>> list(container)
     []
     >>> list(container2)
-    [u'foo']
+    ['foo']
     >>> ob.__parent__ is container2
     True
 
     We can also specify a name:
 
-    >>> mover.moveTo(container2, u'bar')
-    u'bar'
+    >>> mover.moveTo(container2, 'bar')
+    'bar'
     >>> list(container2)
-    [u'bar']
+    ['bar']
     >>> ob.__parent__ is container2
     True
     >>> ob.__name__
-    u'bar'
+    'bar'
 
     But we may not use the same name given, if the name is already in
     use:
 
-    >>> container2[u'splat'] = 1
-    >>> mover.moveTo(container2, u'splat')
-    u'splat_'
+    >>> container2['splat'] = 1
+    >>> mover.moveTo(container2, 'splat')
+    'splat_'
     >>> l = list(container2)
     >>> l.sort()
     >>> l
-    [u'splat', u'splat_']
+    ['splat', 'splat_']
     >>> ob.__name__
-    u'splat_'
+    'splat_'
 
 
     If we try to move to an invalid container, we'll get an error:
 
     >>> mover.moveTo({})
     Traceback (most recent call last):
     ...
@@ -220,25 +221,25 @@
         except Invalid:
             return False
         return True
 
 
 @adapter(IContained)
 @implementer(IObjectCopier)
-class ObjectCopier(object):
+class ObjectCopier:
     """Adapter for copying objects between containers
 
     To use an object copier, pass a contained `object` to the class.
     The contained `object` should implement `IContained`.  It should be
     contained in a container that has an adapter to `INameChooser`.
 
     >>> from zope.container.contained import Contained
     >>> ob = Contained()
     >>> container = ExampleContainer()
-    >>> container[u'foo'] = ob
+    >>> container['foo'] = ob
     >>> copier = ObjectCopier(ob)
 
     In addition to moving objects, object copiers can tell you if the
     object is movable:
 
     >>> copier.copyable()
     True
@@ -255,57 +256,57 @@
     ...
     TypeError: Container is not a valid Zope container.
 
     Of course, once we've decided we can copy an object, we can use
     the copier to do so:
 
     >>> copier.copyTo(container2)
-    u'foo'
+    'foo'
     >>> list(container)
-    [u'foo']
+    ['foo']
     >>> list(container2)
-    [u'foo']
+    ['foo']
     >>> ob.__parent__ is container
     True
-    >>> container2[u'foo'] is ob
+    >>> container2['foo'] is ob
     False
-    >>> container2[u'foo'].__parent__ is container2
+    >>> container2['foo'].__parent__ is container2
     True
-    >>> container2[u'foo'].__name__
-    u'foo'
+    >>> container2['foo'].__name__
+    'foo'
 
     We can also specify a name:
 
-    >>> copier.copyTo(container2, u'bar')
-    u'bar'
+    >>> copier.copyTo(container2, 'bar')
+    'bar'
     >>> l = list(container2)
     >>> l.sort()
     >>> l
-    [u'bar', u'foo']
+    ['bar', 'foo']
 
     >>> ob.__parent__ is container
     True
-    >>> container2[u'bar'] is ob
+    >>> container2['bar'] is ob
     False
-    >>> container2[u'bar'].__parent__ is container2
+    >>> container2['bar'].__parent__ is container2
     True
-    >>> container2[u'bar'].__name__
-    u'bar'
+    >>> container2['bar'].__name__
+    'bar'
 
     But we may not use the same name given, if the name is already in
     use:
 
-    >>> copier.copyTo(container2, u'bar')
-    u'bar_'
+    >>> copier.copyTo(container2, 'bar')
+    'bar_'
     >>> l = list(container2)
     >>> l.sort()
     >>> l
-    [u'bar', u'bar_', u'foo']
-    >>> container2[u'bar_'].__name__
-    u'bar_'
+    ['bar', 'bar_', 'foo']
+    >>> container2['bar_'].__name__
+    'bar_'
 
 
     If we try to copy to an invalid container, we'll get an error:
 
     >>> copier.copyTo({})
     Traceback (most recent call last):
     ...
@@ -408,15 +409,15 @@
         except Invalid:
             return False
         return True
 
 
 @adapter(IContainer)
 @implementer(IContainerItemRenamer)
-class ContainerItemRenamer(object):
+class ContainerItemRenamer:
     """An IContainerItemRenamer adapter for containers.
 
     This adapter uses IObjectMover to move an item within the same container
     to a different name. We need to first setup an adapter for IObjectMover:
 
       >>> from zope.location.interfaces import IContained
       >>> gsm = zope.component.getGlobalSiteManager()
@@ -435,15 +436,15 @@
       >>> container['foo'] = foo
       >>> container['foo'] is foo
       True
 
     to 'bar':
 
       >>> renamer.renameItem('foo', 'bar')
-      u'bar'
+      'bar'
       >>> container['foo'] is foo
       Traceback (most recent call last):
       KeyError: 'foo'
       >>> container['bar'] is foo
       True
 
     If the item being renamed isn't in the container, a NotFoundError is
@@ -507,29 +508,29 @@
       >>> container['3'] = 'Item 3'
       >>> container.items()
       [('1', 'Item 1'), ('2', 'Item 2'), ('3', 'Item 3')]
 
     When we rename one of the items:
 
       >>> renamer.renameItem('1', 'I')
-      u'I'
+      'I'
 
     the order is preserved:
 
       >>> container.items()
-      [(u'I', 'Item 1'), ('2', 'Item 2'), ('3', 'Item 3')]
+      [('I', 'Item 1'), ('2', 'Item 2'), ('3', 'Item 3')]
 
     Renaming the other two items also preserves the origina order:
 
       >>> renamer.renameItem('2', 'II')
-      u'II'
+      'II'
       >>> renamer.renameItem('3', 'III')
-      u'III'
+      'III'
       >>> container.items()
-      [(u'I', 'Item 1'), (u'II', 'Item 2'), (u'III', 'Item 3')]
+      [('I', 'Item 1'), ('II', 'Item 2'), ('III', 'Item 3')]
 
     As with the standard renamer, trying to rename a non-existent item raises
     an error:
 
       >>> renamer.renameItem('IV', '4') # doctest:+ELLIPSIS
       Traceback (most recent call last):
       ItemNotFoundError: (<...OrderedContainer...>, 'IV')
@@ -548,15 +549,15 @@
         order[order.index(oldName)] = newName
         self.container.updateOrder(order)
         return newName
 
 
 @adapter(IAnnotations)
 @implementer(IPrincipalClipboard)
-class PrincipalClipboard(object):
+class PrincipalClipboard:
     """Principal clipboard
 
     Clipboard information consists of mappings of
     ``{'action':action, 'target':target}``.
     """
 
     def __init__(self, annotation):
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/configure.zcml` & `zope.copypastemove-5.0/src/zope/copypastemove/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/interfaces.py` & `zope.copypastemove-5.0/src/zope/copypastemove/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Copy and Move support
 """
 __docformat__ = 'restructuredtext'
 
-from zope.interface import Interface, implementer
+from zope.interface import Interface
+from zope.interface import implementer
 
 
 class IObjectMover(Interface):
     """Use `IObjectMover(obj)` to move an object somewhere."""
 
     def moveTo(target, new_name=None):
         """Move this object to the target given.
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_clipboard.py` & `zope.copypastemove-5.0/src/zope/copypastemove/tests/test_clipboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 """Clipboard tests
 """
 import unittest
 
 import zope.component
 from zope.annotation.interfaces import IAnnotations
 from zope.component.testing import PlacelessSetup
-from zope.principalannotation.utility import PrincipalAnnotationUtility
 from zope.principalannotation.interfaces import IPrincipalAnnotationUtility
+from zope.principalannotation.utility import PrincipalAnnotationUtility
 
 from zope.copypastemove import PrincipalClipboard
 from zope.copypastemove.interfaces import IPrincipalClipboard
 
 
-class PrincipalStub(object):
+class PrincipalStub:
 
     def __init__(self, id):
         self.id = id
 
 
 class PrincipalClipboardTest(PlacelessSetup, unittest.TestCase):
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_configure.py` & `zope.copypastemove-5.0/src/zope/copypastemove/tests/test_configure.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import unittest
-import zope.copypastemove
+
 import zope.component
 import zope.configuration.xmlconfig
 
+import zope.copypastemove
+
 
 class ZCMLTest(unittest.TestCase):
 
     def test_configure_zcml_should_be_loadable(self):
         zope.configuration.xmlconfig.XMLConfig(
             'configure.zcml', zope.copypastemove)()
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_metadata.py` & `zope.copypastemove-5.0/src/zope/copypastemove/tests/test_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,36 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Object copier metadata tests"""
 
 import datetime
 import unittest
+
 import zope.annotation
 import zope.annotation.attribute
 import zope.component
 import zope.container.contained
 import zope.container.interfaces
 import zope.container.sample
 import zope.container.testing
-import zope.copypastemove
 import zope.dublincore.testing
 import zope.dublincore.timeannotators
 import zope.lifecycleevent.interfaces
 import zope.location.interfaces
 import zope.traversing.api
 
+import zope.copypastemove
+
 
 class CopyCreationTimeTest(zope.container.testing.ContainerPlacefulSetup,
                            unittest.TestCase):
 
     def setUp(self):
-        super(CopyCreationTimeTest, self).setUp()
+        super().setUp()
         # We need a folder hierarchy for copying:
         self.buildFolders()
         # We need the default zope.dublincore adapters:
         zope.dublincore.testing.setUpDublinCore()
         # And the created annotator for the ObjectCopiedEvent
         zope.component.provideHandler(
             zope.dublincore.timeannotators.CreatedAnnotator,
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_objectcopier.py` & `zope.copypastemove-5.0/src/zope/copypastemove/tests/test_objectcopier.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,37 +10,27 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Object Copier Tests
 """
 import doctest
-import re
 import unittest
 
 import zope.component
-from zope.traversing.api import traverse
 from zope.component.eventtesting import clearEvents
 from zope.component.eventtesting import getEvents
-from zope.copypastemove import ObjectCopier
-from zope.copypastemove.interfaces import IObjectCopier
-from zope.testing import renormalizing
-
 from zope.container import testing
+from zope.traversing.api import traverse
 
-checker = renormalizing.RENormalizing([
-    # Python 3 unicode removed the "u".
-    (re.compile("u('.*?')"),
-     r"\1"),
-    (re.compile('u(".*?")'),
-     r"\1"),
-])
+from zope.copypastemove import ObjectCopier
+from zope.copypastemove.interfaces import IObjectCopier
 
 
-class File(object):
+class File:
     pass
 
 
 def test_copy_events():
     """
     Prepare an IObjectCopier::
 
@@ -51,43 +41,43 @@
 
       >>> from zope.container.sample import SampleContainer
       >>> root = SampleContainer()
 
     Prepare some objects::
 
       >>> folder = SampleContainer()
-      >>> root[u'foo'] = File()
-      >>> root[u'folder'] = folder
+      >>> root['foo'] = File()
+      >>> root['folder'] = folder
       >>> list(folder.keys())
       []
       >>> foo = traverse(root, 'foo') # wrap in ContainedProxy
 
     Now make a copy::
 
       >>> clearEvents()
       >>> copier = IObjectCopier(foo)
-      >>> copier.copyTo(folder, u'bar')
-      u'bar'
+      >>> copier.copyTo(folder, 'bar')
+      'bar'
 
     Check that the copy has been done::
 
       >>> list(folder.keys())
-      [u'bar']
+      ['bar']
 
     Check what events have been sent::
 
       >>> events = getEvents()
       >>> [event.__class__.__name__ for event in events]
       ['ObjectCopiedEvent', 'ObjectAddedEvent', 'ContainerModifiedEvent']
 
     Check that the ObjectCopiedEvent includes the correct data::
 
-      >>> events[0].object is folder[u'bar']
+      >>> events[0].object is folder['bar']
       True
-      >>> events[0].original is root[u'foo']
+      >>> events[0].original is root['foo']
       True
     """
 
 
 class ObjectCopierTest(testing.ContainerPlacefulSetup, unittest.TestCase):
 
     def setUp(self):
@@ -210,13 +200,12 @@
         copier = IObjectCopier(source)
         copier.copyTo(target)
         self.assertTrue('folder1' in target)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(ObjectCopierTest),
+        unittest.defaultTestLoader.loadTestsFromTestCase(ObjectCopierTest),
         doctest.DocTestSuite(
             setUp=testing.ContainerPlacefulSetup().setUp,
-            tearDown=testing.ContainerPlacefulSetup().tearDown,
-            checker=checker),
+            tearDown=testing.ContainerPlacefulSetup().tearDown),
     ))
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_objectmover.py` & `zope.copypastemove-5.0/src/zope/copypastemove/tests/test_objectmover.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,37 +10,27 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Object Mover Tests
 """
 import doctest
-import re
 import unittest
 
 import zope.component
-from zope.traversing.api import traverse
 from zope.component.eventtesting import clearEvents
 from zope.component.eventtesting import getEvents
-from zope.copypastemove import ObjectMover
-from zope.copypastemove.interfaces import IObjectMover
-from zope.testing import renormalizing
-
 from zope.container import testing
+from zope.traversing.api import traverse
 
-checker = renormalizing.RENormalizing([
-    # Python 3 unicode removed the "u".
-    (re.compile("u('.*?')"),
-     r"\1"),
-    (re.compile('u(".*?")'),
-     r"\1"),
-])
+from zope.copypastemove import ObjectMover
+from zope.copypastemove.interfaces import IObjectMover
 
 
-class File(object):
+class File:
     pass
 
 
 def test_move_events():
     """
     We need a root folder::
 
@@ -51,46 +41,46 @@
 
       >>> from zope import component
       >>> component.provideAdapter(ObjectMover, (None,), IObjectMover)
 
     Prepare some objects::
 
       >>> folder = SampleContainer()
-      >>> root[u'foo'] = File()
-      >>> root[u'folder'] = folder
+      >>> root['foo'] = File()
+      >>> root['folder'] = folder
       >>> list(folder.keys())
       []
       >>> foo = traverse(root, 'foo') # wrap in ContainedProxy
 
     Now move it::
 
       >>> clearEvents()
       >>> mover = IObjectMover(foo)
       >>> mover.moveableTo(folder)
       True
-      >>> mover.moveTo(folder, u'bar')
-      u'bar'
+      >>> mover.moveTo(folder, 'bar')
+      'bar'
 
     Check that the move has been done::
 
       >>> list(root.keys())
-      [u'folder']
+      ['folder']
       >>> list(folder.keys())
-      [u'bar']
+      ['bar']
 
     Check what events have been sent::
 
       >>> events = getEvents()
       >>> [event.__class__.__name__ for event in events]
       ['ObjectMovedEvent', 'ContainerModifiedEvent', 'ContainerModifiedEvent']
 
     Verify that the ObjectMovedEvent includes the correct data::
 
       >>> events[0].oldName, events[0].newName
-      (u'foo', u'bar')
+      ('foo', 'bar')
       >>> events[0].oldParent is root
       True
       >>> events[0].newParent is folder
       True
 
     Let's look the other events:
 
@@ -226,13 +216,12 @@
         mover = IObjectMover(source)
         mover.moveTo(target)
         self.assertTrue('folder1' in target)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(ObjectMoverTest),
+        unittest.defaultTestLoader.loadTestsFromTestCase(ObjectMoverTest),
         doctest.DocTestSuite(
             setUp=testing.ContainerPlacefulSetup().setUp,
-            tearDown=testing.ContainerPlacefulSetup().tearDown,
-            checker=checker),
+            tearDown=testing.ContainerPlacefulSetup().tearDown),
     ))
```

### Comparing `zope.copypastemove-4.2.1/src/zope/copypastemove/tests/test_rename.py` & `zope.copypastemove-5.0/src/zope/copypastemove/tests/test_rename.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,60 +10,57 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test renaming of components
 """
 import doctest
-import re
 import unittest
 
-from zope.component import testing, eventtesting, provideAdapter, adapter
-from zope.container.testing import PlacelessSetup, ContainerPlacefulSetup
-from zope.copypastemove import ContainerItemRenamer, ObjectMover
-from zope.copypastemove.interfaces import IContainerItemRenamer
-from zope.container.contained import Contained, NameChooser
+from zope.component import adapter
+from zope.component import eventtesting
+from zope.component import provideAdapter
+from zope.component import testing
+from zope.container.contained import Contained
+from zope.container.contained import NameChooser
 from zope.container.sample import SampleContainer
-from zope.testing import renormalizing
+from zope.container.testing import ContainerPlacefulSetup
+from zope.container.testing import PlacelessSetup
 
-checker = renormalizing.RENormalizing([
-    # Python 3 unicode removed the "u".
-    (re.compile("u('.*?')"),
-     r"\1"),
-    (re.compile('u(".*?")'),
-     r"\1"),
-])
+from zope.copypastemove import ContainerItemRenamer
+from zope.copypastemove import ObjectMover
+from zope.copypastemove.interfaces import IContainerItemRenamer
 
 
 class TestContainer(SampleContainer):
     pass
 
 
 @adapter(TestContainer)
 class ObstinateNameChooser(NameChooser):
 
     def chooseName(self, name, ob):
-        return u'foobar'
+        return 'foobar'
 
 
 class RenamerTest(ContainerPlacefulSetup, unittest.TestCase):
 
     def setUp(self):
         ContainerPlacefulSetup.setUp(self)
         provideAdapter(ObjectMover)
         provideAdapter(ContainerItemRenamer)
         provideAdapter(ObstinateNameChooser)
 
     def test_obstinatenamechooser(self):
         container = TestContainer()
-        container[u'foobar'] = Contained()
+        container['foobar'] = Contained()
         renamer = IContainerItemRenamer(container)
 
-        renamer.renameItem(u'foobar', u'newname')
-        self.assertEqual(list(container), [u'foobar'])
+        renamer.renameItem('foobar', 'newname')
+        self.assertEqual(list(container), ['foobar'])
 
 
 container_setup = PlacelessSetup()
 
 
 def globalSetUp(test):
     testing.setUp()
@@ -101,22 +98,24 @@
         container['foo'] = objects[0]
         container['bar'] = objects[1]
         container['baz'] = objects[2]
 
         # with a custom name chooser
 
         import codecs
-        from zope.interface import implementer, Interface
+
         from zope.container.interfaces import INameChooser
+        from zope.interface import Interface
+        from zope.interface import implementer
 
         class IMyContainer(Interface):
             "An interface"
         @adapter(IMyContainer)
         @implementer(INameChooser)
-        class MyNameChooser(object):
+        class MyNameChooser:
             def __init__(self, container):
                 self.container = container
 
             def chooseName(self, name, obj):
                 return codecs.getencoder('rot-13')(name)[0]
         provideAdapter(MyNameChooser)
 
@@ -124,26 +123,26 @@
         alsoProvides(container, IMyContainer)
 
         # OrderedContainerItemRenamer renames and preserves the order of items
 
         from zope.copypastemove import OrderedContainerItemRenamer
         renamer = OrderedContainerItemRenamer(container)
         self.assertEqual(renamer.renameItem('bar', 'quux'),
-                         u'dhhk')
+                         'dhhk')
 
         self.assertEqual(list(container.keys()),
-                         [u'foo', u'dhhk', u'baz'])
+                         ['foo', 'dhhk', 'baz'])
         self.assertEqual(container.values(),
                          objects)
 
 
 def test_suite():
     flags = (doctest.NORMALIZE_WHITESPACE
              | doctest.ELLIPSIS
              | doctest.IGNORE_EXCEPTION_DETAIL)
     return unittest.TestSuite((
         unittest.defaultTestLoader.loadTestsFromName(__name__),
         doctest.DocTestSuite(
             'zope.copypastemove',
             setUp=globalSetUp, tearDown=testing.tearDown,
-            checker=checker, optionflags=flags),
+            optionflags=flags),
     ))
```

### Comparing `zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/PKG-INFO` & `zope.copypastemove-5.0/src/zope.copypastemove.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: zope.copypastemove
-Version: 4.2.1
+Version: 5.0
 Summary: Copy, Paste and Move support for content components.
 Home-page: http://github.com/zopefoundation/zope.copypastemove
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
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
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: zcml
 License-File: LICENSE.txt
 
 ========================
  ``zope.copypastemove``
 ========================
@@ -64,14 +61,24 @@
 objects as known from the ``zope.container`` package.
 
 
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop deprecated support for ``python setup.py test``.
+
+
 4.2.1 (2022-08-25)
 ==================
 
 - Fix DeprecationWarnings.
 
 
 4.2.0 (2022-01-24)
@@ -183,9 +190,7 @@
 - No further changes since 3.4.0a1.
 
 3.4.0a1 (2007-04-22)
 ====================
 
 - Initial release as a separate project, corresponds to
   ``zope.copypastemove`` from Zope 3.4.0a1
-
-
```

### Comparing `zope.copypastemove-4.2.1/src/zope.copypastemove.egg-info/SOURCES.txt` & `zope.copypastemove-5.0/src/zope.copypastemove.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 setup.cfg
 setup.py
```

### Comparing `zope.copypastemove-4.2.1/tox.ini` & `zope.copypastemove-5.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,67 @@
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
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
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
 source = zope.copypastemove
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

