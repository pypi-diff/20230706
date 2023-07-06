# Comparing `tmp/zope.error-4.6.tar.gz` & `tmp/zope.error-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.error-4.6.tar", last modified: Mon Aug 29 06:00:52 2022, max compression
+gzip compressed data, was "zope.error-5.0.tar", last modified: Thu Jul  6 06:13:05 2023, max compression
```

## Comparing `zope.error-4.6.tar` & `zope.error-5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-29 06:00:52.934836 zope.error-4.6/
--rw-r--r--   0 mac        (513) staff       (20)     3565 2022-08-29 06:00:51.000000 zope.error-4.6/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-08-29 06:00:51.000000 zope.error-4.6/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-08-29 06:00:51.000000 zope.error-4.6/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-08-29 06:00:51.000000 zope.error-4.6/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      225 2022-08-29 06:00:51.000000 zope.error-4.6/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     5348 2022-08-29 06:00:52.934981 zope.error-4.6/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      450 2022-08-29 06:00:51.000000 zope.error-4.6/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      106 2022-08-29 06:00:51.000000 zope.error-4.6/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      417 2022-08-29 06:00:52.935685 zope.error-4.6/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3215 2022-08-29 06:00:51.000000 zope.error-4.6/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-29 06:00:52.925716 zope.error-4.6/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-29 06:00:52.929997 zope.error-4.6/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-08-29 06:00:51.000000 zope.error-4.6/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-29 06:00:52.934565 zope.error-4.6/src/zope/error/
--rw-r--r--   0 mac        (513) staff       (20)       14 2022-08-29 06:00:51.000000 zope.error-4.6/src/zope/error/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      948 2022-08-29 06:00:51.000000 zope.error-4.6/src/zope/error/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     9901 2022-08-29 06:00:51.000000 zope.error-4.6/src/zope/error/error.py
--rw-r--r--   0 mac        (513) staff       (20)     1968 2022-08-29 06:00:51.000000 zope.error-4.6/src/zope/error/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)    14814 2022-08-29 06:00:51.000000 zope.error-4.6/src/zope/error/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-29 06:00:52.932687 zope.error-4.6/src/zope.error.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     5348 2022-08-29 06:00:52.000000 zope.error-4.6/src/zope.error.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      544 2022-08-29 06:00:52.000000 zope.error-4.6/src/zope.error.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-29 06:00:52.000000 zope.error-4.6/src/zope.error.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-29 06:00:52.000000 zope.error-4.6/src/zope.error.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-29 06:00:52.000000 zope.error-4.6/src/zope.error.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      113 2022-08-29 06:00:52.000000 zope.error-4.6/src/zope.error.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-29 06:00:52.000000 zope.error-4.6/src/zope.error.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1413 2022-08-29 06:00:51.000000 zope.error-4.6/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:13:05.705839 zope.error-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3675 2023-07-06 06:13:05.000000 zope.error-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-06 06:13:05.000000 zope.error-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-06 06:13:05.000000 zope.error-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-06 06:13:05.000000 zope.error-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-06 06:13:05.000000 zope.error-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5291 2023-07-06 06:13:05.705916 zope.error-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      450 2023-07-06 06:13:05.000000 zope.error-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      106 2023-07-06 06:13:05.000000 zope.error-5.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      418 2023-07-06 06:13:05.706154 zope.error-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3048 2023-07-06 06:13:05.000000 zope.error-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:13:05.701786 zope.error-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:13:05.703624 zope.error-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:13:05.705676 zope.error-5.0/src/zope/error/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       14 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope/error/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      948 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope/error/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9844 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope/error/error.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1968 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope/error/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14369 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope/error/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:13:05.704856 zope.error-5.0/src/zope.error.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5291 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope.error.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      544 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope.error.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope.error.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope.error.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope.error.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      109 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope.error.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 06:13:05.000000 zope.error-5.0/src/zope.error.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1389 2023-07-06 06:13:05.000000 zope.error-5.0/tox.ini
```

### Comparing `zope.error-4.6/CHANGES.rst` & `zope.error-5.0/CHANGES.rst`

 * *Files 3% similar despite different names*

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
 4.6 (2022-08-29)
 ================
 
 - Add support for Python 3.8, 3.9, 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.error-4.6/CONTRIBUTING.md` & `zope.error-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.error-4.6/LICENSE.txt` & `zope.error-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.error-4.6/PKG-INFO` & `zope.error-5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: zope.error
-Version: 4.6
+Version: 5.0
 Summary: An error reporting utility for Zope3
 Home-page: https://github.com/zopefoundation/zope.error
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope3 error
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
 Provides-Extra: test
@@ -44,14 +40,22 @@
 This package provides an error reporting utility which is able to store errors.
 
 
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
 4.6 (2022-08-29)
 ================
 
 - Add support for Python 3.8, 3.9, 3.10.
 
 - Drop support for Python 3.4.
 
@@ -197,9 +201,7 @@
 
 3.5.0
 =====
 
 - Initial documented release
 
 - Moved core components from ``zope.app.error`` to this package.
-
-
```

### Comparing `zope.error-4.6/setup.py` & `zope.error-5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
 setup(name='zope.error',
-      version='4.6',
+      version='5.0',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       description="An error reporting utility for Zope3",
       long_description=(
           read('README.rst')
           + '\n\n' +
           read('CHANGES.rst')
@@ -44,23 +44,20 @@
       keywords="zope3 error",
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
@@ -70,15 +67,14 @@
       namespace_packages=['zope', ],
       install_requires=[
           'setuptools',
           'zope.exceptions',
           'zope.interface',
           'zope.location',
           'persistent',  # error.py imports from persistent
-          'six',
       ],
       extras_require={
           'test': [
               'zope.testing >= 3.8',
               'zope.testrunner',
           ],
       },
```

### Comparing `zope.error-4.6/src/zope/error/configure.zcml` & `zope.error-5.0/src/zope/error/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.error-4.6/src/zope/error/error.py` & `zope.error-5.0/src/zope/error/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 import codecs
 import logging
 import time
 from random import random
 from threading import Lock
 from xml.sax.saxutils import escape as xml_escape
 
-from six import text_type
-
 import zope.location.interfaces
 from persistent import Persistent
 from zope.exceptions.exceptionformatter import format_exception
 from zope.interface import implementer
 
 from zope.error.interfaces import IErrorReportingUtility
 from zope.error.interfaces import ILocalErrorReportingUtility
@@ -52,62 +50,62 @@
 
 cleanup_lock = Lock()
 
 logger = logging.getLogger('SiteError')
 
 
 def printedreplace(error):
-    symbols = (u"\\x%02x" % (s if isinstance(s, int) else ord(s))
+    symbols = ("\\x%02x" % (s if isinstance(s, int) else ord(s))
                for s in error.object[error.start:error.end])
-    return u"".join(symbols), error.end
+    return "".join(symbols), error.end
 
 
 codecs.register_error("zope.error.printedreplace", printedreplace)
 
 
 def getPrintable(value, as_html=False):
-    if not isinstance(value, text_type):
+    if not isinstance(value, str):
         if not isinstance(value, bytes):
             # A call to str(obj) could raise anything at all.
             # We'll ignore these errors, and print something
             # useful instead, but also log the error.
             try:
                 value = str(value)
             except Exception:
                 logger.exception(
                     "Error in ErrorReportingUtility while getting a str"
                     " representation of an object")
-                return u"<unprintable %s object>" % (
+                return "<unprintable %s object>" % (
                     xml_escape(type(value).__name__))
         if isinstance(value, bytes):
             value = value.decode('utf-8', errors="zope.error.printedreplace")
     return value if as_html else xml_escape(value)
 
 
 def getFormattedException(info, as_html=False):
     lines = []
     for line in format_exception(as_html=as_html, *info):
         line = getPrintable(line, as_html=as_html)
         if not line.endswith("\n"):
             line += "<br />\n" if as_html else "\n"
         lines.append(line)
-    return u"".join(lines)
+    return "".join(lines)
 
 
 @implementer(IErrorReportingUtility,
              ILocalErrorReportingUtility,
              zope.location.interfaces.IContained)
 class ErrorReportingUtility(Persistent):
     """Error Reporting Utility"""
 
     __parent__ = __name__ = None
 
     keep_entries = 20
     copy_to_zlog = True
-    _ignored_exceptions = (u'Unauthorized',)
+    _ignored_exceptions = ('Unauthorized',)
 
     def _getLog(self):
         """Returns the log for this object.
         Careful, the log is shared between threads.
         """
         log = _temp_logs.get(self._p_oid, None)
         if log is None:
@@ -128,37 +126,37 @@
             login = "unauthenticated"
         else:
             try:
                 login = getLogin()
             except Exception:
                 logger.exception("Error in ErrorReportingUtility while"
                                  " getting login of the principal")
-                login = u"<error getting login>"
+                login = "<error getting login>"
 
         parts = []
         for part in [
                 login,
                 getattr(principal, "id",
-                        u"<error getting 'principal.id'>"),
+                        "<error getting 'principal.id'>"),
                 getattr(principal, "title",
-                        u"<error getting 'principal.title'>"),
+                        "<error getting 'principal.title'>"),
                 getattr(principal, "description",
-                        u"<error getting 'principal.description'>")
+                        "<error getting 'principal.description'>")
         ]:
             part = getPrintable(part)
             parts.append(part)
-        username = u", ".join(parts)
+        username = ", ".join(parts)
         return username
 
     def _getRequestAsHTML(self, request):
         lines = []
         for key, value in sorted(request.items()):
-            lines.append(u"%s: %s<br />\n" % (
+            lines.append("{}: {}<br />\n".format(
                 getPrintable(key), getPrintable(value)))
-        return u"".join(lines)
+        return "".join(lines)
 
     # Exceptions that happen all the time, so we dont need
     # to log them. Eventually this should be configured
     # through-the-web.
     def raising(self, info, request=None):
         """Log an exception.
         Called by ZopePublication.handleException method.
@@ -170,15 +168,15 @@
             strtype = strtype.decode(
                 "utf-8") if isinstance(strtype, bytes) else strtype
             if strtype in self._ignored_exceptions:
                 return
 
             tb_text = None
             tb_html = None
-            if isinstance(tb, (text_type, bytes)):
+            if isinstance(tb, (str, bytes)):
                 tb_text = getPrintable(tb)
             else:
                 tb_text = getFormattedException(info)
                 tb_html = getFormattedException(info, True)
 
             url = None
             username = None
@@ -240,17 +238,17 @@
     def setProperties(self, keep_entries, copy_to_zlog=True,
                       ignored_exceptions=()):
         """Sets the properties of this site error log.
         """
         self.keep_entries = int(keep_entries)
         self.copy_to_zlog = bool(copy_to_zlog)
         self._ignored_exceptions = tuple(
-            (e.decode('utf-8') if not isinstance(e, text_type) else e
-             for e in ignored_exceptions
-             if e)
+            e.decode('utf-8') if not isinstance(e, str) else e
+            for e in ignored_exceptions
+            if e
         )
 
     def getLogEntries(self):
         """Returns the entries in the log, most recent first.
 
         Makes a copy to prevent changes.
         """
```

### Comparing `zope.error-4.6/src/zope/error/interfaces.py` & `zope.error-5.0/src/zope/error/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.error-4.6/src/zope/error/tests.py` & `zope.error-5.0/src/zope/error/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,50 +9,44 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Error Reporting Utility Tests
 """
-import io
 import logging
 import sys
 import unittest
-
-from six import text_type
+from io import StringIO
 
 from zope.exceptions.exceptionformatter import format_exception
 from zope.testing import cleanup
 
 from zope.error.error import ErrorReportingUtility
 from zope.error.error import getFormattedException
 
 
-class StringIO(io.BytesIO if str is bytes else io.StringIO):
-    pass
-
-
 class Error(Exception):
 
     def __init__(self, value):
-        super(Error, self).__init__()
+        super().__init__()
         self.value = value
 
     def __str__(self):
         return self.value
 
 
 def getAnErrorInfo(value=""):
     try:
         raise Error(value)
     except Error:
         return sys.exc_info()
 
 
-class TestRequest(object):
+class TestRequest:
     """Mock request that mimics the zope.publisher request."""
 
     principal = None
     URL = None
 
     def __init__(self, environ=None):
         self._environ = environ or {}
@@ -64,36 +58,36 @@
     def items(self):
         return self._items
 
     def getURL(self):
         return self._environ['PATH_INFO']
 
 
-class URLGetter(object):
+class URLGetter:
 
     __slots__ = ("__request",)
 
     def __init__(self, request):
         self.__request = request
 
     def __str__(self):
         return self.__request.getURL()
 
 
 class ErrorReportingUtilityTests(cleanup.CleanUp, unittest.TestCase):
 
     def setUp(self):
-        super(ErrorReportingUtilityTests, self).setUp()
+        super().setUp()
         self.log_buffer = StringIO()
         self.log_handler = logging.StreamHandler(self.log_buffer)
         logging.getLogger().addHandler(self.log_handler)
 
     def tearDown(self):
         logging.getLogger().removeHandler(self.log_handler)
-        super(ErrorReportingUtilityTests, self).tearDown()
+        super().tearDown()
 
     def makeOne(self):
         return ErrorReportingUtility()
 
     def test_checkForEmptyLog(self):
         # Test Check Empty Log
         errUtility = self.makeOne()
@@ -128,60 +122,60 @@
                          errUtility.getLogEntryById(err_id)['tb_text'])
 
     def test_ErrorLog_unicode(self):
         # Emulate a unicode url, it gets encoded to utf-8 before it's passed
         # to the request. Also add some unicode field to the request's
         # environment and make the principal's title unicode.
         request = TestRequest(environ={'PATH_INFO': '/\xd1\x82',
-                                       'SOME_UNICODE': u'\u0441'})
+                                       'SOME_UNICODE': '\u0441'})
 
-        class PrincipalStub(object):
-            id = u'\u0441'
-            title = u'\u0441'
-            description = u'\u0441'
+        class PrincipalStub:
+            id = '\u0441'
+            title = '\u0441'
+            description = '\u0441'
         request.setPrincipal(PrincipalStub())
 
         errUtility = self.makeOne()
-        exc_info = getAnErrorInfo(u"Error (\u0441)")
+        exc_info = getAnErrorInfo("Error (\u0441)")
         errUtility.raising(exc_info, request=request)
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         tb_text = getFormattedException(exc_info)
 
         err_id = getErrLog[0]['id']
         self.assertEqual(tb_text,
                          errUtility.getLogEntryById(err_id)['tb_text'])
 
         username = getErrLog[0]['username']
-        self.assertEqual(username, u'unauthenticated, \u0441, \u0441, \u0441')
+        self.assertEqual(username, 'unauthenticated, \u0441, \u0441, \u0441')
 
     def test_ErrorLog_url(self):
         # We want a string for the URL in the error log, nothing else
         request = TestRequest(environ={'PATH_INFO': '/foobar'})
         # set request.URL as zope.publisher would
         request.URL = URLGetter(request)
 
         errUtility = self.makeOne()
-        exc_info = getAnErrorInfo(u"Error")
+        exc_info = getAnErrorInfo("Error")
         errUtility.raising(exc_info, request=request)
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         url = getErrLog[0]['url']
         self.assertIsInstance(url, str)
 
     def test_ErrorLog_nonascii(self):
         # Emulate a unicode url, it gets encoded to utf-8 before it's passed
         # to the request. Also add some unicode field to the request's
         # environment and make the principal's title unicode.
         request = TestRequest(environ={'PATH_INFO': '/\xd1\x82',
                                        'SOME_NONASCII': '\xe1'})
 
-        class PrincipalStub(object):
+        class PrincipalStub:
             id = b'\xe1'
             title = b'\xe1'
             description = b'\xe1'
         request.setPrincipal(PrincipalStub())
 
         errUtility = self.makeOne()
         exc_info = getAnErrorInfo("Error (\xe1)")
@@ -199,15 +193,15 @@
         self.assertEqual(username, r"unauthenticated, \xe1, \xe1, \xe1")
 
     def test_getLogEntryById_not_found(self):
         errUtility = self.makeOne()
         self.assertIsNone(errUtility.getLogEntryById('no such id'))
 
     def test_getLogin_error(self):
-        class PrincipalStub(object):
+        class PrincipalStub:
             id = 'id'
             title = 'title'
             description = 'description'
 
             def getLogin(self):
                 raise Exception()
         request = TestRequest()
@@ -218,58 +212,58 @@
         errUtility.raising(exc_info, request=request)
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         username = getErrLog[0]['username']
         self.assertEqual(
             username,
-            u'&lt;error getting login&gt;, id, title, description')
+            '&lt;error getting login&gt;, id, title, description')
 
     def test_request_items(self):
         request = TestRequest()
         request.items().append(('request&key', '<request&value>'))
 
         errUtility = self.makeOne()
         exc_info = getAnErrorInfo("Error")
         errUtility.raising(exc_info, request=request)
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         req_html = getErrLog[0]['req_html']
         self.assertEqual(
             req_html,
-            u'request&amp;key: &lt;request&amp;value&gt;<br />\n')
+            'request&amp;key: &lt;request&amp;value&gt;<br />\n')
 
     def test_request_items_bytes(self):
         request = TestRequest()
         request.items().append((b'request&key', b'<request&value\xe1>'))
 
         errUtility = self.makeOne()
         exc_info = getAnErrorInfo(b"Error")
         errUtility.raising(exc_info, request=request)
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         req_html = getErrLog[0]['req_html']
         self.assertEqual(
             req_html,
-            u'request&amp;key: &lt;request&amp;value\\xe1&gt;<br />\n')
+            'request&amp;key: &lt;request&amp;value\\xe1&gt;<br />\n')
 
     def test_request_items_int(self):
         request = TestRequest()
         request.items().append((b'request&key', 1))
 
         errUtility = self.makeOne()
         exc_info = getAnErrorInfo(b"Error")
         errUtility.raising(exc_info, request=request)
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         req_html = getErrLog[0]['req_html']
-        self.assertEqual(req_html, u'request&amp;key: 1<br />\n')
+        self.assertEqual(req_html, 'request&amp;key: 1<br />\n')
 
     def test_default_ignored_exception(self):
         class Unauthorized(Exception):
             pass
 
         errUtility = self.makeOne()
         exc_info = (Unauthorized, None, None)
@@ -284,27 +278,27 @@
 
         errUtility.raising((exc_info[0], exc_info[1], 'a string tb'))
 
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         self.assertIsNone(getErrLog[0]['tb_html'])
-        self.assertEqual(u'a string tb', getErrLog[0]['tb_text'])
+        self.assertEqual('a string tb', getErrLog[0]['tb_text'])
 
     def test_tb_preformatted_bytes(self):
         errUtility = self.makeOne()
         exc_info = getAnErrorInfo("Error")
 
         errUtility.raising((exc_info[0], exc_info[1], b'a string tb \xe1'))
 
         getErrLog = errUtility.getLogEntries()
         self.assertEqual(1, len(getErrLog))
 
         self.assertIsNone(getErrLog[0]['tb_html'])
-        self.assertEqual(u'a string tb \\xe1', getErrLog[0]['tb_text'])
+        self.assertEqual('a string tb \\xe1', getErrLog[0]['tb_text'])
 
     def test_cleanup(self):
         errUtility = self.makeOne()
         errUtility.keep_entries = 1
 
         exc_info = getAnErrorInfo("Error 1")
         errUtility.raising(exc_info)
@@ -330,48 +324,48 @@
     """Testing .error.getPrintable(value)"""
 
     def getPrintable(self, value):
         from zope.error.error import getPrintable
         return getPrintable(value)
 
     def test_xml_tags_get_escaped(self):
-        self.assertEqual(u'&lt;script&gt;', self.getPrintable(u'<script>'))
+        self.assertEqual('&lt;script&gt;', self.getPrintable('<script>'))
 
     def test_byte_values_get_converted_to_unicode(self):
         # This one isn't much of a test because it's the literal bytes
         # '\', 'u', '0', etc.
-        self.assertEqual(u'\\u0441', self.getPrintable(br'\u0441'))
-        self.assertIsInstance(self.getPrintable(br'\u0441'), text_type)
+        self.assertEqual('\\u0441', self.getPrintable(br'\u0441'))
+        self.assertIsInstance(self.getPrintable(br'\u0441'), str)
 
         # This is a bit better because it can't be encoded in UTF-8
-        self.assertEqual(u'\\xe1', self.getPrintable(b'\xe1'))
-        self.assertIsInstance(self.getPrintable(b'\xe1'), text_type)
+        self.assertEqual('\\xe1', self.getPrintable(b'\xe1'))
+        self.assertIsInstance(self.getPrintable(b'\xe1'), str)
 
     def test_non_str_values_get_converted_using_a_str_call(self):
-        class NonStr(object):
+        class NonStr:
             def __str__(self):
                 return 'non-str'
-        self.assertEqual(u'non-str', self.getPrintable(NonStr()))
-        self.assertIsInstance(self.getPrintable(NonStr()), text_type)
+        self.assertEqual('non-str', self.getPrintable(NonStr()))
+        self.assertIsInstance(self.getPrintable(NonStr()), str)
 
     def test_non_str_those_conversion_fails_are_returned_specially(self):
-        class NonStr(object):
+        class NonStr:
             def __str__(self):
                 raise ValueError('non-str')
-        self.assertEqual(u'<unprintable NonStr object>',
+        self.assertEqual('<unprintable NonStr object>',
                          self.getPrintable(NonStr()))
-        self.assertIsInstance(self.getPrintable(NonStr()), text_type)
+        self.assertIsInstance(self.getPrintable(NonStr()), str)
 
     def test_non_str_those_conversion_fails_are_returned_with_escaped_name(
             self):
-        class NonStr(object):
+        class NonStr:
             def __str__(self):
                 raise ValueError('non-str')
         NonStr.__name__ = '<script>'
-        self.assertEqual(u'<unprintable &lt;script&gt; object>',
+        self.assertEqual('<unprintable &lt;script&gt; object>',
                          self.getPrintable(NonStr()))
 
     def test_getFormattedException(self):
         try:
             raise Exception('<boom>')
         except Exception:
             self.assertIn("Exception: &lt;boom&gt;",
@@ -391,45 +385,39 @@
             self.fail("Exception was not raised (should never happen)")
 
         # If this fails because you get '&lt;br /&gt;' instead of '<br />' at
         # the end of the penultimate line, you need zope.exceptions 4.0.3 with
         # the bugfix for that.
 
     def setUp(self):
-        super(GetPrintableTests, self).setUp()
+        super().setUp()
         self.log_buffer = StringIO()
         self.log_handler = logging.StreamHandler(self.log_buffer)
         logging.getLogger().addHandler(self.log_handler)
 
     def tearDown(self):
         logging.getLogger().removeHandler(self.log_handler)
-        super(GetPrintableTests, self).tearDown()
+        super().tearDown()
 
 
 class TestErrorHandler(unittest.TestCase):
 
     def test_round_trip(self):
         # We don't round trip.
 
         text = b'\xe1'.decode('ascii', errors="zope.error.printedreplace")
-        self.assertEqual(text, u"\\xe1")
-        self.assertIsInstance(text, text_type)
+        self.assertEqual(text, "\\xe1")
+        self.assertIsInstance(text, str)
 
         # Note that this is *NOT* what we actually started with.
         # The error handler is never even invoked. It seems that
         # all of Python's built-in encodings can successfully encode
         # ascii-range characters without error
         byte = text.encode('ascii', errors="zope.error.printedreplace")
         self.assertIsInstance(byte, bytes)
         self.assertEqual(byte, b'\\xe1')
 
         # If we do start with  a character outside the ascii range, our
         # handler is invoked and once again escapes.
-        byte = u'\xe1'.encode("ascii", errors="zope.error.printedreplace")
+        byte = '\xe1'.encode("ascii", errors="zope.error.printedreplace")
         self.assertIsInstance(byte, bytes)
         self.assertEqual(byte, b'\\xe1')
-
-
-def test_suite():
-    return unittest.TestSuite([
-        unittest.defaultTestLoader.loadTestsFromName(__name__),
-    ])
```

### Comparing `zope.error-4.6/src/zope.error.egg-info/PKG-INFO` & `zope.error-5.0/src/zope.error.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: zope.error
-Version: 4.6
+Version: 5.0
 Summary: An error reporting utility for Zope3
 Home-page: https://github.com/zopefoundation/zope.error
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope3 error
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
 Provides-Extra: test
@@ -44,14 +40,22 @@
 This package provides an error reporting utility which is able to store errors.
 
 
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
 4.6 (2022-08-29)
 ================
 
 - Add support for Python 3.8, 3.9, 3.10.
 
 - Drop support for Python 3.4.
 
@@ -197,9 +201,7 @@
 
 3.5.0
 =====
 
 - Initial documented release
 
 - Moved core components from ``zope.app.error`` to this package.
-
-
```

### Comparing `zope.error-4.6/src/zope.error.egg-info/SOURCES.txt` & `zope.error-5.0/src/zope.error.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.error-4.6/tox.ini` & `zope.error-5.0/tox.ini`

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
-    coverage report -m --fail-under=99
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=99
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.error
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

