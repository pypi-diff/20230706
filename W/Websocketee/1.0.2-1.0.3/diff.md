# Comparing `tmp/Websocketee-1.0.2.tar.gz` & `tmp/Websocketee-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Websocketee-1.0.2.tar", last modified: Thu Jul  6 10:14:53 2023, max compression
+gzip compressed data, was "dist\Websocketee-1.0.3.tar", last modified: Thu Jul  6 10:25:26 2023, max compression
```

## Comparing `Websocketee-1.0.2.tar` & `Websocketee-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:14:53.632736 Websocketee-1.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-05 10:45:18.000000 Websocketee-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1290 2023-07-06 10:14:53.633736 Websocketee-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-07-05 10:55:31.000000 Websocketee-1.0.2/README.md
--rw-rw-rw-   0        0        0      110 2023-07-06 06:11:35.000000 Websocketee-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      826 2023-07-06 10:14:53.636734 Websocketee-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 10:14:53.590762 Websocketee-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 10:14:53.631737 Websocketee-1.0.2/src/Websocketee.egg-info/
--rw-rw-rw-   0        0        0     1290 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:14:53.000000 Websocketee-1.0.2/src/Websocketee.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 10:25:26.000000 Websocketee-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-05 10:45:18.000000 Websocketee-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1598 2023-07-06 10:25:26.000000 Websocketee-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-07-05 10:55:31.000000 Websocketee-1.0.3/README.md
+-rw-rw-rw-   0        0        0      110 2023-07-06 06:11:35.000000 Websocketee-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      826 2023-07-06 10:25:26.000000 Websocketee-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1680 2023-07-06 10:24:45.000000 Websocketee-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/Websocketee/
+-rw-rw-rw-   0        0        0     7221 2023-07-06 09:57:21.000000 Websocketee-1.0.3/src/Websocketee/overview.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/Websocketee.egg-info/
+-rw-rw-rw-   0        0        0     1598 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/Websocketee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/Websocketee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/Websocketee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/Websocketee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-06 10:25:26.000000 Websocketee-1.0.3/src/Websocketee.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `Websocketee-1.0.2/LICENSE` & `Websocketee-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Websocketee-1.0.2/PKG-INFO` & `Websocketee-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: Websocketee
-Version: 1.0.2
-Summary: Python Isnta-Bot for spaming
-Home-page: https://github.com/pypa/Insta-Spam
-Author: sm02present , SM02
-Author-email: rajnikantmahato@gmail.com
+Version: 1.0.3
+Summary: TYPE YOUR DESCRIPTION HERE
+Home-page: https://github.com/user/reponame
+Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Author: YOUR NAME
+Author-email: your.email@domain.com
+License: MIT
 Project-URL: Bug Tracker, https://github.com/pypa/Insta-Spam/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.7
+Keywords: SOME,MEANINGFULL,KEYWORDS
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <center>Hi  everyone ,
 <marquee> Auther : SM02 , Sm02present </marquee>
 this project only for edeqution perposal
```

### Comparing `Websocketee-1.0.2/README.md` & `Websocketee-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Websocketee-1.0.2/setup.cfg` & `Websocketee-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `Websocketee-1.0.2/src/Websocketee.egg-info/PKG-INFO` & `Websocketee-1.0.3/src/Websocketee.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: Websocketee
-Version: 1.0.2
-Summary: Python Isnta-Bot for spaming
-Home-page: https://github.com/pypa/Insta-Spam
-Author: sm02present , SM02
-Author-email: rajnikantmahato@gmail.com
+Version: 1.0.3
+Summary: TYPE YOUR DESCRIPTION HERE
+Home-page: https://github.com/user/reponame
+Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Author: YOUR NAME
+Author-email: your.email@domain.com
+License: MIT
 Project-URL: Bug Tracker, https://github.com/pypa/Insta-Spam/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.7
+Keywords: SOME,MEANINGFULL,KEYWORDS
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <center>Hi  everyone ,
 <marquee> Auther : SM02 , Sm02present </marquee>
 this project only for edeqution perposal
```

