# Comparing `tmp/limberer-0.3.1.tar.gz` & `tmp/limberer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.3.1.tar", last modified: Tue Jul  4 03:26:12 2023, max compression
+gzip compressed data, was "limberer-0.3.2.tar", last modified: Wed Jul  5 21:44:04 2023, max compression
```

## Comparing `limberer-0.3.1.tar` & `limberer-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.3.1/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.3.1/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.3.1/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     9524 2023-07-04 03:26:12.620758 limberer-0.3.1/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     7462 2023-07-04 03:21:11.000000 limberer-0.3.1/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-04 03:25:28.000000 limberer-0.3.1/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-04 03:26:12.620758 limberer-0.3.1/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    11855 2023-07-04 03:17:00.000000 limberer-0.3.1/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6752 2023-07-04 03:01:36.000000 limberer-0.3.1/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5535 2023-07-04 03:22:51.000000 limberer-0.3.1/src/limberer/static/assets/core.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.3.1/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.3.1/src/limberer/static/assets/style.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.3.1/src/limberer/static/custom/custom.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer/static/images/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.3.1/src/limberer/static/images/test1.jpg
--rw-r--r--   0 jtd       (1000) jtd       (1000)      363 2023-07-04 00:11:03.000000 limberer-0.3.1/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3887 2023-07-04 03:17:45.000000 limberer-0.3.1/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1643 2023-07-04 02:27:36.000000 limberer-0.3.1/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.3.1/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.3.1/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-04 01:55:47.000000 limberer-0.3.1/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.3.1/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 03:26:12.620758 limberer-0.3.1/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     9524 2023-07-04 03:26:12.000000 limberer-0.3.1/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-04 03:26:12.000000 limberer-0.3.1/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-04 03:26:12.000000 limberer-0.3.1/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-04 03:26:12.000000 limberer-0.3.1/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-04 03:26:12.000000 limberer-0.3.1/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-04 03:26:12.000000 limberer-0.3.1/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.3.2/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.3.2/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.3.2/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     9524 2023-07-05 21:44:04.253697 limberer-0.3.2/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     7462 2023-07-04 03:21:11.000000 limberer-0.3.2/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-05 19:36:49.000000 limberer-0.3.2/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-05 21:44:04.253697 limberer-0.3.2/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.249698 limberer-0.3.2/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11884 2023-07-05 19:36:00.000000 limberer-0.3.2/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6752 2023-07-04 03:01:36.000000 limberer-0.3.2/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5535 2023-07-04 03:22:51.000000 limberer-0.3.2/src/limberer/static/assets/core.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.3.2/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.3.2/src/limberer/static/assets/style.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.3.2/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.3.2/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      363 2023-07-04 00:11:03.000000 limberer-0.3.2/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3887 2023-07-04 03:17:45.000000 limberer-0.3.2/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1643 2023-07-04 02:27:36.000000 limberer-0.3.2/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.3.2/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.3.2/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-04 01:55:47.000000 limberer-0.3.2/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      576 2023-07-05 19:36:31.000000 limberer-0.3.2/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     9524 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.3.1/LICENSE` & `limberer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/PKG-INFO` & `limberer-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.3.1
+Version: 0.3.2
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.3.1/README.md` & `limberer-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/pyproject.toml` & `limberer-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
```

### Comparing `limberer-0.3.1/src/limberer/__init__.py` & `limberer-0.3.2/src/limberer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     toc.append(opts | {"name": opts['section_name'] + "-columns-title", "issubsection": False})
 
   #print(repr(headers))
   header_level = int(opts.get('toc_header_level', ['1'])[0])
 
   for h in headers:
     if h.level <= header_level:
-      toc.append(opts | {"name": h.identifier, "issubsection": h.level != 1})
+      toc.append(opts | {"name": opts['section_name'] + "-" + h.identifier, "issubsection": h.level != 1})
 
   # pass back to pandoc
   proc2 = subprocess.run(['pandoc', '-f', 'json',
                           '-t', 'html',
                           '--wrap=none'],
                          input=o2, text=True,
                          capture_output=True)
```

### Comparing `limberer-0.3.1/src/limberer/pf.py` & `limberer-0.3.2/src/limberer/pf.py`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/assets/core.css` & `limberer-0.3.2/src/limberer/static/assets/core.css`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/assets/logo.svg` & `limberer-0.3.2/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/assets/style.css` & `limberer-0.3.2/src/limberer/static/assets/style.css`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/images/test1.jpg` & `limberer-0.3.2/src/limberer/static/images/test1.jpg`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/sections/example.md` & `limberer-0.3.2/src/limberer/static/sections/example.md`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/sections/example2.md` & `limberer-0.3.2/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/templates/cover.html` & `limberer-0.3.2/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.3.1/src/limberer/static/templates/toc.html` & `limberer-0.3.2/src/limberer/static/templates/toc.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
     <article id="contents">
       <h3>Table of Contents</h3>
       <ul class="toc">
       {{#sections}}
       {{^issubsection}}
         <li><a class="toc" href="#{{name}}"><div href="#{{name}}" class="toctext"></div><div href="#{{name}}" class="tocpagenr"></div></a></li>
-        <!--<li><a class="toc" href="#{{name}}">{{title}}<div href="#{{name}}" class="tocpagenr"></div></a></li>-->
       {{/issubsection}}
       {{#issubsection}}
         <ul class="toc">
           <li><a class="toc" href="#{{name}}"><div href="#{{name}}" class="toctext"></div><div href="#{{name}}" class="tocpagenr"></div></a></li>
-          <!--<li><a class="toc" href="#{{name}}">{{title}}<div href="#{{name}}" class="tocpagenr"></div></a></li>-->
         </ul>
       {{/issubsection}}
       {{/sections}}
       </ul>
     </article>
```

### Comparing `limberer-0.3.1/src/limberer.egg-info/PKG-INFO` & `limberer-0.3.2/src/limberer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.3.1
+Version: 0.3.2
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.3.1/src/limberer.egg-info/SOURCES.txt` & `limberer-0.3.2/src/limberer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

