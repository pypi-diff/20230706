# Comparing `tmp/session-repository-0.1.6.tar.gz` & `tmp/session-repository-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.1.6.tar", last modified: Tue Jul  4 11:22:14 2023, max compression
+gzip compressed data, was "session-repository-0.1.7.tar", last modified: Thu Jul  6 07:25:01 2023, max compression
```

## Comparing `session-repository-0.1.6.tar` & `session-repository-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 11:22:14.013910 session-repository-0.1.6/
--rw-rw-rw-   0        0        0      599 2023-07-04 11:22:14.011911 session-repository-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 11:22:13.977531 session-repository-0.1.6/session_repository/
--rw-rw-rw-   0        0        0     8446 2023-07-04 11:21:39.000000 session-repository-0.1.6/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.6/session_repository/enum.py
--rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.6/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:22:14.006794 session-repository-0.1.6/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 11:22:13.000000 session-repository-0.1.6/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 11:22:14.014910 session-repository-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-04 11:21:46.000000 session-repository-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:01.333123 session-repository-0.1.7/
+-rw-rw-rw-   0        0        0      599 2023-07-06 07:25:01.331092 session-repository-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:01.305547 session-repository-0.1.7/session_repository/
+-rw-rw-rw-   0        0        0     8431 2023-07-06 07:21:41.000000 session-repository-0.1.7/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.7/session_repository/enum.py
+-rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.7/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:01.326988 session-repository-0.1.7/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 07:25:01.334193 session-repository-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-06 07:21:55.000000 session-repository-0.1.7/setup.py
```

### Comparing `session-repository-0.1.6/PKG-INFO` & `session-repository-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.6
+Version: 0.1.7
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.6.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.6/session_repository/core.py` & `session-repository-0.1.7/session_repository/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         logger: Logger,
         literal_binds: bool = True,
     ) -> None:
         self._session_factory = session_factory
         self._logger = logger
         self._literal_binds = literal_binds
 
-    @property
     def session_manager(self):
         return self._session_factory()
 
     def _select(
         self,
         model,
         filters: Optional[_FilterType] = None,
```

### Comparing `session-repository-0.1.6/session_repository/utils.py` & `session-repository-0.1.7/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.1.6/session_repository.egg-info/PKG-INFO` & `session-repository-0.1.7/session_repository.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.6
+Version: 0.1.7
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.6.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.6/setup.py` & `session-repository-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.1.6"
+version = "0.1.7"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

