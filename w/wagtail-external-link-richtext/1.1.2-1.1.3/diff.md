# Comparing `tmp/wagtail-external-link-richtext-1.1.2.tar.gz` & `tmp/wagtail-external-link-richtext-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-external-link-richtext-1.1.2.tar", last modified: Wed Jul  5 12:23:09 2023, max compression
+gzip compressed data, was "wagtail-external-link-richtext-1.1.3.tar", last modified: Thu Jul  6 13:07:02 2023, max compression
```

## Comparing `wagtail-external-link-richtext-1.1.2.tar` & `wagtail-external-link-richtext-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.312514 wagtail-external-link-richtext-1.1.2/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1058 2023-07-04 11:49:42.000000 wagtail-external-link-richtext-1.1.2/LICENSE
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       77 2023-07-05 12:06:28.000000 wagtail-external-link-richtext-1.1.2/MANIFEST.in
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     3690 2023-07-05 12:23:09.312039 wagtail-external-link-richtext-1.1.2/PKG-INFO
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1721 2023-07-05 12:19:42.000000 wagtail-external-link-richtext-1.1.2/README.md
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.302396 wagtail-external-link-richtext-1.1.2/external_link/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.2/external_link/__init__.py
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      894 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.2/external_link/handlers.py
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.303435 wagtail-external-link-richtext-1.1.2/external_link/migrations/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        0 2023-07-03 11:48:23.000000 wagtail-external-link-richtext-1.1.2/external_link/migrations/__init__.py
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.298012 wagtail-external-link-richtext-1.1.2/external_link/static/
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.304023 wagtail-external-link-richtext-1.1.2/external_link/static/css/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      617 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.2/external_link/static/css/newtab_form.css
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.305016 wagtail-external-link-richtext-1.1.2/external_link/static/js/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     6401 2023-07-03 11:51:09.000000 wagtail-external-link-richtext-1.1.2/external_link/static/js/newtab.js
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1310 2023-07-03 12:07:09.000000 wagtail-external-link-richtext-1.1.2/external_link/wagtail_hooks.py
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     1158 2023-07-05 12:22:52.000000 wagtail-external-link-richtext-1.1.2/pyproject.toml
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       38 2023-07-05 12:23:09.312657 wagtail-external-link-richtext-1.1.2/setup.cfg
-drwxr-xr-x   0 rubenhesselink   (501) staff       (20)        0 2023-07-05 12:23:09.311246 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/
--rw-r--r--   0 rubenhesselink   (501) staff       (20)     3690 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/PKG-INFO
--rw-r--r--   0 rubenhesselink   (501) staff       (20)      508 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/SOURCES.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)        1 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/dependency_links.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       35 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/requires.txt
--rw-r--r--   0 rubenhesselink   (501) staff       (20)       14 2023-07-05 12:23:09.000000 wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/external_link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/external_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/external_link/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/external_link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/external_link/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/external_link/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/external_link/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/external_link/static/css/newtab_form.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/external_link/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/external_link/static/js/newtab.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/external_link/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 13:06:46.000000 wagtail-external-link-richtext-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:07:02.516934 wagtail-external-link-richtext-1.1.3/wagtail_external_link_richtext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-06 13:07:02.000000 wagtail-external-link-richtext-1.1.3/wagtail_external_link_richtext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-06 13:07:02.000000 wagtail-external-link-richtext-1.1.3/wagtail_external_link_richtext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:07:02.000000 wagtail-external-link-richtext-1.1.3/wagtail_external_link_richtext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 13:07:02.000000 wagtail-external-link-richtext-1.1.3/wagtail_external_link_richtext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 13:07:02.000000 wagtail-external-link-richtext-1.1.3/wagtail_external_link_richtext.egg-info/top_level.txt
```

### Comparing `wagtail-external-link-richtext-1.1.2/LICENSE` & `wagtail-external-link-richtext-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.2/PKG-INFO` & `wagtail-external-link-richtext-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-external-link-richtext
-Version: 1.1.2
+Version: 1.1.3
 Summary: A feature for the richtext fields in Wagtail
 Author-email: Ruben Hesselink <ruben@fourdigits.nl>
 License: Copyright 2023 Four Digits
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `wagtail-external-link-richtext-1.1.2/README.md` & `wagtail-external-link-richtext-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.2/external_link/handlers.py` & `wagtail-external-link-richtext-1.1.3/external_link/handlers.py`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.2/external_link/static/css/newtab_form.css` & `wagtail-external-link-richtext-1.1.3/external_link/static/css/newtab_form.css`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.2/external_link/static/js/newtab.js` & `wagtail-external-link-richtext-1.1.3/external_link/static/js/newtab.js`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.2/external_link/wagtail_hooks.py` & `wagtail-external-link-richtext-1.1.3/external_link/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-external-link-richtext-1.1.2/wagtail_external_link_richtext.egg-info/PKG-INFO` & `wagtail-external-link-richtext-1.1.3/wagtail_external_link_richtext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-external-link-richtext
-Version: 1.1.2
+Version: 1.1.3
 Summary: A feature for the richtext fields in Wagtail
 Author-email: Ruben Hesselink <ruben@fourdigits.nl>
 License: Copyright 2023 Four Digits
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

