# Comparing `tmp/ifileoperation-1.2.4.tar.gz` & `tmp/ifileoperation-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifileoperation-1.2.4.tar", last modified: Tue May 16 03:42:13 2023, max compression
+gzip compressed data, was "ifileoperation-1.2.5.tar", last modified: Thu Jul  6 00:30:45 2023, max compression
```

## Comparing `ifileoperation-1.2.4.tar` & `ifileoperation-1.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.706300 ifileoperation-1.2.4/
--rw-rw-rw-   0        0        0     1514 2023-01-21 01:14:44.000000 ifileoperation-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    10719 2023-05-16 03:42:13.704970 ifileoperation-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     9745 2023-02-06 21:24:02.000000 ifileoperation-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.625270 ifileoperation-1.2.4/ifileoperation/
--rw-rw-rw-   0        0        0      118 2023-05-16 01:34:52.000000 ifileoperation-1.2.4/ifileoperation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.672236 ifileoperation-1.2.4/ifileoperation/com/
--rw-rw-rw-   0        0        0      123 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/__init__.py
--rw-rw-rw-   0        0        0     2796 2023-05-16 01:33:55.000000 ifileoperation-1.2.4/ifileoperation/com/common.py
--rw-rw-rw-   0        0        0      354 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/fileoperation.py
--rw-rw-rw-   0        0        0     9918 2023-01-24 21:26:33.000000 ifileoperation-1.2.4/ifileoperation/com/fileoperationprogresssink.py
--rw-rw-rw-   0        0        0     2153 2023-01-24 21:00:56.000000 ifileoperation-1.2.4/ifileoperation/com/filesysbinddata.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.699455 ifileoperation-1.2.4/ifileoperation/com/interfaces/
--rw-rw-rw-   0        0        0      130 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3311 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperation.py
--rw-rw-rw-   0        0        0     4293 2023-01-24 21:26:33.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperationprogresssink.py
--rw-rw-rw-   0        0        0      798 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ifilesysbinddata.py
--rw-rw-rw-   0        0        0     1185 2023-01-24 21:26:34.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ishellitem.py
--rw-rw-rw-   0        0        0     1903 2023-05-16 01:33:55.000000 ifileoperation-1.2.4/ifileoperation/errors.py
--rw-rw-rw-   0        0        0    11034 2023-05-16 01:45:06.000000 ifileoperation-1.2.4/ifileoperation/fileoperator.py
--rw-rw-rw-   0        0        0    12219 2023-05-16 01:33:55.000000 ifileoperation-1.2.4/ifileoperation/flags.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.643261 ifileoperation-1.2.4/ifileoperation.egg-info/
--rw-rw-rw-   0        0        0    10719 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1714 2023-01-24 21:00:56.000000 ifileoperation-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 03:42:13.706300 ifileoperation-1.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.703959 ifileoperation-1.2.4/tests/
--rw-rw-rw-   0        0        0      849 2023-05-16 01:34:17.000000 ifileoperation-1.2.4/tests/test_ifileoperation.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.171008 ifileoperation-1.2.5/
+-rw-rw-rw-   0        0        0     1514 2023-01-21 01:14:44.000000 ifileoperation-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0    10719 2023-07-06 00:30:45.171008 ifileoperation-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9745 2023-02-06 21:24:02.000000 ifileoperation-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.142041 ifileoperation-1.2.5/ifileoperation/
+-rw-rw-rw-   0        0        0      118 2023-07-06 00:19:55.000000 ifileoperation-1.2.5/ifileoperation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.163850 ifileoperation-1.2.5/ifileoperation/com/
+-rw-rw-rw-   0        0        0      123 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/__init__.py
+-rw-rw-rw-   0        0        0     2796 2023-05-16 01:33:55.000000 ifileoperation-1.2.5/ifileoperation/com/common.py
+-rw-rw-rw-   0        0        0      354 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/fileoperation.py
+-rw-rw-rw-   0        0        0     9918 2023-01-24 21:26:33.000000 ifileoperation-1.2.5/ifileoperation/com/fileoperationprogresssink.py
+-rw-rw-rw-   0        0        0     2168 2023-07-06 00:14:05.000000 ifileoperation-1.2.5/ifileoperation/com/filesysbinddata.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.168851 ifileoperation-1.2.5/ifileoperation/com/interfaces/
+-rw-rw-rw-   0        0        0      130 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3311 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperation.py
+-rw-rw-rw-   0        0        0     4293 2023-01-24 21:26:33.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperationprogresssink.py
+-rw-rw-rw-   0        0        0      798 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ifilesysbinddata.py
+-rw-rw-rw-   0        0        0     1185 2023-01-24 21:26:34.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ishellitem.py
+-rw-rw-rw-   0        0        0     1903 2023-05-16 01:33:55.000000 ifileoperation-1.2.5/ifileoperation/errors.py
+-rw-rw-rw-   0        0        0    11034 2023-05-16 01:45:06.000000 ifileoperation-1.2.5/ifileoperation/fileoperator.py
+-rw-rw-rw-   0        0        0    12219 2023-05-16 01:33:55.000000 ifileoperation-1.2.5/ifileoperation/flags.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.159109 ifileoperation-1.2.5/ifileoperation.egg-info/
+-rw-rw-rw-   0        0        0    10719 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1714 2023-01-24 21:00:56.000000 ifileoperation-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 00:30:45.171008 ifileoperation-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.169851 ifileoperation-1.2.5/tests/
+-rw-rw-rw-   0        0        0      849 2023-05-16 01:34:17.000000 ifileoperation-1.2.5/tests/test_ifileoperation.py
```

### Comparing `ifileoperation-1.2.4/LICENSE` & `ifileoperation-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/PKG-INFO` & `ifileoperation-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifileoperation
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python wrapper for using Win32's IFileOperation for manipulating the filesystem.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: Homepage, https://github.com/lojack5/IFileOperation
 Project-URL: Bug Tracker, https://github.com/lojack5/IFileOperation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ifileoperation-1.2.4/README.md` & `ifileoperation-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/com/common.py` & `ifileoperation-1.2.5/ifileoperation/com/common.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/com/fileoperationprogresssink.py` & `ifileoperation-1.2.5/ifileoperation/com/fileoperationprogresssink.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/com/filesysbinddata.py` & `ifileoperation-1.2.5/ifileoperation/com/filesysbinddata.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,28 +43,28 @@
     bind_ctx.RegisterObjectParam('File System Bind Data', com_ptr(bind_data))
     return bind_ctx
 
 
 FOLDER_BIND_CTX = create_bind_ctx(WIN32_FIND_DATAW(DWORD(FileAttributeFlags.DIRECTORY)))
 
 
-E_FILE_NOT_FOUND = -2147024894
+E_FILE_NOT_FOUND = (-2147024894, -2147024893)
 
 
 def parse_filename(path: StrPath, force: bool = False):
     """Parse a filename into an IShellItem2 instance. If `force` is True, then
     an IShellItem2 instance will be returned even if the file does not exist.
     """
     path = fspath(path)
     try:
         return shell.SHCreateItemFromParsingName(
             path, None, shell.IID_IShellItem2  # type: ignore
         )
     except pywintypes.com_error as e:
-        if e.hresult == E_FILE_NOT_FOUND:  # type: ignore
+        if e.hresult in E_FILE_NOT_FOUND:  # type: ignore
             if force:
                 return shell.SHCreateItemFromParsingName(
                     path, FOLDER_BIND_CTX, shell.IID_IShellItem2
                 )
             else:
                 raise FileNotFoundError(path) from None
         else:
```

### Comparing `ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperation.py` & `ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperation.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperationprogresssink.py` & `ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperationprogresssink.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/com/interfaces/ifilesysbinddata.py` & `ifileoperation-1.2.5/ifileoperation/com/interfaces/ifilesysbinddata.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/com/interfaces/ishellitem.py` & `ifileoperation-1.2.5/ifileoperation/com/interfaces/ishellitem.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/errors.py` & `ifileoperation-1.2.5/ifileoperation/errors.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/fileoperator.py` & `ifileoperation-1.2.5/ifileoperation/fileoperator.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation/flags.py` & `ifileoperation-1.2.5/ifileoperation/flags.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/ifileoperation.egg-info/PKG-INFO` & `ifileoperation-1.2.5/ifileoperation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifileoperation
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python wrapper for using Win32's IFileOperation for manipulating the filesystem.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: Homepage, https://github.com/lojack5/IFileOperation
 Project-URL: Bug Tracker, https://github.com/lojack5/IFileOperation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ifileoperation-1.2.4/ifileoperation.egg-info/SOURCES.txt` & `ifileoperation-1.2.5/ifileoperation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/pyproject.toml` & `ifileoperation-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.4/tests/test_ifileoperation.py` & `ifileoperation-1.2.5/tests/test_ifileoperation.py`

 * *Files identical despite different names*

