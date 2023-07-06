# Comparing `tmp/cubicweb-folder-2.1.1.tar.gz` & `tmp/cubicweb-folder-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-folder-2.1.1.tar", last modified: Fri Nov 22 09:04:37 2019, max compression
+gzip compressed data, was "cubicweb-folder-2.2.0.tar", last modified: Thu Jul  6 14:19:56 2023, max compression
```

## Comparing `cubicweb-folder-2.1.1.tar` & `cubicweb-folder-2.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      380 2019-11-22 09:03:24.000000 cubicweb-folder-2.1.1/MANIFEST.in
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1459 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      802 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/README
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      181 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/__init__.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      709 2019-11-22 09:03:51.000000 cubicweb-folder-2.1.1/cubicweb_folder/__pkginfo__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder/data/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      383 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/data/icon_folder.gif
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      632 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/entities.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1874 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/hooks.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder/i18n/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2248 2019-03-05 11:03:16.000000 cubicweb-folder-2.1.1/cubicweb_folder/i18n/en.po
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2593 2019-03-05 11:03:20.000000 cubicweb-folder-2.1.1/cubicweb_folder/i18n/fr.po
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder/migration/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       46 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/migration/1.0.1_Any.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       73 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/migration/1.5.0_Any.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       67 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/migration/postcreate.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1168 2019-03-01 16:57:53.000000 cubicweb-folder-2.1.1/cubicweb_folder/schema.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       46 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/uiprops.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     7149 2019-03-05 08:33:09.000000 cubicweb-folder-2.1.1/cubicweb_folder/views.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder/wdoc/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      235 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/wdoc/add_folder_fr.rst
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      185 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/cubicweb_folder/wdoc/toc.xml
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1459 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      910 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       94 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       28 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       16 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/cubicweb_folder.egg-info/top_level.txt
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       65 2019-03-01 16:57:53.000000 cubicweb-folder-2.1.1/dev-requirements.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/setup.cfg
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2487 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/setup.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/test/
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-11-22 09:04:37.000000 cubicweb-folder-2.1.1/test/data/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       12 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/test/data/bootstrap_cubes
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      130 2019-03-01 16:57:33.000000 cubicweb-folder-2.1.1/test/data/schema.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      309 2019-03-01 16:57:53.000000 cubicweb-folder-2.1.1/test/test_folder.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     3577 2019-03-01 16:57:53.000000 cubicweb-folder-2.1.1/test/unittest_folder.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2734 2019-03-01 16:57:53.000000 cubicweb-folder-2.1.1/test/unittest_hooks.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      555 2019-11-22 09:02:58.000000 cubicweb-folder-2.1.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.395717 cubicweb-folder-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-07-06 14:19:56.391716 cubicweb-folder-2.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.371716 cubicweb-folder-2.2.0/cubicweb_folder/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.375716 cubicweb-folder-2.2.0/cubicweb_folder/data/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/data/icon_folder.gif
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.375716 cubicweb-folder-2.2.0/cubicweb_folder/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.379716 cubicweb-folder-2.2.0/cubicweb_folder/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/migration/1.0.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/migration/1.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)     7153 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.379716 cubicweb-folder-2.2.0/cubicweb_folder/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/wdoc/add_folder_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/cubicweb_folder/wdoc/toc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.375716 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-07-06 14:19:56.000000 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      914 2023-07-06 14:19:56.000000 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:19:56.000000 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-06 14:19:56.000000 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:19:56.000000 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-06 14:19:56.000000 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 14:19:56.000000 cubicweb-folder-2.2.0/cubicweb_folder.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:19:56.395717 cubicweb-folder-2.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2491 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.383716 cubicweb-folder-2.2.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:19:56.387716 cubicweb-folder-2.2.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/test/test_folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/test/unittest_folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2734 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2023-07-06 14:19:08.000000 cubicweb-folder-2.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-folder-2.1.1/PKG-INFO` & `cubicweb-folder-2.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-folder
-Version: 2.1.1
+Version: 2.2.0
 Summary: folder component for the CubicWeb framework
 Home-page: http://www.cubicweb.org/project/cubicweb-folder
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Description: Summary
-        -------
-        The `folder` cube allows to create a tree of categories and classify entities
-        as you're used to do in a file-system.
-        
-        Usage
-        -----
-        
-        Define the relation `filed_under` in the schema, object must
-        contain all entities which can be classified in a folder.
-        
-        .. sourcecode:: python
-        
-          class missing_filed_under(RelationDefinition):
-              name = 'filed_under'
-              subject = ('ExtProject', 'Project', 'Card', 'File')
-              object = 'Folder'
-        
-        
-        The `FoldersBox` shows the folders hierarchy as a tree view. It's not visible by
-        default (user can activate it using their preferences) but you can activate it
-        by default using the code snippet below:
-        
-        .. sourcecode:: python
-        
-            from cubicweb_folder.views import FoldersBox
-            # make the folders box visible by default
-            FoldersBox.visible = True
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
+
+Summary
+-------
+The `folder` cube allows to create a tree of categories and classify entities
+as you're used to do in a file-system.
+
+Usage
+-----
+
+Define the relation `filed_under` in the schema, object must
+contain all entities which can be classified in a folder.
+
+.. sourcecode:: python
+
+  class missing_filed_under(RelationDefinition):
+      name = 'filed_under'
+      subject = ('ExtProject', 'Project', 'Card', 'File')
+      object = 'Folder'
+
+
+The `FoldersBox` shows the folders hierarchy as a tree view. It's not visible by
+default (user can activate it using their preferences) but you can activate it
+by default using the code snippet below:
+
+.. sourcecode:: python
+
+    from cubicweb_folder.views import FoldersBox
+    # make the folders box visible by default
+    FoldersBox.visible = True
```

### Comparing `cubicweb-folder-2.1.1/README` & `cubicweb-folder-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder/__pkginfo__.py` & `cubicweb-folder-2.2.0/cubicweb_folder/__pkginfo__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pylint: disable-msg=W0622
 """cubicweb-classification-folder packaging information"""
 
 modname = 'cubicweb_folder'
 distname = "cubicweb-folder"
 
-numversion = (2, 1, 1)
+numversion = (2, 2, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = 'http://www.cubicweb.org/project/%s' % distname
 description = "folder component for the CubicWeb framework"
 classifiers = [
            'Environment :: Web Environment',
            'Framework :: CubicWeb',
            'Programming Language :: Python',
            'Programming Language :: JavaScript',
            ]
 
-__depends__ = {'cubicweb': '>= 3.26.0',
-               'six': '>= 1.4.0', }
+__depends__ = {'cubicweb': ">=3.38.0,<3.39.0",
+               'six': ">=1.16.0,<1.17.0", }
 
 __recommends__ = {}
```

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder/entities.py` & `cubicweb-folder-2.2.0/cubicweb_folder/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder/hooks.py` & `cubicweb-folder-2.2.0/cubicweb_folder/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder/i18n/en.po` & `cubicweb-folder-2.2.0/cubicweb_folder/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder/i18n/fr.po` & `cubicweb-folder-2.2.0/cubicweb_folder/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder/schema.py` & `cubicweb-folder-2.2.0/cubicweb_folder/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder/views.py` & `cubicweb-folder-2.2.0/cubicweb_folder/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 :copyright: 2003-2018 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 from six import text_type
 
 from cubicweb.utils import UStringIO
-from cubicweb.view import EntityView, EntityStartupView
+from cubicweb_web.view import EntityView, EntityStartupView
 from cubicweb.predicates import (none_rset, is_instance, relation_possible,
                                  score_entity)
-from cubicweb.web import component
-from cubicweb.web.views import primary, baseviews, uicfg
-from cubicweb.web.views.treeview import BaseTreeView
+from cubicweb_web import component
+from cubicweb_web.views import primary, baseviews, uicfg
+from cubicweb_web.views.treeview import BaseTreeView
 
 
 from cubicweb import _
 
 
 def folder_tree(req, done=None):
     """yield folder entities according to the tree structure in a depth search
```

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder.egg-info/PKG-INFO` & `cubicweb-folder-2.2.0/cubicweb_folder.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-folder
-Version: 2.1.1
+Version: 2.2.0
 Summary: folder component for the CubicWeb framework
 Home-page: http://www.cubicweb.org/project/cubicweb-folder
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Description: Summary
-        -------
-        The `folder` cube allows to create a tree of categories and classify entities
-        as you're used to do in a file-system.
-        
-        Usage
-        -----
-        
-        Define the relation `filed_under` in the schema, object must
-        contain all entities which can be classified in a folder.
-        
-        .. sourcecode:: python
-        
-          class missing_filed_under(RelationDefinition):
-              name = 'filed_under'
-              subject = ('ExtProject', 'Project', 'Card', 'File')
-              object = 'Folder'
-        
-        
-        The `FoldersBox` shows the folders hierarchy as a tree view. It's not visible by
-        default (user can activate it using their preferences) but you can activate it
-        by default using the code snippet below:
-        
-        .. sourcecode:: python
-        
-            from cubicweb_folder.views import FoldersBox
-            # make the folders box visible by default
-            FoldersBox.visible = True
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
+
+Summary
+-------
+The `folder` cube allows to create a tree of categories and classify entities
+as you're used to do in a file-system.
+
+Usage
+-----
+
+Define the relation `filed_under` in the schema, object must
+contain all entities which can be classified in a folder.
+
+.. sourcecode:: python
+
+  class missing_filed_under(RelationDefinition):
+      name = 'filed_under'
+      subject = ('ExtProject', 'Project', 'Card', 'File')
+      object = 'Folder'
+
+
+The `FoldersBox` shows the folders hierarchy as a tree view. It's not visible by
+default (user can activate it using their preferences) but you can activate it
+by default using the code snippet below:
+
+.. sourcecode:: python
+
+    from cubicweb_folder.views import FoldersBox
+    # make the folders box visible by default
+    FoldersBox.visible = True
```

### Comparing `cubicweb-folder-2.1.1/cubicweb_folder.egg-info/SOURCES.txt` & `cubicweb-folder-2.2.0/cubicweb_folder.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MANIFEST.in
-README
+README.rst
 dev-requirements.txt
 setup.py
 tox.ini
 cubicweb_folder/__init__.py
 cubicweb_folder/__pkginfo__.py
 cubicweb_folder/entities.py
 cubicweb_folder/hooks.py
```

### Comparing `cubicweb-folder-2.1.1/setup.py` & `cubicweb-folder-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 license = __pkginfo__['license']
 description = __pkginfo__['description']
 web = __pkginfo__['web']
 author = __pkginfo__['author']
 author_email = __pkginfo__['author_email']
 classifiers = __pkginfo__['classifiers']
 
-with open(join(here, 'README')) as f:
+with open(join(here, 'README.rst')) as f:
     long_description = f.read()
 
 # get optional metadatas
 dependency_links = __pkginfo__.get('dependency_links', ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
```

### Comparing `cubicweb-folder-2.1.1/test/unittest_folder.py` & `cubicweb-folder-2.2.0/test/unittest_folder.py`

 * *Files identical despite different names*

### Comparing `cubicweb-folder-2.1.1/test/unittest_hooks.py` & `cubicweb-folder-2.2.0/test/unittest_hooks.py`

 * *Files identical despite different names*

