# Comparing `tmp/avidtools-0.1.1.tar.gz` & `tmp/avidtools-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avidtools-0.1.1.tar", last modified: Wed Jul  5 21:37:09 2023, max compression
+gzip compressed data, was "avidtools-0.1.1.1.tar", last modified: Wed Jul  5 22:23:22 2023, max compression
```

## Comparing `avidtools-0.1.1.tar` & `avidtools-0.1.1.1.tar`

### file list

```diff
@@ -1,14 +1,25 @@
-drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 21:37:09.783896 avidtools-0.1.1/
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)    11357 2023-02-05 19:34:36.000000 avidtools-0.1.1/LICENSE
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      162 2023-07-05 21:37:09.781894 avidtools-0.1.1/PKG-INFO
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      473 2023-07-05 20:58:56.000000 avidtools-0.1.1/README.md
-drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 21:37:09.722894 avidtools-0.1.1/avidtools/
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-02-05 19:35:41.000000 avidtools-0.1.1/avidtools/__init__.py
-drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 21:37:09.770892 avidtools-0.1.1/avidtools.egg-info/
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      162 2023-07-05 21:37:09.000000 avidtools-0.1.1/avidtools.egg-info/PKG-INFO
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      212 2023-07-05 21:37:09.000000 avidtools-0.1.1/avidtools.egg-info/SOURCES.txt
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        1 2023-07-05 21:37:09.000000 avidtools-0.1.1/avidtools.egg-info/dependency_links.txt
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)       50 2023-07-05 21:37:09.000000 avidtools-0.1.1/avidtools.egg-info/requires.txt
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)       10 2023-07-05 21:37:09.000000 avidtools-0.1.1/avidtools.egg-info/top_level.txt
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)       38 2023-07-05 21:37:09.784895 avidtools-0.1.1/setup.cfg
--rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      410 2023-07-05 21:36:47.000000 avidtools-0.1.1/setup.py
+drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 22:23:22.087630 avidtools-0.1.1.1/
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)    11357 2023-02-05 19:34:36.000000 avidtools-0.1.1.1/LICENSE
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      164 2023-07-05 22:23:22.085632 avidtools-0.1.1.1/PKG-INFO
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      617 2023-07-05 22:21:25.000000 avidtools-0.1.1.1/README.md
+drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 22:23:21.911630 avidtools-0.1.1.1/avidtools/
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-02-05 19:35:41.000000 avidtools-0.1.1.1/avidtools/__init__.py
+drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 22:23:22.009630 avidtools-0.1.1.1/avidtools/connectors/
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-02-05 19:36:18.000000 avidtools-0.1.1.1/avidtools/connectors/__init__.py
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-02-05 20:10:17.000000 avidtools-0.1.1.1/avidtools/connectors/aiid.py
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)     2411 2023-06-15 02:17:34.000000 avidtools-0.1.1.1/avidtools/connectors/atlas.py
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)     2418 2023-06-15 19:33:28.000000 avidtools-0.1.1.1/avidtools/connectors/cve.py
+drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 22:23:22.073630 avidtools-0.1.1.1/avidtools/datamodels/
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-02-05 19:36:15.000000 avidtools-0.1.1.1/avidtools/datamodels/__init__.py
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)     1870 2023-06-15 02:17:34.000000 avidtools-0.1.1.1/avidtools/datamodels/components.py
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)     3016 2023-06-15 02:17:34.000000 avidtools-0.1.1.1/avidtools/datamodels/enums.py
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)     1759 2023-06-15 02:17:34.000000 avidtools-0.1.1.1/avidtools/datamodels/report.py
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)     2878 2023-06-15 18:50:16.000000 avidtools-0.1.1.1/avidtools/datamodels/vulnerability.py
+drwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        0 2023-07-05 22:23:21.960630 avidtools-0.1.1.1/avidtools.egg-info/
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      164 2023-07-05 22:23:21.000000 avidtools-0.1.1.1/avidtools.egg-info/PKG-INFO
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      499 2023-07-05 22:23:21.000000 avidtools-0.1.1.1/avidtools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)        1 2023-07-05 22:23:21.000000 avidtools-0.1.1.1/avidtools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)       58 2023-07-05 22:23:21.000000 avidtools-0.1.1.1/avidtools.egg-info/requires.txt
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)       10 2023-07-05 22:23:21.000000 avidtools-0.1.1.1/avidtools.egg-info/top_level.txt
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)       38 2023-07-05 22:23:22.087630 avidtools-0.1.1.1/setup.cfg
+-rwxrwxrwx   0 shubhobm  (1000) shubhobm  (1000)      412 2023-07-05 22:17:22.000000 avidtools-0.1.1.1/setup.py
```

### Comparing `avidtools-0.1.1/LICENSE` & `avidtools-0.1.1.1/LICENSE`

 * *Files identical despite different names*

