# Comparing `tmp/mly_pipeline-0.5.3.tar.gz` & `tmp/mly_pipeline-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.5.3.tar", last modified: Wed Jul  5 16:41:05 2023, max compression
+gzip compressed data, was "mly_pipeline-0.5.4.tar", last modified: Thu Jul  6 09:25:44 2023, max compression
```

## Comparing `mly_pipeline-0.5.3.tar` & `mly_pipeline-0.5.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.843629 mly_pipeline-0.5.3/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.3/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.3/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.3/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-05 16:41:05.842629 mly_pipeline-0.5.3/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.3/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.353625 mly_pipeline-0.5.3/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.3/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.344625 mly_pipeline-0.5.3/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.581627 mly_pipeline-0.5.3/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.3/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.3/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.3/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.3/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.3/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.673628 mly_pipeline-0.5.3/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.694628 mly_pipeline-0.5.3/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.3/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.699628 mly_pipeline-0.5.3/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.785629 mly_pipeline-0.5.3/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.3/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.3/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.3/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.3/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.3/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.3/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.3/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.792629 mly_pipeline-0.5.3/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.3/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.3/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.3/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.3/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.3/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.833629 mly_pipeline-0.5.3/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.3/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-06-28 14:28:41.000000 mly_pipeline-0.5.3/mly_pipeline/continuous_FAR.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.3/mly_pipeline/continuous_FAR_test.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    31499 2023-06-29 14:15:00.000000 mly_pipeline-0.5.3/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.3/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33496 2023-06-30 13:55:36.000000 mly_pipeline-0.5.3/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6330 2023-07-05 16:37:33.000000 mly_pipeline-0.5.3/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    21032 2023-06-15 11:06:35.000000 mly_pipeline-0.5.3/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16735 2023-07-05 16:36:01.000000 mly_pipeline-0.5.3/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49651 2023-06-30 11:52:05.000000 mly_pipeline-0.5.3/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.841629 mly_pipeline-0.5.3/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.3/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.3/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-05 16:41:05.839629 mly_pipeline-0.5.3/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-05 16:41:05.000000 mly_pipeline-0.5.3/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-05 16:39:50.000000 mly_pipeline-0.5.3/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-05 16:41:05.843629 mly_pipeline-0.5.3/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:44.434517 mly_pipeline-0.5.4/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.4/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.4/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.4/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-06 09:25:44.433517 mly_pipeline-0.5.4/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.4/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:28.512379 mly_pipeline-0.5.4/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.4/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:28.434378 mly_pipeline-0.5.4/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:30.927400 mly_pipeline-0.5.4/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.4/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.4/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.4/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.4/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.4/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:32.345412 mly_pipeline-0.5.4/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:33.501422 mly_pipeline-0.5.4/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.4/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:35.737442 mly_pipeline-0.5.4/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:42.874503 mly_pipeline-0.5.4/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.4/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.4/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.4/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.4/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.4/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.4/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.4/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:43.245507 mly_pipeline-0.5.4/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.4/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.4/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.4/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.4/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.4/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:44.414517 mly_pipeline-0.5.4/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.4/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-06-28 14:28:41.000000 mly_pipeline-0.5.4/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.4/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    31499 2023-06-29 14:15:00.000000 mly_pipeline-0.5.4/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.4/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33496 2023-06-30 13:55:36.000000 mly_pipeline-0.5.4/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6330 2023-07-05 16:37:33.000000 mly_pipeline-0.5.4/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    21032 2023-06-15 11:06:35.000000 mly_pipeline-0.5.4/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16729 2023-07-06 09:18:53.000000 mly_pipeline-0.5.4/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49651 2023-06-30 11:52:05.000000 mly_pipeline-0.5.4/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:44.431517 mly_pipeline-0.5.4/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.4/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.4/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-06 09:25:44.427517 mly_pipeline-0.5.4/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-06 09:25:28.000000 mly_pipeline-0.5.4/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-06 09:25:28.000000 mly_pipeline-0.5.4/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-06 09:25:28.000000 mly_pipeline-0.5.4/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-06 09:25:28.000000 mly_pipeline-0.5.4/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-06 09:25:28.000000 mly_pipeline-0.5.4/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-06 09:25:28.000000 mly_pipeline-0.5.4/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-06 09:18:28.000000 mly_pipeline-0.5.4/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-06 09:25:44.434517 mly_pipeline-0.5.4/setup.cfg
```

### Comparing `mly_pipeline-0.5.3/.gitlab-ci.yml` & `mly_pipeline-0.5.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/LICENSE` & `mly_pipeline-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/PKG-INFO` & `mly_pipeline-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.5.3
+Version: 0.5.4
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.3/README.md` & `mly_pipeline-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/Makefile` & `mly_pipeline-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.5.4/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/index.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.5.4/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/Getting Started.html` & `mly_pipeline-0.5.4/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/GettingStarted.html` & `mly_pipeline-0.5.4/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/How to use.html` & `mly_pipeline-0.5.4/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/HowToUse.html` & `mly_pipeline-0.5.4/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/Installation.html` & `mly_pipeline-0.5.4/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_modules/index.html` & `mly_pipeline-0.5.4/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_modules/io.html` & `mly_pipeline-0.5.4/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.5.4/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.5.4/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.5.4/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.5.4/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.5.4/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.5.4/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/basic.css` & `mly_pipeline-0.5.4/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.5.4/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.5.4/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.5.4/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.5.4/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/doctools.js` & `mly_pipeline-0.5.4/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.5.4/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/jquery.js` & `mly_pipeline-0.5.4/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/language_data.js` & `mly_pipeline-0.5.4/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/pygments.css` & `mly_pipeline-0.5.4/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.5.4/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.5.4/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/underscore.js` & `mly_pipeline-0.5.4/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/_static/websupport.js` & `mly_pipeline-0.5.4/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/genindex.html` & `mly_pipeline-0.5.4/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/gettingstarted.html` & `mly_pipeline-0.5.4/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/howtouse.html` & `mly_pipeline-0.5.4/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/index.html` & `mly_pipeline-0.5.4/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/installation.html` & `mly_pipeline-0.5.4/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/objects.inv` & `mly_pipeline-0.5.4/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/py-modindex.html` & `mly_pipeline-0.5.4/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/runningasearch.html` & `mly_pipeline-0.5.4/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/search.html` & `mly_pipeline-0.5.4/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/searchindex.js` & `mly_pipeline-0.5.4/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/build/html/settingupasearch.html` & `mly_pipeline-0.5.4/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/source/conf.py` & `mly_pipeline-0.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/source/index.rst` & `mly_pipeline-0.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/source/installation.rst` & `mly_pipeline-0.5.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/source/runningasearch.rst` & `mly_pipeline-0.5.4/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/docs/source/settingupasearch.rst` & `mly_pipeline-0.5.4/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/__init__.py` & `mly_pipeline-0.5.4/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/continuous_FAR.py` & `mly_pipeline-0.5.4/mly_pipeline/continuous_FAR.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/continuous_FAR_test.py` & `mly_pipeline-0.5.4/mly_pipeline/continuous_FAR_test.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/initialization.py` & `mly_pipeline-0.5.4/mly_pipeline/initialization.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.5.4/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/manager.py` & `mly_pipeline-0.5.4/mly_pipeline/manager.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.5.4/mly_pipeline/mly_to_grace.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/offline_search.py` & `mly_pipeline-0.5.4/mly_pipeline/offline_search.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/search.py` & `mly_pipeline-0.5.4/mly_pipeline/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
         # Perform time- and frequency-domain parameter estimation.
         # It adds parameter estimation to events.
         pe_t0 = time.time()
         mly_output = runTimeFrequencyParameterEstimation(thepod,  mly_output)
         logger.info(f"PE time {time.time()- pe_t0}s")
         # If result us above threshold, do all even relate actions 
-        if mly_output["scores"]["combined"] >= 1e-8:#threshold:
+        if mly_output["scores"]["combined"] >= threshold:
 
 
 
             # Saving trigger into the trigger_directory
             with open(f"{config['trigger_directory']}/T_{mly_output['gpstime']}_{detectors}.json", "w") as mly_json:
                 json.dump(mly_output, mly_json,indent=4)
                 mly_json.close()
```

### Comparing `mly_pipeline-0.5.3/mly_pipeline/search_functions.py` & `mly_pipeline-0.5.4/mly_pipeline/search_functions.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.5.4/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.5.4/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.5.4/mly_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.5.3
+Version: 0.5.4
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.3/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.5.4/mly_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.3/pyproject.toml` & `mly_pipeline-0.5.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.5.3"
+version = "0.5.4"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
```

