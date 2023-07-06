# Comparing `tmp/zope.app.onlinehelp-4.2.0.tar.gz` & `tmp/zope.app.onlinehelp-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.app.onlinehelp-4.2.0.tar", last modified: Tue Apr  5 06:05:32 2022, max compression
+gzip compressed data, was "zope.app.onlinehelp-5.0.tar", last modified: Thu Jul  6 06:27:07 2023, max compression
```

## Comparing `zope.app.onlinehelp-4.2.0.tar` & `zope.app.onlinehelp-5.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.144591 zope.app.onlinehelp-4.2.0/
--rw-r--r--   0 mac        (513) staff       (20)     2455 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)      651 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4702 2022-04-05 06:05:32.144838 zope.app.onlinehelp-4.2.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      888 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      108 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      295 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.099535 zope.app.onlinehelp-4.2.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7610 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      612 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)    11236 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      530 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)      174 2022-04-05 06:05:32.146033 zope.app.onlinehelp-4.2.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     4406 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.085844 zope.app.onlinehelp-4.2.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.100333 zope.app.onlinehelp-4.2.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.106385 zope.app.onlinehelp-4.2.0/src/zope/app/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.117312 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/
--rw-r--r--   0 mac        (513) staff       (20)      153 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/DEPENDENCIES.cfg
--rw-r--r--   0 mac        (513) staff       (20)      121 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/SETUP.cfg
--rw-r--r--   0 mac        (513) staff       (20)     5721 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.126646 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/
--rw-r--r--   0 mac        (513) staff       (20)     3451 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2094 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)      331 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/helptopic.pt
--rw-r--r--   0 mac        (513) staff       (20)      110 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/item.gif
--rw-r--r--   0 mac        (513) staff       (20)      107 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/minus.gif
--rw-r--r--   0 mac        (513) staff       (20)     2791 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/onlinehelp.css
--rw-r--r--   0 mac        (513) staff       (20)     2292 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/onlinehelp_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)      300 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/onlinehelp_navigation_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)      111 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/plus.gif
--rw-r--r--   0 mac        (513) staff       (20)     6538 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tests.py
--rw-r--r--   0 mac        (513) staff       (20)      623 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tree.css
--rw-r--r--   0 mac        (513) staff       (20)     4529 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tree.js
--rw-r--r--   0 mac        (513) staff       (20)     4743 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tree.py
--rw-r--r--   0 mac        (513) staff       (20)     2263 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     5225 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/ftesting.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.132681 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/
--rw-r--r--   0 mac        (513) staff       (20)     3287 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/README.stx
--rw-r--r--   0 mac        (513) staff       (20)      694 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      888 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)      149 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/developer.txt
--rw-r--r--   0 mac        (513) staff       (20)    44222 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/mgmt-main-1.png
--rw-r--r--   0 mac        (513) staff       (20)       64 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/samples.txt
--rw-r--r--   0 mac        (513) staff       (20)     1191 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/ui.stx
--rw-r--r--   0 mac        (513) staff       (20)      721 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/welcome.stx
--rw-r--r--   0 mac        (513) staff       (20)     5966 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      418 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1771 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/metaconfigure.py
--rw-r--r--   0 mac        (513) staff       (20)     2574 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/metadirectives.py
--rw-r--r--   0 mac        (513) staff       (20)       41 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/onlinehelp-configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)       58 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/onlinehelp-meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     5698 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/onlinehelp.py
--rw-r--r--   0 mac        (513) staff       (20)    12782 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/onlinehelptopic.py
--rw-r--r--   0 mac        (513) staff       (20)      898 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.142616 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/
--rw-r--r--   0 mac        (513) staff       (20)      789 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       20 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help.html
--rw-r--r--   0 mac        (513) staff       (20)      204 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help.pt
--rw-r--r--   0 mac        (513) staff       (20)       66 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help.rst
--rw-r--r--   0 mac        (513) staff       (20)       64 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help.stx
--rw-r--r--   0 mac        (513) staff       (20)       15 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help.txt
--rw-r--r--   0 mac        (513) staff       (20)      933 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help.zcml
--rw-r--r--   0 mac        (513) staff       (20)       78 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help2.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.144034 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/output/
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/output/test1.xml
--rw-r--r--   0 mac        (513) staff       (20)      269 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/output/test2.xml
--rw-r--r--   0 mac        (513) staff       (20)      602 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test1.png
--rw-r--r--   0 mac        (513) staff       (20)      602 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test2.png
--rw-r--r--   0 mac        (513) staff       (20)     2898 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test_helpdirectives.py
--rw-r--r--   0 mac        (513) staff       (20)     3518 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test_onlinehelp.py
--rw-r--r--   0 mac        (513) staff       (20)     2882 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test_treeview.py
--rw-r--r--   0 mac        (513) staff       (20)     1000 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/util.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-05 06:05:32.105703 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4702 2022-04-05 06:05:30.000000 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2716 2022-04-05 06:05:31.000000 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-04-05 06:05:30.000000 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       14 2022-04-05 06:05:31.000000 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-04-05 06:05:30.000000 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      779 2022-04-05 06:05:31.000000 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-04-05 06:05:31.000000 zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1390 2022-04-05 06:05:28.000000 zope.app.onlinehelp-4.2.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.432993 zope.app.onlinehelp-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2565 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)      651 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4643 2023-07-06 06:27:07.433057 zope.app.onlinehelp-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      888 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      108 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      295 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.423119 zope.app.onlinehelp-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7610 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      612 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11236 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      559 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      447 2023-07-06 06:27:07.433300 zope.app.onlinehelp-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4277 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.420412 zope.app.onlinehelp-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.423260 zope.app.onlinehelp-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.424553 zope.app.onlinehelp-5.0/src/zope/app/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.426933 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      153 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/DEPENDENCIES.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      121 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/SETUP.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5713 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.429035 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3485 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2094 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      331 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/helptopic.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      110 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/item.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)      107 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/minus.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2791 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/onlinehelp.css
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2292 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/onlinehelp_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      300 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/onlinehelp_navigation_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      111 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/plus.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6500 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      623 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tree.css
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4529 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tree.js
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4753 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tree.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2263 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5225 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/ftesting.zcml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.430450 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3287 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/README.stx
+-rw-r--r--   0 m.howitz   (502) staff       (20)      694 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      888 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      149 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/developer.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    44222 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/mgmt-main-1.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)       64 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/samples.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1191 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/ui.stx
+-rw-r--r--   0 m.howitz   (502) staff       (20)      721 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/welcome.stx
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5985 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      418 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1763 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/metaconfigure.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2692 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/metadirectives.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/onlinehelp-configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/onlinehelp-meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5750 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/onlinehelp.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12648 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/onlinehelptopic.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      900 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.432590 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      789 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help.html
+-rw-r--r--   0 m.howitz   (502) staff       (20)      204 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       66 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       64 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help.stx
+-rw-r--r--   0 m.howitz   (502) staff       (20)       15 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      933 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       78 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help2.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.432860 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/output/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/output/test1.xml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      269 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/output/test2.xml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      602 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test1.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)      602 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test2.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2875 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test_helpdirectives.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3528 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test_onlinehelp.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2882 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test_treeview.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      997 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/util.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:27:07.424398 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4643 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2716 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       14 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      779 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1580 2023-07-06 06:27:07.000000 zope.app.onlinehelp-5.0/tox.ini
```

### Comparing `zope.app.onlinehelp-4.2.0/CHANGES.rst` & `zope.app.onlinehelp-5.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  CHANGES
 =========
 
+5.0 (2023-07-06)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.2.0 (2022-04-05)
 ==================
 
 - Add support for Python 3.7, 3.8, 3.9, and 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.app.onlinehelp-4.2.0/CONTRIBUTING.md` & `zope.app.onlinehelp-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/MANIFEST.in` & `zope.app.onlinehelp-5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/PKG-INFO` & `zope.app.onlinehelp-5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: zope.app.onlinehelp
-Version: 4.2.0
+Version: 5.0
 Summary: Framework for Context-Sensitive Help Pages
 Home-page: http://github.com/zopefoundation/zope.app.onlinehelp
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope3 online help
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
 Provides-Extra: test
@@ -50,14 +46,22 @@
 Documentation is hosted at https://zopeapponlinehelp.readthedocs.io
 
 
 =========
  CHANGES
 =========
 
+5.0 (2023-07-06)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.2.0 (2022-04-05)
 ==================
 
 - Add support for Python 3.7, 3.8, 3.9, and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -140,9 +144,7 @@
 - Enhance the API of topics and simplyfie the view part.
 
 - Implemented getSubTopics() method on topics. This way we can sublist topics.
 
 - Remove unused onlinehelp code in rotterdam template.pt
 
 - Add type to directive, this supports registration of README.txt as 'rest' topics
-
-
```

### Comparing `zope.app.onlinehelp-4.2.0/README.rst` & `zope.app.onlinehelp-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/docs/Makefile` & `zope.app.onlinehelp-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/docs/api.rst` & `zope.app.onlinehelp-5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/docs/conf.py` & `zope.app.onlinehelp-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/setup.py` & `zope.app.onlinehelp-5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.app.onlinehelp package
 
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
 setup(name='zope.app.onlinehelp',
-      version='4.2.0',
+      version='5.0',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       description='Framework for Context-Sensitive Help Pages',
       long_description=(
           read('README.rst')
           + '\n\n' +
           read('CHANGES.rst')
@@ -41,23 +43,20 @@
       keywords="zope3 online help",
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Environment :: Web Environment',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
           'Programming Language :: Python',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: Implementation :: PyPy',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Topic :: Internet :: WWW/HTTP',
           'Framework :: Zope :: 3',
       ],
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/__init__.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     @non_overridable
     def __reduce__(self, proto=None):
         raise TypeError("Not picklable")
     __reduce_ex__ = __reduce__
 
 
-class helpNamespace(object):
+class helpNamespace:
     """ help namespace handler """
 
     def __init__(self, context, request=None):
         self.context = context
 
     def traverse(self, name, ignored):
         """
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/__init__.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """`OnlineHelp` views
 """
 __docformat__ = 'restructuredtext'
 
-from zope.component import createObject, getMultiAdapter
-
+from zope.app.pagetemplate.viewpagetemplatefile import ViewPageTemplateFile
+from zope.component import createObject
+from zope.component import getMultiAdapter
 from zope.publisher.browser import BrowserView
 from zope.publisher.interfaces.browser import IBrowserView
-from zope.traversing.api import getName, getParent
-
-from zope.app.pagetemplate.viewpagetemplatefile import ViewPageTemplateFile
+from zope.traversing.api import getName
+from zope.traversing.api import getParent
 
 from zope.app.onlinehelp import getTopicFor
 
 
 class OnlineHelpTopicView(BrowserView):
     """View for one particular help topic."""
 
@@ -49,15 +49,15 @@
         return view(self)
 
 
 class ContextHelpView(BrowserView):
     """Contextual help view."""
 
     def __init__(self, context, request):
-        super(ContextHelpView, self).__init__(context, request)
+        super().__init__(context, request)
         self.topic = None
 
     def getContextualTopicView(self):
         """Retrieve and render the source of a context help topic """
         topic = self.getContextHelpTopic()
         view = getMultiAdapter((topic, self.request), name='index.html')
         return view.renderTopic()
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/configure.zcml` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/onlinehelp.css` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/onlinehelp.css`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/onlinehelp_macros.pt` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/onlinehelp_macros.pt`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tests.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Functional Tests for Onlinehelp
 
 """
 import os
-import transaction
 import unittest
 
+import transaction
+from webtest import TestApp
 from zope.site.interfaces import IRootFolder
-from zope.app.onlinehelp.tests.test_onlinehelp import testdir
+
 from zope.app.onlinehelp import globalhelp
 from zope.app.onlinehelp.testing import OnlineHelpLayer
-
-from webtest import TestApp
+from zope.app.onlinehelp.tests.test_onlinehelp import testdir
 
 
 class BrowserTestCase(unittest.TestCase):
 
     layer = OnlineHelpLayer
 
     def setUp(self):
-        super(BrowserTestCase, self).setUp()
+        super().setUp()
         self._testapp = TestApp(self.layer.make_wsgi_app())
 
     def checkForBrokenLinks(self, orig_response, path, basic=None):
         response = self.publish(path, basic=basic)
         links = response.html.find_all('a')
 
         for link in links:
@@ -75,16 +75,16 @@
         globalhelp.registerHelpTopic('help2', 'Help2', '', path, IRootFolder,
                                      'contents.html')
 
         transaction.commit()
 
         response = self.publish("/+/action.html", basic='mgr:mgrpw',
                                 form={
-                                    'type_name': u'zope.app.content.File',
-                                    'id': u'file'
+                                    'type_name': 'zope.app.content.File',
+                                    'id': 'file'
                                 })
 
         self.assertEqual(response.getStatus(), 302)
 
         response = self.publish('/contents.html', basic='mgr:mgrpw')
 
         self.assertEqual(response.getStatus(), 200)
@@ -127,21 +127,22 @@
 
 
 class TestZPT(unittest.TestCase):
 
     layer = OnlineHelpLayer
 
     def test_render(self):
-        from zope.app.onlinehelp.browser import ZPTOnlineHelpTopicView
-        from zope.publisher.browser import TestRequest
-        from zope.location.interfaces import LocationError
         from zope.app.rotterdam import Rotterdam
+        from zope.location.interfaces import LocationError
+        from zope.publisher.browser import TestRequest
         from zope.publisher.skinnable import applySkin
 
-        class Context(object):
+        from zope.app.onlinehelp.browser import ZPTOnlineHelpTopicView
+
+        class Context:
             path = os.path.join(os.path.dirname(__file__),
                                 'helptopic.pt')
             title = 'title'
 
         request = TestRequest()
         applySkin(request, Rotterdam)
 
@@ -167,15 +168,15 @@
         view.topic = self
 
         self.assertIs(self, view.getContextHelpTopic())
 
     def test_without_view(self):
         from zope.app.onlinehelp.browser import ContextHelpView
 
-        class Context(object):
+        class Context:
             @property
             def context(self):
                 return self
         context = Context()
         view = ContextHelpView(context, None)
         topic = view.getContextHelpTopic()
         self.assertIs(context, topic)
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tree.css` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tree.css`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tree.js` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tree.js`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/browser/tree.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/browser/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 
 """
 __docformat__ = 'restructuredtext'
 
 from zope.component import getUtility
 from zope.i18n import translate
 from zope.publisher.browser import BrowserView
-from zope.traversing.api import getPath, joinPath
+from zope.traversing.api import getPath
+from zope.traversing.api import joinPath
 
 from zope.app.onlinehelp.interfaces import IOnlineHelp
 
 
 class OnlineHelpTopicTreeView(BrowserView):
     """Online help topic tree view."""
 
     def __init__(self, context, request):
-        super(OnlineHelpTopicTreeView, self).__init__(context, request)
+        super().__init__(context, request)
         self.onlinehelp = getUtility(IOnlineHelp, "OnlineHelp")
 
     def getTopicTree(self):
         """Return the tree of help topics.
 
         We build a flat list of tpoics info dict.
         Iterate this dict oan build from the level info
@@ -104,30 +105,30 @@
             if self.isExpanded(topic):
                 res.append('  %s<li class="expand">' % intend)
             else:
                 res.append('  %s<li>' % intend)
 
             res.append(self.renderLink(item))
             if len(item.getSubTopics()) > 0:
-                res.append('    %s%s' % (
+                res.append('    {}{}'.format(
                     self.renderItemList(item, intend), intend))
             res.append('  %s</li>' % intend)
         res.append('%s</ul>' % intend)
 
         return '\n'.join(res)
 
     def renderLink(self, topic):
         """Render a href element."""
         title = translate(topic.title, context=self.request,
                           default=topic.title)
         if topic.parentPath:
             url = joinPath(topic.parentPath, topic.id)
         else:
             url = topic.id
-        return '<a href="/++help++/%s">%s</a>\n' % (url, title)
+        return '<a href="/++help++/{}">{}</a>\n'.format(url, title)
 
     def isExpanded(self, topic):
         if topic.parentPath:
             path = joinPath(topic.parentPath, topic.id)
         else:
             path = topic.id
         try:
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/configure.zcml` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/ftesting.zcml` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/ftesting.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/README.stx` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/README.stx`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/__init__.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/configure.zcml` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/mgmt-main-1.png` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/mgmt-main-1.png`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/ui.stx` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/ui.stx`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/help/welcome.stx` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/help/welcome.stx`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/interfaces.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 """OnlineHelp Interfaces
 
 These are the interfaces designed for the `OnlineHelp` system.
 
 """
 __docformat__ = 'restructuredtext'
 
-from zope.schema import TextLine, SourceText, Choice
+import zope.i18nmessageid
+from zope.app.file.interfaces import IFile
+from zope.app.publication.interfaces import IFileContent
 from zope.configuration.fields import GlobalInterface
 from zope.container.interfaces import IContainer
-from zope.app.publication.interfaces import IFileContent
-from zope.app.file.interfaces import IFile
-
-import zope.i18nmessageid
+from zope.schema import Choice
+from zope.schema import SourceText
+from zope.schema import TextLine
 
 
 _ = zope.i18nmessageid.MessageFactory("zope")
 
 
 class IOnlineHelpTopic(IContainer):
     """A Topic is a single help page that you can view. Topics are able to
@@ -52,48 +53,48 @@
     have to take care on the registration order.
     The topic resources are stored in the
     :class:`zope.container.interfaces.IContainer` implementation of the topic,
     too.
     """
 
     id = TextLine(
-        title=_(u"Id"),
-        description=_(u"The Id of this Help Topic"),
-        default=u"",
+        title=_("Id"),
+        description=_("The Id of this Help Topic"),
+        default="",
         required=True)
 
     parentPath = TextLine(
-        title=_(u"Parent Path"),
-        description=_(u"The Path to the Parent of this Help Topic"),
-        default=u"",
+        title=_("Parent Path"),
+        description=_("The Path to the Parent of this Help Topic"),
+        default="",
         required=False)
 
     title = TextLine(
-        title=_(u"Help Topic Title"),
-        description=_(u"The Title of a Help Topic"),
-        default=_(u"Help Topic"),
+        title=_("Help Topic Title"),
+        description=_("The Title of a Help Topic"),
+        default=_("Help Topic"),
         required=True)
 
     path = TextLine(
-        title=_(u"Path to the Topic"),
-        description=_(u"The Path to the Definition of a Help Topic"),
-        default=u"./README.TXT",
+        title=_("Path to the Topic"),
+        description=_("The Path to the Definition of a Help Topic"),
+        default="./README.TXT",
         required=True)
 
     interface = GlobalInterface(
-        title=_(u"Object Interface"),
-        description=_(u"Interface for which this Help Topic is registered."),
+        title=_("Object Interface"),
+        description=_("Interface for which this Help Topic is registered."),
         default=None,
         required=False)
 
     view = TextLine(
-        title=_(u"View Name"),
-        description=_(u"The View Name for which this Help Topic"
+        title=_("View Name"),
+        description=_("The View Name for which this Help Topic"
                       " is registered"),
-        default=_(u""),
+        default=_(""),
         required=True)
 
     def addResources(resources):
         """Add resources to this Help Topic.
 
         The resources must be located in the same directory
         as the Help Topic itself.
@@ -107,24 +108,24 @@
         """Returns IOnlineHelpTopic provided childs."""
 
 
 class ISourceTextOnlineHelpTopic(IOnlineHelpTopic):
     """REstructed text based online help topic."""
 
     source = SourceText(
-        title=_(u"Source Text"),
-        description=_(u"Renderable source text of the topic."),
-        default=u"",
+        title=_("Source Text"),
+        description=_("Renderable source text of the topic."),
+        default="",
         required=True,
         readonly=True)
 
     type = Choice(
-        title=_(u"Source Type"),
-        description=_(u"Type of the source text, e.g. structured text"),
-        default=u"zope.source.rest",
+        title=_("Source Type"),
+        description=_("Type of the source text, e.g. structured text"),
+        default="zope.source.rest",
         required=True,
         vocabulary="SourceTypes")
 
 
 class IRESTOnlineHelpTopic(ISourceTextOnlineHelpTopic):
     """REstructed text based online help topic."""
 
@@ -172,12 +173,12 @@
         """
 
 
 class IOnlineHelpResource(IFile, IFileContent):
     """A resource, which can be used in a help topic """
 
     path = TextLine(
-        title=_(u"Path to the Resource"),
-        description=_(u"The Path to the Resource, assumed to be "
+        title=_("Path to the Resource"),
+        description=_("The Path to the Resource, assumed to be "
                       "in the same directory as the Help Topic"),
-        default=u"",
+        default="",
         required=True)
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/metaconfigure.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/metaconfigure.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 """
 __docformat__ = 'restructuredtext'
 
 from zope.app.onlinehelp import globalhelp
 
 
-class OnlineHelpTopicDirective(object):
+class OnlineHelpTopicDirective:
 
     def __init__(self, _context, id, title, parent="", doc_path=None,
                  for_=None, view=None, class_=None, resources=None):
         self._context = _context
         self.id = id
         self.title = title
         self.parent = parent
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/metadirectives.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/metadirectives.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,69 +11,73 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Schemas for the ``help`` ZCML namespace
 """
 __docformat__ = 'restructuredtext'
 
+from zope.configuration.fields import GlobalInterface
+from zope.configuration.fields import GlobalObject
+from zope.configuration.fields import MessageID
+from zope.configuration.fields import Path
+from zope.configuration.fields import Tokens
 from zope.interface import Interface
-from zope.schema import NativeStringLine, TextLine
-from zope.configuration.fields import GlobalInterface, GlobalObject
-from zope.configuration.fields import Path, MessageID, Tokens
+from zope.schema import NativeStringLine
+from zope.schema import TextLine
 
 
 class IOnlineHelpTopicDirective(Interface):
     """Register an online topic.
 
     Optionally you can register a topic for a component and view.
     """
 
     id = NativeStringLine(
-        title=u"Topic Id",
-        description=u"Id of the topic as it will appear in the URL.",
+        title="Topic Id",
+        description="Id of the topic as it will appear in the URL.",
         required=True)
 
     title = MessageID(
-        title=u"Title",
-        description=u"Provides a title for the online Help Topic.",
+        title="Title",
+        description="Provides a title for the online Help Topic.",
         required=True)
 
     parent = NativeStringLine(
-        title=u"Parent Topic",
-        description=u"Id of the parent topic.",
+        title="Parent Topic",
+        description="Id of the parent topic.",
         default="",
         required=False)
 
     for_ = GlobalInterface(
-        title=u"Object Interface",
-        description=u"Interface for which this Help Topic is registered.",
+        title="Object Interface",
+        description="Interface for which this Help Topic is registered.",
         default=None,
         required=False)
 
     view = NativeStringLine(
-        title=u"View Name",
-        description=u"The view name for which this Help Topic is registered.",
+        title="View Name",
+        description="The view name for which this Help Topic is registered.",
         default="",
         required=False)
 
     doc_path = Path(
-        title=u"Path to File",
-        description=u"Path to the file that contains the Help Topic content.",
+        title="Path to File",
+        description="Path to the file that contains the Help Topic content.",
         required=True)
 
     class_ = GlobalObject(
-        title=u"Factory",
-        description=u"""
+        title="Factory",
+        description="""
         The factory is the topic class used for initializeing the topic""",
         required=False,
     )
 
     resources = Tokens(
-        title=u"A list of resources.",
-        description=u"""
+        title="A list of resources.",
+        description="""
         A list of resources which shall be used for the Help Topic.
         The resources must be located in the same directory as
         the Help Topic definition.
         """,
         value_type=TextLine(),
         required=False
     )
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/onlinehelp.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/onlinehelp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 `OnlineHelp` in which all basic Zope-core help screens are registered.
 
 """
 __docformat__ = 'restructuredtext'
 
 import os
 
-from zope.component import getGlobalSiteManager, getUtilitiesFor
-from zope.interface import implementer
+from zope.component import getGlobalSiteManager
+from zope.component import getUtilitiesFor
 from zope.configuration.exceptions import ConfigurationError
-from zope.traversing.interfaces import IContainmentRoot
+from zope.interface import implementer
 from zope.traversing.api import traverse
+from zope.traversing.interfaces import IContainmentRoot
 
-from zope.app.onlinehelp.interfaces import IOnlineHelp, IOnlineHelpTopic
+from zope.app.onlinehelp.interfaces import IOnlineHelp
+from zope.app.onlinehelp.interfaces import IOnlineHelpTopic
 from zope.app.onlinehelp.onlinehelptopic import OnlineHelpTopic
 
 
 @implementer(IOnlineHelp, IContainmentRoot)
 class OnlineHelp(OnlineHelpTopic):
     """
     Implementation of :class:`~.IOnlineHelp`.
@@ -110,15 +112,15 @@
     This topic should now have 'help3' as a child
     >>> 'help3' in missing.keys()
     True
 
     """
 
     def __init__(self, title, path):
-        super(OnlineHelp, self).__init__('', title, path, None)
+        super().__init__('', title, path, None)
 
     def registerHelpTopic(self, parent_path, id, title,
                           doc_path, interface=None, view=None,
                           class_=None, resources=None):
         "See zope.app.onlineHelp.interfaces.IOnlineHelp"
 
         if not os.path.exists(doc_path):
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/onlinehelptopic.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/onlinehelptopic.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Implementation of an Online Help Topic.
 
 """
-from __future__ import absolute_import
+
+
 __docformat__ = 'restructuredtext'
 
 import os
 
 from persistent import Persistent
-from zope.interface import implementer
+from zope.app.file.image import getImageInfo
 from zope.configuration.exceptions import ConfigurationError
-from zope.contenttype import guess_content_type
-
 from zope.container.sample import SampleContainer
-from zope.app.file.image import getImageInfo
+from zope.contenttype import guess_content_type
+from zope.interface import implementer
 
+from zope.app.onlinehelp.interfaces import IOnlineHelpResource
 from zope.app.onlinehelp.interfaces import IOnlineHelpTopic
-from zope.app.onlinehelp.interfaces import ISourceTextOnlineHelpTopic
 from zope.app.onlinehelp.interfaces import IRESTOnlineHelpTopic
+from zope.app.onlinehelp.interfaces import ISourceTextOnlineHelpTopic
 from zope.app.onlinehelp.interfaces import ISTXOnlineHelpTopic
 from zope.app.onlinehelp.interfaces import IZPTOnlineHelpTopic
-from zope.app.onlinehelp.interfaces import IOnlineHelpResource
 
 
 DEFAULT_ENCODING = "utf-8"
 
 try:
     text_type = unicode
 except NameError:
@@ -135,18 +135,18 @@
       >>> topic.addResources(['test1.png', 'test2.png'])
       >>> topic['test1.png'].contentType
       'image/png'
       >>> topic['test2.png'].contentType
       'image/png'
     """
 
-    id = u""
-    title = u""
-    path = u""
-    parentPath = u""
+    id = ""
+    title = ""
+    path = ""
+    parentPath = ""
     interface = None
     view = None
 
     def __init__(self, id, title, path, parentPath, interface=None, view=None):
         """Initialize object."""
         self.id = id
         self.parentPath = parentPath
@@ -156,15 +156,15 @@
         self.view = view
 
         if not os.path.exists(self.path):
             raise ConfigurationError(
                 "Help Topic definition %s does not exist" % self.path
             )
 
-        super(BaseOnlineHelpTopic, self).__init__()
+        super().__init__()
 
     def _newContainerData(self):
         # Ensure consistent iteration order for tests.
         from collections import OrderedDict
         return OrderedDict()
 
     def addResources(self, resources):
@@ -278,16 +278,15 @@
       'image/png'
       >>> topic['test2.png'].contentType
       'image/png'
     """
 
     def __init__(self, id, title, path, parentPath, interface=None, view=None):
         """Initialize object."""
-        super(OnlineHelpTopic, self).__init__(id, title, path, parentPath,
-                                              interface, view)
+        super().__init__(id, title, path, parentPath, interface, view)
 
         filename = os.path.basename(path.lower())
         file_ext = 'txt'
         if len(filename.split('.')) > 1:
             file_ext = filename.split('.')[-1]
 
         self.type = 'zope.source.plaintext'
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/testing.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,12 @@
 """zope.app.onlinehelp common test related classes/functions/objects.
 
 """
 
 __docformat__ = "reStructuredText"
 
 from zope.app.wsgi.testlayer import BrowserLayer
+
 import zope.app.onlinehelp
 
+
 OnlineHelpLayer = BrowserLayer(zope.app.onlinehelp, allowTearDown=True)
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/__init__.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/help.zcml` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/help.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test1.png` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test1.png`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test2.png` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test2.png`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test_helpdirectives.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test_helpdirectives.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,45 +10,47 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test the gts ZCML namespace directives.
 
 """
-from zope.component import testing
-from zope.app.onlinehelp.onlinehelptopic import ZPTOnlineHelpTopic
-from zope.app.onlinehelp.onlinehelptopic import STXOnlineHelpTopic
-from zope.app.onlinehelp.onlinehelptopic import RESTOnlineHelpTopic
-from zope.app.onlinehelp.onlinehelptopic import OnlineHelpTopic
-from zope.app.onlinehelp import globalhelp
 import unittest
 
-from zope.interface import Interface
-from zope.configuration.xmlconfig import XMLConfig
-from zope.component.interfaces import IFactory
+import zope.app.component
+import zope.app.security
+import zope.traversing
+from zope.component import testing
 from zope.component.factory import Factory
+from zope.component.interfaces import IFactory
+from zope.configuration.xmlconfig import XMLConfig
+from zope.interface import Interface
 from zope.security.interfaces import IPermission
 from zope.security.permission import Permission
 
-import zope.traversing
-import zope.app.component
-import zope.app.security
 import zope.app.onlinehelp
+from zope.app.onlinehelp import globalhelp
 from zope.app.onlinehelp import tests
+from zope.app.onlinehelp.onlinehelptopic import OnlineHelpTopic
+from zope.app.onlinehelp.onlinehelptopic import RESTOnlineHelpTopic
+from zope.app.onlinehelp.onlinehelptopic import STXOnlineHelpTopic
+from zope.app.onlinehelp.onlinehelptopic import ZPTOnlineHelpTopic
+
+
 ztapi = tests
 
 
 class I1(Interface):
     pass
 
 
 class DirectivesTest(testing.PlacelessSetup, unittest.TestCase):
 
     def setUp(self):
-        super(DirectivesTest, self).setUp()
+        super().setUp()
         ztapi.provideUtility(IPermission, Permission('zope.View', 'View', ''),
                              'zope.View')
         XMLConfig('meta.zcml', zope.app.security)()
         XMLConfig('meta.zcml', zope.app.component)()
         XMLConfig('meta.zcml', zope.app.onlinehelp)()
         XMLConfig('configure.zcml', zope.traversing)
 
@@ -60,15 +62,15 @@
         ztapi.provideUtility(IFactory, rest, 'onlinehelp.topic.rest')
         ztapi.provideUtility(IFactory, stx, 'onlinehelp.topic.stx')
         ztapi.provideUtility(IFactory, zpt, 'onlinehelp.topic.zpt')
 
     def test_register(self):
         self.assertEqual(list(globalhelp.keys()), [])
         XMLConfig('help.zcml', tests)()
-        res = [u'help4', u'help5', u'help2', u'help3', u'help1']
+        res = ['help4', 'help5', 'help2', 'help3', 'help1']
         res.sort()
 
         helpList = sorted(globalhelp.keys())
         self.assertEqual(helpList, res)
         topic = globalhelp['help1']
         self.assertIn('test1.png', topic.keys())
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test_onlinehelp.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test_onlinehelp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test OnlineHelp
 
 """
-import re
 import os
+import re
 import unittest
 from doctest import DocTestSuite
 
-from zope.interface import Interface, implementer
-from zope.configuration import xmlconfig
 import zope.traversing
 from zope.component import testing
-
+from zope.configuration import xmlconfig
+from zope.interface import Interface
+from zope.interface import implementer
 from zope.testing import renormalizing
 
-from zope.app.onlinehelp import onlinehelptopic
 from zope.app.onlinehelp import onlinehelp
+from zope.app.onlinehelp import onlinehelptopic
 
 
 class I1(Interface):
     pass
 
 
 @implementer(I1)
-class Dummy1(object):
+class Dummy1:
     pass
 
 
-class Dummy2(object):
+class Dummy2:
     pass
 
 
 class TestOnlineHelpResource(unittest.TestCase):
 
     def test_size(self):
         r = onlinehelptopic.OnlineHelpResource(
@@ -83,17 +83,18 @@
         from zope.app.onlinehelp import helpNamespace
 
         traversed = helpNamespace(self).traverse(None, None)
         self.assertIs(traversed.context, self)
         self.assertIsNone(getattr(globalhelp, 'context', None))
 
     def test_cannot_pickle(self):
-        from zope.app.onlinehelp import helpNamespace
         import pickle
 
+        from zope.app.onlinehelp import helpNamespace
+
         traversed = helpNamespace(self).traverse(None, None)
         self.assertRaises(TypeError,
                           pickle.dumps, traversed)
 
 
 def testdir():
     return os.path.dirname(__file__)
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/test_treeview.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/test_treeview.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Onlinehelp tree view Tests
 
 """
 import os
-
 import unittest
 
-from zope import component
+from zope.app.component.testing import PlacefulSetup
 from zope.pagetemplate.tests.util import check_xml
 from zope.publisher.browser import TestRequest
-from zope.app.component.testing import PlacefulSetup
-from zope.app.onlinehelp.tests import util
+
+from zope import component
+from zope.app.onlinehelp.browser.tree import OnlineHelpTopicTreeView
 from zope.app.onlinehelp.interfaces import IOnlineHelp
 from zope.app.onlinehelp.onlinehelp import OnlineHelp
 from zope.app.onlinehelp.onlinehelptopic import OnlineHelpTopic
-from zope.app.onlinehelp.browser.tree import OnlineHelpTopicTreeView
+from zope.app.onlinehelp.tests import util
 
 
 def testdir():
     import zope.app.onlinehelp.tests
     return os.path.dirname(zope.app.onlinehelp.tests.__file__)
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope/app/onlinehelp/tests/util.py` & `zope.app.onlinehelp-5.0/src/zope/app/onlinehelp/tests/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Onlinehelp test utilities
 
 """
 import os
+
 import zope.app.onlinehelp.tests
 
+
 here = os.path.dirname(zope.app.onlinehelp.tests.__file__)
 input_dir = os.path.join(here, 'input')
 output_dir = os.path.join(here, 'output')
 
 
 def read_output(filename):
     filename = os.path.join(output_dir, filename)
-    with open(filename, 'r') as f:
+    with open(filename) as f:
         return f.read()
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/PKG-INFO` & `zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: zope.app.onlinehelp
-Version: 4.2.0
+Version: 5.0
 Summary: Framework for Context-Sensitive Help Pages
 Home-page: http://github.com/zopefoundation/zope.app.onlinehelp
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope3 online help
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
 Provides-Extra: test
@@ -50,14 +46,22 @@
 Documentation is hosted at https://zopeapponlinehelp.readthedocs.io
 
 
 =========
  CHANGES
 =========
 
+5.0 (2023-07-06)
+================
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.2.0 (2022-04-05)
 ==================
 
 - Add support for Python 3.7, 3.8, 3.9, and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -140,9 +144,7 @@
 - Enhance the API of topics and simplyfie the view part.
 
 - Implemented getSubTopics() method on topics. This way we can sublist topics.
 
 - Remove unused onlinehelp code in rotterdam template.pt
 
 - Add type to directive, this supports registration of README.txt as 'rest' topics
-
-
```

### Comparing `zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/SOURCES.txt` & `zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/src/zope.app.onlinehelp.egg-info/requires.txt` & `zope.app.onlinehelp-5.0/src/zope.app.onlinehelp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `zope.app.onlinehelp-4.2.0/tox.ini` & `zope.app.onlinehelp-5.0/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
@@ -23,23 +20,34 @@
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 extras =
     docs
 commands_pre =
@@ -48,24 +56,22 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=98
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=98
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.app.onlinehelp
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

