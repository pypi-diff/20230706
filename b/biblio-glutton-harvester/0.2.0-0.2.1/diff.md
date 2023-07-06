# Comparing `tmp/biblio_glutton_harvester-0.2.0.tar.gz` & `tmp/biblio_glutton_harvester-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblio_glutton_harvester-0.2.0.tar", last modified: Thu Jul  6 10:36:54 2023, max compression
+gzip compressed data, was "biblio_glutton_harvester-0.2.1.tar", last modified: Thu Jul  6 18:17:59 2023, max compression
```

## Comparing `biblio_glutton_harvester-0.2.0.tar` & `biblio_glutton_harvester-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-06 10:36:54.206351 biblio_glutton_harvester-0.2.0/
--rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-07-06 10:18:15.000000 biblio_glutton_harvester-0.2.0/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-06 10:36:54.206351 biblio_glutton_harvester-0.2.0/PKG-INFO
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-06 10:36:54.206351 biblio_glutton_harvester-0.2.0/biblio_glutton_harvester.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-06 10:36:54.000000 biblio_glutton_harvester-0.2.0/biblio_glutton_harvester.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      208 2023-07-06 10:36:54.000000 biblio_glutton_harvester-0.2.0/biblio_glutton_harvester.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-06 10:36:54.000000 biblio_glutton_harvester-0.2.0/biblio_glutton_harvester.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-06 10:36:54.000000 biblio_glutton_harvester-0.2.0/biblio_glutton_harvester.egg-info/top_level.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-06 10:36:54.206351 biblio_glutton_harvester-0.2.0/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      209 2023-07-06 10:35:19.000000 biblio_glutton_harvester-0.2.0/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-06 18:17:59.496637 biblio_glutton_harvester-0.2.1/
+-rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-07-06 10:18:15.000000 biblio_glutton_harvester-0.2.1/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-06 18:17:59.496637 biblio_glutton_harvester-0.2.1/PKG-INFO
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-06 18:17:59.496637 biblio_glutton_harvester-0.2.1/biblio_glutton_harvester.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-06 18:17:59.000000 biblio_glutton_harvester-0.2.1/biblio_glutton_harvester.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      208 2023-07-06 18:17:59.000000 biblio_glutton_harvester-0.2.1/biblio_glutton_harvester.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-06 18:17:59.000000 biblio_glutton_harvester-0.2.1/biblio_glutton_harvester.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-06 18:17:59.000000 biblio_glutton_harvester-0.2.1/biblio_glutton_harvester.egg-info/top_level.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-06 18:17:59.496637 biblio_glutton_harvester-0.2.1/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      209 2023-07-06 18:15:01.000000 biblio_glutton_harvester-0.2.1/setup.py
```

### Comparing `biblio_glutton_harvester-0.2.0/LICENSE` & `biblio_glutton_harvester-0.2.1/LICENSE`

 * *Files identical despite different names*

