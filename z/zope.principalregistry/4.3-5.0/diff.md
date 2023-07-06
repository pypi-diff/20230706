# Comparing `tmp/zope.principalregistry-4.3.tar.gz` & `tmp/zope.principalregistry-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.principalregistry-4.3.tar", last modified: Thu Jul 14 07:56:49 2022, max compression
+gzip compressed data, was "zope.principalregistry-5.0.tar", last modified: Thu Jul  6 07:50:53 2023, max compression
```

## Comparing `zope.principalregistry-4.3.tar` & `zope.principalregistry-5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-07-14 07:56:49.711704 zope.principalregistry-4.3/
--rw-r--r--   0 mac        (513) staff       (20)     2170 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      372 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4934 2022-07-14 07:56:49.711840 zope.principalregistry-4.3/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1341 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      403 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-07-14 07:56:49.704514 zope.principalregistry-4.3/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7610 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      265 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)    11036 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      485 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)       54 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/docs/narr.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/docs-requirements.txt
--rw-r--r--   0 mac        (513) staff       (20)      446 2022-07-14 07:56:49.712500 zope.principalregistry-4.3/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3624 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-07-14 07:56:49.697351 zope.principalregistry-4.3/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-07-14 07:56:49.704853 zope.principalregistry-4.3/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-07-14 07:56:49.709981 zope.principalregistry-4.3/src/zope/principalregistry/
--rw-r--r--   0 mac        (513) staff       (20)    11153 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       17 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      502 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1126 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     5428 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/metaconfigure.py
--rw-r--r--   0 mac        (513) staff       (20)     2629 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/metadirectives.py
--rw-r--r--   0 mac        (513) staff       (20)     7956 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/principalregistry.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-07-14 07:56:49.711451 zope.principalregistry-4.3/src/zope/principalregistry/tests/
--rw-r--r--   0 mac        (513) staff       (20)       17 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      511 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/tests/principal.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1848 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/tests/test_doc.py
--rw-r--r--   0 mac        (513) staff       (20)     8438 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/src/zope/principalregistry/tests/test_principalregistry.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-07-14 07:56:49.707402 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4934 2022-07-14 07:56:49.000000 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1094 2022-07-14 07:56:49.000000 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-07-14 07:56:49.000000 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-07-14 07:56:49.000000 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-07-14 07:56:49.000000 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      169 2022-07-14 07:56:49.000000 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-07-14 07:56:49.000000 zope.principalregistry-4.3/src/zope.principalregistry.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1607 2022-07-14 07:56:47.000000 zope.principalregistry-4.3/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:50:53.730629 zope.principalregistry-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2337 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      372 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4957 2023-07-06 07:50:53.730695 zope.principalregistry-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1341 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      403 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:50:53.727362 zope.principalregistry-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7610 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      265 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11036 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      485 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       54 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/docs/narr.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/docs-requirements.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      447 2023-07-06 07:50:53.730959 zope.principalregistry-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2897 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:50:53.724277 zope.principalregistry-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:50:53.727587 zope.principalregistry-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:50:53.729877 zope.principalregistry-5.0/src/zope/principalregistry/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11137 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      502 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1126 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5428 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/metaconfigure.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2553 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/metadirectives.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7921 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/principalregistry.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:50:53.730489 zope.principalregistry-5.0/src/zope/principalregistry/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      511 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/tests/principal.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1525 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/tests/test_doc.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8416 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope/principalregistry/tests/test_principalregistry.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 07:50:53.728740 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4957 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1094 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      169 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/src/zope.principalregistry.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1583 2023-07-06 07:50:53.000000 zope.principalregistry-5.0/tox.ini
```

### Comparing `zope.principalregistry-4.3/CHANGES.rst` & `zope.principalregistry-5.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.3 (2022-07-14)
 ================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10.
```

### Comparing `zope.principalregistry-4.3/CONTRIBUTING.md` & `zope.principalregistry-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/LICENSE.txt` & `zope.principalregistry-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/PKG-INFO` & `zope.principalregistry-5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.principalregistry
-Version: 4.3
+Version: 5.0
 Summary: Global principal registry component for Zope3
 Home-page: https://github.com/zopefoundation/zope.principalregistry
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope security authentication principal registry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
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
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ============================
  ``zope.principalregistry``
 ============================
@@ -62,14 +59,24 @@
 Documentation is hosted at https://zopeprincipalregistry.readthedocs.io
 
 
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.3 (2022-07-14)
 ================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10.
 
@@ -146,9 +153,7 @@
 
   Set ``__name__`` and ``__parent__`` by hand to provide some backward-compatibility and
   to save a pointer to registry from principal objects.
 
 - Initial release. This package was split from zope.app.security as a part
   of the refactoring process to provide global principal registry without extra
   dependencies.
-
-
```

### Comparing `zope.principalregistry-4.3/README.rst` & `zope.principalregistry-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/docs/Makefile` & `zope.principalregistry-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/docs/conf.py` & `zope.principalregistry-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/setup.py` & `zope.principalregistry-5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,74 +20,55 @@
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
-def alltests():
-    import os
-    import sys
-    import unittest
-
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
 TESTS_REQUIRE = [
     'zope.testing',
     'zope.testrunner',
 ]
 
 setup(name='zope.principalregistry',
-      version='4.3',
+      version='5.0',
       author='Zope Foundation and Contributors',
-      author_email='zope-dev@zope.org',
+      author_email='zope-dev@zope.dev',
       description='Global principal registry component for Zope3',
       long_description=(
           read('README.rst')
           + '\n\n' +
           read('CHANGES.rst')
       ),
       keywords="zope security authentication principal registry",
       classifiers=[
           'Development Status :: 5 - Production/Stable',
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
       url='https://github.com/zopefoundation/zope.principalregistry',
       license='ZPL 2.1',
       packages=find_packages('src'),
       package_dir={'': 'src'},
       namespace_packages=['zope'],
+      python_requires='>=3.7',
       install_requires=[
           'setuptools',
           'zope.authentication',
           'zope.component',
           'zope.interface',
           'zope.password',
           'zope.security',
@@ -95,12 +76,10 @@
       extras_require={
           'test': TESTS_REQUIRE,
           'docs': [
               'Sphinx',
               'repoze.sphinx.autointerface',
           ],
       },
-      tests_require=TESTS_REQUIRE,
-      test_suite='__main__.alltests',
       include_package_data=True,
       zip_safe=False,
       )
```

### Comparing `zope.principalregistry-4.3/src/zope/principalregistry/README.rst` & `zope.principalregistry-5.0/src/zope/principalregistry/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ...
     ...    </configure>
     ... """)
 
     >>> from zope.principalregistry.principalregistry import principalRegistry
     >>> [p] = principalRegistry.getPrincipals('')
     >>> p.id, p.title, p.description, p.getLogin(), p.validate('123')
-    ('zope.manager', u'Manager', u'System Manager', u'admin', True)
+    ('zope.manager', 'Manager', 'System Manager', 'admin', True)
 
 We can verify that it conforms to the
 :class:`zope.security.interfaces.IPrincipal` interface:
 
     >>> from zope.security.interfaces import IPrincipal
     >>> from zope.interface.verify import verifyObject
     >>> from zope.schema import getValidationErrors
@@ -73,15 +73,15 @@
     ...         />
     ...
     ...    </configure>
     ... """)
 
     >>> p = principalRegistry.unauthenticatedPrincipal()
     >>> p.id, p.title, p.description
-    ('zope.unknown', u'Anonymous user', u"A person we don't know")
+    ('zope.unknown', 'Anonymous user', "A person we don't know")
 
 It implements :class:`zope.authentication.interfaces.IUnauthenticatedPrincipal`:
 
     >>> from zope.authentication import interfaces
     >>> verifyObject(interfaces.IUnauthenticatedPrincipal, p)
     True
     >>> getValidationErrors(interfaces.IUnauthenticatedPrincipal, p)
@@ -92,15 +92,15 @@
 This is to provide easy access to the data defined for the principal so
 that other (more featureful) principal objects can be created for the
 same principal.
 
     >>> from zope import component
     >>> p = component.getUtility(interfaces.IUnauthenticatedPrincipal)
     >>> p.id, p.title, p.description
-    ('zope.unknown', u'Anonymous user', u"A person we don't know")
+    ('zope.unknown', 'Anonymous user', "A person we don't know")
 
 The unauthenticated group
 =========================
 
 An unauthenticated group can also be defined in ZCML:
 
     >>> zcml("""
@@ -118,15 +118,15 @@
     ... """)
 
 This directive creates a group and registers it as a utility providing
 IUnauthenticatedGroup:
 
     >>> g = component.getUtility(interfaces.IUnauthenticatedGroup)
     >>> g.id, g.title, g.description
-    ('zope.unknowngroup', u'Anonymous users', u"People we don't know")
+    ('zope.unknowngroup', 'Anonymous users', "People we don't know")
 
 It implements :class:`zope.authentication.interfaces.IUnauthenticatedGroup`:
 
     >>> verifyObject(interfaces.IUnauthenticatedGroup, g)
     True
     >>> getValidationErrors(interfaces.IUnauthenticatedGroup, g)
     []
@@ -160,15 +160,15 @@
     ...         />
     ...
     ...    </configure>
     ... """)
 
     >>> g = component.getUtility(interfaces.IUnauthenticatedGroup)
     >>> g.id, g.title, g.description
-    ('zope.unknowngroup2', u'Anonymous users', u"People we don't know")
+    ('zope.unknowngroup2', 'Anonymous users', "People we don't know")
     >>> p = principalRegistry.unauthenticatedPrincipal()
     >>> p.id, g.id in p.groups
     ('zope.unknown2', True)
     >>> p = component.getUtility(interfaces.IUnauthenticatedPrincipal)
     >>> p.id, g.id in p.groups
     ('zope.unknown2', True)
 
@@ -217,15 +217,15 @@
     ...    </configure>
     ... """)
 
 It defines an IAuthenticatedGroup utility:
 
     >>> g = component.getUtility(interfaces.IAuthenticatedGroup)
     >>> g.id, g.title, g.description
-    ('zope.authenticated', u'Authenticated users', u'People we know')
+    ('zope.authenticated', 'Authenticated users', 'People we know')
 
 It implements :class:`zope.authentication.interfaces.IUnauthenticatedGroup`:
 
     >>> verifyObject(interfaces.IAuthenticatedGroup, g)
     True
     >>> getValidationErrors(interfaces.IAuthenticatedGroup, g)
     []
@@ -288,15 +288,15 @@
     ...    </configure>
     ... """)
 
 The everybodyGroup directive defines an IEveryoneGroup utility:
 
     >>> g = component.getUtility(interfaces.IEveryoneGroup)
     >>> g.id, g.title, g.description
-    ('zope.everybody', u'Everybody', u'All People')
+    ('zope.everybody', 'Everybody', 'All People')
 
 It implements :class:`zope.authentication.interfaces.IEveryoneGroup`:
 
     >>> verifyObject(interfaces.IEveryoneGroup, g)
     True
     >>> getValidationErrors(interfaces.IEveryoneGroup, g)
     []
@@ -350,10 +350,10 @@
 
 There is also a system_user that is defined in the code.  It will be returned
 from the getPrincipal method of the registry.
 
     >>> import zope.security.management
     >>> import zope.principalregistry.principalregistry
     >>> auth = zope.principalregistry.principalregistry.PrincipalRegistry()
-    >>> system_user = auth.getPrincipal(u'zope.security.management.system_user')
+    >>> system_user = auth.getPrincipal('zope.security.management.system_user')
     >>> system_user is zope.security.management.system_user
     True
```

### Comparing `zope.principalregistry-4.3/src/zope/principalregistry/meta.zcml` & `zope.principalregistry-5.0/src/zope/principalregistry/meta.zcml`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/src/zope/principalregistry/metaconfigure.py` & `zope.principalregistry-5.0/src/zope/principalregistry/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/src/zope/principalregistry/metadirectives.py` & `zope.principalregistry-5.0/src/zope/principalregistry/metadirectives.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,54 +22,54 @@
     """
     An Id that is the text type instead of a native string.
 
     This is required because ``IPrincipal`` defines *id* to be
     the text type.
     """
 
-    _type = str if str is not bytes else unicode  # PY2 # noqa: F821 undefined
+    _type = str
 
 
 class IBasePrincipalDirective(Interface):
     """Base interface for principal definition directives."""
 
     id = TextId(
-        title=u"Id",
-        description=u"Id as which this object will be known and used.",
+        title="Id",
+        description="Id as which this object will be known and used.",
         required=True)
 
     title = TextLine(
-        title=u"Title",
-        description=u"Provides a title for the object.",
+        title="Title",
+        description="Provides a title for the object.",
         required=True)
 
     description = TextLine(
-        title=u"Title",
-        description=u"Provides a description for the object.",
+        title="Title",
+        description="Provides a description for the object.",
         required=False)
 
 
 class IDefinePrincipalDirective(IBasePrincipalDirective):
     """Define a new principal."""
 
     login = TextLine(
-        title=u"Username/Login",
-        description=u"Specifies the Principal's Username/Login.",
+        title="Username/Login",
+        description="Specifies the Principal's Username/Login.",
         required=True)
 
     password = TextLine(
-        title=u"Password",
-        description=u"Specifies the Principal's Password.",
+        title="Password",
+        description="Specifies the Principal's Password.",
         required=True)
 
     password_manager = TextLine(
-        title=u"Password Manager Name",
-        description=(u"Name of the password manager will be used"
+        title="Password Manager Name",
+        description=("Name of the password manager will be used"
                      " for encode/check the password"),
-        default=u"Plain Text"
+        default="Plain Text"
     )
 
 
 class IDefineUnauthenticatedPrincipalDirective(IBasePrincipalDirective):
     """Define a new unauthenticated principal."""
```

### Comparing `zope.principalregistry-4.3/src/zope/principalregistry/principalregistry.py` & `zope.principalregistry-5.0/src/zope/principalregistry/principalregistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 class DuplicateId(Exception):
     pass
 
 
 @implementer(IAuthentication, ILogout)
-class PrincipalRegistry(object):
+class PrincipalRegistry:
     """
     An in-memory implementation of
     :class:`zope.authentication.interfaces.IAuthentication`
     and :class:`zope.authentication.interfaces.ILogout`.
     """
 
     # Methods implementing IAuthentication
@@ -63,15 +63,15 @@
                     if p.validate(password):
                         return p
         return None
 
     __defaultid = None
     __defaultObject = None
 
-    def defineDefaultPrincipal(self, id, title, description=u'',
+    def defineDefaultPrincipal(self, id, title, description='',
                                principal=None):
         id = _as_text(id)
         title = _as_text(title)
         description = _as_text(description)
 
         if id in self.__principalsById:
             raise DuplicateId(id)
@@ -120,16 +120,16 @@
         self.__principalsById = {}
         self.__principalsByLogin = {}
 
     def definePrincipal(
             self,
             principal,
             title,
-            description=u'',
-            login=u'',
+            description='',
+            login='',
             password=b'',
             passwordManagerName='Plain Text'):
         id = _as_text(principal)
         title = _as_text(title)
         description = _as_text(description)
         login = _as_text(login)
         if login in self.__principalsByLogin:
@@ -172,42 +172,42 @@
 except ImportError:  # pragma: no cover
     pass
 else:
     addCleanUp(principalRegistry._clear)
     del addCleanUp
 
 
-class PrincipalBase(object):
+class PrincipalBase:
 
     __name__ = __parent__ = None
 
     def __init__(self, id, title, description):
         self.id = _as_text(id)
         self.title = _as_text(title)
         self.description = _as_text(description)
         self.groups = []
 
 
 class Group(PrincipalBase):
 
     def getLogin(self):
-        return u''  # to make registry search happy
+        return ''  # to make registry search happy
 
 
 @implementer(IGroupAwarePrincipal)
 class Principal(PrincipalBase):
     """
     The default implementation of
     :class:`zope.security.interfaces.IGroupAwarePrincipal`
     that :class:`PrincipalRegistry` will create.
     """
 
     def __init__(self, id, title, description, login,
                  pw, pwManagerName="Plain Text"):
-        super(Principal, self).__init__(id, title, description)
+        super().__init__(id, title, description)
         self.__login = _as_text(login)
         self.__pwManagerName = pwManagerName
         self.__pw = pw
 
     def __getPasswordManager(self):
         return getUtility(IPasswordManager, self.__pwManagerName)
```

### Comparing `zope.principalregistry-4.3/src/zope/principalregistry/tests/test_doc.py` & `zope.principalregistry-5.0/src/zope/principalregistry/tests/test_doc.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,34 +9,22 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for the principal registry ZCML directives
 """
-from __future__ import print_function
 
 import doctest
-import re
 import unittest
 
 from zope.component.testing import setUp as setUpComponent
 from zope.component.testing import tearDown as tearDownComponent
 from zope.configuration import xmlconfig
 from zope.password.testing import setUpPasswordManagers
-from zope.testing import renormalizing
-
-
-checker = renormalizing.RENormalizing([
-    # Python 3 unicode removed the "u".
-    (re.compile("u('.*?')"),
-     r"\1"),
-    (re.compile('u(".*?")'),
-     r"\1"),
-])
 
 
 def setUp(test=None):
     setUpComponent()
     setUpPasswordManagers()
 
 
@@ -55,14 +43,13 @@
     setUp()
 
 
 def test_suite():
     return unittest.TestSuite((
         doctest.DocFileSuite(
             '../README.rst',
-            setUp=setUp, tearDown=tearDown, checker=checker,
+            setUp=setUp, tearDown=tearDown,
             globs={
                 'zcml': zcml,
                 'reset': reset,
-                'print_function': print_function,
             }),
     ))
```

### Comparing `zope.principalregistry-4.3/src/zope/principalregistry/tests/test_principalregistry.py` & `zope.principalregistry-5.0/src/zope/principalregistry/tests/test_principalregistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     challenge = None
 
     def __init__(self, lpw):
         if lpw is not None:
             login, password = lpw
         else:
             login = password = None
-        super(Request, self).__init__(login, password)
+        super().__init__(login, password)
 
     def needLogin(self, realm):
         self.challenge = 'basic realm="%s"' % realm
 
 
 class Test(unittest.TestCase):
 
@@ -158,15 +158,15 @@
         # It complies with IPrincipal
         self._validatePrincipal(anybody)
 
     def test_logout(self):
         self.assertIsNone(self.reg.logout(None))
 
     def test_duplicate_group(self):
-        class Group(object):
+        class Group:
             id = "id"
 
         self.reg.registerGroup(Group)
 
         with self.assertRaises(DuplicateId):
             self.reg.registerGroup(Group)
 
@@ -179,15 +179,15 @@
 
     def _getTargetInterface(self):
         from zope.interface import Interface
         return Interface
 
     def test_login(self):
         cls = self._getTargetClass()
-        self.assertEqual(u'', cls("id", "title", "desc").getLogin())
+        self.assertEqual('', cls("id", "title", "desc").getLogin())
 
     def test_valid(self):
         from zope.interface.verify import verifyObject
         from zope.schema import getValidationErrors
 
         schema = self._getTargetInterface()
         group = self._getTargetClass()("id", "title", "desc")
```

### Comparing `zope.principalregistry-4.3/src/zope.principalregistry.egg-info/PKG-INFO` & `zope.principalregistry-5.0/src/zope.principalregistry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.principalregistry
-Version: 4.3
+Version: 5.0
 Summary: Global principal registry component for Zope3
 Home-page: https://github.com/zopefoundation/zope.principalregistry
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope security authentication principal registry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
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
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ============================
  ``zope.principalregistry``
 ============================
@@ -62,14 +59,24 @@
 Documentation is hosted at https://zopeprincipalregistry.readthedocs.io
 
 
 =========
  Changes
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.11.
+
+
 4.3 (2022-07-14)
 ================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10.
 
@@ -146,9 +153,7 @@
 
   Set ``__name__`` and ``__parent__`` by hand to provide some backward-compatibility and
   to save a pointer to registry from principal objects.
 
 - Initial release. This package was split from zope.app.security as a part
   of the refactoring process to provide global principal registry without extra
   dependencies.
-
-
```

### Comparing `zope.principalregistry-4.3/src/zope.principalregistry.egg-info/SOURCES.txt` & `zope.principalregistry-5.0/src/zope.principalregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.principalregistry-4.3/tox.ini` & `zope.principalregistry-5.0/tox.ini`

 * *Files 24% similar despite different names*

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
-    coverage report -m --fail-under=99
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=99
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.principalregistry
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

