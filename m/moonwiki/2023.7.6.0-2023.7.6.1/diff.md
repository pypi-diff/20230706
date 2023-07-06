# Comparing `tmp/moonwiki-2023.7.6.0.tar.gz` & `tmp/moonwiki-2023.7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonwiki-2023.7.6.0.tar", last modified: Thu Jul  6 07:55:06 2023, max compression
+gzip compressed data, was "moonwiki-2023.7.6.1.tar", last modified: Thu Jul  6 07:58:04 2023, max compression
```

## Comparing `moonwiki-2023.7.6.0.tar` & `moonwiki-2023.7.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 07:55:06.267166 moonwiki-2023.7.6.0/
--rw-rw-rw-   0        0        0      955 2023-07-06 07:55:06.267166 moonwiki-2023.7.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-07-06 07:20:23.000000 moonwiki-2023.7.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 07:55:06.220289 moonwiki-2023.7.6.0/moonwiki/
--rw-rw-rw-   0        0        0      877 2023-07-05 10:33:38.000000 moonwiki-2023.7.6.0/moonwiki/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:55:06.251533 moonwiki-2023.7.6.0/moonwiki.egg-info/
--rw-rw-rw-   0        0        0      955 2023-07-06 07:55:05.000000 moonwiki-2023.7.6.0/moonwiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-07-06 07:55:06.000000 moonwiki-2023.7.6.0/moonwiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 07:55:05.000000 moonwiki-2023.7.6.0/moonwiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 07:55:05.000000 moonwiki-2023.7.6.0/moonwiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 07:55:06.267166 moonwiki-2023.7.6.0/setup.cfg
--rw-rw-rw-   0        0        0      412 2023-07-06 07:54:54.000000 moonwiki-2023.7.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:04.598734 moonwiki-2023.7.6.1/
+-rw-rw-rw-   0        0        0      918 2023-07-06 07:58:04.598734 moonwiki-2023.7.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-07-06 07:57:21.000000 moonwiki-2023.7.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:04.567481 moonwiki-2023.7.6.1/moonwiki/
+-rw-rw-rw-   0        0        0      877 2023-07-05 10:33:38.000000 moonwiki-2023.7.6.1/moonwiki/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:04.598734 moonwiki-2023.7.6.1/moonwiki.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-07-06 07:58:04.000000 moonwiki-2023.7.6.1/moonwiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-07-06 07:58:04.000000 moonwiki-2023.7.6.1/moonwiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:58:04.000000 moonwiki-2023.7.6.1/moonwiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 07:58:04.000000 moonwiki-2023.7.6.1/moonwiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 07:58:04.614355 moonwiki-2023.7.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      412 2023-07-06 07:57:27.000000 moonwiki-2023.7.6.1/setup.py
```

### Comparing `moonwiki-2023.7.6.0/PKG-INFO` & `moonwiki-2023.7.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: moonwiki
-Version: 2023.7.6.0
+Version: 2023.7.6.1
 Summary: moonwiki is a wiki application made with Python
 Home-page: https://github.com/RixTheTyrunt/moonwiki
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 
 # moonwiki
 <center>
-[![](https://img.shields.io/pypi/v/moonwiki?logo=python&logoColor=ffffff)](https://pypi.org/project/moonwiki)
+![](https://img.shields.io/pypi/v/moonwiki?logo=python&logoColor=ffffff)
 </center>
 moonwiki is a wiki application made with Python that doesn't require:
 - A database
 - External modules
 - Too much configuration
 ## Install
 You can install moonwiki by using `pip`
```

### Comparing `moonwiki-2023.7.6.0/README.md` & `moonwiki-2023.7.6.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # moonwiki
 <center>
-[![](https://img.shields.io/pypi/v/moonwiki?logo=python&logoColor=ffffff)](https://pypi.org/project/moonwiki)
+![](https://img.shields.io/pypi/v/moonwiki?logo=python&logoColor=ffffff)
 </center>
 moonwiki is a wiki application made with Python that doesn't require:
 - A database
 - External modules
 - Too much configuration
 ## Install
 You can install moonwiki by using `pip`
```

### Comparing `moonwiki-2023.7.6.0/moonwiki/__init__.py` & `moonwiki-2023.7.6.1/moonwiki/__init__.py`

 * *Files identical despite different names*

### Comparing `moonwiki-2023.7.6.0/moonwiki.egg-info/PKG-INFO` & `moonwiki-2023.7.6.1/moonwiki.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: moonwiki
-Version: 2023.7.6.0
+Version: 2023.7.6.1
 Summary: moonwiki is a wiki application made with Python
 Home-page: https://github.com/RixTheTyrunt/moonwiki
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 
 # moonwiki
 <center>
-[![](https://img.shields.io/pypi/v/moonwiki?logo=python&logoColor=ffffff)](https://pypi.org/project/moonwiki)
+![](https://img.shields.io/pypi/v/moonwiki?logo=python&logoColor=ffffff)
 </center>
 moonwiki is a wiki application made with Python that doesn't require:
 - A database
 - External modules
 - Too much configuration
 ## Install
 You can install moonwiki by using `pip`
```

