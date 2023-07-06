# Comparing `tmp/wagtail-opengraph-image-generator-1.1.tar.gz` & `tmp/wagtail-opengraph-image-generator-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-opengraph-image-generator-1.1.tar", last modified: Wed Apr 22 10:23:49 2020, max compression
+gzip compressed data, was "wagtail-opengraph-image-generator-2.0.tar", last modified: Thu Jul  6 09:36:37 2023, max compression
```

## Comparing `wagtail-opengraph-image-generator-1.1.tar` & `wagtail-opengraph-image-generator-2.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/
--rw-r--r--   0 bkaspar    (502) staff       (20)      612 2020-01-07 10:05:59.000000 wagtail-opengraph-image-generator-1.1/MANIFEST.in
--rw-r--r--   0 bkaspar    (502) staff       (20)     4844 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/PKG-INFO
--rw-r--r--   0 bkaspar    (502) staff       (20)     3557 2020-04-22 10:20:06.000000 wagtail-opengraph-image-generator-1.1/README.md
--rw-r--r--   0 bkaspar    (502) staff       (20)       38 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/setup.cfg
--rw-r--r--   0 bkaspar    (502) staff       (20)     1248 2020-01-07 10:05:59.000000 wagtail-opengraph-image-generator-1.1/setup.py
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/tests/
--rw-r--r--   0 bkaspar    (502) staff       (20)        0 2019-12-20 10:46:41.000000 wagtail-opengraph-image-generator-1.1/tests/__init__.py
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/tests/factories/
--rw-r--r--   0 bkaspar    (502) staff       (20)        0 2019-12-20 11:45:19.000000 wagtail-opengraph-image-generator-1.1/tests/factories/__init__.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      201 2020-01-10 10:39:00.000000 wagtail-opengraph-image-generator-1.1/tests/factories/page.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      592 2019-12-20 14:05:41.000000 wagtail-opengraph-image-generator-1.1/tests/factories/user.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     2424 2020-01-07 12:33:43.000000 wagtail-opengraph-image-generator-1.1/tests/settings.py
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/tests/units/
--rw-r--r--   0 bkaspar    (502) staff       (20)        0 2020-01-07 12:48:00.000000 wagtail-opengraph-image-generator-1.1/tests/units/__init__.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      231 2020-01-08 15:02:09.000000 wagtail-opengraph-image-generator-1.1/tests/units/test_page_factory.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     2479 2020-01-07 10:05:51.000000 wagtail-opengraph-image-generator-1.1/tests/units/test_views.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      245 2019-12-20 10:49:06.000000 wagtail-opengraph-image-generator-1.1/tests/urls.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      333 2020-01-07 10:05:51.000000 wagtail-opengraph-image-generator-1.1/tests/utils.py
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/
--rw-r--r--   0 bkaspar    (502) staff       (20)      380 2020-04-22 10:20:06.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/__init__.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      235 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/apps.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     1111 2020-04-22 10:20:06.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/conf.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     9698 2020-04-22 10:20:06.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/generator.py
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/
--rw-r--r--   0 bkaspar    (502) staff       (20)     1005 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/0001_initial.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     3396 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/0002_auto_20191212_1236.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     1549 2020-04-22 10:20:06.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/0003_auto_20200421_1058.py
--rw-r--r--   0 bkaspar    (502) staff       (20)        0 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/__init__.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     1841 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/models.py
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/
--rw-r--r--   0 bkaspar    (502) staff       (20)    65156 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_black.png
--rw-r--r--   0 bkaspar    (502) staff       (20)    66032 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_white.png
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/
--rw-r--r--   0 bkaspar    (502) staff       (20)   224452 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-bold.ttf
--rw-r--r--   0 bkaspar    (502) staff       (20)   217276 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-regular.ttf
--rw-r--r--   0 bkaspar    (502) staff       (20)     1962 2020-04-22 10:20:06.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/scripts.js
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/templates/
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/templates/wagtail_opengraph_image_generator/
--rw-r--r--   0 bkaspar    (502) staff       (20)     1771 2020-03-11 09:17:23.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/templates/wagtail_opengraph_image_generator/opengraph_tab.html
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/templatetags/
--rw-r--r--   0 bkaspar    (502) staff       (20)        0 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/templatetags/__init__.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      508 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/templatetags/wagtail_opengraph_image_generator_tags.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      239 2019-12-18 08:35:33.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/urls.py
--rw-r--r--   0 bkaspar    (502) staff       (20)      528 2020-03-10 14:46:50.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/views.py
--rw-r--r--   0 bkaspar    (502) staff       (20)     2578 2020-04-22 10:20:06.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/wagtail_hooks.py
-drwxr-xr-x   0 bkaspar    (502) staff       (20)        0 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/
--rw-r--r--   0 bkaspar    (502) staff       (20)     4844 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/PKG-INFO
--rw-r--r--   0 bkaspar    (502) staff       (20)     1869 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/SOURCES.txt
--rw-r--r--   0 bkaspar    (502) staff       (20)        1 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/dependency_links.txt
--rw-r--r--   0 bkaspar    (502) staff       (20)       89 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/requires.txt
--rw-r--r--   0 bkaspar    (502) staff       (20)       40 2020-04-22 10:23:49.000000 wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/top_level.txt
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.881467 wagtail-opengraph-image-generator-2.0/
+-rw-rw-r--   0 benny     (1000) benny     (1000)     1099 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/LICENSE
+-rw-rw-r--   0 benny     (1000) benny     (1000)      612 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/MANIFEST.in
+-rw-rw-r--   0 benny     (1000) benny     (1000)     4133 2023-07-06 09:36:37.881467 wagtail-opengraph-image-generator-2.0/PKG-INFO
+-rw-rw-r--   0 benny     (1000) benny     (1000)     3519 2023-07-06 09:22:55.000000 wagtail-opengraph-image-generator-2.0/README.md
+-rw-rw-r--   0 benny     (1000) benny     (1000)       38 2023-07-06 09:36:37.881467 wagtail-opengraph-image-generator-2.0/setup.cfg
+-rw-rw-r--   0 benny     (1000) benny     (1000)     1238 2023-07-06 09:22:14.000000 wagtail-opengraph-image-generator-2.0/setup.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.877467 wagtail-opengraph-image-generator-2.0/tests/
+-rw-rw-r--   0 benny     (1000) benny     (1000)        0 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/__init__.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.877467 wagtail-opengraph-image-generator-2.0/tests/factories/
+-rw-rw-r--   0 benny     (1000) benny     (1000)        0 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/factories/__init__.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)      201 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/factories/page.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)      592 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/factories/user.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)     2424 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/settings.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.877467 wagtail-opengraph-image-generator-2.0/tests/units/
+-rw-rw-r--   0 benny     (1000) benny     (1000)        0 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/units/__init__.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)      231 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/units/test_page_factory.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)     2479 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/units/test_views.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)      245 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/urls.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)      333 2023-07-06 07:44:47.000000 wagtail-opengraph-image-generator-2.0/tests/utils.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.877467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/
+-rwxrwxr-x   0 benny     (1000) benny     (1000)      380 2023-07-06 09:30:35.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/__init__.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)      235 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/apps.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     1111 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/conf.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     9710 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/generator.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.877467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     1005 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/0001_initial.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     3396 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/0002_auto_20191212_1236.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     1549 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/0003_auto_20200421_1058.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/__init__.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     1805 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/models.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.873467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.877467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/
+-rwxrwxr-x   0 benny     (1000) benny     (1000)    65156 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_black.png
+-rwxrwxr-x   0 benny     (1000) benny     (1000)    66032 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_white.png
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.881467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/
+-rwxrwxr-x   0 benny     (1000) benny     (1000)   224452 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-bold.ttf
+-rwxrwxr-x   0 benny     (1000) benny     (1000)   217276 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-regular.ttf
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     1962 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/scripts.js
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.873467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/templates/
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.881467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/templates/wagtail_opengraph_image_generator/
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     1766 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/templates/wagtail_opengraph_image_generator/opengraph_tab.html
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.881467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/templatetags/
+-rwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/templatetags/__init__.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)      508 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/templatetags/wagtail_opengraph_image_generator_tags.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)      239 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/urls.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)      523 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/views.py
+-rwxrwxr-x   0 benny     (1000) benny     (1000)     2553 2023-07-06 08:36:22.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/wagtail_hooks.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-07-06 09:36:37.877467 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/
+-rw-rw-r--   0 benny     (1000) benny     (1000)     4133 2023-07-06 09:36:37.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/PKG-INFO
+-rw-rw-r--   0 benny     (1000) benny     (1000)     1877 2023-07-06 09:36:37.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benny     (1000) benny     (1000)        1 2023-07-06 09:36:37.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benny     (1000) benny     (1000)       79 2023-07-06 09:36:37.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/requires.txt
+-rw-rw-r--   0 benny     (1000) benny     (1000)       40 2023-07-06 09:36:37.000000 wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wagtail-opengraph-image-generator-1.1/MANIFEST.in` & `wagtail-opengraph-image-generator-2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/PKG-INFO` & `wagtail-opengraph-image-generator-2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,101 @@
 Metadata-Version: 2.1
 Name: wagtail-opengraph-image-generator
-Version: 1.1
+Version: 2.0
 Summary: Wagtail addon to assist in creating Open Graph images for your pages
 Home-page: https://github.com/candylabshq/wagtail-opengraph-image-generator
 Author: Candylabs GmbH
 Author-email: info@candylabs.de
 License: MIT
-Description: # wagtail-opengraph-image-generator
-        
-        Wagtail Open Graph Image Generator will assist you in automatically creating [Open Graph](https://ogp.me/) images for your pages.
-        
-        There are a handful of configuration options to popuplate images with your page's content.
-        Besides the title, there are options to provide a static company logo, subtitle, background image and page logo in the SVG format. While the resulting image will be a little bit opinionated, the defaults should work just fine in most cases.
-        
-        The final image will be saved in the PNG format in a configurable Wagtail collection. It then can be used in your templates and code.
-        
-        ## Features
-        
-        * Automatic creation of Open Graph protocol compatible images
-        * Live preview and configuration in a seperate tab in the Edit and Create views
-        * Several dynamic fields that can be configured to supply content for your generated image
-        
-        ## Requirements
-        
-        * Python 3.6+
-        * Wagtail 2.7 LTS or Wagtail 2.8
-        * Django 2.2 LTS or Django 3.0
-        * `wagtail.contrib.settings` in `INSTALLED_APPS`
-        
-        _Other versions might work but have not been tested._
-        
-        ## Installation
-        
-        Install with pip:
-        `pip install wagtail-opengraph-image-generator`
-        
-        Add `wagtail_opengraph_image_generator` to your `INSTALLED_APPS`
-        
-        Finally, apply the migrations with `python manage.py migrate`
-        
-        ## Usage
-        
-        Once the addon is installed, you will notice a new tab in your edit/create view.
-        
-        ![The injected new tab](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/edit_view.png)
-        
-        This new panel will allow you to preview your new Open Graph image before you save it.
-        Depending on your exact configuration this panel will provide slightly different options and customizations.
-        
-        ### Embedding in your template
-        
-        Accessing the generated image is done with an image tag. Make sure to load it in your template and call `get_existing_og_image [page-object]` to save the image in a variable. You can then use it as any other Wagtail image.
-        
-        ```
-        {% load wagtail_opengraph_image_generator_tags %}
-        
-        {% get_existing_og_image self as og_image %}
-        
-        {% if og_image %}
-            {% image og_image original as og_image %}
-            <meta property="og:image" content="{{ self.get_site.root_url }}{{ og_image.url }}">
-        {% endif %}
-        ```
-        
-        ## Examples
-        
-        A basic example with a default background image, company logo and subtitle might look like this:
-        
-        ![Basic image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/basic_image_example.png)
-        
-        A more advanced example with additional background and page logo fields might look like this:
-        
-        ![Full image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/full_image_example.png)
-        
-        
-        ## Documentation
-        
-        For more information on getting started, an overview of all available settings and release notes, please see [our documentation on Read the Docs](https://wagtail-opengraph-image-generator.readthedocs.io/en/latest/).
-        
-        ## Support
-        
-        Feel free to open issues and, even better, pull requests!
-        
-        The development of this plugin is supported by [candylabs GmbH](https://go.candylabs.de/aqPw)
-        
-        If you need commerical support developing a Wagtail site, Django application, MVP or digital platform, we'd love to hear from you at [info@candylabs.de](mailto:info@candylabs.de)!
-        
-        ![https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg](https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg)
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
+License-File: LICENSE
+
+# wagtail-opengraph-image-generator
+
+Wagtail Open Graph Image Generator will assist you in automatically creating [Open Graph](https://ogp.me/) images for your pages.
+
+There are a handful of configuration options to popuplate images with your page's content.
+Besides the title, there are options to provide a static company logo, subtitle, background image and page logo in the SVG format. While the resulting image will be a little bit opinionated, the defaults should work just fine in most cases.
+
+The final image will be saved in the PNG format in a configurable Wagtail collection. It then can be used in your templates and code.
+
+## Features
+
+* Automatic creation of Open Graph protocol compatible images
+* Live preview and configuration in a seperate tab in the Edit and Create views
+* Several dynamic fields that can be configured to supply content for your generated image
+
+## Requirements
+
+* Python 3.7+
+* Wagtail 4
+* Django 3.0+
+* `wagtail.contrib.settings` in `INSTALLED_APPS`
+
+_Other versions might work but have not been tested._
+
+## Installation
+
+Install with pip:
+`pip install wagtail-opengraph-image-generator`
+
+Add `wagtail_opengraph_image_generator` to your `INSTALLED_APPS`
+
+Finally, apply the migrations with `python manage.py migrate`
+
+## Usage
+
+Once the addon is installed, you will notice a new tab in your edit/create view.
+
+![The injected new tab](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/edit_view.png)
+
+This new panel will allow you to preview your new Open Graph image before you save it.
+Depending on your exact configuration this panel will provide slightly different options and customizations.
+
+### Embedding in your template
+
+Accessing the generated image is done with an image tag. Make sure to load it in your template and call `get_existing_og_image [page-object]` to save the image in a variable. You can then use it as any other Wagtail image.
+
+```
+{% load wagtail_opengraph_image_generator_tags %}
+
+{% get_existing_og_image self as og_image %}
+
+{% if og_image %}
+    {% image og_image original as og_image %}
+    <meta property="og:image" content="{{ self.get_site.root_url }}{{ og_image.url }}">
+{% endif %}
+```
+
+## Examples
+
+A basic example with a default background image, company logo and subtitle might look like this:
+
+![Basic image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/basic_image_example.png)
+
+A more advanced example with additional background and page logo fields might look like this:
+
+![Full image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/full_image_example.png)
+
+
+## Documentation
+
+For more information on getting started, an overview of all available settings and release notes, please see [our documentation on Read the Docs](https://wagtail-opengraph-image-generator.readthedocs.io/en/latest/).
+
+## Support
+
+Feel free to open issues and, even better, pull requests!
+
+The development of this plugin is supported by [candylabs GmbH](https://go.candylabs.de/aqPw)
+
+If you need commerical support developing a Wagtail site, Django application, MVP or digital platform, we'd love to hear from you at [info@candylabs.de](mailto:info@candylabs.de)!
+
+![https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg](https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg)
+
+
```

### Comparing `wagtail-opengraph-image-generator-1.1/README.md` & `wagtail-opengraph-image-generator-2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 * Automatic creation of Open Graph protocol compatible images
 * Live preview and configuration in a seperate tab in the Edit and Create views
 * Several dynamic fields that can be configured to supply content for your generated image
 
 ## Requirements
 
-* Python 3.6+
-* Wagtail 2.7 LTS or Wagtail 2.8
-* Django 2.2 LTS or Django 3.0
+* Python 3.7+
+* Wagtail 4
+* Django 3.0+
 * `wagtail.contrib.settings` in `INSTALLED_APPS`
 
 _Other versions might work but have not been tested._
 
 ## Installation
 
 Install with pip:
```

### Comparing `wagtail-opengraph-image-generator-1.1/setup.py` & `wagtail-opengraph-image-generator-2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     author="Candylabs GmbH",
     author_email="info@candylabs.de",
     description="Wagtail addon to assist in creating Open Graph images for your pages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/candylabshq/wagtail-opengraph-image-generator",
     packages=setuptools.find_packages(),
-    license='MIT',
+    license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Framework :: Django",
         "Framework :: Wagtail",
     ],
     install_requires=[
-        'wagtail>=2.6,<3.0',
-        'CairoSVG>=2.4.0,<2.5',
-        'Pillow>=6.2.0,<6.3',
+        "wagtail>=4.0,<5.0",
+        "CairoSVG==2.7.0",
+        "Pillow==9.5.0",
     ],
     tests_require=[
-        'pytest',
-        'pytest-pythonpath',
-        'pytest-django',
-        'pytest-factoryboy',
-        'psycopg2>=2.5.4',
+        "pytest",
+        "pytest-pythonpath",
+        "pytest-django",
+        "pytest-factoryboy",
+        "psycopg2>=2.5.4",
     ],
-    extras_require={'doc': ['mkdocs', 'markdown-include']},
-    python_requires='>=3.6',
+    extras_require={"doc": ["mkdocs", "markdown-include"]},
+    python_requires=">=3.7",
     include_package_data=True,
 )
```

### Comparing `wagtail-opengraph-image-generator-1.1/tests/factories/user.py` & `wagtail-opengraph-image-generator-2.0/tests/factories/user.py`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/tests/settings.py` & `wagtail-opengraph-image-generator-2.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/tests/units/test_views.py` & `wagtail-opengraph-image-generator-2.0/tests/units/test_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/conf.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/conf.py`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/generator.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 from cairosvg import svg2png
 from base64 import urlsafe_b64encode
 
 from django.utils.html import strip_tags
 from django.core.files.uploadedfile import InMemoryUploadedFile
 from django.templatetags.static import static
 
-from wagtail.core import hooks
-from wagtail.core.models import Collection
-from wagtail.images.models import Image as WagtailImage
+from wagtail import hooks
+from wagtail.models import Collection
+from wagtail.images import get_image_model
 from wagtail.documents.models import Document
 
 from .conf import setting
 from .models import OpenGraphImageGeneratorSettings
 
 
+WagtailImage = get_image_model()
+
+
 OG_WIDTH = setting('IMAGE_WIDTH')
 OG_HEIGHT = setting('IMAGE_HEIGHT')
 OG_PADDING = setting('IMAGE_PADDING')
 
 TEXT_START_X = OG_PADDING
 TEXT_START_Y = OG_HEIGHT - OG_PADDING
 COLOR_WHITE = (255, 255, 255, 255)
```

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/0001_initial.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/0002_auto_20191212_1236.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/0002_auto_20191212_1236.py`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/migrations/0003_auto_20200421_1058.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/migrations/0003_auto_20200421_1058.py`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/models.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.db import models
 
 from wagtail.images import get_image_model_string
 from wagtail.contrib.settings.models import BaseSetting, register_setting
-from wagtail.images.edit_handlers import ImageChooserPanel
+from wagtail.admin.panels import FieldPanel
 
 from .conf import get_page_model
 
 
 class OpenGraphImage(models.Model):
     page = models.ForeignKey(
         get_page_model(),
@@ -51,11 +51,11 @@
         blank=True,
         on_delete=models.CASCADE,
         related_name='+',
         help_text='Alternative version of your logo for the dark OpenGraph image variant. You may want to supply a differently colored logo.',
     )
 
     panels = [
-        ImageChooserPanel('default_background_image'),
-        ImageChooserPanel('company_logo'),
-        ImageChooserPanel('company_logo_alternative'),
+        FieldPanel('default_background_image'),
+        FieldPanel('company_logo'),
+        FieldPanel('company_logo_alternative'),
     ]
```

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_black.png` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_black.png`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_white.png` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fade_white.png`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-bold.ttf` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-regular.ttf` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/fonts/opensans-regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/scripts.js` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/static/wagtail_opengraph_image_generator/scripts.js`

 * *Files identical despite different names*

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/templates/wagtail_opengraph_image_generator/opengraph_tab.html` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/templates/wagtail_opengraph_image_generator/opengraph_tab.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% include "wagtailadmin/edit_handlers/object_list.html" %}
+{% include "wagtailadmin/panels/object_list.html" %}
 
 {% load wagtail_opengraph_image_generator_tags wagtailimages_tags %}
 
 <style>
 .og-field {
     display: block;
     float: none;
@@ -26,39 +26,42 @@
 }
 </style>
 
 {% get_existing_og_image self.instance as og_img %}
 {% get_og_image_generator_setting 'CREATE_AUTOMATICALLY' as CREATE_AUTOMATICALLY %}
 
 {% if og_img %}
-    <div class="nice-padding">
+    <div>
         <h2>Current image</h2>
 
         {% image og_img width-600 %}
     </div>
 
     <hr>
 {% endif %}
 
-<div class="nice-padding">
+<div>
     <h2>Preview &amp; save new image</h2>
 
     {% if CREATE_AUTOMATICALLY %}
         <p>Since you have <code>WAGTAIL_OG_GENERATOR_CREATE_AUTOMATICALLY</code> set to <code>True</code>, a new image will be created and saved automatically when you save this page.</p>
     {% endif %}
 
     <label class="og-field">
         <input type="checkbox" id="id_og_dark_variant" name="og_dark_variant" value="dark"> Use dark variant
     </label>
 
-    <p>Please click the button to generate a preview of your OpenGraph image for this page.</p>
-    <p>Saving a new image will overwrite any existing image.</p>
+    <p style="margin-top: 1rem;">
+        Please click the button to generate a preview of your OpenGraph image for this page.<br/>
+        Saving a new image will overwrite any existing image.
+    </p>
+
     <button class="button" id="btnCreateOGPreview">Generate OpenGraph preview</button>
     
     <div class="og-preview-placeholder"></div>
 
     {% if not CREATE_AUTOMATICALLY %}
         <label class="og-field" style="display: none;">
             <input type="checkbox" id="id_og_save" name="og_save" value="True"> Save this image
         </label>
     {% endif %}
-</div>
+</div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% include "wagtailadmin/edit_handlers/object_list.html" %} {% load
+{% include "wagtailadmin/panels/object_list.html" %} {% load
 wagtail_opengraph_image_generator_tags wagtailimages_tags %}
  {% get_existing_og_image self.instance as og_img %} {%
 get_og_image_generator_setting 'CREATE_AUTOMATICALLY' as CREATE_AUTOMATICALLY
 %} {% if og_img %}
 ***** Current image *****
 {% image og_img width-600 %}
 ===============================================================================
```

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/views.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 
 from django.http import HttpResponse
 from django.views.decorators.csrf import csrf_exempt
 
-from wagtail.core.models import Page
+from wagtail.models import Page
 
 from .conf import get_page_model
 from .generator import create_og_image
 
 
 @csrf_exempt
 def show_preview(request, page_id):
```

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator/wagtail_hooks.py` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator/wagtail_hooks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 from django.conf.urls import include
 from django.urls import path
 from django.utils.html import format_html
 from django.templatetags.static import static
 
-from wagtail.core import hooks
-from wagtail.admin.edit_handlers import FieldPanel, ObjectList
+from wagtail import hooks
+from wagtail.admin.panels import ObjectList, extract_panel_definitions_from_model_class, HelpPanel
+from wagtail.utils.decorators import cached_classmethod
 
 from .conf import setting, get_page_model
 from .generator import create_og_image
 from .models import OpenGraphImage
 
 
 class OpenGraphTemplateTab(ObjectList):
     template = 'wagtail_opengraph_image_generator/opengraph_tab.html'
 
 
-@hooks.register('before_edit_page')
-@hooks.register('before_create_page')
-def add_og_tab(request, page, page_class=None):
-    if not isinstance(page, get_page_model()):
-        return
+@cached_classmethod
+def get_edit_handler(cls):
+    if hasattr(cls, "edit_handler"):
+        edit_handler = cls.edit_handler
+    else:
+        panels = extract_panel_definitions_from_model_class(cls)
+        edit_handler = ObjectList(panels)
 
-    tab = OpenGraphTemplateTab([], heading=setting('TAB_NAME'))
+    tab = OpenGraphTemplateTab(
+        [HelpPanel(template="wagtail_opengraph_image_generator/opengraph_tab.html")], heading=setting('TAB_NAME')
+    )
+    edit_handler.children.append(tab)
+
+    return edit_handler.bind_to_model(cls)
 
-    # page_class is passed to the function when a new page is created
-    if page_class:
-        children = page_class.get_edit_handler().children
-    else:
-        children = page.get_edit_handler().children
 
-    exists = False
-    for child in children:
-        if child.heading == tab.heading:
-            exists = True
-    if not exists:
-        children.append(tab)
+get_page_model().get_edit_handler = get_edit_handler
 
 
 @hooks.register('after_edit_page')
 @hooks.register('after_create_page')
 def save_og_image(request, page):
     if not isinstance(page, get_page_model()):
         return
@@ -71,17 +69,15 @@
             setting('FIELD_TITLE'),
             setting('FIELD_SUBTITLE'),
             setting('FIELD_BACKGROUND_IMAGE'),
             setting('FIELD_LOGO'),
         )
     )
     return str_js + format_html(
-        '<script src="{}"></script>'.format(
-            static('wagtail_opengraph_image_generator/scripts.js')
-        )
+        '<script src="{}"></script>'.format(static('wagtail_opengraph_image_generator/scripts.js'))
     )
 
 
 @hooks.register('register_admin_urls')
 def register_admin_urls():
     from . import urls
```

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/PKG-INFO` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,101 @@
 Metadata-Version: 2.1
 Name: wagtail-opengraph-image-generator
-Version: 1.1
+Version: 2.0
 Summary: Wagtail addon to assist in creating Open Graph images for your pages
 Home-page: https://github.com/candylabshq/wagtail-opengraph-image-generator
 Author: Candylabs GmbH
 Author-email: info@candylabs.de
 License: MIT
-Description: # wagtail-opengraph-image-generator
-        
-        Wagtail Open Graph Image Generator will assist you in automatically creating [Open Graph](https://ogp.me/) images for your pages.
-        
-        There are a handful of configuration options to popuplate images with your page's content.
-        Besides the title, there are options to provide a static company logo, subtitle, background image and page logo in the SVG format. While the resulting image will be a little bit opinionated, the defaults should work just fine in most cases.
-        
-        The final image will be saved in the PNG format in a configurable Wagtail collection. It then can be used in your templates and code.
-        
-        ## Features
-        
-        * Automatic creation of Open Graph protocol compatible images
-        * Live preview and configuration in a seperate tab in the Edit and Create views
-        * Several dynamic fields that can be configured to supply content for your generated image
-        
-        ## Requirements
-        
-        * Python 3.6+
-        * Wagtail 2.7 LTS or Wagtail 2.8
-        * Django 2.2 LTS or Django 3.0
-        * `wagtail.contrib.settings` in `INSTALLED_APPS`
-        
-        _Other versions might work but have not been tested._
-        
-        ## Installation
-        
-        Install with pip:
-        `pip install wagtail-opengraph-image-generator`
-        
-        Add `wagtail_opengraph_image_generator` to your `INSTALLED_APPS`
-        
-        Finally, apply the migrations with `python manage.py migrate`
-        
-        ## Usage
-        
-        Once the addon is installed, you will notice a new tab in your edit/create view.
-        
-        ![The injected new tab](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/edit_view.png)
-        
-        This new panel will allow you to preview your new Open Graph image before you save it.
-        Depending on your exact configuration this panel will provide slightly different options and customizations.
-        
-        ### Embedding in your template
-        
-        Accessing the generated image is done with an image tag. Make sure to load it in your template and call `get_existing_og_image [page-object]` to save the image in a variable. You can then use it as any other Wagtail image.
-        
-        ```
-        {% load wagtail_opengraph_image_generator_tags %}
-        
-        {% get_existing_og_image self as og_image %}
-        
-        {% if og_image %}
-            {% image og_image original as og_image %}
-            <meta property="og:image" content="{{ self.get_site.root_url }}{{ og_image.url }}">
-        {% endif %}
-        ```
-        
-        ## Examples
-        
-        A basic example with a default background image, company logo and subtitle might look like this:
-        
-        ![Basic image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/basic_image_example.png)
-        
-        A more advanced example with additional background and page logo fields might look like this:
-        
-        ![Full image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/full_image_example.png)
-        
-        
-        ## Documentation
-        
-        For more information on getting started, an overview of all available settings and release notes, please see [our documentation on Read the Docs](https://wagtail-opengraph-image-generator.readthedocs.io/en/latest/).
-        
-        ## Support
-        
-        Feel free to open issues and, even better, pull requests!
-        
-        The development of this plugin is supported by [candylabs GmbH](https://go.candylabs.de/aqPw)
-        
-        If you need commerical support developing a Wagtail site, Django application, MVP or digital platform, we'd love to hear from you at [info@candylabs.de](mailto:info@candylabs.de)!
-        
-        ![https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg](https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg)
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
+License-File: LICENSE
+
+# wagtail-opengraph-image-generator
+
+Wagtail Open Graph Image Generator will assist you in automatically creating [Open Graph](https://ogp.me/) images for your pages.
+
+There are a handful of configuration options to popuplate images with your page's content.
+Besides the title, there are options to provide a static company logo, subtitle, background image and page logo in the SVG format. While the resulting image will be a little bit opinionated, the defaults should work just fine in most cases.
+
+The final image will be saved in the PNG format in a configurable Wagtail collection. It then can be used in your templates and code.
+
+## Features
+
+* Automatic creation of Open Graph protocol compatible images
+* Live preview and configuration in a seperate tab in the Edit and Create views
+* Several dynamic fields that can be configured to supply content for your generated image
+
+## Requirements
+
+* Python 3.7+
+* Wagtail 4
+* Django 3.0+
+* `wagtail.contrib.settings` in `INSTALLED_APPS`
+
+_Other versions might work but have not been tested._
+
+## Installation
+
+Install with pip:
+`pip install wagtail-opengraph-image-generator`
+
+Add `wagtail_opengraph_image_generator` to your `INSTALLED_APPS`
+
+Finally, apply the migrations with `python manage.py migrate`
+
+## Usage
+
+Once the addon is installed, you will notice a new tab in your edit/create view.
+
+![The injected new tab](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/edit_view.png)
+
+This new panel will allow you to preview your new Open Graph image before you save it.
+Depending on your exact configuration this panel will provide slightly different options and customizations.
+
+### Embedding in your template
+
+Accessing the generated image is done with an image tag. Make sure to load it in your template and call `get_existing_og_image [page-object]` to save the image in a variable. You can then use it as any other Wagtail image.
+
+```
+{% load wagtail_opengraph_image_generator_tags %}
+
+{% get_existing_og_image self as og_image %}
+
+{% if og_image %}
+    {% image og_image original as og_image %}
+    <meta property="og:image" content="{{ self.get_site.root_url }}{{ og_image.url }}">
+{% endif %}
+```
+
+## Examples
+
+A basic example with a default background image, company logo and subtitle might look like this:
+
+![Basic image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/basic_image_example.png)
+
+A more advanced example with additional background and page logo fields might look like this:
+
+![Full image example](https://raw.githubusercontent.com/candylabshq/wagtail-opengraph-image-generator/master/docs/images/full_image_example.png)
+
+
+## Documentation
+
+For more information on getting started, an overview of all available settings and release notes, please see [our documentation on Read the Docs](https://wagtail-opengraph-image-generator.readthedocs.io/en/latest/).
+
+## Support
+
+Feel free to open issues and, even better, pull requests!
+
+The development of this plugin is supported by [candylabs GmbH](https://go.candylabs.de/aqPw)
+
+If you need commerical support developing a Wagtail site, Django application, MVP or digital platform, we'd love to hear from you at [info@candylabs.de](mailto:info@candylabs.de)!
+
+![https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg](https://candylabs-production.fra1.cdn.digitaloceanspaces.com/website/media/documents/standard_logo_black.svg)
+
+
```

### Comparing `wagtail-opengraph-image-generator-1.1/wagtail_opengraph_image_generator.egg-info/SOURCES.txt` & `wagtail-opengraph-image-generator-2.0/wagtail_opengraph_image_generator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 tests/__init__.py
 tests/settings.py
 tests/urls.py
 tests/utils.py
```

