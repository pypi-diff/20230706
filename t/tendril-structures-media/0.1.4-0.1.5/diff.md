# Comparing `tmp/tendril-structures-media-0.1.4.tar.gz` & `tmp/tendril-structures-media-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-structures-media-0.1.4.tar", last modified: Mon Jul  3 21:51:28 2023, max compression
+gzip compressed data, was "tendril-structures-media-0.1.5.tar", last modified: Thu Jul  6 20:10:49 2023, max compression
```

## Comparing `tendril-structures-media-0.1.4.tar` & `tendril-structures-media-0.1.5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.1.4/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.1.4/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.1.4/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.231627 tendril-structures-media-0.1.4/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.4/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.1.4/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.1.4/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.1.4/src/tendril/apiserver/routers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.1.4/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8204 2023-07-03 21:30:19.000000 tendril-structures-media-0.1.4/src/tendril/apiserver/templates/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.1.4/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/common/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.1.4/src/tendril/common/content/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.1.4/src/tendril/common/content/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.1.4/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.1.4/src/tendril/config/media.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.4/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.235627 tendril-structures-media-0.1.4/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.1.4/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2825 2023-07-02 06:35:46.000000 tendril-structures-media-0.1.4/src/tendril/db/controllers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.4/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5413 2023-07-03 21:34:35.000000 tendril-structures-media-0.1.4/src/tendril/db/models/content.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3958 2023-06-30 09:31:29.000000 tendril-structures-media-0.1.4/src/tendril/db/models/content_formats.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.1.4/src/tendril/db/models/content_thumbnails.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.1.4/src/tendril/interests/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-25 07:24:31.000000 tendril-structures-media-0.1.4/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    12190 2023-07-03 21:22:57.000000 tendril-structures-media-0.1.4/src/tendril/interests/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.1.4/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-23 19:45:28.000000 tendril-structures-media-0.1.4/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1014 2023-07-02 06:35:46.000000 tendril-structures-media-0.1.4/src/tendril/libraries/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/structures/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.1.4/src/tendril/structures/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/structures/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.1.4/src/tendril/structures/content/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril/structures/content/providers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.1.4/src/tendril/structures/content/providers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.1.4/src/tendril/structures/content/providers/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.1.4/src/tendril/structures/content/providers/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-03 21:51:28.000000 tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-07-03 21:51:28.000000 tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-03 21:51:28.000000 tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-07-03 21:51:28.000000 tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-03 21:51:28.000000 tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-03 21:51:28.239627 tendril-structures-media-0.1.4/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.4/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.1.5/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.975284 tendril-structures-media-0.1.5/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.1.5/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-06 20:10:49.987285 tendril-structures-media-0.1.5/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.1.5/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.971284 tendril-structures-media-0.1.5/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.5/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.1.5/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.1.5/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.1.5/src/tendril/apiserver/routers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.1.5/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11378 2023-07-06 20:09:25.000000 tendril-structures-media-0.1.5/src/tendril/apiserver/templates/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.1.5/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/common/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.1.5/src/tendril/common/content/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.1.5/src/tendril/common/content/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.1.5/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.1.5/src/tendril/config/media.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.5/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.979285 tendril-structures-media-0.1.5/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.1.5/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5991 2023-07-06 20:06:27.000000 tendril-structures-media-0.1.5/src/tendril/db/controllers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.5/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6884 2023-07-06 19:13:19.000000 tendril-structures-media-0.1.5/src/tendril/db/models/content.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3958 2023-06-30 09:31:29.000000 tendril-structures-media-0.1.5/src/tendril/db/models/content_formats.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.1.5/src/tendril/db/models/content_thumbnails.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.1.5/src/tendril/interests/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-25 07:24:31.000000 tendril-structures-media-0.1.5/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    15628 2023-07-06 20:06:27.000000 tendril-structures-media-0.1.5/src/tendril/interests/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.1.5/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-23 19:45:28.000000 tendril-structures-media-0.1.5/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1014 2023-07-02 06:35:46.000000 tendril-structures-media-0.1.5/src/tendril/libraries/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/structures/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.1.5/src/tendril/structures/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/structures/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.1.5/src/tendril/structures/content/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril/structures/content/providers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.1.5/src/tendril/structures/content/providers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.1.5/src/tendril/structures/content/providers/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.1.5/src/tendril/structures/content/providers/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-06 20:10:49.000000 tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-07-06 20:10:49.000000 tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-06 20:10:49.000000 tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-07-06 20:10:49.000000 tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-06 20:10:49.000000 tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-06 20:10:49.983285 tendril-structures-media-0.1.5/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.5/tox.ini
```

### Comparing `tendril-structures-media-0.1.4/.gitignore` & `tendril-structures-media-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/.readthedocs.yml` & `tendril-structures-media-0.1.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/.travis.yml` & `tendril-structures-media-0.1.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/LICENSE` & `tendril-structures-media-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/PKG-INFO` & `tendril-structures-media-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.1.4
+Version: 0.1.5
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.1.4/README.rst` & `tendril-structures-media-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/Makefile` & `tendril-structures-media-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/_static/custom.css` & `tendril-structures-media-0.1.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/_static/favicon.ico` & `tendril-structures-media-0.1.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/_static/logo.png` & `tendril-structures-media-0.1.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/_static/logo_packed.png` & `tendril-structures-media-0.1.5/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/_templates/about.html` & `tendril-structures-media-0.1.5/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/conf.py` & `tendril-structures-media-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/index.rst` & `tendril-structures-media-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/docs/installation.rst` & `tendril-structures-media-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/setup.py` & `tendril-structures-media-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/apiserver/templates/content.py` & `tendril-structures-media-0.1.5/src/tendril/apiserver/templates/content.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 
 import os
 from typing import Dict
 from typing import Union
+from typing import Optional
 from pydantic.fields import Field
 
 from fastapi import APIRouter
 from fastapi import Request
 from fastapi import Depends
 from fastapi import File
 from fastapi import Body
@@ -15,14 +16,15 @@
 
 from tendril.authn.users import auth_spec
 from tendril.authn.users import AuthUserModel
 from tendril.authn.users import authn_dependency
 
 from tendril.apiserver.templates.base import ApiRouterGenerator
 from tendril.utils.pydantic import TendrilTORMModel
+from tendril.utils.pydantic import TendrilTBaseModel
 from tendril.utils.db import get_session
 
 from tendril.caching import tokens
 from tendril.caching.tokens import GenericTokenTModel
 
 from tendril.structures.content import content_models
 from tendril.config import MEDIA_EXTENSIONS
@@ -35,14 +37,25 @@
 from tendril.db.models.content import MediaContentInfoFullTModel
 
 
 class ContentTypeDetailTModel(TendrilTORMModel):
     type_description: str = Field(..., alias='display_name')
 
 
+class SequenceDefaultDurationResponseTModel(TendrilTBaseModel):
+    interest_id: int
+    default_duration: int
+
+
+class SequenceAddTModel(TendrilTBaseModel):
+    content_id: int
+    position: Optional[int]
+    duration: Optional[int]
+
+
 class InterestContentRouterGenerator(ApiRouterGenerator):
     def __init__(self, actual):
         super(InterestContentRouterGenerator, self).__init__()
         self._actual = actual
 
     async def accepted_types(self, request: Request,
                              user: AuthUserModel = auth_spec()):
@@ -129,39 +142,91 @@
     async def generate_provider_content(self, request:Request, id:int,
                                         provider_id:int, args: dict=Body(...),
                                         user: AuthUserModel = auth_spec()):
         with get_session() as session:
             interest: MediaContentInterest = self._actual.item(id=id, session=session)
             return interest.generate_from_provider(provider_id, args=args, auth_user=user, session=session)
 
+    async def set_sequence_default_duration(self, request:Request, id:int,
+                                            duration:int = 10000,
+                                            user: AuthUserModel = auth_spec()):
+        with get_session() as session:
+            interest: MediaContentInterest = self._actual.item(id=id, session=session)
+            return interest.sequence_set_default_duration(default_duration=duration, auth_user=user, session=session)
+
+    async def add_to_sequence(self, request:Request, id:int, item: SequenceAddTModel,
+                              full=True, user: AuthUserModel = auth_spec()):
+        with get_session() as session:
+            interest: MediaContentInterest = self._actual.item(id=id, session=session)
+            result = interest.sequence_add(**item.dict(), auth_user=user, session=session)
+
+        if not result:
+            raise Exception
+
+        with get_session() as session:
+            interest: MediaContentInterest = self._actual.item(id=id, session=session)
+            return interest.content_information(full=full, auth_user=user, session=session)
+
+    async def remove_from_sequence(self, request:Request, id:int, position:int,
+                                   full=True, user: AuthUserModel = auth_spec()):
+        with get_session() as session:
+            interest: MediaContentInterest = self._actual.item(id=id, session=session)
+            result = interest.sequence_remove(position=position, auth_user=user, session=session)
+
+        if not result:
+            raise Exception
+
+        with get_session() as session:
+            interest: MediaContentInterest = self._actual.item(id=id, session=session)
+            return interest.content_information(full=full, auth_user=user, session=session)
+
+    async def change_item_duration(self, request:Request, id:int,
+                                   position:int, duration:int,
+                                   user: AuthUserModel = auth_spec()):
+        pass
+
     def generate(self, name):
         desc = f'Content API for {name} Interests'
         prefix = self._actual.interest_class.model.role_spec.prefix
         router = APIRouter(prefix=f'/{name}', tags=[desc],
                            dependencies=[Depends(authn_dependency)])
 
         router.add_api_route("/allowed_types", self.accepted_types, methods=["GET"],
                              response_model=Dict[str, ContentTypeDetailTModel],
                              response_model_exclude_none=True,
                              dependencies=[auth_spec(scopes=[f'{prefix}:read'])], )
 
         router.add_api_route("/{id}/content_info", self.content_info, methods=["GET"],
                              response_model=Union[MediaContentInfoFullTModel, MediaContentInfoTModel],
+                             response_model_exclude_none=True,
                              dependencies=[auth_spec(scopes=[f'{prefix}:read'])])
 
         router.add_api_route("/{id}/formats/info/{format_id}", self.format_info, methods=["GET"],
                              response_model=Union[MediaContentFormatInfoFullTModel, MediaContentFormatInfoTModel],
+                             response_model_exclude_none=True,
                              dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
 
         router.add_api_route("/{id}/formats/upload", self.upload_media_format, methods=["POST"],
                              response_model=GenericTokenTModel,
                              dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
 
         # router.add_api_route("/{id}/formats/delete", self.delete_media_format, methods=["POST"],
         #                      # response_model=[],
         #                      dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
 
         router.add_api_route("/{id}/provider/{provider_id}/generate", self.generate_provider_content, methods=['POST'],
                              # response_model=,
                              dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
 
+        router.add_api_route("/{id}/sequence/duration", self.set_sequence_default_duration, methods=['POST'],
+                             response_model=SequenceDefaultDurationResponseTModel,
+                             dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
+
+        router.add_api_route("/{id}/sequence/add", self.add_to_sequence, methods=['POST'],
+                             # response_model=,
+                             dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
+
+        router.add_api_route("/{id}/sequence/remove/{position}", self.remove_from_sequence, methods=['POST'],
+                             # response_model=,
+                             dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
+
         return [router]
```

### Comparing `tendril-structures-media-0.1.4/src/tendril/common/content/exceptions.py` & `tendril-structures-media-0.1.5/src/tendril/common/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/config/__init__.py` & `tendril-structures-media-0.1.5/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/config/media.py` & `tendril-structures-media-0.1.5/src/tendril/config/media.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/db/models/content.py` & `tendril-structures-media-0.1.5/src/tendril/db/models/content.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from typing import List
 from typing import Union
 from typing import Optional
 from sqlalchemy import Column
 from sqlalchemy import String
 from sqlalchemy import Integer
 from sqlalchemy import ForeignKey
+from sqlalchemy import UniqueConstraint
 from sqlalchemy.orm import Mapped
 from sqlalchemy.orm import mapped_column
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy_json import mutable_json_type
 
+
 from tendril.utils.db import DeclBase
 from tendril.utils.db import BaseMixin
 from tendril.utils.db import TimestampMixin
 from tendril.utils.pydantic import TendrilTBaseModel
 from .content_formats import MediaContentFormatModel
 from .content_formats import ThumbnailListingTModel
 from .content_formats import MediaContentFormatInfoTModel
@@ -30,23 +32,37 @@
 
 class MediaContentInfoTModel(TendrilTBaseModel):
     # TODO Split this into a union of types
     content_type: str
     bg_color: Optional[Any]
     path: Optional[str]
     args: Optional[dict]
-    formats: List[Union[MediaContentFormatInfoFullTModel,
-                        MediaContentFormatInfoTModel]] = []
+    formats: Optional[List[Union[MediaContentFormatInfoFullTModel,
+                                 MediaContentFormatInfoTModel]]]
     thumbnails: Optional[ThumbnailListingTModel]
+    default_duration: Optional[int]
+    contents: Optional[List['SequenceMemberTModel']]
 
 
 class MediaContentInfoFullTModel(MediaContentInfoTModel):
+    estimated_duration: Any
     published: bool
 
 
+class SequenceMemberTModel(TendrilTBaseModel):
+    position: int
+    duration: Optional[int]
+    content: Union[MediaContentInfoFullTModel,
+                   MediaContentInfoTModel]
+
+
+MediaContentInfoTModel.update_forward_refs()
+MediaContentInfoFullTModel.update_forward_refs()
+
+
 class ContentModel(DeclBase, BaseMixin, TimestampMixin):
     type_name = 'generic'
     type_description = "Other"
     content_type = Column(String(32), nullable=False, default=type_name)
     allows_actual_media = False
 
     bg_color = Column(String(20))
@@ -64,14 +80,15 @@
     __mapper_args__ = {
         "polymorphic_identity": type_name,
         "polymorphic_on": content_type
     }
 
     def export(self, full=False):
         rv = {'content_type': self.content_type}
+        rv['estimated_duration'] = self.estimated_duration()
         if self.bg_color:
             rv['bg_color'] = self.bg_color
         return rv
 
     def estimated_duration(self):
         return None
 
@@ -97,15 +114,23 @@
         for fmt in self.formats:
             if len(fmt.thumbnails):
                 rv['thumbnails'] = fmt.export_thumbnails()
                 break
         return rv
 
     def estimated_duration(self):
-        return max([x.estimated_duration for x in self.formats])
+        durations = [x.duration for x in self.formats]
+        simple_durations = [x for x in durations if x > 0]
+        step_durations = [x for x in durations if x < 0]
+        if not len(step_durations):
+            return max(simple_durations)
+        if not len(simple_durations):
+            return min(step_durations)
+        step_durations = [x * -1 * 10000 for x in step_durations]
+        return max(max([simple_durations, step_durations]))
 
 
 class StructuredContentModel(ContentModel):
     type_name = 'structured'
     type_description = "Device Assembled Structured Content"
 
     id = Column(Integer, ForeignKey("Content.id"), primary_key=True)
@@ -128,15 +153,15 @@
 
 
 class SequenceContentModel(ContentModel):
     type_name = 'sequence'
     type_description = "Sequence of other content types"
 
     id = Column(Integer, ForeignKey("Content.id"), primary_key=True)
-    default_duration = Column(Integer, nullable=False, default=10)
+    default_duration = Column(Integer, nullable=False, default=10000)
 
     contents: Mapped[List["SequenceContentAssociationModel"]] = \
         relationship(order_by="SequenceContentAssociationModel.position")
 
     __mapper_args__ = {
         "polymorphic_identity": type_name
     }
@@ -144,20 +169,35 @@
     def export(self, full=False):
         rv = super(SequenceContentModel, self).export(full=full)
         rv['default_duration'] = self.default_duration
         rv['contents'] = [x.export(full=full) for x in self.contents]
         return rv
 
     def estimated_duration(self):
-        contents = self.contents
-        return sum([x.estimated_duration() or self.default_duration
-                    for x in contents]) + len(contents)
+        durations = [x.duration or x.content.estimated_duration() for x in self.contents]
+        actual_durations = []
+        for duration in durations:
+            if duration < 0:
+                padding = 0
+                if duration != -1:
+                    padding = (-1 - duration) * 1000
+                duration = self.default_duration * -1 * duration + padding
+
+            actual_durations.append(duration)
+        return sum(actual_durations) + 1000 * len(durations)
 
 
 class SequenceContentAssociationModel(DeclBase):
     __tablename__ = "SequenceContentAssociation"
     sequence_id: Mapped[int] = mapped_column(ForeignKey("SequenceContent.id"), primary_key=True)
-    content_id: Mapped[int] = mapped_column(ForeignKey("Content.id"), primary_key=True)
-    position: Mapped[int]
+    content_id: Mapped[int] = mapped_column(ForeignKey("Content.id"))
+    position: Mapped[int] = mapped_column(primary_key=True)
     duration: Mapped[Optional[int]]
-    sequence: Mapped[SequenceContentModel] = relationship(back_populates="contents", foreign_keys=[sequence_id])
-    content: Mapped[ContentModel] = relationship(back_populates="sequence_usages", foreign_keys=[content_id])
+    sequence: Mapped[SequenceContentModel] = relationship(back_populates="contents", foreign_keys=[sequence_id], lazy='selectin')
+    content: Mapped[ContentModel] = relationship(back_populates="sequence_usages", foreign_keys=[content_id], lazy='joined')
+
+    def export(self, full=False):
+        return {
+            'position': self.position,
+            'duration': self.duration,
+            'content': self.content.export(full=full)
+        }
```

### Comparing `tendril-structures-media-0.1.4/src/tendril/db/models/content_formats.py` & `tendril-structures-media-0.1.5/src/tendril/db/models/content_formats.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/db/models/content_thumbnails.py` & `tendril-structures-media-0.1.5/src/tendril/db/models/content_thumbnails.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/interests/mixins/content.py` & `tendril-structures-media-0.1.5/src/tendril/interests/mixins/content.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,20 +17,23 @@
 from tendril.common.states import LifecycleStatus
 from tendril.authz.roles.interests import require_state
 from tendril.authz.roles.interests import require_permission
 
 from tendril.caching import tokens
 from tendril.caching.tokens import TokenStatus
 
-from tendril.structures.content import providers
 from tendril.structures.content import content_types
 from tendril.db.models.content import ContentModel
 from tendril.db.controllers.content import create_content
 from tendril.db.controllers.content import create_content_format_file
 from tendril.db.controllers.content import create_content_format_thumbnail
+from tendril.db.controllers.content import sequence_next_position
+from tendril.db.controllers.content import sequence_heal_positions
+from tendril.db.controllers.content import sequence_add_content
+from tendril.db.controllers.content import sequence_remove_content
 from tendril.common.content.exceptions import ContentNotReady
 
 from tendril.utils.parsers.media.info import get_media_info
 from tendril.utils.parsers.media.thumbnails import generate_thumbnails
 
 from tendril.utils.fsutils import TEMPDIR
 from tendril.utils import log
@@ -60,14 +63,15 @@
 
     def __init__(self, *args, content_type=None, **kwargs):
         self._content_type = content_type
         super(MediaContentInterest, self).__init__(*args, **kwargs)
         self._upload_bucket = None
         self._publish_bucket = None
 
+    # Common
     @property
     def content_type(self):
         if not self._content_type:
             self._content_type = self._model_instance.content.content_type
         return self._content_type
 
     @with_db
@@ -77,35 +81,76 @@
                              f"and cannot be changed. Create a new device_content instead.")
         if content_type not in content_types:
             raise ValueError(f"Content Type {content_type} is not recognized. Try one of {content_types}")
         self._content_type = content_type
         self._commit_to_db(session=session)
 
     @property
+    def content(self):
+        return self.model_instance.content
+
+    def published(self):
+        if self.status != LifecycleStatus.ACTIVE:
+            return False
+        content = self.model_instance.content
+        if hasattr(content, "formats"):
+            for fmt in self.model_instance.content.formats:
+                if hasattr(fmt, 'stored_file'):
+                    if fmt.stored_file.bucket != self.publish_bucket:
+                        return False
+        return True
+
+    @with_db
+    @require_state((LifecycleStatus.ACTIVE, LifecycleStatus.APPROVAL, LifecycleStatus.NEW))
+    @require_permission('read_artefacts', strip_auth=False)
+    def content_information(self, full=False, auth_user=None, session=None):
+        if not self._model_instance.content:
+            raise ContentNotReady('read_content_info', self.id, self.name)
+        else:
+            content: ContentModel = self._model_instance.content
+            rv = content.export(full=full)
+            if full:
+                if 'formats' in rv.keys():
+                    for fmt_info in rv['formats']:
+                        fmt_info['published'] = self.format_published(fmt_info['format_id'])
+                rv['published'] = self.published()
+            return rv
+
+    @with_db
+    @require_state((LifecycleStatus.ACTIVE, LifecycleStatus.APPROVAL, LifecycleStatus.NEW))
+    @require_permission('read_artefacts', strip_auth=False)
+    def estimated_duration(self, auth_user=None, session=None):
+        return self._model_instance.content.estimated_duration()
+
+    @with_db
+    def _commit_to_db(self, must_create=False, can_create=True, session=None):
+        super(MediaContentInterest, self)._commit_to_db(must_create=must_create,
+                                                        can_create=can_create,
+                                                        session=session)
+        if not self.model_instance.content_id:
+            content = create_content(type=self._content_type, session=session)
+            self.model_instance.content_id = content.id
+            session.add(self.model_instance)
+            session.commit()
+            session.flush()
+
+    # Media Content
+
+    @property
     def upload_bucket(self):
         if not self._upload_bucket:
             self._upload_bucket = buckets.get_bucket(self.upload_bucket_name)
         return self._upload_bucket
 
     @property
     def publish_bucket(self):
         if not self._publish_bucket:
             self._publish_bucket = buckets.get_bucket(self.publish_bucket_name)
         return self._publish_bucket
 
-    # @with_db
-    # @require_state((LifecycleStatus.NEW))
-    # @require_permission('add_artefact', strip_auth=False)
-    # def create_content(self, content_type, auth_user=None, session=None):
-    #     print("CREATE_CONTENT", content_type, self)
-
-    @property
-    def content(self):
-        return self.model_instance.content
-
     @property
     def formats(self):
         return self.content.formats
 
     @with_db
     @require_state((LifecycleStatus.NEW))
     @require_permission('add_artefact')
@@ -245,14 +290,16 @@
 
     @with_db
     @require_state((LifecycleStatus.NEW))
     @require_permission('delete_artefact', strip_auth=False)
     def delete_format(self, format_id, auth_user=None, session=None):
         pass
 
+    # Content Providers
+
     @with_db
     @require_state((LifecycleStatus.NEW))
     @require_permission('add_artefact', strip_auth=False)
     def generate_from_provider(self, provider_id, args, auth_user=None, session=None):
         if self.content_type != 'structured':
             raise ContentTypeMismatchError(self.content_type, 'structured',
                                            'add_artefact', self.id, self.name)
@@ -261,44 +308,70 @@
         generated = provider.generate(args, auth_user=auth_user, session=session)
         for k, v in generated.items():
             setattr(self.model_instance.content, k, v)
         session.add(self.model_instance.content)
         session.flush()
         return self.model_instance.content
 
-    def published(self):
-        if self.status != LifecycleStatus.ACTIVE:
-            return False
-        content = self.model_instance.content
-        if hasattr(content, "formats"):
-            for fmt in self.model_instance.content.formats:
-                if hasattr(fmt, 'stored_file'):
-                    if fmt.stored_file.bucket != self.publish_bucket:
-                        return False
-        return True
+    # Content Sequence
 
     @with_db
-    @require_state((LifecycleStatus.ACTIVE, LifecycleStatus.APPROVAL, LifecycleStatus.NEW))
-    @require_permission('read_artefacts', strip_auth=False)
-    def content_information(self, full=False, auth_user=None, session=None):
-        if not self._model_instance.content:
-            raise ContentNotReady('read_content_info', self.id, self.name)
-        else:
-            content: ContentModel = self._model_instance.content
-            rv = content.export(full=full)
-            if full:
-                for fmt_info in rv['formats']:
-                    fmt_info['published'] = self.format_published(fmt_info['format_id'])
-                rv['published'] = self.published()
-            return rv
+    @require_state((LifecycleStatus.NEW, LifecycleStatus.APPROVAL, LifecycleStatus.ACTIVE))
+    @require_permission('add_artefact', strip_auth=False)
+    def sequence_set_default_duration(self, default_duration=10, auth_user=None, session=None):
+        if self.content_type != 'sequence':
+            raise ContentTypeMismatchError(self.content_type, 'sequence',
+                                           'add_artefact', self.id, self.name)
+
+        if not isinstance(default_duration, int) or default_duration < 0:
+            raise ValueError("Expecting a non-negative integer for duration")
+
+        self.model_instance.content.default_duration = default_duration
+        session.add(self.model_instance.content)
+        session.flush()
+        return {'interest_id': self.id,
+                'default_duration': self.model_instance.content.default_duration}
 
     @with_db
-    def _commit_to_db(self, must_create=False, can_create=True, session=None):
-        super(MediaContentInterest, self)._commit_to_db(must_create=must_create,
-                                                        can_create=can_create,
-                                                        session=session)
-        if not self.model_instance.content_id:
-            content = create_content(type=self._content_type, session=session)
-            self.model_instance.content_id = content.id
-            session.add(self.model_instance)
-            session.commit()
-            session.flush()
+    @require_state((LifecycleStatus.NEW))
+    @require_permission('add_artefact', strip_auth=False)
+    def sequence_add(self, content_id, position=None, duration=None, auth_user=None, session=None):
+        if self.content_type != 'sequence':
+            raise ContentTypeMismatchError(self.content_type, 'sequence',
+                                           'add_artefact', self.id, self.name)
+
+        # Get Content and Verify Access
+        content = get_interest(content_id, type=self.type_name, session=session).actual
+        if not content.check_user_access(auth_user, 'read', session=session):
+            raise PermissionError("User does not seem to have access to the underlying content. "
+                                  "Cannot add to sequence.")
+
+        if not duration:
+            duration = content.estimated_duration(auth_user=auth_user, session=session)
+
+        if not duration:
+            raise ValueError("We need a duration, however none is provided and the content does "
+                             "not provide it intrinsically.")
+
+        # Create and commit Association Model
+        sequence_add_content(id=self.model_instance.content_id,
+                             content=content.model_instance.content_id,
+                             position=position,
+                             duration=duration,
+                             session=session)
+
+        sequence_heal_positions(id=self.model_instance.content_id, session=session)
+        return True
+
+    @with_db
+    @require_state((LifecycleStatus.NEW))
+    @require_permission('add_artefact', strip_auth=False)
+    def sequence_remove(self, position=None, auth_user=None, session=None):
+        if self.content_type != 'sequence':
+            raise ContentTypeMismatchError(self.content_type, 'sequence',
+                                           'add_artefact', self.id, self.name)
+
+        sequence_remove_content(id=self.model_instance.content_id,
+                                position=position,
+                                session=session)
+        sequence_heal_positions(id=self.model_instance.content_id, session=session)
+        return True
```

### Comparing `tendril-structures-media-0.1.4/src/tendril/libraries/mixins/content.py` & `tendril-structures-media-0.1.5/src/tendril/libraries/mixins/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/structures/content/providers/base.py` & `tendril-structures-media-0.1.5/src/tendril/structures/content/providers/base.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril/structures/content/providers/manager.py` & `tendril-structures-media-0.1.5/src/tendril/structures/content/providers/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/PKG-INFO` & `tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.1.4
+Version: 0.1.5
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/SOURCES.txt` & `tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/src/tendril_structures_media.egg-info/requires.txt` & `tendril-structures-media-0.1.5/src/tendril_structures_media.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/tests/coveralls.py` & `tendril-structures-media-0.1.5/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.4/tox.ini` & `tendril-structures-media-0.1.5/tox.ini`

 * *Files identical despite different names*

