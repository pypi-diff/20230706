# Comparing `tmp/zope.app.apidoc-4.3.0.tar.gz` & `tmp/zope.app.apidoc-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.app.apidoc-4.3.0.tar", last modified: Wed Dec 15 07:24:20 2021, max compression
+gzip compressed data, was "zope.app.apidoc-5.0.tar", last modified: Thu Jul  6 06:24:12 2023, max compression
```

## Comparing `zope.app.apidoc-4.3.0.tar` & `zope.app.apidoc-5.0.tar`

### file list

```diff
@@ -1,215 +1,216 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.418193 zope.app.apidoc-4.3.0/
--rw-r--r--   0 mac        (513) staff       (20)     6952 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)       32 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      497 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     9267 2021-12-15 07:24:20.418336 zope.app.apidoc-4.3.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      897 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      234 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      331 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.370762 zope.app.apidoc-4.3.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7610 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)     3278 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       55 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/browser.rst
--rw-r--r--   0 mac        (513) staff       (20)       58 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/browser_nodevmode.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)       54 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/classregistry.rst
--rw-r--r--   0 mac        (513) staff       (20)       58 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/codemodule.rst
--rw-r--r--   0 mac        (513) staff       (20)       66 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/codemodule_browser.rst
--rw-r--r--   0 mac        (513) staff       (20)       72 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/codemodule_browser_introspector.rst
--rw-r--r--   0 mac        (513) staff       (20)       62 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/codemodule_directives.rst
--rw-r--r--   0 mac        (513) staff       (20)       50 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/component.rst
--rw-r--r--   0 mac        (513) staff       (20)    11150 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)       59 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/ifacemodule.rst
--rw-r--r--   0 mac        (513) staff       (20)       60 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/ifacemodule_browser.rst
--rw-r--r--   0 mac        (513) staff       (20)     1182 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)       50 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/interface.rst
--rw-r--r--   0 mac        (513) staff       (20)       47 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/overview.rst
--rw-r--r--   0 mac        (513) staff       (20)       53 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/presentation.rst
--rw-r--r--   0 mac        (513) staff       (20)      425 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/static.rst
--rw-r--r--   0 mac        (513) staff       (20)       50 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/utilities.rst
--rw-r--r--   0 mac        (513) staff       (20)       61 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/utilitymodule.rst
--rw-r--r--   0 mac        (513) staff       (20)       62 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/utilitymodule_browser.rst
--rw-r--r--   0 mac        (513) staff       (20)       58 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/zcmlmodule.rst
--rw-r--r--   0 mac        (513) staff       (20)       59 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/docs/zcmlmodule_browser.rst
--rw-r--r--   0 mac        (513) staff       (20)      174 2021-12-15 07:24:20.418919 zope.app.apidoc-4.3.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     4899 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.358419 zope.app.apidoc-4.3.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.371028 zope.app.apidoc-4.3.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.373738 zope.app.apidoc-4.3.0/src/zope/app/
--rw-r--r--   0 mac        (513) staff       (20)       76 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.381384 zope.app.apidoc-4.3.0/src/zope/app/apidoc/
--rw-r--r--   0 mac        (513) staff       (20)     3345 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       17 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     3581 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/apidoc.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.385206 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/
--rw-r--r--   0 mac        (513) staff       (20)       17 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2178 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/book.py
--rw-r--r--   0 mac        (513) staff       (20)      316 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/book.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1736 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/browser.py
--rw-r--r--   0 mac        (513) staff       (20)      161 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/chapter.pt
--rw-r--r--   0 mac        (513) staff       (20)     1324 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/empty.txt
--rw-r--r--   0 mac        (513) staff       (20)       87 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/intro.txt
--rw-r--r--   0 mac        (513) staff       (20)       78 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/menu.pt
--rw-r--r--   0 mac        (513) staff       (20)      316 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1409 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/metaconfigure.py
--rw-r--r--   0 mac        (513) staff       (20)     1858 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/metadirectives.py
--rw-r--r--   0 mac        (513) staff       (20)       85 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/static_menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     1050 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.393890 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/
--rw-r--r--   0 mac        (513) staff       (20)     1293 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       33 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     8707 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/apidoc.css
--rw-r--r--   0 mac        (513) staff       (20)     1650 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/apidoc.py
--rw-r--r--   0 mac        (513) staff       (20)     3547 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1293 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/contents.pt
--rw-r--r--   0 mac        (513) staff       (20)     2526 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/details_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)      250 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/disabled.pt
--rw-r--r--   0 mac        (513) staff       (20)      501 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/disabled.zcml
--rw-r--r--   0 mac        (513) staff       (20)      838 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/favicon.png
--rw-r--r--   0 mac        (513) staff       (20)      151 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/harrow.png
--rw-r--r--   0 mac        (513) staff       (20)      458 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/index.pt
--rw-r--r--   0 mac        (513) staff       (20)      956 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/macros.py
--rw-r--r--   0 mac        (513) staff       (20)      279 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     3578 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/menu_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)      811 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/modules.pt
--rw-r--r--   0 mac        (513) staff       (20)      872 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/nodevmode.rst
--rw-r--r--   0 mac        (513) staff       (20)      403 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/notfound.pt
--rw-r--r--   0 mac        (513) staff       (20)     2879 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/prefIndex.pt
--rw-r--r--   0 mac        (513) staff       (20)     1514 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/preference.py
--rw-r--r--   0 mac        (513) staff       (20)     2392 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/prefmenu.pt
--rw-r--r--   0 mac        (513) staff       (20)      962 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/skin.py
--rw-r--r--   0 mac        (513) staff       (20)     1299 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_contents.pt
--rw-r--r--   0 mac        (513) staff       (20)      470 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_index.pt
--rw-r--r--   0 mac        (513) staff       (20)      286 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     3891 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_menu_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)      638 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_modules.pt
--rw-r--r--   0 mac        (513) staff       (20)     3406 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     5612 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/utilities.js
--rw-r--r--   0 mac        (513) staff       (20)     1181 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/utilities.py
--rw-r--r--   0 mac        (513) staff       (20)      160 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/varrow.png
--rw-r--r--   0 mac        (513) staff       (20)     3012 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/classregistry.py
--rw-r--r--   0 mac        (513) staff       (20)     5647 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/classregistry.rst
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.398578 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/
--rw-r--r--   0 mac        (513) staff       (20)    10425 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       17 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       34 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/_test_cr.txt
--rw-r--r--   0 mac        (513) staff       (20)       41 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/_test_crlf.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.405900 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/
--rw-r--r--   0 mac        (513) staff       (20)    22535 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       18 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     6495 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/class_.py
--rw-r--r--   0 mac        (513) staff       (20)     6317 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/class_index.pt
--rw-r--r--   0 mac        (513) staff       (20)     2152 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1519 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/directive.pt
--rw-r--r--   0 mac        (513) staff       (20)      111 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/displayClosingElement.pt
--rw-r--r--   0 mac        (513) staff       (20)       97 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/displayComment.pt
--rw-r--r--   0 mac        (513) staff       (20)     1858 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/function.py
--rw-r--r--   0 mac        (513) staff       (20)     1787 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/function_index.pt
--rw-r--r--   0 mac        (513) staff       (20)     9632 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.pt
--rw-r--r--   0 mac        (513) staff       (20)     9221 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.py
--rw-r--r--   0 mac        (513) staff       (20)     7208 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.rst
--rw-r--r--   0 mac        (513) staff       (20)     1689 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1069 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     4543 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/menu.py
--rw-r--r--   0 mac        (513) staff       (20)     5411 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/module.py
--rw-r--r--   0 mac        (513) staff       (20)     3814 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/module_index.pt
--rw-r--r--   0 mac        (513) staff       (20)     1453 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/static_menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     7539 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     1132 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/text.py
--rw-r--r--   0 mac        (513) staff       (20)      563 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/textfile_index.pt
--rw-r--r--   0 mac        (513) staff       (20)     1726 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/utilities.py
--rw-r--r--   0 mac        (513) staff       (20)     6542 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/zcml.py
--rw-r--r--   0 mac        (513) staff       (20)     1087 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/zcmlfile_index.pt
--rw-r--r--   0 mac        (513) staff       (20)     4929 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/class_.py
--rw-r--r--   0 mac        (513) staff       (20)     4557 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/codemodule.py
--rw-r--r--   0 mac        (513) staff       (20)     1778 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2610 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/directives.rst
--rw-r--r--   0 mac        (513) staff       (20)     2108 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/function.py
--rw-r--r--   0 mac        (513) staff       (20)     7186 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      513 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1500 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/metaconfigure.py
--rw-r--r--   0 mac        (513) staff       (20)     1425 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/metadirectives.py
--rw-r--r--   0 mac        (513) staff       (20)    11609 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/module.py
--rw-r--r--   0 mac        (513) staff       (20)     7189 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     1402 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/text.py
--rw-r--r--   0 mac        (513) staff       (20)     5899 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/zcml.py
--rw-r--r--   0 mac        (513) staff       (20)     9451 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/component.py
--rw-r--r--   0 mac        (513) staff       (20)    17356 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/component.rst
--rw-r--r--   0 mac        (513) staff       (20)      358 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1094 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/disabled.py
--rw-r--r--   0 mac        (513) staff       (20)      600 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/disabled.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2742 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/enabled.zcml
--rw-r--r--   0 mac        (513) staff       (20)     5513 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ftesting-base.zcml
--rw-r--r--   0 mac        (513) staff       (20)      213 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ftesting.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.410344 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/
--rw-r--r--   0 mac        (513) staff       (20)     1423 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       17 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    12258 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/browser.py
--rw-r--r--   0 mac        (513) staff       (20)     9800 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/browser.rst
--rw-r--r--   0 mac        (513) staff       (20)     3878 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/component_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)     2540 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     4708 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/iface_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)     3284 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/ifacemodule.py
--rw-r--r--   0 mac        (513) staff       (20)    11239 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/index.pt
--rw-r--r--   0 mac        (513) staff       (20)     5468 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      929 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/macros.py
--rw-r--r--   0 mac        (513) staff       (20)     1237 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     2479 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/menu.py
--rw-r--r--   0 mac        (513) staff       (20)     2644 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/presentation_macros.pt
--rw-r--r--   0 mac        (513) staff       (20)     1630 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/static_menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     2966 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     4928 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/interface.py
--rw-r--r--   0 mac        (513) staff       (20)     7765 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/interface.rst
--rw-r--r--   0 mac        (513) staff       (20)     1567 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      298 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     6848 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/presentation.py
--rw-r--r--   0 mac        (513) staff       (20)    15697 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/presentation.rst
--rw-r--r--   0 mac        (513) staff       (20)    21749 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/static.py
--rw-r--r--   0 mac        (513) staff       (20)      298 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/static.zcml
--rw-r--r--   0 mac        (513) staff       (20)      664 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/test.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1179 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/testing.py
--rw-r--r--   0 mac        (513) staff       (20)    17841 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.412473 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/
--rw-r--r--   0 mac        (513) staff       (20)       17 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1688 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/browser.py
--rw-r--r--   0 mac        (513) staff       (20)     1126 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)       78 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/menu.pt
--rw-r--r--   0 mac        (513) staff       (20)       85 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/static_menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     1867 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     3998 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/type.py
--rw-r--r--   0 mac        (513) staff       (20)    13117 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilities.py
--rw-r--r--   0 mac        (513) staff       (20)    21814 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilities.rst
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.415422 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/
--rw-r--r--   0 mac        (513) staff       (20)     3762 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       17 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     3246 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/browser.py
--rw-r--r--   0 mac        (513) staff       (20)     4812 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/browser.rst
--rw-r--r--   0 mac        (513) staff       (20)     1488 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1461 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/index.pt
--rw-r--r--   0 mac        (513) staff       (20)       78 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/menu.pt
--rw-r--r--   0 mac        (513) staff       (20)       85 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/static_menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     2872 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     5440 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/utilitymodule.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.417946 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/
--rw-r--r--   0 mac        (513) staff       (20)     2778 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/README.rst
--rw-r--r--   0 mac        (513) staff       (20)     5936 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     4873 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/browser.py
--rw-r--r--   0 mac        (513) staff       (20)     5510 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/browser.rst
--rw-r--r--   0 mac        (513) staff       (20)     1395 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     3473 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/index.pt
--rw-r--r--   0 mac        (513) staff       (20)      254 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/menu.pt
--rw-r--r--   0 mac        (513) staff       (20)      261 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/static_menu.pt
--rw-r--r--   0 mac        (513) staff       (20)     2195 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2021-12-15 07:24:20.373465 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     9267 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     7693 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       83 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)       14 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)     1372 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2021-12-15 07:24:20.000000 zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1386 2021-12-15 07:24:19.000000 zope.app.apidoc-4.3.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.455232 zope.app.apidoc-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7062 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      510 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9208 2023-07-06 06:24:12.455314 zope.app.apidoc-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      897 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      234 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      331 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.427465 zope.app.apidoc-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7610 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3278 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       55 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/browser_nodevmode.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       54 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/classregistry.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/codemodule.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       66 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/codemodule_browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       72 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/codemodule_browser_introspector.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       62 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/codemodule_directives.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/component.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11150 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       59 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/ifacemodule.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       60 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/ifacemodule_browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1182 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/interface.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       47 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/overview.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/presentation.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      425 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/static.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/utilities.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/utilitymodule.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       62 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/utilitymodule_browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/zcmlmodule.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       59 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/docs/zcmlmodule_browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      447 2023-07-06 06:24:12.455598 zope.app.apidoc-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4776 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.420706 zope.app.apidoc-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.427630 zope.app.apidoc-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.429163 zope.app.apidoc-5.0/src/zope/app/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.434046 zope.app.apidoc-5.0/src/zope/app/apidoc/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3343 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3573 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/apidoc.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.436451 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2180 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/book.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      316 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/book.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1728 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/browser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      161 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/chapter.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1324 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/empty.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       87 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/intro.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       78 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      316 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1412 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/metaconfigure.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1945 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/metadirectives.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       85 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/static_menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      959 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.441123 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1499 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       33 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8707 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/apidoc.css
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1643 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/apidoc.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3547 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1293 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/contents.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2526 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/details_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      250 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/disabled.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      501 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/disabled.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      838 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/favicon.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)      151 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/harrow.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)      458 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      957 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/macros.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      279 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3578 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/menu_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      811 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/modules.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      872 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/nodevmode.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      403 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/notfound.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2879 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/prefIndex.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1483 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/preference.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2392 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/prefmenu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      962 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/skin.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1299 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_contents.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      470 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      286 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3891 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_menu_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      638 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_modules.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3231 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5612 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/utilities.js
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1182 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/utilities.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      160 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/browser/varrow.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2983 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/classregistry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5436 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/classregistry.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.443585 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10396 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       34 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/_test_cr.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/_test_crlf.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.447314 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    22491 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6591 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/class_.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6317 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/class_index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2152 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1519 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/directive.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      111 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/displayClosingElement.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       97 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/displayComment.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1850 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/function.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1787 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/function_index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9632 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9244 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7208 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1689 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1069 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4537 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/menu.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5429 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/module.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3814 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/module_index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1453 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/static_menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7525 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1124 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/text.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      563 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/textfile_index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1750 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/utilities.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6687 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/zcml.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1087 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/zcmlfile_index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4228 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/class_.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4340 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/codemodule.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1778 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2609 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/directives.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2100 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/function.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7169 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      513 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1500 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/metaconfigure.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1421 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/metadirectives.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11038 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/module.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7082 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/text.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5846 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/zcml.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9455 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/component.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17291 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/component.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      358 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1078 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/disabled.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      600 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/disabled.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2742 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/enabled.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5513 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ftesting-base.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      213 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ftesting.zcml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.450027 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1406 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12350 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/browser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9743 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3878 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/component_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2540 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4708 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/iface_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3284 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/ifacemodule.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11239 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5467 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      929 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/macros.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1237 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2473 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/menu.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2644 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/presentation_macros.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1630 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/static_menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2965 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5134 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7749 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/interface.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1586 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      298 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6837 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/presentation.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    15680 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/presentation.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21706 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/static.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      298 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/static.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      664 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/test.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1180 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    15150 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.451275 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1728 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/browser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1126 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)       78 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       85 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/static_menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1753 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4023 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/type.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10761 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilities.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21034 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilities.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.453338 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3755 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       17 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3372 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/browser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4806 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1488 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1461 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       78 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       85 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/static_menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2871 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5469 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/utilitymodule.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.455069 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2778 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5927 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4974 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/browser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5507 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/browser.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1395 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3473 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/index.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      254 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      261 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/static_menu.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2193 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-06 06:24:12.428996 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9208 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7709 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       62 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/entry_points.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       14 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1372 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-06 06:24:12.000000 zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1576 2023-07-06 06:24:11.000000 zope.app.apidoc-5.0/tox.ini
```

### Comparing `zope.app.apidoc-4.3.0/CHANGES.rst` & `zope.app.apidoc-5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  CHANGES
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.3.0 (2021-12-15)
 ==================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
```

### Comparing `zope.app.apidoc-4.3.0/LICENSE.txt` & `zope.app.apidoc-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/PKG-INFO` & `zope.app.apidoc-5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: zope.app.apidoc
-Version: 4.3.0
+Version: 5.0
 Summary: API Documentation and Component Inspection for Zope 3
 Home-page: http://github.com/zopefoundation/zope.app.apidoc
 Author: Zope Corporation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope3 api documentation
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
@@ -52,14 +48,22 @@
 Documentation is available at  https://zopeappapidoc.readthedocs.io/
 
 
 =========
  CHANGES
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.3.0 (2021-12-15)
 ==================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -284,9 +288,7 @@
 - Fixed the code to at least gracefully ignore unzipped eggs. Eventually we
   want to handle eggs well.
 
 3.4.0a1 (2007-04-22)
 ====================
 
 - Initial release independent of the main Zope tree.
-
-
```

### Comparing `zope.app.apidoc-4.3.0/README.rst` & `zope.app.apidoc-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/docs/Makefile` & `zope.app.apidoc-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/docs/api.rst` & `zope.app.apidoc-5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/docs/conf.py` & `zope.app.apidoc-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/docs/index.rst` & `zope.app.apidoc-5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/setup.py` & `zope.app.apidoc-5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.app.apidoc package
 
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -56,15 +58,15 @@
     'zope.app.schema[test]',
 ]
 
 static_requires = tests_require
 
 setup(
     name='zope.app.apidoc',
-    version='4.3.0',
+    version='5.0',
     author='Zope Corporation and Contributors',
     author_email='zope-dev@zope.org',
     description='API Documentation and Component Inspection for Zope 3',
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
@@ -73,23 +75,20 @@
     keywords="zope3 api documentation",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Framework :: Zope :: 3',
     ],
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/README.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 '++apidoc++') and get a list of available modules:
 
   >>> from zope.app.apidoc.apidoc import APIDocumentation
   >>> doc = APIDocumentation(None, '++apidoc++')
 
   >>> modules = sorted(doc.keys())
   >>> modules
-  [u'Interface', u'ZCML']
+  ['Interface', 'ZCML']
 
   >>> doc['ZCML']
   <zope.app.apidoc.zcmlmodule.ZCMLModule 'ZCML' at ...>
 
 
 Developing a Module
 ===================
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/apidoc.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/apidoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """Zope 3 API Documentation
 
 """
 __docformat__ = 'restructuredtext'
 
 import zope.component
 from zope.interface import implementer
-from zope.publisher.browser import applySkin
 from zope.location.interfaces import ILocation
+from zope.publisher.browser import applySkin
 
 from zope.app.apidoc.interfaces import IDocumentationModule
 from zope.app.apidoc.utilities import ReadContainerBase
 
 
 @implementer(ILocation)
 class APIDocumentation(ReadContainerBase):
@@ -72,15 +72,15 @@
         """
         items = sorted(zope.component.getUtilitiesFor(IDocumentationModule))
         return [(key, value.withParentAndName(self, key))
                 for key, value
                 in items]
 
 
-class apidocNamespace(object):
+class apidocNamespace:
     """Used to traverse to an API Documentation.
 
     Instantiating this object with a request will apply the
     :class:`zope.app.apidoc.browser.skin.APIDOC` skin automatically.
     """
 
     def __init__(self, ob, request=None):
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/book.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/book.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Help books.
 """
 from zope.testing import cleanup
+
+
 __docformat__ = 'restructuredtext'
 import os.path
 
+from zope.app.onlinehelp.onlinehelp import OnlineHelp
 from zope.i18nmessageid import ZopeMessageFactory as _
 from zope.interface import implementer
 
 import zope.app.apidoc.bookmodule
 from zope.app.apidoc.interfaces import IDocumentationModule
-from zope.app.onlinehelp.onlinehelp import OnlineHelp
 
 
 class IBookModule(IDocumentationModule):
     """Interface API Documentation Module
 
     This is a marker interface, so that we can write adapters for objects
     implementing this interface.
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/browser.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Browser Views for Book
 
 """
 __docformat__ = 'restructuredtext'
 from zope.app.apidoc.bookmodule.metaconfigure import EMPTYPATH
 
 
-class Menu(object):
+class Menu:
     """Menu View Helper Class
 
     >>> class Chapter(object):
     ...     title = 'Read Me'
     ...     path = 'README.txt'
     ...
     ...     def getTopicPath(self):
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/metaconfigure.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/metaconfigure.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 #
 ##############################################################################
 """Meta-Configuration Handlers for "apidoc:bookchapter" directive.
 
 """
 __docformat__ = 'restructuredtext'
 import os.path
-import zope.app.apidoc.bookmodule
+
 from zope.app.onlinehelp.onlinehelptopic import RESTOnlineHelpTopic
+
+import zope.app.apidoc.bookmodule
 from zope.app.apidoc.bookmodule.book import book
 
+
 EMPTYPATH = os.path.join(
     os.path.dirname(zope.app.apidoc.bookmodule.__file__),
     'empty.txt')
 
 
 def bookchapter(_context, id, title, doc_path=EMPTYPATH,
                 parent="", resources=None):
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/metadirectives.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/metadirectives.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,45 +12,48 @@
 #
 ##############################################################################
 """Schema for the ``apidoc:bookchapter`` directive
 
 """
 __docformat__ = 'restructuredtext'
 
-from zope.configuration.fields import Path, MessageID, Tokens
+from zope.configuration.fields import MessageID
+from zope.configuration.fields import Path
+from zope.configuration.fields import Tokens
 from zope.interface import Interface
-from zope.schema import NativeStringLine, TextLine
+from zope.schema import NativeStringLine
+from zope.schema import TextLine
 
 
 class IBookChapterDirective(Interface):
     """Register a new Book Chapter"""
 
     id = NativeStringLine(
-        title=u"Topic Id",
-        description=u"Id of the chapter as it will appear in the URL.",
+        title="Topic Id",
+        description="Id of the chapter as it will appear in the URL.",
         required=True)
 
     title = MessageID(
-        title=u"Title",
-        description=u"Provides a title for the chapter.",
+        title="Title",
+        description="Provides a title for the chapter.",
         required=True)
 
     doc_path = Path(
-        title=u"Path to File",
-        description=u"Path to the file that contains the chapter content.",
+        title="Path to File",
+        description="Path to the file that contains the chapter content.",
         required=False)
 
     parent = NativeStringLine(
-        title=u"Parent Chapter",
-        description=u"Id of the parent chapter.",
+        title="Parent Chapter",
+        description="Id of the parent chapter.",
         default="",
         required=False)
 
     resources = Tokens(
-        title=u"A list of resources.",
-        description=u"""
+        title="A list of resources.",
+        description="""
         A list of resources which shall be user for the chapter. The
         resources must be located in the same directory as the chapter.
         """,
         value_type=TextLine(),
         required=False
     )
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/bookmodule/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/bookmodule/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for the Book Documentation Module
 
 """
-import unittest
 import doctest
+import unittest
 
-from zope.app.apidoc.tests import standard_checker
 from zope.app.apidoc.tests import standard_option_flags
 
 
 def test_suite():
     return unittest.TestSuite((
         doctest.DocTestSuite(
             'zope.app.apidoc.bookmodule.browser',
-            checker=standard_checker(),
             optionflags=standard_option_flags),
     ))
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/README.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,25 @@
 
 Not Found View
 ==============
 
 The `APIDOC` skin defines a custom not found view, since it fits the look and
 feel better and does not have all the O-wrap clutter:
 
+  >>> # work around for https://github.com/python/cpython/issues/90113
+  >>> browser.handleErrors = False
+  >>> browser.raiseHttpErrors = False
+
   >>> browser.open('http://localhost/++apidoc++/non-existent/')
   Traceback (most recent call last):
   ...
-  urllib.error.HTTPError: HTTP Error 404: Not Found
+  zope.publisher.interfaces.NotFound: ...
 
+  >>> browser.handleErrors = True
+  >>> browser.raiseHttpErrors = True
   >>> try:
   ...     browser.open('http://localhost/++apidoc++/non-existent/')
   ... except Exception:
   ...     pass
 
   >>> print(browser.contents)
   <...
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
 ======================= Generic API Doc Views ======================= Get a
 browser started: >>> from zope.testbrowser.wsgi import Browser >>> browser =
 Browser() >>> browser.addHeader('Authorization', 'Basic mgr:mgrpw') Not Found
 View ============== The `APIDOC` skin defines a custom not found view, since it
-fits the look and feel better and does not have all the O-wrap clutter: >>>
+fits the look and feel better and does not have all the O-wrap clutter: >>> #
+work around for https://github.com/python/cpython/issues/90113 >>>
+browser.handleErrors = False >>> browser.raiseHttpErrors = False >>>
 browser.open('http://localhost/++apidoc++/non-existent/') Traceback (most
-recent call last): ... urllib.error.HTTPError: HTTP Error 404: Not Found >>>
-try: ... browser.open('http://localhost/++apidoc++/non-existent/') ... except
-Exception: ... pass >>> print(browser.contents) <...
+recent call last): ... zope.publisher.interfaces.NotFound: ... >>>
+browser.handleErrors = True >>> browser.raiseHttpErrors = True >>> try: ...
+browser.open('http://localhost/++apidoc++/non-existent/') ... except Exception:
+... pass >>> print(browser.contents) <...
 ****** Page Not Found ******
 While broken links occur occassionally, they are considered bugs. Please report
 any broken link to zope-dev@zope.org.
 ... Preferences =========== The ``APIDOC`` skin also does the same for editing
 preference groups: >>> browser.open('http://localhost/++preferences++apidoc/
 InterfaceDetails/apidocIndex.html') >>> print(browser.contents) <...
 Preferences for API Docs' Interface Details Screen
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/apidoc.css` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/apidoc.css`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/apidoc.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/apidoc.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 """Main API Documentation View
 
 """
 __docformat__ = 'restructuredtext'
 
 from zope.i18n import translate
 from zope.security.proxy import removeSecurityProxy
+
 from zope.app.apidoc.utilities import renderText
 
 
-class APIDocumentationView(object):
+class APIDocumentationView:
     """View for the API Documentation"""
 
     context = None
     request = None
 
     def getModuleList(self):
         """Get a list of all available documentation modules."""
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/contents.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/contents.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/details_macros.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/details_macros.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/favicon.png` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/favicon.png`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/macros.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/macros.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 ##############################################################################
 """API Documentation macros
 
 """
 from zope.app.basicskin.standardmacros import StandardMacros
 
+
 BaseMacros = StandardMacros
 
 
 class APIDocumentationMacros(BaseMacros):
     """Page Template METAL macros for API Documentation"""
 
     #: Macro pages
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/menu_macros.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/menu_macros.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/modules.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/modules.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/nodevmode.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/nodevmode.rst`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/prefIndex.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/prefIndex.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/preference.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/preference.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 #
 ##############################################################################
 """API Doc Preference Views
 
 """
 __docformat__ = "reStructuredText"
 
+from zope.app.preference.browser import EditPreferenceGroup
+from zope.app.preference.browser import PreferenceGroupFilter
+from zope.app.tree.browser.cookie import CookieTreeView
 from zope.publisher.browser import applySkin
 from zope.traversing.api import getRoot
 
 from zope.app.apidoc.browser.skin import APIDOC
-from zope.app.tree.browser.cookie import CookieTreeView
-from zope.app.preference.browser import PreferenceGroupFilter
-from zope.app.preference.browser import EditPreferenceGroup
 
 
 class APIDocPreferencesTree(CookieTreeView):
     """Preferences Tree using the stateful cookie tree."""
 
     def apidocTree(self):
         root = getRoot(self.context)['apidoc']
@@ -34,8 +34,8 @@
 
 
 class ApidocEditPreferenceGroup(EditPreferenceGroup):
 
     def __init__(self, context, request):
         # Make sure we enter APIDOC territory.
         applySkin(request, APIDOC)
-        super(ApidocEditPreferenceGroup, self).__init__(context, request)
+        super().__init__(context, request)
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/prefmenu.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/prefmenu.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/skin.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/skin.py`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_contents.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_contents.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_menu_macros.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_menu_macros.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/static_modules.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/static_modules.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,84 +10,75 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Functional Tests for API Documentation.
 
 """
-import re
-import unittest
 import doctest
+import unittest
 
-
-from zope.app.apidoc.testing import APIDocLayer, APIDocNoDevModeLayer
-
+from zope.app.apidoc.testing import APIDocLayer
+from zope.app.apidoc.testing import APIDocNoDevModeLayer
 from zope.app.apidoc.tests import BrowserTestCase
-from zope.app.apidoc.tests import standard_checker
 from zope.app.apidoc.tests import standard_option_flags
 
 
 class APIDocTests(BrowserTestCase):
     """Just a couple of tests ensuring that the templates render."""
 
     layer = APIDocLayer
 
     def testMenu(self):
         response = self.publish('/++apidoc++/menu.html',
                                 basic='mgr:mgrpw')
         self.assertEqual(response.getStatus(), 200)
         body = response.getBody()
-        self.assert_(body.find('Click on one of the Documentation') > 0)
+        self.assertTrue(body.find('Click on one of the Documentation') > 0)
         self.checkForBrokenLinks(body, '/++apidoc++/menu.html',
                                  basic='mgr:mgrpw')
 
     def testIndexView(self):
         response = self.publish('/++apidoc++/index.html',
                                 basic='mgr:mgrpw')
         self.assertEqual(response.getStatus(), 200)
         body = response.getBody()
-        self.assert_(body.find('Zope 3 API Documentation') > 0)
+        self.assertTrue(body.find('Zope 3 API Documentation') > 0)
         self.checkForBrokenLinks(body, '/++apidoc++/index.html',
                                  basic='mgr:mgrpw')
 
     def testContentsView(self):
         response = self.publish('/++apidoc++/contents.html',
                                 basic='mgr:mgrpw')
         self.assertEqual(response.getStatus(), 200)
         body = response.getBody()
-        self.assert_(body.find('<h1>Zope 3 API Documentation</h1>') > 0)
+        self.assertTrue(body.find('<h1>Zope 3 API Documentation</h1>') > 0)
         self.checkForBrokenLinks(body, '/++apidoc++/contents.html',
                                  basic='mgr:mgrpw')
 
     def testModuleListView(self):
         response = self.publish('/++apidoc++/modulelist.html',
                                 basic='mgr:mgrpw')
         self.assertEqual(response.getStatus(), 200)
         body = response.getBody()
-        self.assert_(body.find(
+        self.assertTrue(body.find(
             '<a href="contents.html" target="main">Zope') > 0)
         self.checkForBrokenLinks(body, '/++apidoc++/modulelist.html',
                                  basic='mgr:mgrpw')
 
 
 def test_suite():
-    checker = standard_checker(
-        (re.compile(r'httperror_seek_wrapper:', re.M), 'HTTPError:'),
-    )
-
     apidoc_doctest = doctest.DocFileSuite(
         "README.rst",
-        optionflags=standard_option_flags,
-        checker=checker)
+        optionflags=standard_option_flags)
     apidoc_doctest.layer = APIDocLayer
 
     nodevmode = doctest.DocFileSuite(
         "nodevmode.rst",
-        optionflags=standard_option_flags,
-        checker=checker)
+        optionflags=standard_option_flags)
     nodevmode.layer = APIDocNoDevModeLayer
 
     return unittest.TestSuite((
         apidoc_doctest,
         nodevmode,
         unittest.defaultTestLoader.loadTestsFromName(__name__),
     ))
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/utilities.js` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/utilities.js`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/browser/utilities.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/browser/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Common Utilities for Browser View
 
 """
-from zope.app.apidoc.apidoc import APIDocumentation
-from zope.traversing.browser import absoluteURL
-from zope.traversing.api import getParent
 from zope.security.proxy import isinstance
+from zope.traversing.api import getParent
+from zope.traversing.browser import absoluteURL
+
+from zope.app.apidoc.apidoc import APIDocumentation
 
 
 def findAPIDocumentationRoot(context, request=None):
     if isinstance(context, APIDocumentation):
         return context
     return findAPIDocumentationRoot(getParent(context), request)
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/classregistry.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/classregistry.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Class Registry
 """
-from zope.testing.cleanup import addCleanUp
-from six import iteritems
-import sys
 import operator
+import sys
+
+from zope.testing.cleanup import addCleanUp
+
+
 __docformat__ = 'restructuredtext'
 
 __import_unknown_modules__ = False
 
 # List of modules that should never be imported.
 # TODO: List hard-coded for now.
 IGNORE_MODULES = ['twisted']
@@ -40,24 +42,24 @@
     # which happens (usually only) with test tear downs.
 
     def getClassesThatImplement(self, iface):
         """Return all class items that implement iface.
 
         Methods returns a sorted list of 2-tuples of the form (path, class).
         """
-        return sorted(((path, klass) for path, klass in iteritems(self)
+        return sorted(((path, klass) for path, klass in self.items()
                        if iface.implementedBy(klass)),
                       key=_pathgetter)
 
     def getSubclassesOf(self, klass):
         """Return all class items that are proper subclasses of klass.
 
         Methods returns a sorted list of 2-tuples of the form (path, class).
         """
-        return sorted(((path, klass2) for path, klass2 in iteritems(self)
+        return sorted(((path, klass2) for path, klass2 in self.items()
                        if issubclass(klass2, klass) and klass2 is not klass),
                       key=_pathgetter)
 
 
 #: The global class registry object. Cleaned up
 #: in tests by :mod:`zope.testing.cleanup`.
 classRegistry = ClassRegistry()
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/classregistry.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/classregistry.rst`

 * *Files 3% similar despite different names*

```diff
@@ -37,37 +37,32 @@
 
   >>> @implementer(IA)
   ... class A(object):
   ...    pass
   >>> reg['A'] = A
 
   >>> @implementer(IB)
-  ... class B: # Old style on Python 2
+  ... class B:
   ...    pass
   >>> reg['B'] = B
 
-  >>> @implementer(IB)
-  ... class B2(object):
-  ...    pass
-  >>> reg['B2'] = B2
-
   >>> @implementer(IC)
   ... class C(object):
   ...    pass
   >>> reg['C'] = C
   >>> class A2(A):
   ...    pass
   >>> reg['A2'] = A2
 
 Since the registry is just a dictionary, we can ask for all its keys, which
 are the names of the classes:
 
   >>> names = sorted(reg.keys())
   >>> names
-  ['A', 'A2', 'B', 'B2', 'C']
+  ['A', 'A2', 'B', 'C']
 
   >>> reg['A'] is A
   True
 
 There are two API methods specific to the class registry:
 
 :meth:`ClassRegistry.getClassesThatImplement`
@@ -75,20 +70,18 @@
 
 This method returns all classes that implement the specified interface:
 
   >>> from pprint import pprint
   >>> pprint(reg.getClassesThatImplement(IA))
   [('A', <class 'zope.app.apidoc.doctest.A'>),
    ('A2', <class 'zope.app.apidoc.doctest.A2'>),
-   ('B', <class 'zope.app.apidoc.doctest.B'>),
-   ('B2', <class 'zope.app.apidoc.doctest.B2'>)]
+   ('B', <class 'zope.app.apidoc.doctest.B'>)]
 
   >>> pprint(reg.getClassesThatImplement(IB))
-  [('B', <class 'zope.app.apidoc.doctest.B'>),
-   ('B2', <class 'zope.app.apidoc.doctest.B2'>)]
+  [('B', <class 'zope.app.apidoc.doctest.B'>)]
 
   >>> pprint(reg.getClassesThatImplement(IC))
   [('C', <class 'zope.app.apidoc.doctest.C'>)]
 
   >>> pprint(reg.getClassesThatImplement(ID))
   []
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/README.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 provides systematic and autogenerated documentation about the content of your
 Zope 3 related Python packages. The code module can be created like this:
 
   >>> cm = codemodule.codemodule.CodeModule()
 
   >>> cm.getDocString()
-  u'Zope 3 root.'
+  'Zope 3 root.'
 
 
 This object extends the
 :class:`zope.app.apidoc.codemodule.module.Module` class, since it can
 be seen as some sort of root package. However, its sementacs are
 obviously a bit different:
 
@@ -26,15 +26,15 @@
   ''
   >>> cm.getPath()
   ''
   >>> cm.isPackage()
   True
 
   >>> sorted(cm.keys())
-  [u'BTrees', u'ZConfig', u'ZODB', u'builtins', u'persistent', u'transaction', ...]
+  ['BTrees', 'ZConfig', 'ZODB', 'builtins', 'persistent', 'transaction', ...]
 
 
 Module
 ======
 
 The :class:`module.Module` class represents a Python module or package
 in the documentation tree. It can be easily setup by simply passing
@@ -176,16 +176,16 @@
 listed in the interface. Now we create the class documentation wrapper:
 
   >>> klass = codemodule.class_.Class(module, 'Blah', Blah)
 
   >>> from pprint import pprint
   >>> pprint(klass.getAttributes())
   [('bar', 'b', None),
-   ('bli', 'i', <InterfaceClass __builtin__.IBlie>),
-   ('foo', 'f', <InterfaceClass __builtin__.IBlah>)]
+   ('bli', 'i', <InterfaceClass builtins.IBlie>),
+   ('foo', 'f', <InterfaceClass builtins.IBlah>)]
 
 So, the function returns a list of tuples of the form (name, value,
 interface), where the interface is the interface in which the attribute was
 declared. The interface is ``None``, if the attribute was not declared. Also
 note that attributes starting with an underscore are ignored.
 
 
@@ -211,15 +211,15 @@
 
   >>> klass = codemodule.class_.Class(module, 'Blah', Blah)
 
 and get the method documentation:
 
   >>> pprint(klass.getMethods())
   [('bar', <function Blah.bar at ...>, None),
-   ('foo', <function Blah.foo at ...>, <InterfaceClass __builtin__.IBlah>)]
+   ('foo', <function Blah.foo at ...>, <InterfaceClass builtins.IBlah>)]
 
 
 .. cleanup
 
   >>> from zope.app.apidoc.classregistry import classRegistry
   >>> del classRegistry[klass.getPath()]
 
@@ -305,20 +305,20 @@
 The interesting attribute of the object is the ``rootElement``, since it
 contains the root XML element and thus the entire XML tree. The ``rootElement``
 attribute is a lazy property, so that it is not loaded until accessed for the
 first time:
 
   >>> root = zcml.rootElement
   >>> root
-  <Directive (u'http://namespaces.zope.org/zope', u'configure')>
+  <Directive ('http://namespaces.zope.org/zope', 'configure')>
 
 A directive component has some interesting atrributes, such as the name,
 
   >>> root.name
-  (u'http://namespaces.zope.org/zope', u'configure')
+  ('http://namespaces.zope.org/zope', 'configure')
 
 the schema that describes the directive,
 
   >>> root.schema
   <InterfaceClass zope.configuration.zopeconfigure.IZopeConfigure>
 
 the attributes of the XML element,
@@ -339,16 +339,16 @@
 
   >>> print(info)
   File ".../zope/app/apidoc/codemodule/configure.zcml", ...
 
 the sub-directives,
 
   >>> root.subs[:2]
-  [<Directive (u'http://namespaces.zope.org/zope', u'class')>,
-   <Directive (u'http://namespaces.zope.org/zope', u'class')>]
+  [<Directive ('http://namespaces.zope.org/zope', 'class')>,
+   <Directive ('http://namespaces.zope.org/zope', 'class')>]
 
 and finally a list of all prefixes.
 
   >>> pprint(root.prefixes)
-  {u'http://namespaces.zope.org/apidoc': u'apidoc',
-   u'http://namespaces.zope.org/browser': u'browser',
-   u'http://namespaces.zope.org/zope': None}
+  {'http://namespaces.zope.org/apidoc': 'apidoc',
+   'http://namespaces.zope.org/browser': 'browser',
+   'http://namespaces.zope.org/zope': None}
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/README.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,17 @@
 way up to the root, but we just want to go to the root module.
 
   >>> from zope.app.apidoc.codemodule.browser import utilities
   >>> bc = utilities.CodeBreadCrumbs()
   >>> bc.context = details.context
   >>> bc.request = details.request
   >>> pprint(bc(), width=1)
-  [{'name': u'[top]',
+  [{'name': '[top]',
     'url': 'http://127.0.0.1/++apidoc++/Code'},
-   {'name': u'zope',
+   {'name': 'zope',
     'url': 'http://127.0.0.1/++apidoc++/Code/zope'},
    {'name': 'app',
     'url': 'http://127.0.0.1/++apidoc++/Code/zope/app'},
    {'name': 'apidoc',
     'url': 'http://127.0.0.1/++apidoc++/Code/zope/app/apidoc'},
    {'name': 'codemodule',
     'url': 'http://127.0.0.1/++apidoc++/Code/zope/app/apidoc/codemodule'},
@@ -188,50 +188,50 @@
 
 :meth:`class_.ClassDetails.getConstructor`
 ------------------------------------------
 
 Get info about the class' __init__ method, which is its constructor.
 
   >>> pprint(details.getConstructor())
-  {'doc': u'<p>Initialize object.</p>\n',
+  {'doc': '<p>Initialize object.</p>\n',
    'signature': '()'}
 
 :meth:`class_.ClassDetails.getAttributes`
 -----------------------------------------
 
 Get all attributes of this class.
 
   >>> pprint(details.getAttributes()[1])
   {'interface': {'path': 'zope.app.apidoc.interfaces.IDocumentationModule',
                  'url': 'zope.app.apidoc.interfaces.IDocumentationModule'},
    'name': 'title',
    'read_perm': 'zope.Public',
    'type': 'Message',
    'type_link': 'zope/i18nmessageid/message/Message',
-   'value': "u'Code Browser'",
-   'write_perm': u'n/a'}
+   'value': "'Code Browser'",
+   'write_perm': 'n/a'}
 
 :meth:`class_.ClassDetails.getMethods`
 --------------------------------------
 Get all methods of this class.
 
   >>> pprint(details.getMethods()[-3:-1])
-  [{'doc': u'<p>Setup module and class tree.</p>\n',
+  [{'doc': '<p>Setup module and class tree.</p>\n',
     'interface': None,
     'name': 'setup',
-    'read_perm': u'n/a',
+    'read_perm': 'n/a',
     'signature': '()',
-    'write_perm': u'n/a'},
-   {'doc': u'',
+    'write_perm': 'n/a'},
+   {'doc': '',
     'interface': {'path': 'zope.interface.common.mapping.IEnumerableMapping',
                   'url': 'zope.interface.common.mapping.IEnumerableMapping'},
     'name': 'values',
     'read_perm': 'zope.Public',
     'signature': '()',
-    'write_perm': u'n/a'}]
+    'write_perm': 'n/a'}]
 
 :meth:`class_.ClassDetails.getDoc`
 ----------------------------------
 
 Get the doc string of the class STX formatted.
 
   >>> print(details.getDoc()[:-1])
@@ -253,26 +253,26 @@
 
 :meth:`function.FunctionDetails.getDocString`
 ---------------------------------------------
 
 Get the doc string of the function in a rendered format.
 
   >>> details.getDocString()
-  u'<p>This is the foo function.</p>\n'
+  '<p>This is the foo function.</p>\n'
 
 :meth:`function.FunctionDetails.getAttributes`
 ----------------------------------------------
 
 Get all attributes of this function.
 
   >>> attr = details.getAttributes()[0]
   >>> pprint(attr)
   {'name': 'deprecated',
    'type': 'bool',
-   'type_link': '__builtin__/bool',
+   'type_link': 'builtins/bool',
    'value': 'True'}
 
 :meth:`function.FunctionDetails.getBaseURL`
 -------------------------------------------
 
 Return the URL for the API Documentation Tool.
 
@@ -320,15 +320,15 @@
 
 :meth:`zcml.DirectiveDetails.fullTagName`
 -----------------------------------------
 
 Return the name of the directive, including prefix, if applicable.
 
   >>> details.fullTagName()
-  u'configure'
+  'configure'
 
 :meth:`zcml.DirectiveDetails.line`
 ----------------------------------
 
 Return the line (as a string) at which this directive starts.
 
   >>> details.line()
@@ -352,15 +352,15 @@
 :meth:`zcml.DirectiveDetails.url`
 ---------------------------------
 
 Returns the URL of the directive docuemntation in the ZCML documentation
 module.
 
   >>> details.url()
-  u'http://127.0.0.1/++apidoc++/ZCML/ALL/configure/index.html'
+  'http://127.0.0.1/++apidoc++/ZCML/ALL/configure/index.html'
 
 :meth:`zcml.DirectiveDetails.objectURL`
 ---------------------------------------
 
 This method converts the string value of the field to an object and then
 crafts a documentation URL for it:
 
@@ -379,30 +379,30 @@
 Returns a list of info dictionaries representing all the attributes in the
 directive. If the directive is the root directive, all namespace declarations
 will be listed too.
 
   >>> pprint(details.attributes())
   [{'name': 'xmlns',
     'url': None,
-    'value': u'http://namespaces.zope.org/zope',
+    'value': 'http://namespaces.zope.org/zope',
     'values': []},
-   {'name': u'xmlns:apidoc',
+   {'name': 'xmlns:apidoc',
     'url': None,
-    'value': u'http://namespaces.zope.org/apidoc',
+    'value': 'http://namespaces.zope.org/apidoc',
     'values': []},
-   {'name': u'xmlns:browser',
+   {'name': 'xmlns:browser',
     'url': None,
-    'value': u'http://namespaces.zope.org/browser',
+    'value': 'http://namespaces.zope.org/browser',
     'values': []}]
 
   >>> details.context = details.context.subs[0]
   >>> pprint(details.attributes())
-  [{'name': u'class',
+  [{'name': 'class',
     'url': 'http://127.0.0.1/++apidoc++/Code/zope/app/apidoc/codemodule/module/Module/index.html',
-    'value': u'.module.Module',
+    'value': '.module.Module',
     'values': []}]
 
 :meth:`zcml.DirectiveDetails.hasSubDirectives`
 ----------------------------------------------
 
 Returns `True`, if the directive has subdirectives; otherwise `False` is
 returned.
@@ -412,15 +412,15 @@
 
 :meth:`zcml.DirectiveDetails.getElements`
 -----------------------------------------
 
 Returns a list of all sub-directives:
 
   >>> details.getElements()
-  [<Directive (u'http://namespaces.zope.org/zope', u'allow')>]
+  [<Directive ('http://namespaces.zope.org/zope', 'allow')>]
 
 Other Examples
 --------------
 
 Let's look at sub-directive that has a namespace:
 
   >>> details = browser.zcml.DirectiveDetails()
@@ -510,15 +510,15 @@
 This little helper function returns the path to the type class:
 
   >>> from zope.app.apidoc.apidoc import APIDocumentation
   >>> introspector.getTypeLink(APIDocumentation)
   'zope/app/apidoc/apidoc/APIDocumentation'
 
   >>> introspector.getTypeLink(dict)
-  '__builtin__/dict'
+  'builtins/dict'
 
   >>> introspector.getTypeLink(type(None)) is None
   True
 
 ``++annotations++`` Namespace
 -----------------------------
 
@@ -627,44 +627,44 @@
 request to the class documentation view. Thus the next method is
 ``getAttributes()``, which collects all sorts of useful information about the
 object's attributes:
 
   >>> pprint(list(inspect.getAttributes()))
   [{'interface': None,
     'name': 'data',
-    'read_perm': u'n/a',
+    'read_perm': 'n/a',
     'type': 'OOBTree',
     'type_link': 'BTrees/OOBTree/OOBTree',
     'value': '<BTrees.OOBTree.OOBTree object at ...>',
     'value_linkable': True,
-    'write_perm': u'n/a'}]
+    'write_perm': 'n/a'}]
 
 Of course, the methods are listed as well:
 
   >>> pprint(list(inspect.getMethods()))
   [...
-   {'doc': u'',
+   {'doc': '',
     'interface': 'zope.component.interfaces.IPossibleSite',
     'name': 'getSiteManager',
     'read_perm': 'zope.Public',
     'signature': '()',
-    'write_perm': u'n/a'},
+    'write_perm': 'n/a'},
    ...
-   {'doc': u'',
+   {'doc': '',
     'interface': 'zope.container.interfaces.IBTreeContainer',
     'name': 'keys',
     'read_perm': 'zope.View',
     'signature': '(key=None)',
-    'write_perm': u'n/a'},
-   {'doc': u'',
+    'write_perm': 'n/a'},
+   {'doc': '',
     'interface': 'zope.component.interfaces.IPossibleSite',
     'name': 'setSiteManager',
     'read_perm': 'zope.ManageServices',
     'signature': '(sm)',
-    'write_perm': u'n/a'},
+    'write_perm': 'n/a'},
    ...]
 
 The final methods deal with inspecting the objects data further. For exmaple,
 if we inspect a sequence,
 
   >>> from persistent.list import PersistentList
   >>> list = PersistentList(['one', 'two'])
@@ -681,33 +681,33 @@
 
 and then get the sequence items:
 
   >>> pprint(inspect2.getSequenceItems())
   [{'index': 0,
     'value': "'one'",
     'value_type': 'str',
-    'value_type_link': '__builtin__/str'},
+    'value_type_link': 'builtins/str'},
    {'index': 1,
     'value': "'two'",
     'value_type': 'str',
-    'value_type_link': '__builtin__/str'}]
+    'value_type_link': 'builtins/str'}]
 
 Similar functionality exists for a mapping. But we first have to add an item:
 
   >>> rootFolder['list'] = list
 
 Now let's have a look:
 
   >>> inspect.isMapping()
   True
 
   >>> pprint(inspect.getMappingItems())
   [...
-   {'key': u'list',
-    'key_string': "u'list'",
+   {'key': 'list',
+    'key_string': "'list'",
     'value': "['one', 'two']",
     'value_type': 'ContainedProxy',
     'value_type_link': 'zope/container/contained/ContainedProxy'},
   ...]
 
 The final two methods doeal with the introspection of the annotations. If an
 object is annotatable,
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/class_.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/class_.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 """
 __docformat__ = 'restructuredtext'
 
 import inspect
 
 from zope.proxy import removeAllProxies
 from zope.security.proxy import removeSecurityProxy
-from zope.traversing.api import getParent, traverse
+from zope.traversing.api import getParent
+from zope.traversing.api import traverse
 from zope.traversing.browser import absoluteURL
 from zope.traversing.interfaces import TraversalError
 
-from zope.app.apidoc.utilities import getPythonPath, getPermissionIds
-from zope.app.apidoc.utilities import renderText, getFunctionSignature
-from zope.app.apidoc.utilities import isReferencable
-
 from zope.app.apidoc.browser.utilities import findAPIDocumentationRoot
+from zope.app.apidoc.utilities import getFunctionSignature
+from zope.app.apidoc.utilities import getPermissionIds
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import isReferencable
+from zope.app.apidoc.utilities import renderText
 
 
 def getTypeLink(type, _NoneType=type(None)):
     if type is _NoneType:
         return None
     path = getPythonPath(type)
     return path.replace('.', '/') if isReferencable(path) else None
@@ -42,15 +44,15 @@
     if iface is None:
         return None
     path = getPythonPath(iface)
     return {'path': path,
             'url': isReferencable(path) and path or None}
 
 
-class ClassDetails(object):
+class ClassDetails:
     """Represents the details of the class."""
 
     context = None
     request = None
 
     def getBases(self):
         """Get all bases of this class."""
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/class_index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/class_index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/directive.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/directive.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/function.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 """
 __docformat__ = 'restructuredtext'
 
 from zope.traversing.api import getParent
 from zope.traversing.browser import absoluteURL
 
-from zope.app.apidoc.utilities import renderText
 from zope.app.apidoc.browser.utilities import findAPIDocumentationRoot
 from zope.app.apidoc.codemodule.browser.class_ import getTypeLink
+from zope.app.apidoc.utilities import renderText
 
 
-class FunctionDetails(object):
+class FunctionDetails:
     """Represents the details of the function."""
 
     context = None
     request = None
 
     def getDocString(self):
         """Get the doc string of the function in a rendered format."""
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/function_index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/function_index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,39 @@
 ##############################################################################
 """Introspector view for content components
 
 
 """
 __docformat__ = 'restructuredtext'
 import inspect
-import six
 
 import zope.interface
 import zope.security.proxy
-from zope import annotation
-from zope.interface import directlyProvidedBy, directlyProvides
-from zope.traversing.interfaces import IPhysicallyLocatable, IContainmentRoot
+from zope.interface import directlyProvidedBy
+from zope.interface import directlyProvides
 from zope.location import location
 from zope.publisher.browser import BrowserView
-from zope.traversing.api import getParent, traverse
+from zope.traversing.api import getParent
+from zope.traversing.api import traverse
+from zope.traversing.interfaces import IContainmentRoot
+from zope.traversing.interfaces import IPhysicallyLocatable
 
+from zope import annotation
 from zope.app import apidoc
 
 
 def getTypeLink(type_):
     if isinstance(None, type_):
         return None
     path = apidoc.utilities.getPythonPath(type_)
     importable = apidoc.utilities.isReferencable(path)
     return path.replace('.', '/') if importable else None
 
 
-class annotationsNamespace(object):
+class annotationsNamespace:
     """Used to traverse to the annotations of an object."""
 
     def __init__(self, ob, request=None):
         self.context = ob
 
     def traverse(self, name, ignore):
         # This is pretty unsafe and one of the reasons why the introspector is
@@ -53,28 +55,28 @@
         obj = annotations[name] if name else annotations
         if not IPhysicallyLocatable(obj, False):
             obj = location.LocationProxy(
                 obj, self.context, '++annotations++' + name)
         return obj
 
 
-class sequenceItemsNamespace(object):
+class sequenceItemsNamespace:
     """Used to traverse to the values of a sequence."""
 
     def __init__(self, ob, request=None):
         self.context = ob
 
     def traverse(self, name, ignore):
         obj = self.context[int(name)]
         if not IPhysicallyLocatable(obj, False):
             obj = location.LocationProxy(obj, self.context, '++items++' + name)
         return obj
 
 
-class mappingItemsNamespace(object):
+class mappingItemsNamespace:
     """Used to traverse to the values of a mapping.
 
     Important: This might seem like overkill, but we do not know that (1)
     every mapping has a traverser and (2) whether the location is available. A
     location might not be available, if we have a mapping in the annotations,
     for example.
     """
@@ -87,23 +89,23 @@
         if not IPhysicallyLocatable(obj, False):
             obj = location.LocationProxy(obj, self.context, '++items++' + name)
         return obj
 
 
 # Small hack to simulate a traversal root.
 @zope.interface.implementer(IContainmentRoot)
-class TraversalRoot(object):
+class TraversalRoot:
     pass
 
 
 class Introspector(BrowserView):
     """Introspector browser view"""
 
     def __init__(self, context, request):
-        super(Introspector, self).__init__(context, request)
+        super().__init__(context, request)
         path = apidoc.utilities.getPythonPath(
             context.__class__).replace('.', '/')
 
         # the ++apidoc++ namespace overrides the skin, so make sure we can get
         # it back.
         direct = list(directlyProvidedBy(request))
 
@@ -196,15 +198,15 @@
         return zope.interface.common.sequence.IExtendedReadSequence.providedBy(
             self.context)
 
     def getSequenceItems(self):
         ann = []
         # Make the object naked, so that we can inspect the value types.
         naked = zope.security.proxy.removeSecurityProxy(self.context)
-        for index in six.moves.xrange(0, len(self.context)):
+        for index in range(0, len(self.context)):
             value = naked[index]
             ann.append({
                 'index': index,
                 'value': repr(value),
                 'value_type': type(value).__name__,
                 'value_type_link': getTypeLink(type(value))
             })
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.rst`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/introspector.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/introspector.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/menu.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/menu.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/menu.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 """Code Module Menu
 
 """
 __docformat__ = 'restructuredtext'
 import operator
 
 from zope.security.proxy import removeSecurityProxy
-
 from zope.traversing.api import traverse
 from zope.traversing.browser import absoluteURL
 
 from zope.app.apidoc.browser.utilities import findAPIDocumentationRoot
 from zope.app.apidoc.classregistry import classRegistry
 
+
 _pathgetter = operator.itemgetter("path")
 
 
-class Menu(object):
+class Menu:
     """Menu for the Class Documentation Module.
 
     The menu allows for looking for classes by partial names. See
     `findClasses()` for the simple search implementation.
     """
 
     context = None
@@ -54,17 +54,17 @@
           Testing the method with various inputs.
 
           >>> menu.request = TestRequest(form={'path': 'menu'})
           >>> info = menu.findClasses()
 
           >>> from pprint import pprint
           >>> pprint(info)
-          [{'path': 'zope.app.apidoc.codemodule.browser.menu.Men',
+          [{'path': 'zope.app.apidoc.codemodule.browser.menu.Menu',
             'url': 'http://.../zope/app/apidoc/codemodule/browser/menu/Menu/'},
-           {'path': 'zope.app.apidoc.ifacemodule.menu.Men',
+           {'path': 'zope.app.apidoc.ifacemodule.menu.Menu',
             'url': 'http://...Code/zope/app/apidoc/ifacemodule/menu/Menu/'}...]
 
           >>> menu.request = TestRequest(form={'path': 'illegal name'})
           >>> info = menu.findClasses()
           >>> pprint(info)
           []
         """
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/module.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 __docformat__ = 'restructuredtext'
 
 from zope.interface.interfaces import IInterface
 from zope.proxy import removeAllProxies
 from zope.publisher.browser import BrowserView
 from zope.traversing.browser import absoluteURL
 
-from zope.app.apidoc.utilities import getPythonPath, renderText
-from zope.app.apidoc.codemodule.interfaces import IModuleDocumentation
+from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
 from zope.app.apidoc.codemodule.interfaces import IClassDocumentation
 from zope.app.apidoc.codemodule.interfaces import IFunctionDocumentation
-from zope.app.apidoc.codemodule.interfaces import IZCMLFile
+from zope.app.apidoc.codemodule.interfaces import IModuleDocumentation
 from zope.app.apidoc.codemodule.interfaces import ITextFile
-from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
+from zope.app.apidoc.codemodule.interfaces import IZCMLFile
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import renderText
 
 
 def formatDocString(text, module=None, summary=False):
     """Format a doc string for display.
 
     module is either a Python module (from sys.modules) or the dotted name
     of a module.
@@ -54,15 +55,15 @@
     return renderText('\n'.join(lines), module)
 
 
 class ModuleDetails(BrowserView):
     """Represents the details of a module or package."""
 
     def __init__(self, context, request):
-        super(ModuleDetails, self).__init__(context, request)
+        super().__init__(context, request)
         items = sorted(self.context.items())
         self.text_files = []
         self.zcml_files = []
         self.modules = []
         self.interfaces = []
         self.classes = []
         self.functions = []
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/module_index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/module_index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/static_menu.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/static_menu.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,24 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for the Code Documentation Module
 
 """
 import unittest
-from BTrees import OOBTree
 
+from BTrees import OOBTree
 from zope.traversing.api import traverse
 
+import zope.app.apidoc.codemodule
 from zope.app.apidoc.testing import APIDocLayer
 from zope.app.apidoc.tests import BrowserTestCase
 from zope.app.apidoc.tests import LayerDocFileSuite
 from zope.app.apidoc.tests import LayerDocTestSuite
 
-import zope.app.apidoc.codemodule
-
 
 def foo(cls, bar=1, *args):  # used in README.rst
     """This is the foo function."""
 
 
 foo.deprecated = True
 
@@ -114,16 +113,18 @@
 class TestClass(unittest.TestCase):
 
     layer = APIDocLayer
 
     @unittest.skipIf(OOBTree.OOBTree is OOBTree.OOBTreePy,
                      "Only in the C implementation")
     def test_listClasses_C(self):
-        from zope.app.apidoc.codemodule.browser.class_ import ClassDetails
         from zope.publisher.browser import TestRequest
+
+        from zope.app.apidoc.codemodule.browser.class_ import ClassDetails
+
         # BTree items doesn't set a module.
 
         items_class = type(OOBTree.OOBTree({1: 2}).items())
 
         details = ClassDetails()
         details.request = TestRequest()
         details.context = traverse(self.layer.getRootFolder(), '/++apidoc++')
@@ -132,35 +133,36 @@
         self.assertIsNone(info[0]['url'], None)
 
     def test_not_fail_with_doc_property(self):
         from zope.app.apidoc.codemodule.browser.class_ import ClassDetails
         from zope.app.apidoc.codemodule.class_ import Class
 
         # Such as in zope.hookable._py_hookable
-        class WithProperty(object):
+        class WithProperty:
             @property
             def __doc__(self):
                 return "Some Docs"
 
-        class Parent(object):
+        class Parent:
             def getPath(self):
                 return '/'
 
         details = ClassDetails()
         details.context = Class(Parent(), WithProperty.__name__, WithProperty)
 
         self.assertIn('Failed to render non-text', details.getDoc())
 
 
 class TestIntrospectorNS(unittest.TestCase):
 
     def _check_namespace(self, kind, context, name):
-        from zope.app.apidoc.codemodule.browser import introspector
         from zope.location import LocationProxy
 
+        from zope.app.apidoc.codemodule.browser import introspector
+
         namespace = getattr(introspector, kind + 'Namespace')
         traverser = namespace(context)
         obj = traverser.traverse(name, ())
         self.assertIsInstance(obj, LocationProxy)
 
         self.assertIs(obj.__parent__, context)
         self.assertTrue(obj.__name__.endswith(name))
@@ -181,18 +183,19 @@
 
 class TestIntrospector(unittest.TestCase):
     layer = APIDocLayer
 
     classAttr = 1
 
     def testIntrospector(self):
-        from zope.app.apidoc.codemodule.browser.introspector import (
-            Introspector)
         from zope.publisher.browser import TestRequest
 
+        from zope.app.apidoc.codemodule.browser.introspector import \
+            Introspector
+
         ispect = Introspector(self, TestRequest())
         atts = list(ispect.getAttributes())
         names = [x['name'] for x in atts]
         self.assertIn('classAttr', names)
         self.assertNotIn('testAttributes', names)
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/text.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Function Views
 
 """
 __docformat__ = 'restructuredtext'
 from zope.app.apidoc.utilities import renderText
 
 
-class TextFileDetails(object):
+class TextFileDetails:
     """Represents the details of the text file."""
 
     context = None
     request = None
 
     def renderedContent(self):
         """Render the file content to HTML."""
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/textfile_index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/textfile_index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/utilities.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 ##############################################################################
 """Browser utilities for API documentation.
 
 """
 __docformat__ = 'restructuredtext'
 
 from zope.i18nmessageid import ZopeMessageFactory as _
-from zope.traversing.api import getName, getParent
+from zope.traversing.api import getName
+from zope.traversing.api import getParent
 from zope.traversing.browser import absoluteURL
+
 from zope.app.apidoc.interfaces import IDocumentationModule
 
 
-class CodeBreadCrumbs(object):
+class CodeBreadCrumbs:
     """View that provides breadcrumbs for code objects"""
 
     def __call__(self):
         """Create breadcrumbs for a module or an object in a module or package.
 
         We cannot reuse the system's bread crumbs, since they go all the
         way up to the root, but we just want to go to the root module.
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/zcml.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/zcml.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 #
 ##############################################################################
 """ZCML Element Views
 
 """
 __docformat__ = "reStructuredText"
 
-from zope.configuration.fields import GlobalObject, GlobalInterface, Tokens
+from zope.configuration.fields import GlobalInterface
+from zope.configuration.fields import GlobalObject
+from zope.configuration.fields import Tokens
 from zope.interface.interfaces import IInterface
 from zope.schema import getFieldNamesInOrder
-from zope.security.proxy import isinstance, removeSecurityProxy
+from zope.security.proxy import isinstance
+from zope.security.proxy import removeSecurityProxy
 from zope.traversing.api import getParent
 from zope.traversing.browser import absoluteURL
 
-from zope.app.apidoc.interfaces import IDocumentationModule
-from zope.app.apidoc.utilities import getPythonPath, isReferencable
 from zope.app.apidoc.browser.utilities import findAPIDocumentationRoot
 from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
-
-from zope.app.apidoc.zcmlmodule import quoteNS
 from zope.app.apidoc.codemodule.interfaces import IRootDirective
+from zope.app.apidoc.interfaces import IDocumentationModule
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import isReferencable
+from zope.app.apidoc.zcmlmodule import quoteNS
 
 
 def findDocModule(obj):
     if IDocumentationModule.providedBy(obj):
         return obj
     return findDocModule(getParent(obj))
 
@@ -42,25 +45,25 @@
     if x['name'] in nameOrder:
         valueX = nameOrder.index(x['name'])
     else:
         valueX = 999999
     return valueX
 
 
-class DirectiveDetails(object):
+class DirectiveDetails:
     """Details about ZCML directives."""
 
     context = None
     request = None
 
     def fullTagName(self):
         context = removeSecurityProxy(self.context)
         ns, name = context.name
         if context.prefixes.get(ns):
-            return '%s:%s' % (context.prefixes[ns], name)
+            return '{}:{}'.format(context.prefixes[ns], name)
         return name
 
     def line(self):
         return str(removeSecurityProxy(self.context).info.line)
 
     def highlight(self):
         if self.request.get('line') == self.line():
@@ -79,15 +82,15 @@
         ns, name = directive.name
         # Sometimes ns is `None`, especially in the slug files, where no
         # namespaces are used.
         ns = quoteNS(ns or 'ALL')
         zcml = findAPIDocumentationRoot(self.context, self.request)['ZCML']
         if name not in zcml[ns]:
             ns = 'ALL'
-        link = '%s/ZCML/%s/%s/index.html' % (
+        link = '{}/ZCML/{}/{}/index.html'.format(
             findAPIDocumentationRootURL(self.context, self.request), ns, name)
         if subDirective:
             link += '#' + subDirective.name[1]
         return link
 
     def objectURL(self, value, field, rootURL):
         naked = removeSecurityProxy(self.context)
@@ -104,15 +107,15 @@
         # The object might be an instance; in this case get a link to the class
         if not hasattr(obj, '__name__'):  # pragma: no cover
             obj = getattr(obj, '__class__')
         path = getPythonPath(obj)
         if isInterface:
             apidoc_url = findAPIDocumentationRootURL(
                 self.context, self.request)
-            return '%s/Interface/%s/index.html' % (apidoc_url, path)
+            return '{}/Interface/{}/index.html'.format(apidoc_url, path)
         if isReferencable(path):
             return rootURL + '/%s/index.html' % (path.replace('.', '/'))
 
     def attributes(self):
         context = removeSecurityProxy(self.context)
         attrs = [{'name': (ns and context.prefixes[ns] + ':' or '') + name,
                   'value': value, 'url': None, 'values': []}
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/browser/zcmlfile_index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/browser/zcmlfile_index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/class_.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/class_.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 ##############################################################################
 """Class representation for code browser
 """
 
 __docformat__ = 'restructuredtext'
 
 from inspect import isfunction
-from inspect import ismethod
 from inspect import ismethoddescriptor
 
-from zope.interface import implementer, implementedBy
-from zope.security.checker import getCheckerForInstancesOf
+from zope.interface import implementedBy
+from zope.interface import implementer
 from zope.location.interfaces import ILocation
+from zope.security.checker import getCheckerForInstancesOf
 
 from zope.app.apidoc.classregistry import classRegistry
+from zope.app.apidoc.codemodule.interfaces import IClassDocumentation
 from zope.app.apidoc.utilities import getInterfaceForAttribute
 from zope.app.apidoc.utilities import getPublicAttributes
-from zope.app.apidoc.codemodule.interfaces import IClassDocumentation
 
 
 @implementer(ILocation, IClassDocumentation)
-class Class(object):
+class Class:
     """This class represents a class declared in the module."""
 
     def __init__(self, module, name, klass):
         self.__parent__ = module
         self.__name__ = name
         self.__klass = klass
 
@@ -68,39 +68,25 @@
 
     def _iterAllAttributes(self):
         for name in getPublicAttributes(self.__klass):
             iface = getInterfaceForAttribute(
                 name, self.__all_ifaces, asPath=False)
             yield name, getattr(self.__klass, name), iface
 
-    if str is bytes:
-        # Python 2
-        _ismethod = staticmethod(ismethod)
-    else:
-        # On Python 3, there is no unbound method. But we can't treat
-        # things that are simply callable as methods. Things like the
-        # security proxy are callable, but when `permission =
-        # CheckerPublic` (where zope.security.checker.CheckerPublic is
-        # proxied) is a class attribute, that's *not* a method.
-        # Checking if its actually a function gets us much more accurate
-        # results. (We could also check its qualname to see if it "belongs"
-        # to this class, but this seems to do the trick)
-        _ismethod = staticmethod(isfunction)
-
     def getAttributes(self):
         """See :class:`~zope.app.apidoc.codemodule.interfaces.IClassDocumentation`."""  # noqa: E501 line too long
         return [(name, obj, iface)
                 for name, obj, iface in self._iterAllAttributes()
-                if not self._ismethod(obj) and not ismethoddescriptor(obj)]
+                if not isfunction(obj) and not ismethoddescriptor(obj)]
 
     def getMethods(self):
         """See :class:`~zope.app.apidoc.codemodule.interfaces.IClassDocumentation`."""  # noqa: E501 line too long
         return [(name, obj, iface)
                 for name, obj, iface in self._iterAllAttributes()
-                if self._ismethod(obj)]
+                if isfunction(obj)]
 
     def getMethodDescriptors(self):
         return [(name, obj, iface)
                 for name, obj, iface in self._iterAllAttributes()
                 if ismethoddescriptor(obj)]
 
     def getSecurityChecker(self):
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/codemodule.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/codemodule.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 """Code Documentation Module
 
 This module is able to take a dotted name of any class and display
 documentation for it.
 
 """
 from zope.testing.cleanup import addCleanUp
+
+
 __docformat__ = 'restructuredtext'
 
 import zope.component
 from zope.i18nmessageid import ZopeMessageFactory as _
 from zope.interface import implementer
 
-from zope.app.apidoc.interfaces import IDocumentationModule
 from zope.app.apidoc.classregistry import safe_import
 from zope.app.apidoc.codemodule.interfaces import IAPIDocRootModule
 from zope.app.apidoc.codemodule.module import Module
+from zope.app.apidoc.interfaces import IDocumentationModule
 
 
 @implementer(IDocumentationModule)
 class CodeModule(Module):
     """Represent the code browser documentation root"""
 
     #: The title.
@@ -58,15 +60,15 @@
     implemented interfaces, attributes and methods, but it also lists the
     interface that requires a method or attribute to be implemented and the
     permissions required to access it.
     """)
 
     def __init__(self):
         """Initialize object."""
-        super(CodeModule, self).__init__(None, '', None, False)
+        super().__init__(None, '', None, False)
         self.__isSetup = False
 
     def setup(self):
         """Setup module and class tree."""
         if self.__isSetup:
             return
         self.__isSetup = True
@@ -74,21 +76,18 @@
         for name, mod in zope.component.getUtilitiesFor(IAPIDocRootModule):
             module = safe_import(mod)
             if module is not None:
                 self._children[name] = Module(self, name, module)
 
         # And the builtins are always available, since that's the
         # most common root module linked to from docs.
-        builtin_module = safe_import('__builtin__') or safe_import('builtins')
+        builtin_module = safe_import('builtins')
         assert builtin_module is not None
         builtin_module = Module(self, builtin_module.__name__, builtin_module)
-        # Register with both names for consistency in the tests between Py2 and
-        # Py3
-        self._children['builtins'] = self._children['__builtin__'] = (
-            builtin_module)
+        self._children['builtins'] = builtin_module
 
     def withParentAndName(self, parent, name):
         located = type(self)()
         located.__parent__ = parent
         located.__name__ = name
         self.setup()
         located._children = {name: module.withParentAndName(located, name)
@@ -106,19 +105,19 @@
         return ''
 
     def isPackage(self):
         return True
 
     def get(self, key, default=None):
         self.setup()
-        return super(CodeModule, self).get(key, default)
+        return super().get(key, default)
 
     def items(self):
         self.setup()
-        return super(CodeModule, self).items()
+        return super().items()
 
 
 def _cleanUp():
     from zope.component import getGlobalSiteManager
     code = getGlobalSiteManager().queryUtility(
         IDocumentationModule, name='Code')
     if code is not None:
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/directives.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/directives.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   ...         xmlns="http://namespaces.zope.org/apidoc">
   ...       <rootModule module="zope" />
   ...     </configure>''', context)
 
 and the root module is available:
 
   >>> list(getUtilitiesFor(IAPIDocRootModule))
-  [(u'zope', 'zope')]
+  [('zope', 'zope')]
 
 
 The ``apidoc:importModule`` Directive
 =====================================
 
 The ``importModule`` directive allows you to set the
 ``__import_unknown_modules__`` flag of the class registry. When this flag is
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/function.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 """
 __docformat__ = 'restructuredtext'
 
 from zope.interface import implementer
 from zope.location.interfaces import ILocation
 
-from zope.app.apidoc.utilities import getFunctionSignature
 from zope.app.apidoc.codemodule.interfaces import IFunctionDocumentation
+from zope.app.apidoc.utilities import getFunctionSignature
 
 
 @implementer(ILocation, IFunctionDocumentation)
-class Function(object):
+class Function:
     """This class represents a function declared in the module."""
 
     def __init__(self, module, name, func, doc=None):
         self.__parent__ = module
         self.__name__ = name
         self.__func = func
         if doc is None:
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/interfaces.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 ##############################################################################
 """Interfaces for code browser
 
 """
 __docformat__ = "reStructuredText"
 import zope.interface
 import zope.schema
-from zope.i18nmessageid import ZopeMessageFactory as _
-
 from zope.container.interfaces import IReadContainer
+from zope.i18nmessageid import ZopeMessageFactory as _
 
 
 class IAPIDocRootModule(zope.interface.Interface):
     """Marker interface for utilities that represent class browser root
     modules.
 
     The utilities will be simple strings, representing the modules Python
@@ -140,51 +139,51 @@
         """
 
 
 class IDirective(zope.interface.Interface):
     """Representation of a directive in IZCMLFile."""
 
     name = zope.schema.Tuple(
-        title=u'Name',
-        description=u'Name of the directive in the form (Namespace. Name)',
+        title='Name',
+        description='Name of the directive in the form (Namespace. Name)',
         required=True)
 
     schema = zope.schema.Field(
-        title=u'Schema',
-        description=u'Schema describing the directive attributes',
+        title='Schema',
+        description='Schema describing the directive attributes',
         required=True)
 
     attrs = zope.schema.Field(
-        title=u'Attributes',
-        description=u"SAX parser representation of the directive's attributes",
+        title='Attributes',
+        description="SAX parser representation of the directive's attributes",
         required=True)
 
     context = zope.schema.Field(
-        title=u'Configuration Context',
-        description=u'Configuration context while the directive was parsed.',
+        title='Configuration Context',
+        description='Configuration context while the directive was parsed.',
         required=True)
 
     prefixes = zope.schema.Dict(
-        title=u'Prefixes',
-        description=u'Mapping from namespace URIs to prefixes.',
+        title='Prefixes',
+        description='Mapping from namespace URIs to prefixes.',
         required=True)
 
     info = zope.schema.Field(
-        title=u'Info',
-        description=u'ParserInfo objects containing line and column info.',
+        title='Info',
+        description='ParserInfo objects containing line and column info.',
         required=True)
 
     __parent__ = zope.schema.Field(
-        title=u'Parent',
-        description=u'Parent Directive',
+        title='Parent',
+        description='Parent Directive',
         required=True)
 
     subs = zope.schema.List(
-        title=u'Sub-Directives',
-        description=u'List of sub-directives',
+        title='Sub-Directives',
+        description='List of sub-directives',
         required=True)
 
 
 class IRootDirective(IDirective):
     """Marker interface"""
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/meta.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/meta.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/metaconfigure.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/metaconfigure.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 #
 ##############################################################################
 """This module handles the 'apidoc:rootModule' and 'apidoc:moduleImport'
  namespace directives.
 
 """
 __docformat__ = 'restructuredtext'
-from zope.interface import implementer
 from zope.component.zcml import utility
+from zope.interface import implementer
 
 from zope.app.apidoc import classregistry
 from zope.app.apidoc.codemodule.interfaces import IAPIDocRootModule
 
 
 @implementer(IAPIDocRootModule)
 class RootModule(str):
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/metadirectives.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/metadirectives.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 
 class IRootModule(zope.interface.Interface):
     """Declares a new root module to be available for the class documentation
     module."""
 
     module = zope.schema.TextLine(
-        title=u"Root Module Name",
-        description=u"This is the Python path of the new root module.",
+        title="Root Module Name",
+        description="This is the Python path of the new root module.",
         required=True
     )
 
 
 class IModuleImport(zope.interface.Interface):
     """Set a flag whether new modules can be imported to the class registry or
        not."""
 
     allow = zope.schema.Bool(
-        title=u"Allow Importing Modules",
-        description=u"When set to true, new modules will be imported by path.",
+        title="Allow Importing Modules",
+        description="When set to true, new modules will be imported by path.",
         required=True,
         default=False
     )
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/module.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,34 +13,33 @@
 ##############################################################################
 """Module representation for code browser
 
 """
 __docformat__ = 'restructuredtext'
 import os
 import types
-import six
 
-import zope
 from zope.cachedescriptors.property import Lazy
-from zope.proxy import getProxiedObject
+from zope.hookable import hookable
 from zope.interface import implementer
 from zope.interface import providedBy
 from zope.interface.interface import InterfaceClass
-from zope.location.interfaces import ILocation
 from zope.location import LocationProxy
-from zope.hookable import hookable
+from zope.location.interfaces import ILocation
+from zope.proxy import getProxiedObject
 
+import zope
 from zope.app.apidoc.classregistry import safe_import
-from zope.app.apidoc.utilities import ReadContainerBase
-from zope.app.apidoc.codemodule.interfaces import IModuleDocumentation
-
 from zope.app.apidoc.codemodule.class_ import Class
 from zope.app.apidoc.codemodule.function import Function
+from zope.app.apidoc.codemodule.interfaces import IModuleDocumentation
 from zope.app.apidoc.codemodule.text import TextFile
 from zope.app.apidoc.codemodule.zcml import ZCMLFile
+from zope.app.apidoc.utilities import ReadContainerBase
+
 
 # Ignore these files, since they are not necessary or cannot be imported
 # correctly.
 IGNORE_FILES = frozenset((
     'tests',
     'tests.py',
     'ftests',
@@ -77,36 +76,25 @@
         # __file__ can be None, especially with namespace packages on
         # Python 3.7
         module_file = getattr(self._module, '__file__', None) or ''
         module_path = getattr(self._module, '__path__', None)
         if module_file.endswith(
                 ('__init__.py', '__init__.pyc', '__init__.pyo')):
             self._package = True
-        elif hasattr(self._module, '__package__'):
-            # Detect namespace packages, especially (but not limited
-            # to) Python 3 with implicit namespace packages:
+        else:
+            # Detect namespace packages with implicit namespace packages:
 
             # "When the module is a package, its
             # __package__ value should be set to its __name__. When
             # the module is not a package, __package__ should be set
             # to the empty string for top-level modules, or for
             # submodules, to the parent package's "
 
-            # Note that everything has __package__ on Python 3, but not
-            # necessarily on Python 2.
             pkg_name = self._module.__package__
             self._package = pkg_name and self._module.__name__ == pkg_name
-        else:
-            # Python 2. Lets do some introspection. Namespace packages
-            # often have an empty file. Note that path isn't necessarily
-            # indexable.
-            if (module_file == ''
-                and module_path
-                    and os.path.isdir(list(module_path)[0])):
-                self._package = True
 
         if not self._package:
             return
 
         for mod_dir in module_path:
             # TODO: If we are dealing with eggs, we will not have a
             # directory right away. For now we just ignore zipped eggs;
@@ -118,15 +106,15 @@
                 if mod_file in IGNORE_FILES or mod_file in self._children:
                     continue
 
                 path = os.path.join(mod_dir, mod_file)
 
                 if os.path.isdir(path) and '__init__.py' in os.listdir(path):
                     # subpackage
-                    # XXX Python 3 implicit packages don't have __init__.py
+                    # XXX Implicit packages don't have __init__.py
 
                     fullname = self._module.__name__ + '.' + mod_file
                     module = safe_import(fullname)
                     if module is not None:
                         self._children[mod_file] = Module(
                             self, mod_file, module)
                 elif os.path.isfile(path):
@@ -181,15 +169,15 @@
             attr = getattr(self._module, name, None)
             if attr is None:
                 continue
 
             if isinstance(attr, hookable):
                 attr = attr.implementation
 
-            if isinstance(attr, six.class_types):
+            if isinstance(attr, type):
                 self._children[name] = Class(self, name, attr)
 
             elif isinstance(attr, InterfaceClass):
                 self._children[name] = LocationProxy(attr, self, name)
 
             elif isinstance(attr, types.FunctionType):
                 doc = attr.__doc__
@@ -279,15 +267,15 @@
         # Only publicize public objects, even though we do keep track of
         # private ones
         return [(name, value)
                 for name, value in self._children.items()
                 if not name.startswith('_')]
 
     def __repr__(self):
-        return '<Module %r name %r parent %r at 0x%x>' % (
+        return '<Module {!r} name {!r} parent {!r} at 0x{:x}>'.format(
             self._module, self.__name__, self.__parent__, id(self)
         )
 
 
 class _LazyModule(Module):
 
     copy_from = None
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for the Code Documentation Module
 
 """
+import doctest
 import os.path
 import unittest
-import doctest
 
 from zope.component import testing
 
-from zope.app.apidoc.codemodule.text import TextFile
+import zope.app.apidoc.codemodule
 from zope.app.apidoc.codemodule.module import Module
-
-from zope.app.apidoc.tests import standard_checker
-from zope.app.apidoc.tests import standard_option_flags
+from zope.app.apidoc.codemodule.text import TextFile
 from zope.app.apidoc.tests import LayerDocFileSuite
-import zope.app.apidoc.codemodule
+from zope.app.apidoc.tests import standard_option_flags
+
 
 here = os.path.dirname(__file__)
 
 
 class TestText(unittest.TestCase):
 
     def _read_via_text(self, path):
@@ -41,22 +40,22 @@
             return f.read()
 
     def test_crlf(self):
         self.assertEqual(self._read_bytes('_test_crlf.txt'),
                          b'This file\r\nuses \r\nWindows \r\nline endings.')
 
         self.assertEqual(self._read_via_text('_test_crlf.txt'),
-                         u'This file\nuses \nWindows \nline endings.')
+                         'This file\nuses \nWindows \nline endings.')
 
     def test_cr(self):
         self.assertEqual(self._read_bytes('_test_cr.txt'),
                          b'This file\ruses \rMac \rline endings.')
 
         self.assertEqual(self._read_via_text('_test_cr.txt'),
-                         u'This file\nuses \nMac \nline endings.')
+                         'This file\nuses \nMac \nline endings.')
 
 
 class TestModule(unittest.TestCase):
 
     def test_non_dir_on_path(self):
         path = zope.app.apidoc.codemodule.__path__
         zope.app.apidoc.codemodule.__path__ = ['this is not a path']
@@ -96,29 +95,31 @@
         self.assertIsInstance(zope.component._api.getSiteManager, hookable)
         from zope.app.apidoc.codemodule.function import Function
         mod = Module(None, 'hooks', zope.component._api)
         self.assertIsInstance(mod._children['getSiteManager'], Function)
 
     def test_zope_loaded_correctly(self):
         # Zope is guaranteed to be a namespace package, as is zope.app.
+        import zope.annotation
+
         import zope
         import zope.app
-        import zope.annotation
         import zope.app.apidoc
         mod = Module(None, 'zope', zope)
         self.assertEqual(mod['annotation']._module, zope.annotation)
         self.assertEqual(mod['app']._module, zope.app)
         self.assertEqual(mod['app']['apidoc']._module, zope.app.apidoc)
 
     def test_module_with_file_of_none(self):
         # Sometimes namespace packages have this,
         # especially on Python 3.7.
-        class Mod(object):
+        class Mod:
             __file__ = None
             __name__ = 'name'
+            __package__ = None
 
         mod = Mod()
         mod.__doc__ = 'A module'
 
         inst = Module(None, 'name', mod)
         self.assertEqual(mod.__doc__, inst.getDocString())
 
@@ -170,39 +171,37 @@
 
 
 class TestClass(unittest.TestCase):
 
     def test_permission_is_not_method(self):
         # We don't incorrectly assume that callable objects,
         # like security proxies, are methods
-        from zope.app.apidoc.codemodule.class_ import Class
         from zope.security.checker import CheckerPublic
 
+        from zope.app.apidoc.codemodule.class_ import Class
+
         self.assertTrue(callable(CheckerPublic))
 
-        class Parent(object):
+        class Parent:
             def getPath(self):
                 return ''
 
-        class MyClass(object):
+        class MyClass:
             permission = CheckerPublic
 
         klass = Class(Parent(), MyClass.__name__, MyClass)
 
         self.assertEqual([], klass.getMethods())
 
 
 def test_suite():
-    checker = standard_checker()
-
     return unittest.TestSuite((
         LayerDocFileSuite(
             'README.rst',
             zope.app.apidoc.codemodule),
         doctest.DocFileSuite(
             'directives.rst',
             setUp=testing.setUp,
             tearDown=testing.tearDown,
-            checker=checker,
             optionflags=standard_option_flags),
         unittest.defaultTestLoader.loadTestsFromName(__name__),
     ))
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/text.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from zope.interface import implementer
 from zope.location.interfaces import ILocation
 
 from zope.app.apidoc.codemodule.interfaces import ITextFile
 
 
 @implementer(ILocation, ITextFile)
-class TextFile(object):
+class TextFile:
     """This class represents a function declared in the module."""
 
     def __init__(self, path, name, package):
         self.path = path
         self.__parent__ = package
         self.__name__ = name
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/codemodule/zcml.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/codemodule/zcml.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,55 +12,56 @@
 #
 ##############################################################################
 """ZCML File Representation
 """
 __docformat__ = "reStructuredText"
 import copy
 from xml.sax import make_parser
-from xml.sax.xmlreader import InputSource
 from xml.sax.handler import feature_namespaces
+from xml.sax.xmlreader import InputSource
 
+import zope.app.appsetup.appsetup
 from zope.cachedescriptors.property import Lazy
-from zope.configuration import xmlconfig, config
-from zope.interface import implementer, directlyProvides
+from zope.configuration import config
+from zope.configuration import xmlconfig
+from zope.interface import directlyProvides
+from zope.interface import implementer
 from zope.location.interfaces import ILocation
 
-import zope.app.appsetup.appsetup
-
 from zope.app.apidoc.codemodule.interfaces import IDirective
 from zope.app.apidoc.codemodule.interfaces import IRootDirective
 from zope.app.apidoc.codemodule.interfaces import IZCMLFile
 
 
-class MyConfigHandler(xmlconfig.ConfigurationHandler, object):
+class MyConfigHandler(xmlconfig.ConfigurationHandler):
     """Special configuration handler to generate an XML tree."""
 
     def __init__(self, context):
-        super(MyConfigHandler, self).__init__(context)
+        super().__init__(context)
         self.rootElement = self.currentElement = None
         self.prefixes = {}
 
     def startPrefixMapping(self, prefix, uri):
         self.prefixes[uri] = prefix
 
     def evaluateCondition(self, expression):
         # We always want to process/show all ZCML directives.
         # The exception needs to be `installed` that evaluates to False;
         # if we can't load the package, we can't process the file
         arguments = expression.split(None)
         verb = arguments.pop(0)
         if verb in ('installed', 'not-installed'):
-            return super(MyConfigHandler, self).evaluateCondition(expression)
+            return super().evaluateCondition(expression)
         return True
 
     def startElementNS(self, name, qname, attrs):
         # The last stack item is parent of the stack item that we are about to
         # create
         stackitem = self.context.stack[-1]
-        super(MyConfigHandler, self).startElementNS(name, qname, attrs)
+        super().startElementNS(name, qname, attrs)
 
         # Get the parser info from the correct context
         info = self.context.stack[-1].context.info
 
         # complex stack items behave a bit different than the other ones, so
         # we need to handle it separately
         if isinstance(stackitem, config.ComplexStackItem):
@@ -77,20 +78,20 @@
         else:
             self.currentElement.subs.append(element)
 
         element.__parent__ = self.currentElement
         self.currentElement = element
 
     def endElementNS(self, name, qname):
-        super(MyConfigHandler, self).endElementNS(name, qname)
+        super().endElementNS(name, qname)
         self.currentElement = self.currentElement.__parent__
 
 
 @implementer(IDirective)
-class Directive(object):
+class Directive:
     """Representation of a ZCML directive."""
 
     def __init__(self, name, schema, attrs, context, info, prefixes):
         self.name = name
         self.schema = schema
         self.attrs = attrs
         self.context = context
@@ -100,15 +101,15 @@
         self.prefixes = prefixes
 
     def __repr__(self):
         return '<Directive %s>' % str(self.name)
 
 
 @implementer(ILocation, IZCMLFile)
-class ZCMLFile(object):
+class ZCMLFile:
     """Representation of an entire ZCML file."""
 
     def __init__(self, filename, package, parent, name):
         # Retrieve the directive registry
         self.filename = filename
         self.package = package
         self.__parent__ = parent
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/component.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,42 +11,43 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Component Inspection Utilities
 
 """
 __docformat__ = 'restructuredtext'
-import six
 import types
-import zope.interface.declarations
 
+import zope.interface.declarations
 from zope.component import getGlobalSiteManager
 from zope.component.interfaces import IFactory
 from zope.i18nmessageid import ZopeMessageFactory as _
 from zope.interface import Interface
 from zope.interface.interface import InterfaceClass
 from zope.publisher.interfaces import IRequest
 
 from zope.app.apidoc.classregistry import classRegistry
-from zope.app.apidoc.utilities import relativizePath, truncateSysPath
-from zope.app.apidoc.utilities import getPythonPath, isReferencable, renderText
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import isReferencable
+from zope.app.apidoc.utilities import relativizePath
+from zope.app.apidoc.utilities import renderText
+from zope.app.apidoc.utilities import truncateSysPath
 from zope.app.apidoc.utilitymodule import utilitymodule
 
 
 SPECIFIC_INTERFACE_LEVEL = 1
 EXTENDED_INTERFACE_LEVEL = 2
 GENERIC_INTERFACE_LEVEL = 4
 
 
 def _adapterishRegistrations(registry):
     for registrations in (registry.registeredAdapters,
                           registry.registeredSubscriptionAdapters,
                           registry.registeredHandlers):
-        for r in registrations():
-            yield r
+        yield from registrations()
 
 
 def _ignore_adapter(reg, withViews=False):
     return (
         # Ignore adapters that have no required interfaces
         not reg.required
         # Ignore views
@@ -194,22 +195,22 @@
     factory = getRealFactory(reg.factory)
     path = getPythonPath(factory)
 
     url = None
     if isReferencable(path):
         url = path.replace('.', '/')
 
-    if isinstance(reg.info, six.string_types):
+    if isinstance(reg.info, str):
         doc = reg.info
         zcml = None
     else:
         doc = None
         zcml = getParserInfoInfoDictionary(reg.info)
 
-    name = getattr(reg, 'name', u'')
+    name = getattr(reg, 'name', '')
     name = name.decode('utf-8') if isinstance(name, bytes) else name
     return {
         'provided': getInterfaceInfoDictionary(reg.provided),
         'required': [getSpecificationInfoDictionary(iface)
                      for iface in reg.required
                      if iface is not None],
         'name': name,
@@ -229,45 +230,44 @@
     if IFactory.providedBy(factory) and hasattr(factory, '_callable'):
         callable = factory._callable
     elif hasattr(callable, '__class__'):
         callable = callable.__class__
 
     path = getPythonPath(callable)
 
-    return {'name': six.text_type(reg.name) or _('<i>no name</i>'),
-            'title': getattr(factory, 'title', u''),
-            'description': renderText(getattr(factory, 'description', u''),
+    return {'name': str(reg.name) or _('<i>no name</i>'),
+            'title': getattr(factory, 'title', ''),
+            'description': renderText(getattr(factory, 'description', ''),
                                       module=callable.__module__),
             'url': isReferencable(path) and path.replace('.', '/') or None}
 
 
 def getUtilityInfoDictionary(reg):
     """Return a PT-friendly info dictionary for a factory."""
     component = reg.component
     # Check whether we have an instance of some custom type or not
     # Unfortunately, a lot of utilities have a `__name__` attribute, so we
     # cannot simply check for its absence
     # TODO: Once we support passive display of instances, this insanity can go
     #       away.
     if not isinstance(component, (types.MethodType, types.FunctionType,
-                                  six.class_types,
-                                  InterfaceClass)):
+                                  type, InterfaceClass)):
         component = getattr(component, '__class__', component)
 
     path = getPythonPath(component)
 
     # provided interface id
-    iface_id = '%s.%s' % (reg.provided.__module__, reg.provided.getName())
+    iface_id = '{}.{}'.format(reg.provided.__module__, reg.provided.getName())
 
     # Determine the URL
     if isinstance(component, InterfaceClass):
         url = 'Interface/%s' % path
     else:
         url = None
         if isReferencable(path):
             url = 'Code/%s' % path.replace('.', '/')
 
-    return {'name': six.text_type(reg.name) or _('<i>no name</i>'),
+    return {'name': str(reg.name) or _('<i>no name</i>'),
             'url_name': utilitymodule.encodeName(reg.name or '__noname__'),
             'iface_id': iface_id,
             'path': path,
             'url': url}
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/component.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/component.rst`

 * *Files 8% similar despite different names*

```diff
@@ -43,94 +43,94 @@
   >>> ztapi.provideAdapter(adapts=(IFoo, IRequest), provides=ISpecialResult, factory=None)
   >>> ztapi.provideHandler(adapts=(IFoo,), factory='stubFactory')
 
   >>> regs = list(component.getRequiredAdapters(IFoo))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBar], ISpecialResult, u'', None, u''),
+                       [IFoo, IBar], ISpecialResult, '', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo], IResult, u'', None, u''),
+                       [IFoo], IResult, '', None, ''),
    HandlerRegistration(<BaseGlobalComponents base>,
-                       [IFoo], u'', 'stubFactory', u'')]
+                       [IFoo], '', 'stubFactory', '')]
 
 Note how the adapter requiring an
 :class:`zope.publisher.interfaces.IRequest` at the end of the required
 interfaces is neglected. This is because it is recognized as a view
 and views are not returned by default. But you can simply turn this
 flag on:
 
   >>> regs = list(component.getRequiredAdapters(IFoo, withViews=True))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBar], ISpecialResult, u'', None, u''),
+                       [IFoo, IBar], ISpecialResult, '', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IRequest], ISpecialResult, u'', None, u''),
+                       [IFoo, IRequest], ISpecialResult, '', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo], IResult, u'', None, u''),
+                       [IFoo], IResult, '', None, ''),
    HandlerRegistration(<BaseGlobalComponents base>,
-                       [IFoo], u'', 'stubFactory', u'')]
+                       [IFoo], '', 'stubFactory', '')]
 
 The function will also pick up registrations that have required interfaces the
 specified interface extends:
 
   >>> regs = list(component.getRequiredAdapters(IFoo))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBar], ISpecialResult, u'', None, u''),
+                       [IFoo, IBar], ISpecialResult, '', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo], IResult, u'', None, u''),
+                       [IFoo], IResult, '', None, ''),
    HandlerRegistration(<BaseGlobalComponents base>,
-                       [IFoo], u'', 'stubFactory', u'')]
+                       [IFoo], '', 'stubFactory', '')]
 
 And all of the required interfaces are considered, of course:
 
   >>> regs = list(component.getRequiredAdapters(IBar))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBar], ISpecialResult, u'', None, u'')]
+                       [IFoo, IBar], ISpecialResult, '', None, '')]
 
 
 :func:`getProvidedAdapters`
 ===========================
 
 Of course, we are also interested in the adapters that provide a certain
 interface. This function returns those adapter registrations, again ignoring
 views by default.
 
   >>> regs = list(component.getProvidedAdapters(ISpecialResult))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBar], ISpecialResult, u'', None, u'')]
+                       [IFoo, IBar], ISpecialResult, '', None, '')]
 
 And by specifying the ``withView`` flag, we get views as well:
 
   >>> regs = list(component.getProvidedAdapters(ISpecialResult, withViews=True))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBar], ISpecialResult, u'', None, u''),
+                       [IFoo, IBar], ISpecialResult, '', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IRequest], ISpecialResult, u'', None, u'')]
+                       [IFoo, IRequest], ISpecialResult, '', None, '')]
 
 We can of course also ask for adapters specifying ``IResult``:
 
   >>> regs = list(component.getProvidedAdapters(IResult, withViews=True))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBar], ISpecialResult, u'', None, u''),
+                       [IFoo, IBar], ISpecialResult, '', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IRequest], ISpecialResult, u'', None, u''),
+                       [IFoo, IRequest], ISpecialResult, '', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo], IResult, u'', None, u'')]
+                       [IFoo], IResult, '', None, '')]
 
 
 :func:`getClasses`
 ==================
 
 This package comes with a little tool called the class registry
 (see :doc:`classregistry`). It provides a dictionary of all classes in the
@@ -189,23 +189,23 @@
 Let's see whether we will be able to get them:
 
   >>> regs = list(component.getFactories(IFooBar))
   >>> regs.sort()
   >>> regs
   [UtilityRegistration(<BaseGlobalComponents base>,
       IFactory, 'MyFooBar',
-      <Factory for <class 'zope.app.apidoc.doctest.MyFooBar'>>, None, u'')]
+      <Factory for <class 'zope.app.apidoc.doctest.MyFooBar'>>, None, '')]
 
   >>> regs = list(component.getFactories(IFoo))
   >>> regs.sort()
   >>> regs
   [UtilityRegistration(<BaseGlobalComponents base>, IFactory, 'MyFoo',
-               <Factory for <class 'zope.app.apidoc.doctest.MyFoo'>>, None, u''),
+               <Factory for <class 'zope.app.apidoc.doctest.MyFoo'>>, None, ''),
    UtilityRegistration(<BaseGlobalComponents base>, IFactory, 'MyFooBar',
-            <Factory for <class 'zope.app.apidoc.doctest.MyFooBar'>>, None, u'')]
+            <Factory for <class 'zope.app.apidoc.doctest.MyFooBar'>>, None, '')]
 
 
 :func:`getUtilities`
 ====================
 
 Return all utility registrations for utilities that provide the specified
 interface.
@@ -217,24 +217,24 @@
   >>> ztapi.provideUtility(MyFooBar(), IFooBar)
 
 Now let's have a look what we have:
 
   >>> regs = list(component.getUtilities(IFooBar))
   >>> regs.sort()
   >>> regs
-  [UtilityRegistration(<BaseGlobalComponents base>, IFooBar, u'',
-                       <zope.app.apidoc.doctest.MyFooBar object at ...>, None, u'')]
+  [UtilityRegistration(<BaseGlobalComponents base>, IFooBar, '',
+                       <zope.app.apidoc.doctest.MyFooBar object at ...>, None, '')]
 
   >>> regs = list(component.getUtilities(IFoo))
   >>> regs.sort()
   >>> regs
-  [UtilityRegistration(<BaseGlobalComponents base>, IFoo, u'',
-                       <zope.app.apidoc.doctest.MyFoo object at ...>, None, u''),
-   UtilityRegistration(<BaseGlobalComponents base>, IFooBar, u'',
-                       <zope.app.apidoc.doctest.MyFooBar object at ...>, None, u'')]
+  [UtilityRegistration(<BaseGlobalComponents base>, IFoo, '',
+                       <zope.app.apidoc.doctest.MyFoo object at ...>, None, ''),
+   UtilityRegistration(<BaseGlobalComponents base>, IFooBar, '',
+                       <zope.app.apidoc.doctest.MyFooBar object at ...>, None, '')]
 
 
 :func:`getRealFactory`
 ======================
 
 During registration, factories are commonly masked by wrapper functions. Also,
 factories are sometimes also ``IFactory`` instances, which are not referencable,
@@ -321,17 +321,17 @@
 
 :func:`getTypeInfoDictionary`
 =============================
 
 This function returns the info dictionary of a type.
 
   >>> pprint(component.getTypeInfoDictionary(tuple), width=1)
-  {'module': '__builtin__',
+  {'module': 'builtins',
    'name': 'tuple',
-   'url': '__builtin__/tuple'}
+   'url': 'builtins/tuple'}
 
 
 :func:`getSpecificationInfoDictionary`
 ======================================
 
 Thsi function returns an info dictionary for the given specification. A
 specification can either be an interface or class. If it is an interface, it
@@ -351,17 +351,17 @@
 
   >>> import zope.interface
   >>> tupleSpec = zope.interface.implementedBy(tuple)
 
   >>> pprint(component.getSpecificationInfoDictionary(tupleSpec))
   {'isInterface': False,
    'isType': True,
-   'module': '__builtin__',
+   'module': 'builtins',
    'name': 'tuple',
-   'url': '__builtin__/tuple'}
+   'url': 'builtins/tuple'}
 
 For the type, we simply reuse the type info dictionary function.
 
 
 :func:`getAdapterInfoDictionary`
 ================================
 
@@ -380,15 +380,15 @@
 
 And now get the info dictionary:
 
   >>> pprint(component.getAdapterInfoDictionary(reg), width=50)
   {'doc': 'doc info',
    'factory': 'zope.app.apidoc.doctest.MyResult',
    'factory_url': 'zope/app/apidoc/doctest/MyResult',
-   'name': u'FooToResult',
+   'name': 'FooToResult',
    'provided': {'module': 'zope.app.apidoc.doctest',
                 'name': 'IResult'},
    'required': [{'isInterface': True,
                  'isType': False,
                  'module': 'zope.app.apidoc.doctest',
                  'name': 'IFoo'},
                 {'isInterface': True,
@@ -407,15 +407,15 @@
 
   >>> reg = AdapterRegistration(None, (IFoo, IBar), IResult, 'FooToResult',
   ...                            MyResultType, 'doc info')
   >>> pprint(component.getAdapterInfoDictionary(reg), width=50)
   {'doc': 'doc info',
    'factory': 'zope.app.apidoc.doctest.MyResult2',
    'factory_url': None,
-   'name': u'FooToResult',
+   'name': 'FooToResult',
    'provided': {'module': 'zope.app.apidoc.doctest',
                 'name': 'IResult'},
    'required': [{'isInterface': True,
                  'isType': False,
                  'module': 'zope.app.apidoc.doctest',
                  'name': 'IFoo'},
                 {'isInterface': True,
@@ -431,15 +431,15 @@
   >>> from zope.interface.registry import HandlerRegistration
   >>> reg = HandlerRegistration(None, (IFoo, IBar), '', MyResult, 'doc info')
 
   >>> pprint(component.getAdapterInfoDictionary(reg))
   {'doc': 'doc info',
    'factory': 'zope.app.apidoc.doctest.MyResult',
    'factory_url': 'zope/app/apidoc/doctest/MyResult',
-   'name': u'',
+   'name': '',
    'provided': None,
    'required': [{'isInterface': True,
                  'isType': False,
                  'module': 'zope.app.apidoc.doctest',
                  'name': 'IFoo'},
                 {'isInterface': True,
                  'isType': False,
@@ -455,16 +455,16 @@
 data of a factory (utility) registration in an output-friendly format.
 
 Luckily we have already registered some factories, so we just reuse their
 registrations:
 
   >>> pprint(component.getFactoryInfoDictionary(
   ...     next(component.getFactories(IFooBar))))
-  {'description': u'<p>My Foo Bar</p>\n',
-   'name': u'MyFooBar',
+  {'description': '<p>My Foo Bar</p>\n',
+   'name': 'MyFooBar',
    'title': 'MyFooBar',
    'url': 'zope/app/apidoc/doctest/MyFooBar'}
 
 If the factory's path cannot be referenced, for example if a type has been
 created using the ``type()`` builtin function, then the URL of the factory
 will be ``None``:
 
@@ -477,17 +477,17 @@
   >>> MyFactoryType = type('MyFactory', (FactoryBase,), {})
   >>> from zope.interface import classImplements
   >>> classImplements(MyFactoryType, IFactory)
   >>> ztapi.provideUtility(MyFactoryType(), IFactory, 'MyFactory')
 
   >>> pprint(component.getFactoryInfoDictionary(
   ...     next(component.getFactories(IMine))), width=50)
-  {'description': u'',
-   'name': u'MyFactory',
-   'title': u'',
+  {'description': '',
+   'name': 'MyFactory',
+   'title': '',
    'url': None}
 
 
 :func:`getUtilityInfoDictionary`
 ================================
 
 This function returns a page-template-friendly dictionary representing the
@@ -495,11 +495,11 @@
 
 Luckily we have already registered some utilities, so we just reuse their
 registrations:
 
   >>> pprint(component.getUtilityInfoDictionary(
   ...     next(component.getUtilities(IFooBar))))
   {'iface_id': 'zope.app.apidoc.doctest.IFooBar',
-   'name': u'<i>no name</i>',
+   'name': '<i>no name</i>',
    'path': 'zope.app.apidoc.doctest.MyFooBar',
    'url': 'Code/zope/app/apidoc/doctest/MyFooBar',
-   'url_name': b'X19ub25hbWVfXw=='}
+   'url_name': 'X19ub25hbWVfXw=='}
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/disabled.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/disabled.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 ##############################################################################
 """Stubs for when documentation is disabled.
 
 """
 __docformat__ = 'restructuredtext'
 
 
-class APIDocStub(object):
+class APIDocStub:
     """A stub to use as display context when APIDoc is disabled.
     """
 
 
-class apidocNamespace(object):
+class apidocNamespace:
     """Used to traverse to an API Documentation when it is disabled."""
 
     def __init__(self, ob, request=None):
         self.request = request
         self.context = ob
 
     def traverse(self, name, ignore):
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/disabled.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/disabled.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/enabled.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/enabled.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ftesting-base.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ftesting-base.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/browser.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,40 @@
 """
 
 __docformat__ = 'restructuredtext'
 
 import inspect
 
 from zope.i18nmessageid import ZopeMessageFactory as _
+from zope.proxy import removeAllProxies
+from zope.publisher.browser import BrowserView
 from zope.publisher.interfaces.browser import IBrowserRequest
-from zope.publisher.interfaces.xmlrpc import IXMLRPCRequest
-from zope.publisher.interfaces.http import IHTTPRequest
 from zope.publisher.interfaces.ftp import IFTPRequest
-from zope.publisher.browser import BrowserView
+from zope.publisher.interfaces.http import IHTTPRequest
+from zope.publisher.interfaces.xmlrpc import IXMLRPCRequest
 from zope.security.proxy import removeSecurityProxy
-from zope.proxy import removeAllProxies
-from zope.traversing.api import getName, traverse
+from zope.traversing.api import getName
+from zope.traversing.api import traverse
 from zope.traversing.browser import absoluteURL
 
-from zope.app.apidoc.utilities import getPythonPath, renderText
 from zope.app.apidoc import classregistry
-from zope.app.apidoc import interface, component, presentation
-from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
+from zope.app.apidoc import component
+from zope.app.apidoc import interface
+from zope.app.apidoc import presentation
 from zope.app.apidoc.browser.utilities import findAPIDocumentationRoot
+from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import renderText
 
 
 class InterfaceDetails(BrowserView):
     """View class for an Interface."""
 
     def __init__(self, context, request):
-        super(InterfaceDetails, self).__init__(context, request)
+        super().__init__(context, request)
         self._prepareViews()
 
     def getAPIDocRootURL(self):
         return findAPIDocumentationRootURL(self.context, self.request)
 
     def getId(self):
         """Return the id of the field as it is defined for the interface
@@ -260,15 +264,15 @@
             "xmlrpc": _("XML-RPC"),
             "http": _("HTTP"),
             "ftp": _("FTP"),
             "other": _("Other"),
         }
 
 
-class InterfaceBreadCrumbs(object):
+class InterfaceBreadCrumbs:
     """View that provides breadcrumbs for interface objects"""
 
     context = None
     request = None
 
     def __call__(self):
         """Create breadcrumbs for an interface object.
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/browser.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/browser.rst`

 * *Files 7% similar despite different names*

```diff
@@ -19,32 +19,32 @@
   ...
   ...     def bar(self):
   ...         '''bar'''
   ...
   ...     blah = zope.interface.Attribute('blah', 'blah')
   ...
   ...     field = zope.schema.Field(
-  ...         title = u'title', description = u'description')
+  ...         title = 'title', description = 'description')
 
 Now get the text. Note that there is no particular order during the text
 collection.
 
   >>> from zope.app.apidoc.ifacemodule.menu import getAllTextOfInterface
   >>> text = getAllTextOfInterface(IFoo)
-  >>> u'foo' in text
+  >>> 'foo' in text
   True
-  >>> u'bar' in text
+  >>> 'bar' in text
   True
-  >>> u'blah' in text
+  >>> 'blah' in text
   True
-  >>> u'field' in text
+  >>> 'field' in text
   True
-  >>> u'title' in text
+  >>> 'title' in text
   True
-  >>> u'description' in text
+  >>> 'description' in text
   True
 
 
 ``Menu`` class
 ==============
 
 This is the :class:`menu class <menu.Menu>` for the Interface
@@ -113,22 +113,22 @@
   ...
   ...     More description here...
   ...     """
   ...     foo = zope.interface.Attribute('This is foo.')
   ...     bar = zope.interface.Attribute('This is bar.')
   ...
   ...     title = zope.schema.TextLine(
-  ...         description=u'Title',
+  ...         description='Title',
   ...         required=True,
-  ...         default=u'Foo')
+  ...         default='Foo')
   ...
   ...     description = zope.schema.Text(
-  ...         description=u'Desc',
+  ...         description='Desc',
   ...         required=False,
-  ...         default=u'Foo.')
+  ...         default='Foo.')
   ...
   ...     def blah():
   ...         """This is blah."""
   ...
   ...     def get(key, default=None):
   ...         """This is get."""
 
@@ -142,15 +142,15 @@
   ... class Foo(object):
   ...     pass
 
   >>> from zope import component as ztapi
   >>> ztapi.provideAdapter(adapts=(IBar,), provides=IFoo, factory=Foo)
 
   >>> from zope.app.apidoc.classregistry import classRegistry
-  >>> classRegistry['__builtin__.Foo'] = Foo
+  >>> classRegistry['builtins.Foo'] = Foo
 
 Let's also register a factory for ``Foo``
 
   >>> from zope.component.interfaces import IFactory
   >>> from zope.component.factory import Factory
   >>> ztapi.provideUtility(Factory(Foo, title='Foo Factory'), IFactory,
   ...                      'FooFactory')
@@ -184,15 +184,15 @@
 
 :meth:`InterfaceDetails.getDoc`
 -------------------------------
 
 Return the main documentation string of the interface.
 
   >>> details.getDoc()[:32]
-  u'<p>This is the Foo interface</p>'
+  '<p>This is the Foo interface</p>'
 
 
 :meth:`InterfaceDetails.getBases`
 ---------------------------------
 
 Get all bases of this class
 
@@ -217,71 +217,71 @@
 
   >>> zope.interface.directlyProvides(IFoo, IMyType)
 
 we get a result:
 
   >>> pprint(details.getTypes(), width=1)
   [{'name': 'IMyType',
-    'path': '__builtin__.IMyType'}]
+    'path': 'builtins.IMyType'}]
 
 
 :meth:`InterfaceDetails.getAttributes`
 --------------------------------------
 
 Return a list of attributes in the order they were specified.
 
   >>> pprint(sorted(details.getAttributes(), key=lambda x: x['name']))
-  [{'doc': u'<p>This is bar.</p>\n',
+  [{'doc': '<p>This is bar.</p>\n',
     'name': 'bar'},
-   {'doc': u'<p>This is foo.</p>\n',
+   {'doc': '<p>This is foo.</p>\n',
     'name': 'foo'}]
 
 
 :meth:`InterfaceDetails.getMethods`
 -----------------------------------
 
 Return a list of methods in the order they were specified.
 
   >>> pprint(sorted(details.getMethods(), key=lambda x: x['name']))
-  [{'doc': u'<p>This is blah.</p>\n',
+  [{'doc': '<p>This is blah.</p>\n',
     'name': 'blah',
     'signature': '()'},
-   {'doc': u'<p>This is get.</p>\n',
+   {'doc': '<p>This is get.</p>\n',
     'name': 'get',
     'signature': '(key, default=None)'}]
 
 
 :meth:`InterfaceDetails.getFields`
 ----------------------------------
 
 Return a list of fields in required + alphabetical order.
 
 The required attributes are listed first, then the optional attributes.
 
   >>> pprint(details.getFields(), width=1)
   [{'class': {'name': 'TextLine',
               'path': 'zope/schema/_bootstrapfields/TextLine'},
-    'default': "u'Foo'",
-    'description': u'<p>Title</p>\n',
+    'default': "'Foo'",
+    'description': '<p>Title</p>\n',
     'iface': {'id': 'zope.schema.interfaces.ITextLine',
               'name': 'ITextLine'},
     'name': 'title',
     'required': True,
-    'required_string': u'required',
-    'title': u''},
+    'required_string': 'required',
+    'title': ''},
    {'class': {'name': 'Text',
               'path': 'zope/schema/_bootstrapfields/Text'},
-    'default': "u'Foo.'",
-    'description': u'<p>Desc</p>\n',
+    'default': "'Foo.'",
+    'description': '<p>Desc</p>\n',
     'iface': {'id': 'zope.schema.interfaces.IText',
               'name': 'IText'},
     'name': 'description',
     'required': False,
-    'required_string': u'optional',
-    'title': u''}]
+    'required_string': 'optional',
+    'title': ''}]
 
 :meth:`InterfaceDetails.getSpecificRequiredAdapters`
 ----------------------------------------------------
 
 Get adapters where this interface is required.
 
   >>> pprint(details.getSpecificRequiredAdapters())
@@ -311,53 +311,53 @@
 
 :meth:`InterfaceDetails.getProvidedAdapters`
 --------------------------------------------
 
 Get adapters where this interface is provided.
 
   >>> pprint(details.getProvidedAdapters(), width=1)
-  [{'doc': u'',
-    'factory': '__builtin__.Foo',
+  [{'doc': '',
+    'factory': 'builtins.Foo',
     'factory_url': None,
-    'name': u'',
-    'provided': {'module': '__builtin__',
+    'name': '',
+    'provided': {'module': 'builtins',
                  'name': 'IFoo'},
     'required': [{'isInterface': True,
                   'isType': False,
-                  'module': '__builtin__',
+                  'module': 'builtins',
                   'name': 'IBar'}],
     'zcml': None}]
 
 
 
 :meth:`InterfaceDetails.getClasses`
 -----------------------------------
 
 Get the classes that implement this interface.
 
   >>> pprint(details.getClasses(), width=1)
-  [{'path': '__builtin__.Foo',
-    'url': '__builtin__/Foo'}]
+  [{'path': 'builtins.Foo',
+    'url': 'builtins/Foo'}]
 
 :meth:`InterfaceDetails.getFactories`
 -------------------------------------
 
 Return the factories, who will provide objects implementing this
 interface.
 
   >>> pprint(details.getFactories())
-  [{'description': u'',
-    'name': u'FooFactory',
+  [{'description': '',
+    'name': 'FooFactory',
     'title': 'Foo Factory',
     'url': None}]
 
 :meth:`InterfaceDetails.getUtilities`
 -------------------------------------
 
 Return all utilities that provide this interface.
 
   >>> pprint(details.getUtilities())
-  [{'iface_id': '__builtin__.IFoo',
-    'name': u'The Foo',
-    'path': '__builtin__.Foo',
+  [{'iface_id': 'builtins.IFoo',
+    'name': 'The Foo',
+    'path': 'builtins.Foo',
     'url': None,
     'url_name': 'VGhlIEZvbw=='}]
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/component_macros.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/component_macros.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/iface_macros.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/iface_macros.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/ifacemodule.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/ifacemodule.py`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/interfaces.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 """
 
 __docformat__ = "reStructuredText"
 
 import zope.interface
 import zope.schema
-
 from zope.i18nmessageid import ZopeMessageFactory as _
 
 
 class IInterfaceDetailsPreferences(zope.interface.Interface):
     __doc__ = _("""
     Preferences for API Docs' Interface Details Screen
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/macros.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/macros.py`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/menu.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/menu.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/menu.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 ##############################################################################
 """Interface Module Browser Menu (Tree)
 
 
 """
 __docformat__ = 'restructuredtext'
 import operator
-from zope.security.proxy import removeSecurityProxy
 import re
 
+from zope.security.proxy import removeSecurityProxy
+
+
 whitepattern = re.compile(r'\s{2,}')
 namegetter = operator.itemgetter('name')
 
 
 def getAllTextOfInterface(iface):
     """Get all searchable text from an interface"""
     iface = removeSecurityProxy(iface)
@@ -31,15 +33,15 @@
     for name in iface:
         attr = iface[name]
         text += attr.getName()
         text += attr.getDoc() or ''
     return text
 
 
-class Menu(object):
+class Menu:
     """Menu for the Interface Documentation Module."""
 
     context = None
     request = None
 
     def findInterfaces(self):
         """Find the interface that match any text in the documentation strings
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/presentation_macros.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/presentation_macros.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/static_menu.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/static_menu.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/ifacemodule/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/ifacemodule/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 """Tests for the Interface Documentation Module
 
 """
 
 import unittest
 
 import zope.app.apidoc.ifacemodule
-
 from zope.app.apidoc.testing import APIDocLayer
-from zope.app.apidoc.tests import LayerDocFileSuite
 from zope.app.apidoc.tests import BrowserTestCase
+from zope.app.apidoc.tests import LayerDocFileSuite
 
 
 class InterfaceModuleTests(BrowserTestCase):
     """Just a couple of tests ensuring that the templates render."""
 
     layer = APIDocLayer
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/interface.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,26 @@
 """Interface Inspection Utilities
 
 """
 __docformat__ = 'restructuredtext'
 
 import inspect
 
-from zope.interface import Interface, providedBy
-from zope.interface.interfaces import IInterface, ISpecification
-from zope.interface.interfaces import IElement, IAttribute, IMethod
+from zope.interface import Interface
+from zope.interface import providedBy
+from zope.interface.interfaces import IAttribute
+from zope.interface.interfaces import IElement
+from zope.interface.interfaces import IInterface
+from zope.interface.interfaces import IMethod
+from zope.interface.interfaces import ISpecification
 from zope.schema.interfaces import IField
 
-from zope.app.apidoc.utilities import getPythonPath, renderText, getDocFormat
+from zope.app.apidoc.utilities import getDocFormat
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import renderText
 
 
 def getElements(iface, type=IElement):
     """Return a dictionary containing the elements in an interface.
 
     The type specifies whether we are looking for attributes or methods."""
     items = {}
@@ -103,41 +109,41 @@
     return getDocFormat(module)
 
 
 def getAttributeInfoDictionary(attr, format=None):
     """Return a page-template-friendly information dictionary."""
     format = format or _getDocFormat(attr)
     return {'name': attr.getName(),
-            'doc': renderText(attr.getDoc() or u'', format=format)}
+            'doc': renderText(attr.getDoc() or '', format=format)}
 
 
 def getMethodInfoDictionary(method, format=None):
     """Return a page-template-friendly information dictionary."""
     format = format or _getDocFormat(method)
     return {'name': method.getName(),
             'signature': method.getSignatureString(),
-            'doc': renderText(method.getDoc() or u'', format=format)}
+            'doc': renderText(method.getDoc() or '', format=format)}
 
 
 def getFieldInfoDictionary(field, format=None):
     """Return a page-template-friendly information dictionary."""
     format = format or _getDocFormat(field)
 
     info = {'name': field.getName(),
             'required': field.required,
-            'required_string': field.required and u'required' or u'optional',
+            'required_string': field.required and 'required' or 'optional',
             'default': repr(field.default),
             'title': field.title}
 
     # Determine the interface of the field
     iface = getFieldInterface(field)
     info['iface'] = {'name': iface.getName(), 'id': getPythonPath(iface)}
 
     # Determine the field class
     class_ = field.__class__
     info['class'] = {'name': class_.__name__,
                      'path': getPythonPath(class_).replace('.', '/')}
 
     # Render the field description
-    info['description'] = renderText(field.description or u'', format=format)
+    info['description'] = renderText(field.description or '', format=format)
 
     return info
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/interface.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/interface.rst`

 * *Files 2% similar despite different names*

```diff
@@ -212,39 +212,38 @@
 ==================================
 
 This function returns a page-template-friendly dictionary for a simple
 attribute:
 
   >>> from pprint import pprint
   >>> pprint(interface.getAttributeInfoDictionary(IFoo['baz']))
-  {'doc': u'<p>This is the baz attribute</p>\n',
+  {'doc': '<p>This is the baz attribute</p>\n',
    'name': 'baz'}
 
 
 :func:`getMethodInfoDictionary`
 ===============================
 
 This function returns a page-template-friendly dictionary for a method:
 
-  >>> pprint(interface.getMethodInfoDictionary(IFoo['blah'])) #doc
-  {'doc':
-     u'<p>This is the <cite>blah</cite> method.</p>\n',
+  >>> pprint(interface.getMethodInfoDictionary(IFoo['blah']))
+  {'doc': '<p>This is the <cite>blah</cite> method.</p>\n',
    'name': 'blah',
    'signature': '(one, two, three=None, *args, **kwargs)'}
 
 
 :func:`getFieldInfoDictionary`
 ==============================
 
 This function returns a page-template-friendly dictionary for a field:
 
   >>> pprint(interface.getFieldInfoDictionary(IFoo['bar']), width=50)
   {'class': {'name': 'TextLine',
              'path': 'zope/schema/_bootstrapfields/TextLine'},
-   'default': "u'My Bar'",
-   'description': u'<p>The Bar</p>\n',
+   'default': "'My Bar'",
+   'description': '<p>The Bar</p>\n',
    'iface': {'id': 'zope.schema.interfaces.ITextLine',
              'name': 'ITextLine'},
    'name': 'bar',
    'required': True,
-   'required_string': u'required',
-   'title': u'Bar'}
+   'required_string': 'required',
+   'title': 'Bar'}
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/interfaces.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,35 +12,36 @@
 #
 ##############################################################################
 """Generic API Documentation Interfaces
 """
 __docformat__ = 'restructuredtext'
 
 
-from zope.schema import TextLine, Text
 from zope.location.interfaces import ILocation
+from zope.schema import Text
+from zope.schema import TextLine
 
 
 class IDocumentationModule(ILocation):
     """Zope 3 API Documentation Module
 
     A documentation module contains the documentation for one specific aspect
     of the framework, such as ZCML directives or interfaces.
 
     The interface is used to register module as utilities.
     """
 
     title = TextLine(
-        title=u"Title",
-        description=u"The title of the documentation module.",
+        title="Title",
+        description="The title of the documentation module.",
         required=True)
 
     description = Text(
-        title=u"Module Description",
-        description=u"This text describes the functionality of the module.",
+        title="Module Description",
+        description="This text describes the functionality of the module.",
         required=True)
 
     def withParentAndName(parent, name):
         """
         Return a new object that is a copy of this object, but
         being located at the given parent and name.
         """
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/presentation.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/presentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Views/Presentation Utilities
 
 """
-import six
+from zope.browserresource.icon import IconViewFactory
 from zope.component import getGlobalSiteManager
-from zope.interface import Interface
-
 from zope.i18nmessageid import ZopeMessageFactory as _
-from zope.app.apidoc.utilities import getPythonPath, relativizePath
-from zope.app.apidoc.utilities import getPermissionIds
-from zope.app.apidoc.component import getParserInfoInfoDictionary
-from zope.app.apidoc.component import getInterfaceInfoDictionary
-from zope.browserresource.icon import IconViewFactory
-
+from zope.interface import Interface
 from zope.publisher.interfaces import IRequest
 from zope.publisher.interfaces.browser import IBrowserRequest
-from zope.publisher.interfaces.xmlrpc import IXMLRPCRequest
-from zope.publisher.interfaces.http import IHTTPRequest
 from zope.publisher.interfaces.ftp import IFTPRequest
+from zope.publisher.interfaces.http import IHTTPRequest
+from zope.publisher.interfaces.xmlrpc import IXMLRPCRequest
+
+from zope.app.apidoc.component import getInterfaceInfoDictionary
+from zope.app.apidoc.component import getParserInfoInfoDictionary
+from zope.app.apidoc.utilities import getPermissionIds
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import relativizePath
 
 
 SPECIFIC_INTERFACE_LEVEL = 1
 EXTENDED_INTERFACE_LEVEL = 2
 GENERIC_INTERFACE_LEVEL = 4
 
 BROWSER_DIRECTIVES_MODULE = 'zope.app.publisher.browser.viewmeta'
@@ -58,15 +57,15 @@
         # interested in. Usually the first listed class is the interesting one.
         base = factory.__bases__[0]
         info['path'] = base.__module__ + '.' + base.__name__
         info['template'] = relativizePath(factory.index.filename)
         info['template_obj'] = factory.index
 
     # Basic Type is a factory
-    elif isinstance(factory, (six.string_types, float, int, list, tuple)):
+    elif isinstance(factory, (str, float, int, list, tuple)):
         info['referencable'] = False
 
     elif factory.__module__ is not None:
         if factory.__module__.startswith(BROWSER_DIRECTIVES_MODULE):
             info['path'] = getPythonPath(factory.__bases__[0])
         # XML-RPC view factory, generated during registration
         elif (factory.__module__.startswith(XMLRPC_DIRECTIVES_MODULE)
@@ -144,22 +143,22 @@
                     yield reg
                     continue
 
 
 def getViewInfoDictionary(reg):
     """Build up an information dictionary for a view registration."""
     # get configuration info
-    if isinstance(reg.info, six.string_types):
+    if isinstance(reg.info, str):
         doc = reg.info
         zcml = None
     else:
         doc = None
         zcml = getParserInfoInfoDictionary(reg.info)
 
-    info = {'name': six.text_type(reg.name) or _('<i>no name</i>'),
+    info = {'name': str(reg.name) or _('<i>no name</i>'),
             'type': getPythonPath(getPresentationType(reg.required[-1])),
             'factory': getViewFactoryData(reg.factory),
             'required': [getInterfaceInfoDictionary(iface)
                          for iface in reg.required],
             'provided': getInterfaceInfoDictionary(reg.provided),
             'doc': doc,
             'zcml': zcml
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/presentation.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/presentation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 values will be available. Empty values are marked with ``None``.
 
 Believe it or not, in some cases the factory is just a simple type. In these
 cases we cannot retrieve any useful information:
 
   >>> info = presentation.getViewFactoryData(3)
   >>> pprint(info)
-  {'path': '__builtin__.int',
+  {'path': 'builtins.int',
    'referencable': False,
    'resource': None,
    'template': None,
    'url': None}
 
 In some cases factories are callable class instances, where we cannot directly
 have a referencable name, so we lookup the class and use its name:
@@ -266,25 +266,25 @@
 Now let's see what we've got. If we do not specify a type, all registrations
 should be returned:
 
   >>> regs = list(presentation.getViews(IFoo))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IBrowserRequest], Interface, 'blah', None, u''),
+                       [IFoo, IBrowserRequest], Interface, 'blah', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [IFoo, IHTTPRequest], Interface, 'foo', None, u''),
+                       [IFoo, IHTTPRequest], Interface, 'foo', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                       [Interface, IHTTPRequest], Interface, 'bar', None, u'')]
+                       [Interface, IHTTPRequest], Interface, 'bar', None, '')]
 
   >>> regs = list(presentation.getViews(Interface, IHTTPRequest))
   >>> regs.sort()
   >>> regs
   [AdapterRegistration(<BaseGlobalComponents base>,
-                       [Interface, IHTTPRequest], Interface, 'bar', None, u'')]
+                       [Interface, IHTTPRequest], Interface, 'bar', None, '')]
 
 
 :func:`filterViewRegistrations`
 ===============================
 
 Oftentimes the amount of views that are being returned for a particular
 interface are too much to show at once. It is then good to split the view into
@@ -329,56 +329,56 @@
 Let's now filter those registrations:
 
   >>> result = list(presentation.filterViewRegistrations(
   ...     regs, IFile, level=presentation.SPECIFIC_INTERFACE_LEVEL))
   >>> result.sort()
   >>> result
   [AdapterRegistration(<BaseGlobalComponents base>,
-                     [IFile, IHTTPRequest], Interface, 'view.html', None, u'')]
+                     [IFile, IHTTPRequest], Interface, 'view.html', None, '')]
 
   >>> result = list(presentation.filterViewRegistrations(
   ...     regs, IFile, level=presentation.EXTENDED_INTERFACE_LEVEL))
   >>> result.sort()
   >>> result
   [AdapterRegistration(<BaseGlobalComponents base>,
-                  [IContent, IHTTPRequest], Interface, 'edit.html', None, u''),
+                  [IContent, IHTTPRequest], Interface, 'edit.html', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                  [IContent, IHTTPRequest], Interface, 'view.html', None, u'')]
+                  [IContent, IHTTPRequest], Interface, 'view.html', None, '')]
 
   >>> result = list(presentation.filterViewRegistrations(
   ...     regs, IFile, level=presentation.GENERIC_INTERFACE_LEVEL))
   >>> result.sort()
   >>> result
   [AdapterRegistration(<BaseGlobalComponents base>,
-                 [Interface, IHTTPRequest], Interface, 'view.html', None, u'')]
+                 [Interface, IHTTPRequest], Interface, 'view.html', None, '')]
 
 You can also specify multiple levels at once using the Boolean OR operator,
 since all three levels are mutually exclusive.
 
   >>> result = list(presentation.filterViewRegistrations(
   ...     regs, IFile, level=presentation.SPECIFIC_INTERFACE_LEVEL |
   ...                        presentation.EXTENDED_INTERFACE_LEVEL))
   >>> result.sort()
   >>> result
   [AdapterRegistration(<BaseGlobalComponents base>,
-                  [IContent, IHTTPRequest], Interface, 'edit.html', None, u''),
+                  [IContent, IHTTPRequest], Interface, 'edit.html', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                  [IContent, IHTTPRequest], Interface, 'view.html', None, u''),
+                  [IContent, IHTTPRequest], Interface, 'view.html', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                  [IFile, IHTTPRequest], Interface, 'view.html', None, u'')]
+                  [IFile, IHTTPRequest], Interface, 'view.html', None, '')]
 
   >>> result = list(presentation.filterViewRegistrations(
   ...     regs, IFile, level=presentation.SPECIFIC_INTERFACE_LEVEL |
   ...                        presentation.GENERIC_INTERFACE_LEVEL))
   >>> result.sort()
   >>> result
   [AdapterRegistration(<BaseGlobalComponents base>,
-                [IFile, IHTTPRequest], Interface, 'view.html', None, u''),
+                [IFile, IHTTPRequest], Interface, 'view.html', None, ''),
    AdapterRegistration(<BaseGlobalComponents base>,
-                [Interface, IHTTPRequest], Interface, 'view.html', None, u'')]
+                [Interface, IHTTPRequest], Interface, 'view.html', None, '')]
 
 
 :func:`getViewInfoDictionary`
 =============================
 
 Now that we have all these utilities to select the registrations, we need to
 prepare the them for output. For page templates the best data structures are
@@ -394,15 +394,15 @@
   >>> pprint(presentation.getViewInfoDictionary(reg), width=50)
   {'doc': 'reg info',
    'factory': {'path': 'zope.app.apidoc.doctest.Factory',
                'referencable': True,
                'resource': None,
                'template': None,
                'url': 'zope/app/apidoc/doctest/Factory'},
-   'name': u'view.html',
+   'name': 'view.html',
    'provided': {'module': 'zope.interface',
                 'name': 'Interface'},
    'read_perm': None,
    'required': [{'module': 'zope.app.apidoc.doctest',
                  'name': 'IFile'},
                 {'module': 'zope.interface',
                  'name': 'Interface'},
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/static.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 ##############################################################################
 """Retrieve Static APIDOC
 
 
 """
 __docformat__ = "reStructuredText"
 
+import argparse
 import base64
 import os
 import os.path
 import sys
 import time
-import argparse
-from six.moves.urllib import error as urllib2
-from six.moves.urllib import parse as urlparse
-
 import warnings
+from urllib import error as urllib2
+from urllib import parse as urlparse
 
 import zope.testbrowser.browser
 import zope.testbrowser.wsgi
 
-
 from zope.app.apidoc import classregistry
 
+
 VERBOSITY_MAP = {1: 'ERROR', 2: 'WARNING', 3: 'INFO'}
 
 # A mapping of HTML elements that can contain links to the attribute that
 # actually contains the link, with the exception of standard <a> tags.
 urltags = {
     "area": "href",
     "base": "href",
@@ -88,15 +87,15 @@
         url += '/index.html'
 
     fragments = list(urlparse.urlparse(url))
     fragments[2] = os.path.normpath(fragments[2])
     return urlparse.urlunparse(fragments)
 
 
-class Link(object):
+class Link:
     """A link in the page."""
 
     def __init__(self, url, rootURL, referenceURL='None'):
         self.rootURL = rootURL
         self.referenceURL = referenceURL
         self.originalURL = url
 
@@ -153,15 +152,15 @@
 
     old_appsetup_context = None
     target_package = None
     zcml_file = 'configure.zcml'
 
     def setUserAndPassword(self, user, pw):
         """Specify the username and password to use for the retrieval."""
-        self.addHeader('Authorization', 'Basic %s:%s' % (user, pw))
+        self.addHeader('Authorization', 'Basic {}:{}'.format(user, pw))
 
     @classmethod
     def begin(cls):
         from zope.app.appsetup import appsetup
 
         if cls.target_package:
             import importlib
@@ -185,41 +184,42 @@
         # Fix up path for tests.
         self.old_appsetup_context = appsetup.getConfigContext()
         setattr(appsetup, '__config_context', APIDocLayer.context)
 
         return self
 
     def end(self):
-        from zope.app.apidoc.testing import APIDocLayer
         from zope.app.appsetup import appsetup
+
+        from zope.app.apidoc.testing import APIDocLayer
         APIDocLayer.testTearDown()
         APIDocLayer.tearDown()
         setattr(appsetup, '__config_context', self.old_appsetup_context)
         self.old_appsetup_context = None
 
     def setDebugMode(self, debug):
         self.handleErrors = not debug
 
 
 class ArbitraryLink(zope.testbrowser.browser.Link):
 
     attr_name = 'src'
 
     def __init__(self, elem, browser, base, attr_name=None):
-        super(ArbitraryLink, self).__init__(elem, browser, base)
+        super().__init__(elem, browser, base)
         if attr_name:
             self.attr_name = attr_name
 
     @property
     def url(self):
         relurl = self._link[self.attr_name]
         return self.browser._absoluteUrl(relurl)
 
 
-class StaticAPIDocGenerator(object):
+class StaticAPIDocGenerator:
     """Static API doc Maker"""
 
     counter = 0
     linkErrors = 0
     htmlErrors = 0
     otherErrors = 0
     visited = ()
@@ -448,15 +448,15 @@
 
         # Write the data into the file
         if not isinstance(contents, bytes):
             contents = contents.encode('utf-8')
         try:
             with open(filepath, 'wb') as f:
                 f.write(contents)
-        except IOError:  # pragma: no cover
+        except OSError:  # pragma: no cover
             # The file already exists, so it is a duplicate and a bad one,
             # since the URL misses `index.hml`. ReST can produce strange URLs
             # that produce this problem, and we have little control over it.
 
             # In other words, since we don't specify to open the file
             # in exclusive creation, perhaps it refers to a
             # directory? Or the disk is getting full?
@@ -485,16 +485,17 @@
     ret_kind.add_argument(
         '--publisher',
         '-p',
         action="store_const",
         dest='ret_kind',
         const="publisher",
         default='publisher',
-        help="""Use the publisher directly to retrieve the data. The program will bring up
-        Zope 3 for you. This is the recommended option.
+        help="""Use the publisher directly to retrieve the data.
+        The program will bring up Zope 3 for you. This is the recommended
+        option.
         """)
 
     ret_kind.add_argument(
         '--custom-publisher', '-c', dest='ret_kind',
         help="""Use the publisher directly to retrieve the data and specify
         a custom ZCML file to load in the form of the.package[:the_file.zcml].
         The package name and ZCML filename relative to the package are
@@ -576,21 +577,21 @@
     # XXX: How can this actually be turned off or disallowed?
     retrieval.add_argument(
         '--load-all',
         '-l',
         action="store_true",
         dest='import_unknown_modules',
         default=True,
-        help="""Retrieve all referenced modules, even if they have not been imported during
-        the startup process.""")
+        help="""Retrieve all referenced modules, even if they have not been
+        imported during the startup process.""")
 
     retrieval.add_argument(
         '--max-runtime', action='store', type=int, default=0,
-        help="""If given, the program will attempt to run for no longer than this
-        many seconds, terminating after the time limit and leaving
+        help="""If given, the program will attempt to run for no longer than
+        this many seconds, terminating after the time limit and leaving
         output unfinished. This is most helpful for tests."""
     )
 
     ######################################################################
     # Reporting
 
     reporting = parser.add_argument_group(
@@ -610,16 +611,16 @@
     )
 
     reporting.add_argument(
         '--debug',
         '-d',
         action="store_true",
         dest='debug',
-        help="""Run in debug mode. This will allow you to use the debugger, if the publisher
-        experienced an error.""")
+        help="""Run in debug mode. This will allow you to use the debugger,
+        if the publisher experienced an error.""")
 
     return parser
 
 # #####################################################################
 # Command-line processing
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/test.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/test.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/testing.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """zope.app.apidoc common test related classes/functions/objects.
 
 """
-import zope.app.apidoc
 from zope.app.wsgi.testlayer import BrowserLayer
 from zope.testbrowser.wsgi import TestBrowserLayer
 
+import zope.app.apidoc
+
 
 class _BrowserLayer(TestBrowserLayer, BrowserLayer):
     pass
 
 
 APIDocNoDevModeLayer = _BrowserLayer(
     zope.app.apidoc,
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,38 +10,34 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for the Interface Documentation Module
 
 """
-from zope.app.apidoc import static
 import doctest
 import os
-import re
 import sys
 import unittest
 
 import zope.app.renderer
 import zope.component.testing
 import zope.testing.module
-
 from webtest import TestApp
-
-from zope.app.apidoc.apidoc import APIDocumentation
-from zope.app.apidoc.testing import APIDocLayer
-
 from zope.app.component.testing import PlacefulSetup
 from zope.app.component.testing import setUpTraversal
-
 from zope.configuration import xmlconfig
 from zope.interface import implementer
-from zope.testing import renormalizing
 from zope.traversing.interfaces import IContainmentRoot
 
+from zope.app.apidoc import static
+from zope.app.apidoc.apidoc import APIDocumentation
+from zope.app.apidoc.testing import APIDocLayer
+
+
 _old_appsetup_context = None
 
 
 def _setUp_AppSetup(filename='configure.zcml', execute=False):
     config_file = os.path.join(
         os.path.dirname(zope.app.apidoc.__file__), filename)
 
@@ -84,21 +80,21 @@
 
 
 class BrowserTestCase(unittest.TestCase):
 
     layer = APIDocLayer
 
     def setUp(self):
-        super(BrowserTestCase, self).setUp()
+        super().setUp()
         _setUp_AppSetup()
         self._testapp = TestApp(self.layer.make_wsgi_app())
 
     def tearDown(self):
         _tearDown_AppSetup()
-        super(BrowserTestCase, self).tearDown()
+        super().tearDown()
 
     def checkForBrokenLinks(self, orig_response, path,
                             basic=None, max_links=None):
         response = self.publish(path, basic=basic)
         links = response.html.find_all('a')
 
         seen = set()
@@ -157,98 +153,60 @@
     zope.testing.module.tearDown(test, 'zope.app.apidoc.doctest')
 
 
 class TestPresentation(unittest.TestCase):
 
     def test_iconviewfactory(self):
         from zope.browserresource.icon import IconViewFactory
+
         from .presentation import getViewFactoryData
         factory = IconViewFactory('rname', 'alt', 0, 0)
 
         data = getViewFactoryData(factory)
         self.assertEqual(data['resource'], factory.rname)
 
 
 class TestUtilities(unittest.TestCase):
 
-    # All four implementations (Py2, PyPy2, Python 3, PyPy3) do different
-    # things with slot method descriptors
-    @unittest.skipIf(str is not bytes or hasattr(sys, 'pypy_version_info'),
-                     "Only on CPython2")
-    def test_slot_methods2(self):
-        from zope.app.apidoc.utilities import getFunctionSignature
-        self.assertEqual("(<unknown>)", getFunctionSignature(object.__init__))
-
-    @unittest.skipIf(str is bytes or hasattr(sys, 'pypy_version_info'),
-                     "Only on CPython3")
-    def test_slot_methods3(self):
+    # CPython and PyPy do different things with slot method descriptors
+    @unittest.skipIf(hasattr(sys, 'pypy_version_info'), "Only on CPython")
+    def test_slot_methods_cpython(self):
         from zope.app.apidoc.utilities import getFunctionSignature
         self.assertEqual(
             '(self, /, *args, **kwargs)',
             getFunctionSignature(object.__init__))
 
-    @unittest.skipIf(str is not bytes or not hasattr(sys, 'pypy_version_info'),
-                     "Only on PyPy2")
-    def test_slot_methodspypy2(self):  # pragma: no cover (no coverage on pypy)
+    @unittest.skipIf(not hasattr(sys, 'pypy_version_info'), "Only on PyPy")
+    def test_slot_methods_pypy(self):
         from zope.app.apidoc.utilities import getFunctionSignature
         self.assertEqual(
             "(obj, *args, **keywords)",
-            getFunctionSignature(
-                object.__init__))
-
-    @unittest.skipUnless(str is bytes, "Only on py2")
-    def test_unpack_methods(self):
-        from zope.app.apidoc.utilities import getFunctionSignature
-        import six
-
-        six.exec_("def f((a, b)): pass")
-
-        self.assertEqual("((a, b))", getFunctionSignature(locals()['f']))
+            getFunctionSignature(object.__init__))
 
     def test_keyword_only_arguments(self):
-        from zope.app.apidoc.utilities import getFunctionSignature
-        from zope.app.apidoc.utilities import _simpleGetFunctionSignature
         from socket import socket
 
-        try:
-            simple_sig = _simpleGetFunctionSignature(socket.makefile)
-        except ValueError:
-            # On Python 3, socket.makefile has keyword args, which aren't
-            # handled by the simple function
-            self.assertGreater(sys.version_info, (3, 0))
-            self.assertEqual(
-                "(self, mode='r', buffering=None, *, encoding=None,"
-                " errors=None, newline=None)",
-                getFunctionSignature(
-                    socket.makefile))
-            self.assertEqual(
-                "(mode='r', buffering=None, *, encoding=None, errors=None,"
-                " newline=None)",
-                getFunctionSignature(
-                    socket.makefile,
-                    ignore_self=True))
-            # Extra coverage to make sure the alternate branches are taken
-            self.assertEqual(
-                '()',
-                getFunctionSignature(self.test_keyword_only_arguments))
-            self.assertEqual(
-                '(self)',
-                # Note the difference with Python 2; this is what ignore_self
-                # is for.
-                getFunctionSignature(
-                    TestUtilities.test_keyword_only_arguments))
-        else:
-            self.assertEqual(simple_sig, "(mode='r', bufsize=-1)")
-            # Extra coverage to make sure the alternate branches are taken
-            self.assertEqual(
-                '()',
-                getFunctionSignature(self.test_keyword_only_arguments))
-            self.assertEqual(
-                '()', getFunctionSignature(
-                    TestUtilities.test_keyword_only_arguments))
+        from zope.app.apidoc.utilities import getFunctionSignature
+
+        self.assertEqual(
+            "(self, mode='r', buffering=None, *, encoding=None,"
+            " errors=None, newline=None)",
+            getFunctionSignature(socket.makefile))
+        self.assertEqual(
+            "(mode='r', buffering=None, *, encoding=None, errors=None,"
+            " newline=None)",
+            getFunctionSignature(socket.makefile, ignore_self=True))
+        # Extra coverage to make sure the alternate branches are taken
+        self.assertEqual(
+            '()',
+            getFunctionSignature(self.test_keyword_only_arguments))
+        self.assertEqual(
+            '(self)',
+            getFunctionSignature(
+                TestUtilities.test_keyword_only_arguments))
 
     def test_renderText_non_text(self):
         # If we pass something that isn't actually text, we get a
         # descriptive error back.
         from zope.app.apidoc.utilities import renderText
 
         text = renderText(self)
@@ -257,15 +215,15 @@
     def test__qualname__descriptor_path(self):
         # When the __qualname__ is not a string but a descriptor object,
         # getPythonPath does not raise an AttributeError
         # https://github.com/zopefoundation/zope.app.apidoc/issues/25
 
         from zope.app.apidoc.utilities import getPythonPath
 
-        class Obj(object):
+        class Obj:
             "namespace object"
 
         o = Obj()
         o.__qualname__ = object()
         o.__name__ = 'foo'
 
         self.assertEqual('zope.app.apidoc.tests.foo', getPythonPath(o))
@@ -278,15 +236,15 @@
         from zope.app.apidoc import utilities
 
         # Set up an object that will return itself when looked up
         # as a module attribute via patching safe_import and when
         # asked for its __class__ so we can control the __qualname__
         # on all versions of Python.
 
-        class Obj(object):
+        class Obj:
             "namespace object"
 
             def __getattribute__(self, name):
                 if name in object.__getattribute__(self, '__dict__'):
                     return object.__getattribute__(self, '__dict__')[name]
                 return self
 
@@ -303,16 +261,16 @@
         finally:
             utilities.safe_import = old_safe_import
 
 
 class TestStatic(unittest.TestCase):
 
     def _tempdir(self):
-        import tempfile
         import shutil
+        import tempfile
         tmpdir = tempfile.mkdtemp(suffix='.apidoc.TestStatic')
         self.addCleanup(shutil.rmtree, tmpdir)
         return tmpdir
 
     def test_run(self):
         tmpdir = self._tempdir()
         static.main(['--max-runtime', '10', os.path.join(tmpdir, 'dir')])
@@ -346,43 +304,43 @@
             tmpdir, 'default', '++apidoc++/ZCML/@@staticmenu.html')
         with open(path) as document:
             self.assertNotIn(directive, document.read())
 
         # Make sure that the directive is listed when we specify our custom
         # ZCML file
         static.main(['--max-runtime', '10', os.path.join(tmpdir,
-                    'custom'), '-c', '%s:%s' % (package_name, zcml_file)])
+                    'custom'), '-c', '{}:{}'.format(package_name, zcml_file)])
         path = os.path.join(
             tmpdir, 'custom', '++apidoc++/ZCML/@@staticmenu.html')
         with open(path) as document:
             self.assertIn(
                 directive,
                 document.read(),
                 "The %s directive isn't listed in zcmlmodule" %
                 directive)
 
     def test_processLink_errors(self):
         tmpdir = self._tempdir()
 
-        class ErrorBrowser(object):
+        class ErrorBrowser:
             error_kind = ValueError
             contents = ''
             isHtml = False
 
             def open(self, url):
                 raise self.error_kind(url)
 
         class ErrorGenerator(static.StaticAPIDocGenerator):
             error_kind = ValueError
 
             def processLink(self, link):
                 b = self.browser
                 self.browser = ErrorBrowser()
                 self.browser.error_kind = self.error_kind
-                super(ErrorGenerator, self).processLink(link)
+                super().processLink(link)
                 self.browser = b
 
         maker = static.main(
             ['--max-runtime', '10', os.path.join(tmpdir, 'dir')],
             generator=ErrorGenerator)
         self.assertEqual(7, maker.counter)
         self.assertEqual(7, maker.linkErrors)
@@ -441,75 +399,52 @@
             static._create_arg_parser().parse_args(
                 [tmpdir, '--webserver', '--custom-publisher', 'fake'])
 
 
 # Generally useful classes and functions
 
 @implementer(IContainmentRoot)
-class Root(object):
+class Root:
 
     __parent__ = None
     __name__ = ''
 
 
-standard_checker_patterns = (
-    (re.compile(r"u('[^']*')"), r"\1"),
-    (re.compile(r"b('[^']*')"), r"\1"),
-    (re.compile("__builtin__"), 'builtins'),
-    # repr of old style class is different on py2
-    (re.compile("<class zope.app.apidoc.doctest.B.*>"),
-     "<class 'zope.app.apidoc.doctest.B'>"),
-    # there are no unbound methods on python 3
-    (re.compile("<unbound method ([^>]*)>"),
-     r"<function \1 at 0xabc>")
-)
-
-
-def standard_checker(*extra_patterns):
-    return renormalizing.RENormalizing(
-        standard_checker_patterns + extra_patterns)
-
-
 standard_option_flags = (doctest.NORMALIZE_WHITESPACE
-                         | doctest.ELLIPSIS
-                         | renormalizing.IGNORE_EXCEPTION_MODULE_IN_PYTHON2)
+                         | doctest.ELLIPSIS)
 
 
 def LayerDocFileSuite(filename, package):
     test = doctest.DocFileSuite(
         filename,
         package=package,
         setUp=_setUp_LayerPlace,
         tearDown=_tearDown_LayerPlace,
-        checker=standard_checker(),
         optionflags=standard_option_flags)
     test.layer = APIDocLayer
     return test
 
 
 def LayerDocTestSuite(modulename):
     test = doctest.DocTestSuite(
         modulename,
         setUp=_setUp_LayerPlace,
         tearDown=_tearDown_LayerPlace,
-        checker=standard_checker(),
         optionflags=standard_option_flags)
     test.layer = APIDocLayer
     return test
 
 
 def test_suite():
-    checker = standard_checker()
 
     def file_test(name, **kwargs):
         return doctest.DocFileSuite(
             name,
             setUp=setUp,
             tearDown=tearDown,
-            checker=checker,
             optionflags=standard_option_flags,
             **kwargs)
 
     return unittest.TestSuite((
         doctest.DocTestSuite('zope.app.apidoc.browser.apidoc',
                              setUp=setUp, tearDown=tearDown),
         file_test('README.rst'),
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/browser.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Browser Views for Interface Types
 
 """
 __docformat__ = 'restructuredtext'
-from zope.app.apidoc.typemodule.type import TypeInterface
-
-from zope.security.proxy import isinstance, removeSecurityProxy
+from zope.security.proxy import isinstance
+from zope.security.proxy import removeSecurityProxy
 from zope.traversing.api import getName
+
 from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
+from zope.app.apidoc.typemodule.type import TypeInterface
 
 
-class Menu(object):
+class Menu:
     """Menu View Helper Class"""
 
     context = None
     request = None
 
     def getMenuTitle(self, node):
         """Return the title of the node that is displayed in the menu."""
@@ -36,8 +37,9 @@
             iface = node.context
         # Interfaces have no security declarations, so we have to unwrap.
         return removeSecurityProxy(iface).getName()
 
     def getMenuLink(self, node):
         """Return the HTML link of the node that is displayed in the menu."""
         root_url = findAPIDocumentationRootURL(self.context, self.request)
-        return '%s/Interface/%s/index.html' % (root_url, getName(node.context))
+        return '{}/Interface/{}/index.html'.format(
+            root_url, getName(node.context))
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for the Book Documentation Module
 
 """
 
-import unittest
 import doctest
+import unittest
 
 from zope.component import testing
 
+from zope.app.apidoc.testing import APIDocLayer
 from zope.app.apidoc.tests import BrowserTestCase
-from zope.app.apidoc.tests import standard_checker
 from zope.app.apidoc.tests import standard_option_flags
-from zope.app.apidoc.testing import APIDocLayer
 
 
 class TypeModuleTests(BrowserTestCase):
     """Just a couple of tests ensuring that the templates render."""
 
     layer = APIDocLayer
 
@@ -39,18 +38,15 @@
         body = response.getBody()
         self.assertIn('IBrowserSkinType', body)
         self.checkForBrokenLinks(body, '/++apidoc++/Type/@@menu.html',
                                  basic='mgr:mgrpw')
 
 
 def test_suite():
-    checker = standard_checker()
-
     return unittest.TestSuite((
         doctest.DocTestSuite(
             'zope.app.apidoc.typemodule.type',
             setUp=testing.setUp,
             tearDown=testing.tearDown,
-            checker=checker,
             optionflags=standard_option_flags),
         unittest.defaultTestLoader.loadTestsFromName(__name__),
     ))
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/typemodule/type.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/typemodule/type.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 #
 ##############################################################################
 """Interface Types Documentation Module
 
 """
 __docformat__ = 'restructuredtext'
 
-from zope.interface import implementer
-from zope.component import queryUtility, getUtilitiesFor
+from zope.component import getUtilitiesFor
+from zope.component import queryUtility
 from zope.i18nmessageid import ZopeMessageFactory as _
+from zope.interface import implementer
 from zope.interface.interfaces import IInterface
 from zope.location import LocationProxy
 from zope.location.interfaces import ILocation
 
 from zope.app.apidoc.interfaces import IDocumentationModule
 from zope.app.apidoc.utilities import DocumentationModuleBase
 from zope.app.apidoc.utilities import ReadContainerBase
@@ -46,15 +47,15 @@
       >>> typeiface.interface
       <InterfaceClass zope.app.apidoc.typemodule.type.IFoo>
 
       >>> typeiface.get('Foo').__class__
       <class 'zope.interface.interface.InterfaceClass'>
 
       >>> typeiface.items()
-      [(u'Foo', <InterfaceClass zope.app.apidoc.typemodule.type.IDerivedFoo>)]
+      [('Foo', <InterfaceClass zope.app.apidoc.typemodule.type.IDerivedFoo>)]
 
     """
 
     def __init__(self, interface, parent, name):
         self.__parent__ = parent
         self.__name__ = name
         self.interface = interface
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilities.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,34 +12,37 @@
 #
 ##############################################################################
 """Utilties to make the life of Documentation Modules easier.
 
 """
 __docformat__ = 'restructuredtext'
 
+import inspect
+import os.path
 import re
 import sys
 import types
-import inspect
-import os.path
-
-import six
 
-from zope.component import createObject, getMultiAdapter
-from zope.interface import implementer, implementedBy
+import zope.i18nmessageid
+from zope.component import createObject
+from zope.component import getMultiAdapter
+from zope.container.interfaces import IReadContainer
+from zope.interface import implementedBy
+from zope.interface import implementer
 from zope.publisher.browser import TestRequest
-from zope.security.checker import getCheckerForInstancesOf, Global
+from zope.security.checker import Global
+from zope.security.checker import getCheckerForInstancesOf
 from zope.security.interfaces import INameBasedChecker
-from zope.security.proxy import isinstance, removeSecurityProxy
+from zope.security.proxy import isinstance
+from zope.security.proxy import removeSecurityProxy
 
 import zope.app
-import zope.i18nmessageid
-from zope.container.interfaces import IReadContainer
+from zope.app.apidoc.classregistry import IGNORE_MODULES
+from zope.app.apidoc.classregistry import safe_import
 
-from zope.app.apidoc.classregistry import safe_import, IGNORE_MODULES
 
 _ = zope.i18nmessageid.MessageFactory("zope")
 
 _remove_html_overhead = re.compile(
     r'(?sm)^<html.*<body.*?>\n(.*)</body>\n</html>\n')
 
 space_re = re.compile(r'\n^( *)\S', re.M)
@@ -64,25 +67,25 @@
         return path
     longest_matching_path = max(matching_paths, key=len)
     common_prefix = os.path.commonprefix([longest_matching_path, path])
     return path.replace(common_prefix, '')[1:] if common_prefix else path
 
 
 @implementer(IReadContainer)
-class ReadContainerBase(object):
+class ReadContainerBase:
     """Base for :class:`zope.container.interfaces.IReadContainer` objects."""
 
     __parent__ = None
     __name__ = None
 
     def __repr__(self):
         if self.__name__ is None:
-            return super(ReadContainerBase, self).__repr__()
+            return super().__repr__()
         c = type(self)
-        return "<%s.%s '%s' at 0x%x>" % (
+        return "<{}.{} '{}' at 0x{:x}>".format(
             c.__module__, c.__name__, self.__name__, id(self))
 
     def get(self, key, default=None):
         raise NotImplementedError()
 
     def items(self):
         raise NotImplementedError()
@@ -126,36 +129,29 @@
 
     This method should try very hard to return a string, even if it is not a
     valid Python path.
     """
     if obj is None:
         return None
 
-    # Even for methods `im_class` and `__module__` is not allowed to be
+    # Even methods like `__module__` are not allowed to be
     # accessed (which is probably not a bad idea). So, we remove the security
     # proxies for this check.
     naked = removeSecurityProxy(obj)
     qname = ''
     if isinstance(getattr(naked, '__qualname__', None), str):
-        # Python 3 (being sure to protect against non-str __qualname__
-        # that we could get on some versions of Cython. See
-        # https://github.com/zopefoundation/zope.app.apidoc/issues/25).
-        # This makes unbound functions inside classes do the same
-        # thing as they do an Python 2: return just their class name.
+        # Return just the class name, if `__qualname__` is a string:
         qname = naked.__qualname__
         qname = qname.split('.')[0]
-    if hasattr(naked, 'im_class'):
-        # Python 2, unbound methods
-        naked = naked.im_class
     if isinstance(naked, types.MethodType):
         naked = type(naked.__self__)
     module = getattr(naked, '__module__', _marker)
     if module is _marker:
         return naked.__name__
-    return '%s.%s' % (module, qname or naked.__name__)
+    return '{}.{}'.format(module, qname or naked.__name__)
 
 
 def isReferencable(path):
     """Return whether the Python path is referencable."""
     # Sometimes no path exists, so make a simple check first; example: None
     if path is None:
         return False
@@ -224,86 +220,22 @@
 def _checkFunctionType(func):
     if not callable(func):
         raise TypeError(
             "func must be a function or method not a %s (%r)" %
             (type(func), func))
 
 
-def _simpleGetFunctionSignature(func, ignore_self=False):
-    """Return the signature of a function or method."""
-    _checkFunctionType(func)
-
-    try:
-        args, varargs, varkw, defaults = inspect.getargspec(func)
-    except TypeError:
-        # On Python 2, inspect.getargspec can't handle certain types
-        # of callable things, like object.__init__ (<slot wrapper '__init__'>
-        # is not a python function), but it *can* handle them on Python 3.
-        # Punt on Python 2
-        return '(<unknown>)'
-
-    placeholder = object()
-    sig = '('
-    # By filling up the default tuple, we now have equal indeces for args and
-    # default.
-    if defaults is not None:
-        defaults = (placeholder,) * (len(args) - len(defaults)) + defaults
-    else:
-        defaults = (placeholder,) * len(args)
-
-    str_args = []
-
-    for name, default in zip(args, defaults):
-        # Neglect self, since it is always there and not part of the signature.
-        # This way the implementation and interface signatures should match.
-        if name == 'self' and (
-            isinstance(
-                func,
-                types.MethodType) or ignore_self):
-            # NOTE: this is actually covered, and removing the condition will
-            # break tests. The coverage report doesn't show it, though, for
-            # some reason.
-            continue  # pragma: no cover
-
-        # Make sure the name is a string
-        if isinstance(name, (tuple, list)):
-            name = '(' + ', '.join(name) + ')'
-        elif not isinstance(name, str):  # pragma: no cover
-            name = repr(name)
-
-        if default is placeholder:
-            str_args.append(name)
-        else:
-            str_args.append(name + '=' + repr(default))
-
-    if varargs:
-        str_args.append('*' + varargs)
-    if varkw:
-        str_args.append('**' + varkw)
-
-    sig += ', '.join(str_args)
-    return sig + ')'
-
-
-def _py33GetFunctionSignature(func, ignore_self=False):
+def getFunctionSignature(func, ignore_self=False):
     _checkFunctionType(func)
     result = str(inspect.signature(func))
     if ignore_self and result.startswith("(self"):
         result = result.replace("(self)", "()").replace("(self, ", '(')
     return result
 
 
-try:
-    inspect.signature
-except AttributeError:
-    getFunctionSignature = _simpleGetFunctionSignature
-else:
-    getFunctionSignature = _py33GetFunctionSignature
-
-
 def getPublicAttributes(obj):
     """Return a list of public attribute names."""
     attrs = []
     for attr in dir(obj):
         if attr.startswith('_'):
             continue
 
@@ -388,18 +320,18 @@
     dedent = min([len(match) for match in space_re.findall(text)] or [0])
     return re.compile('\n {%i}' % dedent, re.M).sub('\n', text)
 
 
 def renderText(text, module=None, format=None, dedent=True):
     # dedent is ignored, we always dedent
     if not text:
-        return u''
+        return ''
 
     if module is not None:
-        if isinstance(module, six.string_types):
+        if isinstance(module, str):
             module = sys.modules.get(module, None)
         if format is None:
             format = getDocFormat(module)
 
     if format is None:
         format = 'zope.source.rest'
 
@@ -407,13 +339,13 @@
 
     if isinstance(text, bytes):
         text = text.decode('utf-8', 'replace')
 
     try:
         text = dedentString(text)
     except TypeError as e:
-        return u'Failed to render non-text (%r): %s' % (text, e,)
+        return 'Failed to render non-text ({!r}): {}'.format(text, e)
 
     source = createObject(format, text)
 
     renderer = getMultiAdapter((source, TestRequest()))
     return renderer.render()
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilities.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilities.rst`

 * *Files 2% similar despite different names*

```diff
@@ -167,18 +167,15 @@
   >>> class Sample(object):
   ...     def sample(self):
   ...         pass
 
   >>> utilities.getPythonPath(Sample)
   'zope.app.apidoc.doctest.Sample'
 
-If a method is passed in, its class path is returned. This works for
-both bound and unbound methods (note that there is no such thing as an
-unbound method in Python 3, just functions, but we still get the same
-results):
+If a method is passed in, its class path is returned:
 
   >>> utilities.getPythonPath(Sample().sample)
   'zope.app.apidoc.doctest.Sample'
   >>> utilities.getPythonPath(Sample.sample)
   'zope.app.apidoc.doctest.Sample'
 
 Plain functions are also supported:
@@ -403,17 +400,15 @@
   >>> def func(**kw):
   ...     pass
   >>> utilities.getFunctionSignature(func)
   '(**kw)'
 
 Next we test whether the signature is correctly determined for class
 methods. Note that the ``self`` argument is removed from the signature, since it
-is not essential for documentation; this happens by default on Python
-2 for unbound methods, but since Python 3 doesn't have such a concept
-we have to explicitly ask for that behaviour:
+is not essential for documentation:
 
 We start out with a simple positional argument:
 
   >>> class Klass(object):
   ...     def func(self, attr):
   ...         pass
   >>> utilities.getFunctionSignature(Klass.func, ignore_self=True)
@@ -435,30 +430,14 @@
 If you do not pass a function or method to the function, it will fail:
 
   >>> utilities.getFunctionSignature('func')
   Traceback (most recent call last):
   ...
   TypeError: func must be a function or method not a ...
 
-A very uncommon, but perfectly valid (in Python 2), case is that tuple arguments are
-unpacked inside the argument list of the function. Here is an example
-(we can't actually test it because it fails on Python 3)::
-
-  def func((arg1, arg2)):
-       pass
-  utilities.getFunctionSignature(func)
-  '((arg1, arg2))'
-
-Even default assignment is allowed::
-
-  def func((arg1, arg2)=(1, 2)):
-       pass
-  utilities.getFunctionSignature(func)
-  '((arg1, arg2)=(1, 2))'
-
 However, lists of this type are not allowed inside the argument list::
 
   >>> def func([arg1, arg2]):
   ...     pass
   Traceback (most recent call last):
   ...
   SyntaxError: invalid syntax...
@@ -761,20 +740,20 @@
 If the ``module`` argument is specified, the function will try to determine the
 format using the module. If the ``format`` argument is given, it is simply
 used. Clearly, you cannot specify both, the ``module`` and ``format`` argument.
 
 You specify the format as follows:
 
   >>> utilities.renderText(u'Hello!\n', format='zope.source.rest')
-  u'<p>Hello!</p>\n'
+  '<p>Hello!</p>\n'
 
 Note that the format string must be a valid source factory id; if the factory
 id is not given, 'zope.source.stx' is used. Thus, specifying the module is
 often safer (if available):
 
   >>> utilities.renderText(u'Hello!\n', module=apidoc)
-  u'<p>Hello!</p>\n'
+  '<p>Hello!</p>\n'
 
 Byte input is accepted, so long as it can be decoded:
 
   >>> utilities.renderText(b'Hello!\n', module=apidoc)
-  u'<p>Hello!</p>\n'
+  '<p>Hello!</p>\n'
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/README.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -76,16 +76,16 @@
   >>> ut_iface.get('foo') is None
   True
 
 You can get a list of available utilities as well, of course:
 
   >>> ut_iface.items()
   [...
-   (b'VXRpbGl0eQ==', <...apidoc.utilitymodule.utilitymodule.Utility ...>),
-   (b'X19ub25hbWVfXw==', <...apidoc.utilitymodule.utilitymodule.Utility ...>)]
+   ('VXRpbGl0eQ==', <...apidoc.utilitymodule.utilitymodule.Utility ...>),
+   ('X19ub25hbWVfXw==', <...apidoc.utilitymodule.utilitymodule.Utility ...>)]
 
 Bu what are those strange names? Since utility names can be any string, it is
 hard to deal with them in a URL. Thus the system will advertise and use the
 names in their ``BASE64`` encoded form. However, because it is easier in the
 Python API to use the real utility names, utilities can be looked up in their
 original form as well.
 
@@ -97,19 +97,19 @@
 
   >>> from zope.app.apidoc.utilitymodule.utilitymodule import encodeName
   >>> from zope.app.apidoc.utilitymodule.utilitymodule import decodeName
 
 Round trips of :func:`encoding <encodeName>` and :func:`decoding
 <decodeName>` should be possible:
 
-  >>> encoded = encodeName(u'Some Utility')
+  >>> encoded = encodeName('Some Utility')
   >>> encoded
-  b'U29tZSBVdGlsaXR5'
+  'U29tZSBVdGlsaXR5'
 
   >>> decodeName(encoded)
-  u'Some Utility'
+  'Some Utility'
 
 If a string is not encoded, the decoding process will simply return the
 original string:
 
-  >>> decodeName(u'Some Utility')
-  u'Some Utility'
+  >>> decodeName('Some Utility')
+  'Some Utility'
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/browser.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 #
 ##############################################################################
 """Utility Module Views
 
 """
 __docformat__ = 'restructuredtext'
 
-from zope.security.proxy import isinstance, removeSecurityProxy
 from zope.location import LocationProxy
-from zope.traversing.api import getName, getParent
+from zope.security.proxy import isinstance
+from zope.security.proxy import removeSecurityProxy
+from zope.traversing.api import getName
+from zope.traversing.api import getParent
 
-from zope.app.apidoc.ifacemodule.browser import InterfaceDetails
+from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
 from zope.app.apidoc.component import getUtilityInfoDictionary
+from zope.app.apidoc.ifacemodule.browser import InterfaceDetails
 from zope.app.apidoc.utilities import getPythonPath
-from zope.app.apidoc.utilitymodule.utilitymodule import NONAME, Utility
+from zope.app.apidoc.utilitymodule.utilitymodule import NONAME
+from zope.app.apidoc.utilitymodule.utilitymodule import Utility
 from zope.app.apidoc.utilitymodule.utilitymodule import UtilityInterface
-from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
 
 
-class UtilityDetails(object):
+class UtilityDetails:
     """Utility Details View."""
 
     context = None
     request = None
 
     def getAPIDocRootURL(self):
         return findAPIDocumentationRootURL(self.context, self.request)
@@ -56,15 +59,15 @@
         """Return the python path of the implementation class."""
         # Remove proxy here, so that we can determine the type correctly
         naked = removeSecurityProxy(self.context.registration)
         result = getUtilityInfoDictionary(naked)
         return {'path': result['path'], 'url': result['url']}
 
 
-class Menu(object):
+class Menu:
     """Menu View Helper Class"""
 
     context = None
     request = None
 
     def getMenuTitle(self, node):
         """Return the title of the node that is displayed in the menu."""
@@ -77,11 +80,12 @@
 
     def getMenuLink(self, node):
         """Return the HTML link of the node that is displayed in the menu."""
         obj = node.context
         apidoc_url = findAPIDocumentationRootURL(self.context, self.request)
         if isinstance(obj, Utility):
             iface = getParent(obj)
-            return '%s/Utility/%s/%s/index.html' % (
+            return '{}/Utility/{}/{}/index.html'.format(
                 apidoc_url, getName(iface), getName(obj))
         if isinstance(obj, UtilityInterface):
-            return '%s/Interface/%s/index.html' % (apidoc_url, getName(obj))
+            return '{}/Interface/{}/index.html'.format(
+                apidoc_url, getName(obj))
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/browser.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/browser.rst`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
   >>> details.request = None
 
 Now that we have the details view, we can look up the interface's detail view
 and get the id (for example):
 
   >>> iface = details.getInterface()
   >>> iface.getId()
-  '__builtin__.IBlah'
+  'builtins.IBlah'
 
 
 :meth:`UtilityDetails.getComponent`
 -----------------------------------
 
 Return the Python path and a code browser URL path of the implementation
 class.
@@ -158,8 +158,8 @@
   >>> details = UtilityDetails()
   >>> details.context = Utility(Interface, foo_reg)
 
 Now we can get the component information:
 
   >>> from pprint import pprint
   >>> pprint(details.getComponent(), width=1)
-  {'path': '__builtin__.Foo', 'url': None}
+  {'path': 'builtins.Foo', 'url': None}
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 
 """
 
 import unittest
 
 import zope.deprecation
 
+import zope.app.apidoc.utilitymodule
 from zope.app.apidoc.testing import APIDocLayer
-
 from zope.app.apidoc.tests import BrowserTestCase
 from zope.app.apidoc.tests import LayerDocFileSuite
-import zope.app.apidoc.utilitymodule
 
 
 class UtilityModuleTests(BrowserTestCase):
     """Just a couple of tests ensuring that the templates render."""
 
     layer = APIDocLayer
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/utilitymodule/utilitymodule.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/utilitymodule/utilitymodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 """
 __docformat__ = 'restructuredtext'
 
 import base64
 import binascii
 
 import zope.component
-
+from zope.i18nmessageid import ZopeMessageFactory as _
 from zope.interface import implementer
 from zope.location.interfaces import ILocation
 
-from zope.i18nmessageid import ZopeMessageFactory as _
 from zope.app.apidoc.interfaces import IDocumentationModule
-from zope.app.apidoc.utilities import ReadContainerBase, getPythonPath
 from zope.app.apidoc.utilities import DocumentationModuleBase
+from zope.app.apidoc.utilities import ReadContainerBase
+from zope.app.apidoc.utilities import getPythonPath
+
 
 # Constant used when the utility has no name
 NONAME = '__noname__'
 
 
 def encodeName(name):
     """Encode the name in URL safe base 64."""
@@ -52,15 +53,15 @@
         return base64.urlsafe_b64decode(to_decode).decode('utf-8')
     except (binascii.Error, TypeError):
         # Someone probably passed a non-encoded name, so let's accept that.
         return name
 
 
 @implementer(ILocation)
-class Utility(object):
+class Utility:
     """Representation of a utility for the API Documentation"""
 
     def __init__(self, parent, reg):
         """Initialize Utility object."""
         self.__parent__ = parent
         self.__name__ = encodeName(reg.name or NONAME)
         self.name = reg.name or NONAME
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/README.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/README.rst`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/__init__.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,28 @@
 The ZCML documentation module reads all of the meta directives (but does not
 execute them) and uses the collected data to generate the tree. The result of
 the evaluation is stored in thread-global variables, so that we have to parse
 the files only once.
 
 """
 from zope.testing.cleanup import addCleanUp
+
+
 __docformat__ = 'restructuredtext'
 
+import zope.app.appsetup.appsetup
 from zope.configuration import docutils
 from zope.i18nmessageid import ZopeMessageFactory as _
 from zope.interface import implementer
 from zope.location.interfaces import ILocation
 
-import zope.app.appsetup.appsetup
 from zope.app.apidoc.interfaces import IDocumentationModule
-from zope.app.apidoc.utilities import ReadContainerBase
 from zope.app.apidoc.utilities import DocumentationModuleBase
+from zope.app.apidoc.utilities import ReadContainerBase
+
 
 # Caching variables, so that the meta-ZCML files need to be read only once
 namespaces = None
 subdirs = None
 
 
 def quoteNS(ns):
@@ -88,21 +91,21 @@
         schema, handler, info = namespaces[ns][key]
         sd = subdirs.get((ns, key), [])
         directive = Directive(self, key, schema, handler, info, sd)
         return directive
 
     def items(self):
         _makeDocStructure()
-        return sorted(((key, self.get(key))
-                       for key
-                       in namespaces[self.getFullName()].keys()))
+        return sorted((key, self.get(key))
+                      for key
+                      in namespaces[self.getFullName()].keys())
 
 
 @implementer(ILocation)
-class Directive(object):
+class Directive:
     """Represents a ZCML Directive."""
 
     def __init__(self, ns, name, schema, handler, info, subdirs):
         self.__parent__ = ns
         self.__name__ = name
         self.schema = schema
         self.handler = handler
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/browser.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/browser.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Browser Views for ZCML Reference
 
 """
 __docformat__ = 'restructuredtext'
-import six
 import keyword
 
 from zope.configuration.xmlconfig import ParserInfo
-from zope.security.proxy import isinstance, removeSecurityProxy
 from zope.location import LocationProxy
-from zope.traversing.api import getName, getParent
+from zope.security.proxy import isinstance
+from zope.security.proxy import removeSecurityProxy
+from zope.traversing.api import getName
+from zope.traversing.api import getParent
 
-from zope.app.apidoc.zcmlmodule import Directive, Namespace
+from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
 from zope.app.apidoc.ifacemodule.browser import InterfaceDetails
-from zope.app.apidoc.utilities import getPythonPath, isReferencable
+from zope.app.apidoc.utilities import getPythonPath
+from zope.app.apidoc.utilities import isReferencable
 from zope.app.apidoc.utilities import relativizePath
-from zope.app.apidoc.browser.utilities import findAPIDocumentationRootURL
+from zope.app.apidoc.zcmlmodule import Directive
+from zope.app.apidoc.zcmlmodule import Namespace
 
 
-class Menu(object):
+class Menu:
     """Menu View Helper Class"""
     context = None
     request = None
 
     def getMenuTitle(self, node):
         """Return the title of the node that is displayed in the menu."""
         obj = node.context
@@ -48,27 +51,27 @@
     def getMenuLink(self, node):
         """Return the HTML link of the node that is displayed in the menu."""
         obj = node.context
         if isinstance(obj, Directive):
             ns = getParent(obj)
             apidoc_url = findAPIDocumentationRootURL(
                 self.context, self.request)
-            return '%s/ZCML/%s/%s/index.html' % (
+            return '{}/ZCML/{}/{}/index.html'.format(
                 apidoc_url, getName(ns), getName(obj))
         return None
 
 
 def _getFieldName(field):
     name = field.getName()
     if name.endswith("_") and keyword.iskeyword(name[:-1]):
         name = name[:-1]
     return name
 
 
-class DirectiveDetails(object):
+class DirectiveDetails:
     """View class for a Directive."""
 
     context = None
     request = None
 
     def getAPIDocRootURL(self):
         return findAPIDocumentationRootURL(self.context, self.request)
@@ -103,15 +106,15 @@
                     'line': info.line,
                     'column': info.column,
                     'eline': info.eline,
                     'ecolumn': info.ecolumn}
 
     def getInfo(self):
         """Get the file where the directive was declared."""
-        if isinstance(self.context.info, six.string_types):
+        if isinstance(self.context.info, str):
             return self.context.info
         return None
 
     def getHandler(self):
         """Return information about the handler."""
         if self.context.handler is not None:
             path = getPythonPath(self.context.handler)
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/browser.rst` & `zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/browser.rst`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
   >>> iface_details = details.getSchema()
 
   >>> iface_details
   <zope.app.apidoc.ifacemodule.browser.InterfaceDetails object at ...>
 
   >>> iface_details.context
-  <InterfaceClass __builtin__.IFoo>
+  <InterfaceClass builtins.IFoo>
 
 The :meth:`DirectiveDetails._getFieldName` method of the interface details has been overridden to
 neglect trailing underscores in the field name. This is necessary, since
 Python keywords cannot be used as field names:
 
   >>> iface_details._getFieldName(IFoo['class_'])
   'class'
```

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/configure.zcml` & `zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/index.pt` & `zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/index.pt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/src/zope/app/apidoc/zcmlmodule/tests.py` & `zope.app.apidoc-5.0/src/zope/app/apidoc/zcmlmodule/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 #
 ##############################################################################
 """Tests for the ZCML Documentation Module
 
 """
 import unittest
 
+import zope.app.apidoc.zcmlmodule
 from zope.app.apidoc.testing import APIDocLayer
-
 from zope.app.apidoc.tests import BrowserTestCase
 from zope.app.apidoc.tests import LayerDocFileSuite
 
-import zope.app.apidoc.zcmlmodule
-
 
 class ZCMLModuleTests(BrowserTestCase):
     """Just a couple of tests ensuring that the templates render."""
     layer = APIDocLayer
 
     def testMenu(self):
         response = self.publish(
```

### Comparing `zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/PKG-INFO` & `zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: zope.app.apidoc
-Version: 4.3.0
+Version: 5.0
 Summary: API Documentation and Component Inspection for Zope 3
 Home-page: http://github.com/zopefoundation/zope.app.apidoc
 Author: Zope Corporation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: zope3 api documentation
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
@@ -52,14 +48,22 @@
 Documentation is available at  https://zopeappapidoc.readthedocs.io/
 
 
 =========
  CHANGES
 =========
 
+5.0 (2023-07-06)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.3.0 (2021-12-15)
 ==================
 
 - Add support for Python 3.8, 3.9 and 3.10.
 
 - Drop support for Python 3.4.
 
@@ -284,9 +288,7 @@
 - Fixed the code to at least gracefully ignore unzipped eggs. Eventually we
   want to handle eggs well.
 
 3.4.0a1 (2007-04-22)
 ====================
 
 - Initial release independent of the main Zope tree.
-
-
```

### Comparing `zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/SOURCES.txt` & `zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 doc-requirements.txt
 setup.cfg
```

### Comparing `zope.app.apidoc-4.3.0/src/zope.app.apidoc.egg-info/requires.txt` & `zope.app.apidoc-5.0/src/zope.app.apidoc.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `zope.app.apidoc-4.3.0/tox.ini` & `zope.app.apidoc-5.0/tox.ini`

 * *Files 20% similar despite different names*

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
 source = zope.app.apidoc
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

