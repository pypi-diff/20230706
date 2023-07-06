# Comparing `tmp/zope.applicationcontrol-4.3.tar.gz` & `tmp/zope.applicationcontrol-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.applicationcontrol-4.3.tar", last modified: Fri Jun 24 15:33:32 2022, max compression
+gzip compressed data, was "zope.applicationcontrol-5.0.tar", last modified: Thu Jul  6 06:28:33 2023, max compression
```

## Comparing `zope.applicationcontrol-4.3.tar` & `zope.applicationcontrol-5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 15:33:32.112921 zope.applicationcontrol-4.3/
--rw-r--r--   0 mac        (513) staff       (20)     1042 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      225 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     2999 2022-06-24 15:33:32.113021 zope.applicationcontrol-4.3/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      526 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      112 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      417 2022-06-24 15:33:32.113772 zope.applicationcontrol-4.3/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3227 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 15:33:32.103788 zope.applicationcontrol-4.3/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 15:33:32.108006 zope.applicationcontrol-4.3/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 15:33:32.111670 zope.applicationcontrol-4.3/src/zope/applicationcontrol/
--rw-r--r--   0 mac        (513) staff       (20)       61 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1630 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/applicationcontrol.py
--rw-r--r--   0 mac        (513) staff       (20)      927 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     3741 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     4371 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/runtimeinfo.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 15:33:32.112667 zope.applicationcontrol-4.3/src/zope/applicationcontrol/tests/
--rw-r--r--   0 mac        (513) staff       (20)       61 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1356 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/tests/test_applicationcontrol.py
--rw-r--r--   0 mac        (513) staff       (20)     6380 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/src/zope/applicationcontrol/tests/test_runtimeinfo.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 15:33:32.110175 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     2999 2022-06-24 15:33:31.000000 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      880 2022-06-24 15:33:31.000000 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-06-24 15:33:31.000000 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-06-24 15:33:31.000000 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-06-24 15:33:31.000000 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      129 2022-06-24 15:33:31.000000 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-06-24 15:33:31.000000 zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1427 2022-06-24 15:33:30.000000 zope.applicationcontrol-4.3/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:28:33.250367 zope.applicationcontrol-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1152 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2897 2023-07-06 06:28:33.250434 zope.applicationcontrol-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      526 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      112 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      418 2023-07-06 06:28:33.250702 zope.applicationcontrol-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2960 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:28:33.245682 zope.applicationcontrol-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:28:33.247779 zope.applicationcontrol-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:28:33.249755 zope.applicationcontrol-5.0/src/zope/applicationcontrol/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1630 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/applicationcontrol.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      927 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3741 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3906 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/runtimeinfo.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:28:33.250194 zope.applicationcontrol-5.0/src/zope/applicationcontrol/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1356 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/tests/test_applicationcontrol.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6198 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/src/zope/applicationcontrol/tests/test_runtimeinfo.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:28:33.248974 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2897 2023-07-06 06:28:33.000000 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      880 2023-07-06 06:28:33.000000 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:28:33.000000 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 06:28:33.000000 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:28:33.000000 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      129 2023-07-06 06:28:33.000000 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 06:28:33.000000 zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1403 2023-07-06 06:28:32.000000 zope.applicationcontrol-5.0/tox.ini
```

### Comparing `zope.applicationcontrol-4.3/CHANGES.rst` & `zope.applicationcontrol-5.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,19 @@
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
+
 4.3 (2022-06-24)
 ================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.8, 3.9, 3.10.
```

### Comparing `zope.applicationcontrol-4.3/CONTRIBUTING.md` & `zope.applicationcontrol-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/LICENSE.txt` & `zope.applicationcontrol-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/PKG-INFO` & `zope.applicationcontrol-5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.applicationcontrol
-Version: 4.3
+Version: 5.0
 Summary: Zope applicationcontrol
 Home-page: https://github.com/zopefoundation/zope.applicationcontrol
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope ztk application control
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
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ``zope.applicationcontrol``
 ===========================
 
 .. image:: https://github.com/zopefoundation/zope.applicationcontrol/actions/workflows/tests.yml/badge.svg
@@ -46,14 +42,22 @@
 server.
 
 
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
+
 4.3 (2022-06-24)
 ================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.8, 3.9, 3.10.
 
@@ -104,9 +108,7 @@
 - Drop support for Python 2.4 and 2.5.
 
 
 3.5.5 (2010-01-09)
 ==================
 
 - Initial release, extracted from ``zope.app.applicationcontrol``.
-
-
```

### Comparing `zope.applicationcontrol-4.3/README.rst` & `zope.applicationcontrol-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/setup.py` & `zope.applicationcontrol-5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 tests_require = [
     'zope.testing',
     'zope.testrunner',
 ]
 
 setup(
     name='zope.applicationcontrol',
-    version='4.3',
+    version='5.0',
     author='Zope Foundation and Contributors',
     author_email='zope-dev@zope.org',
     description='Zope applicationcontrol',
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
@@ -47,45 +47,35 @@
     keywords="zope ztk application control",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
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
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Framework :: Zope :: 3',
     ],
     url='https://github.com/zopefoundation/zope.applicationcontrol',
     extras_require={
         'test': tests_require,
     },
     package_dir={'': 'src'},
     packages=find_packages('src'),
     namespace_packages=['zope'],
-    python_requires=', '.join([
-        '>=2.7',
-        '!=3.0.*',
-        '!=3.1.*',
-        '!=3.2.*',
-        '!=3.3.*',
-        '!=3.4.*',
-    ]),
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.interface',
         'zope.component',
         'zope.location',
         'zope.security',
         'zope.traversing>=3.7.0',
```

### Comparing `zope.applicationcontrol-4.3/src/zope/applicationcontrol/applicationcontrol.py` & `zope.applicationcontrol-5.0/src/zope/applicationcontrol/applicationcontrol.py`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/src/zope/applicationcontrol/configure.zcml` & `zope.applicationcontrol-5.0/src/zope/applicationcontrol/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/src/zope/applicationcontrol/interfaces.py` & `zope.applicationcontrol-5.0/src/zope/applicationcontrol/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/src/zope/applicationcontrol/runtimeinfo.py` & `zope.applicationcontrol-5.0/src/zope/applicationcontrol/runtimeinfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,23 +38,18 @@
 
 
 try:
     from zope.app.appsetup import appsetup
 except ImportError:
     appsetup = None
 
-try:
-    text_type = unicode
-except NameError:
-    text_type = str
-
 
 @implementer(IRuntimeInfo)
 @adapter(IApplicationControl)
-class RuntimeInfo(object):
+class RuntimeInfo:
     """Runtime information."""
 
     def __init__(self, context):
         self.context = context
 
     def getDeveloperMode(self):
         """See zope.app.applicationcontrol.interfaces.IRuntimeInfo"""
@@ -90,44 +85,35 @@
             version_utility = getUtility(IZopeVersion)
         except ComponentLookupError:
             return "Unavailable"
         return version_utility.getZopeVersion()
 
     def getPythonVersion(self):
         """See zope.app.applicationcontrol.interfaces.IRuntimeInfo"""
-        return (
-            sys.version
-            if isinstance(sys.version, text_type)
-            else sys.version.decode(self.getPreferredEncoding()))
+        return sys.version
 
     def getPythonPath(self):
         """See zope.app.applicationcontrol.interfaces.IRuntimeInfo"""
-        enc = self.getFileSystemEncoding()
-        return tuple([path if isinstance(path, text_type) else path.decode(enc)
-                      for path in sys.path])
+        return tuple(path for path in sys.path)
 
     def getSystemPlatform(self):
         """See zope.app.applicationcontrol.interfaces.IRuntimeInfo"""
         info = []
         enc = self.getPreferredEncoding()
         for item in platform.uname():
             try:
-                t = item if isinstance(item, text_type) else item.decode(enc)
+                t = item if isinstance(item, str) else item.decode(enc)
             except UnicodeError:
                 continue
             info.append(t)
-        return u' '.join(info)
+        return ' '.join(info)
 
     def getCommandLine(self):
         """See zope.app.applicationcontrol.interfaces.IRuntimeInfo"""
-        cmd = " ".join(sys.argv)
-        return (
-            cmd
-            if isinstance(cmd, text_type)
-            else cmd.decode(self.getPreferredEncoding()))
+        return " ".join(sys.argv)
 
     def getProcessId(self):
         """See zope.app.applicationcontrol.interfaces.IRuntimeInfo"""
         return os.getpid()
 
     def getUptime(self):
         """See zope.app.applicationcontrol.interfaces.IRuntimeInfo"""
```

### Comparing `zope.applicationcontrol-4.3/src/zope/applicationcontrol/tests/test_applicationcontrol.py` & `zope.applicationcontrol-5.0/src/zope/applicationcontrol/tests/test_applicationcontrol.py`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/src/zope/applicationcontrol/tests/test_runtimeinfo.py` & `zope.applicationcontrol-5.0/src/zope/applicationcontrol/tests/test_runtimeinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 try:
     text_type = unicode
 except NameError:
     text_type = str
 
 
 @implementer(IZopeVersion)
-class TestZopeVersion(object):
+class TestZopeVersion:
     """A fallback implementation for the ZopeVersion utility."""
 
     def getZopeVersion(self):
         return stupid_version_string
 
 
 class Test(unittest.TestCase):
@@ -83,52 +83,48 @@
         enc = self._getFileSystemEncoding()
         self.assertEqual(runtime_info.getFileSystemEncoding(), enc)
 
     def test_ZopeVersion(self):
         runtime_info = self._Test__new()
 
         # we expect that there is no utility
-        self.assertEqual(runtime_info.getZopeVersion(), u"Unavailable")
+        self.assertEqual(runtime_info.getZopeVersion(), "Unavailable")
 
         siteManager = component.getSiteManager()
         siteManager.registerUtility(TestZopeVersion(), IZopeVersion)
 
         self.assertEqual(runtime_info.getZopeVersion(), stupid_version_string)
 
     def test_PythonVersion(self):
         runtime_info = self._Test__new()
-        enc = self._getPreferredEncoding()
-        self.assertEqual(
-            runtime_info.getPythonVersion(),
-            sys.version if not isinstance(sys.version, bytes)
-            else sys.version.decode(enc))
+        self.assertEqual(runtime_info.getPythonVersion(), sys.version)
 
     def test_SystemPlatform(self):
         runtime_info = self._Test__new()
         plat = runtime_info.getSystemPlatform()
         self.assertTrue(plat)
         self.assertIsInstance(plat, text_type)
 
         # Now something that can't be decoded
         import platform
         uname = platform.uname
 
         def bad_uname():
-            class BadObject(object):
+            class BadObject:
                 def decode(self, _enc):
                     raise UnicodeError("Not gonna happen")
             return (BadObject(),)
         try:
             platform.uname = bad_uname
             plat = runtime_info.getSystemPlatform()
-            self.assertEqual(plat, u'')
+            self.assertEqual(plat, '')
 
             platform.uname = lambda: ('a', 'b')
             plat = runtime_info.getSystemPlatform()
-            self.assertEqual(plat, u'a b')
+            self.assertEqual(plat, 'a b')
         finally:
             platform.uname = uname
 
     def test_CommandLine(self):
         runtime_info = self._Test__new()
         self.assertEqual(runtime_info.getCommandLine(), " ".join(sys.argv))
 
@@ -163,27 +159,27 @@
 
         try:
             # Module not available
             module.appsetup = None
             self.assertEqual(runtime_info.getDeveloperMode(), 'undefined')
 
             # context not available
-            class Setup(object):
+            class Setup:
                 context = None
 
                 @classmethod
                 def getConfigContext(cls):
                     return cls.context
 
             module.appsetup = Setup
             self.assertEqual(runtime_info.getDeveloperMode(), 'undefined')
 
             features = []
 
-            class Context(object):
+            class Context:
                 @staticmethod
                 def hasFeature(name):
                     return name in features
 
             # Feature off
             Setup.context = Context
             self.assertEqual(runtime_info.getDeveloperMode(), 'Off')
```

### Comparing `zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/PKG-INFO` & `zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.applicationcontrol
-Version: 4.3
+Version: 5.0
 Summary: Zope applicationcontrol
 Home-page: https://github.com/zopefoundation/zope.applicationcontrol
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope ztk application control
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
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ``zope.applicationcontrol``
 ===========================
 
 .. image:: https://github.com/zopefoundation/zope.applicationcontrol/actions/workflows/tests.yml/badge.svg
@@ -46,14 +42,22 @@
 server.
 
 
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
+
 4.3 (2022-06-24)
 ================
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.8, 3.9, 3.10.
 
@@ -104,9 +108,7 @@
 - Drop support for Python 2.4 and 2.5.
 
 
 3.5.5 (2010-01-09)
 ==================
 
 - Initial release, extracted from ``zope.app.applicationcontrol``.
-
-
```

### Comparing `zope.applicationcontrol-4.3/src/zope.applicationcontrol.egg-info/SOURCES.txt` & `zope.applicationcontrol-5.0/src/zope.applicationcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.applicationcontrol-4.3/tox.ini` & `zope.applicationcontrol-5.0/tox.ini`

 * *Files 20% similar despite different names*

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
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
@@ -36,36 +33,35 @@
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
 source = zope.applicationcontrol
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

