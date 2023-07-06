# Comparing `tmp/agrc-sweeper-1.3.5.tar.gz` & `tmp/agrc-sweeper-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/agrc-sweeper-1.3.5.tar", last modified: Mon Dec 12 16:02:17 2022, max compression
+gzip compressed data, was "agrc-sweeper-1.4.1.tar", last modified: Thu Jul  6 19:50:45 2023, max compression
```

## Comparing `agrc-sweeper-1.3.5.tar` & `agrc-sweeper-1.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2022-12-12 16:02:14.000000 agrc-sweeper-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-12 16:02:16.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 16:02:16.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-12 16:02:16.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 16:02:16.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-12 16:02:16.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-12 16:02:16.000000 agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/src/sweeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/credentials_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/street_types.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/UseLimitations.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/empties.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/invalids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/sweepers/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:17.000000 agrc-sweeper-1.3.5/src/sweeper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/tests/test_address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/tests/test_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2022-12-12 16:02:13.000000 agrc-sweeper-1.3.5/src/sweeper/workspace_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 19:50:45.000000 agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/sweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/credentials_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/street_types.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/sweeper/sweepers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/UseLimitations.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/empties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/invalids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/sweepers/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:45.583307 agrc-sweeper-1.4.1/src/sweeper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/test_address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/test_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-06 19:50:44.000000 agrc-sweeper-1.4.1/src/sweeper/workspace_info.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `agrc-sweeper-1.3.5/PKG-INFO` & `agrc-sweeper-1.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: agrc-sweeper
-Version: 1.3.5
+Version: 1.4.1
 Summary: CLI tool for making good data
 Home-page: https://github.com/agrc/sweeper
 Author: AGRC
 Author-email: agrc@utah.gov
 License: MIT
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3
-Provides-Extra: tests
 Provides-Extra: develop
+Provides-Extra: tests
+
+UNKNOWN
+
```

### Comparing `agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/PKG-INFO` & `agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: agrc-sweeper
-Version: 1.3.5
+Version: 1.4.1
 Summary: CLI tool for making good data
 Home-page: https://github.com/agrc/sweeper
 Author: AGRC
 Author-email: agrc@utah.gov
 License: MIT
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3
-Provides-Extra: tests
 Provides-Extra: develop
+Provides-Extra: tests
+
+UNKNOWN
+
```

### Comparing `agrc-sweeper-1.3.5/src/agrc_sweeper.egg-info/SOURCES.txt` & `agrc-sweeper-1.4.1/src/agrc_sweeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/__main__.py` & `agrc-sweeper-1.4.1/src/sweeper/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,21 +18,19 @@
   backup_path   - place to create a temp gdb and import original table
   field_name    - name of the field to check
 
 Examples:
   sweeper sweep           --workspace=c:\\data\\thing --try-fix --save-report=c:\\temp --backup-to=c:\\temp\\backup.gdb
   sweeper sweep addresses --workspace=c:\\data\\thing --try-fix --save-report=c:\\temp --backup-to=c:\\temp\\backup.gdb --field-name=ADDRESS
 '''
-import os
 import sys
 import datetime
 import logging
 import logging.handlers
 import pkg_resources
-from io import StringIO
 from pathlib import Path
 
 from docopt import docopt
 
 from supervisor.models import MessageDetails, Supervisor
 from supervisor.message_handlers import EmailHandler
```

### Comparing `agrc-sweeper-1.3.5/src/sweeper/address_parser.py` & `agrc-sweeper-1.4.1/src/sweeper/address_parser.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/backup.py` & `agrc-sweeper-1.4.1/src/sweeper/backup.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/credentials_template.py` & `agrc-sweeper-1.4.1/src/sweeper/credentials_template.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/report.py` & `agrc-sweeper-1.4.1/src/sweeper/report.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/street_types.json` & `agrc-sweeper-1.4.1/src/sweeper/street_types.json`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/sweepers/UseLimitations.html` & `agrc-sweeper-1.4.1/src/sweeper/sweepers/UseLimitations.html`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/sweepers/addresses.py` & `agrc-sweeper-1.4.1/src/sweeper/sweepers/addresses.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/sweepers/duplicates.py` & `agrc-sweeper-1.4.1/src/sweeper/sweepers/duplicates.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/sweepers/empties.py` & `agrc-sweeper-1.4.1/src/sweeper/sweepers/empties.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, workspace, table_name):
         self.workspace = workspace
         self.table_name = table_name
         self.oids_with_issues = []
 
 
     def sweep(self):
-        '''A method to find empty geometries and return a report dictionarty
+        '''A method to find empty geometries and return a report dictionary
         '''
         report = {'title': 'Empty Test', 'feature_class': self.table_name, 'issues': []}
         fields = ['OID@', 'SHAPE@']
 
         with arcpy.EnvManager(workspace=self.workspace):
             description = arcpy.da.Describe(self.table_name)
```

### Comparing `agrc-sweeper-1.3.5/src/sweeper/sweepers/invalids.py` & `agrc-sweeper-1.4.1/src/sweeper/sweepers/invalids.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/sweepers/metadata.py` & `agrc-sweeper-1.4.1/src/sweeper/sweepers/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from bs4 import BeautifulSoup
 import logging
 
 log = logging.getLogger('sweeper')
 
 #: these constants were copied from https://github.com/agrc/auditor/blob/master/src/auditor/auditor.py
 #: Tags or words that should be uppercased, saved as lower to check against
-UPPERCASED_TAGS = [
+UPPERCASE_TAGS = [
     '2g', '3g', '4g', 'agol', 'aog', 'at&t', 'atv', 'blm', 'brat', 'caf', 'cdl', 'dabc', 'daq', 'dem', 'dfcm', 'dfirm', 'dnr', 'dogm', 'dot', 'dsl', 'dsm',
     'dtm', 'dwq', 'e911', 'ems', 'epa', 'fae', 'fcc', 'fema', 'gcdb', 'gis', 'gnis', 'gsl', 'hava', 'huc', 'lir', 'lrs', 'lte', 'luca', 'mrrc', 'nca', 'ng911', 'ngda',
     'nox', 'npsbn', 'ntia', 'nwi', 'nws', 'osa', 'pli', 'plss', 'pm10', 'ppm', 'psap', 'sao', 'sbdc', 'sbi', 'sgid', 'sitla', 'sligp', 'trax', 'uca', 'udot', 'ugrc',
     'ugs', 'uhp', 'uic', 'uipa', 'us', 'usao', 'usdw', 'usfs', 'usfws', 'usps', 'ustc', 'ut', 'uta', 'utsc', 'vcp', 'vista', 'voc', 'wbd', 'wre'
 ]
 #: Articles that should be left lowercase.
 ARTICLES = ['a', 'the', 'of', 'is', 'in']
@@ -46,25 +46,25 @@
 def title_case_tag(tag):
     '''
     Changes a tag to the correct title case while also removing any periods:
     'U.S. bureau Of Geoinformation' -> 'US Bureau of Geoinformation'. Should
     properly upper-case any words or single tags that are acronyms:
     'ugrc' -> 'UGRC', 'Plss Fabric' -> 'PLSS Fabric'. Any words separated by
     a hyphen will also be title-cased: 'water-related' -> 'Water-Related'.
-    Note: No check is done for articles at the begining of a tag; all articles
+    Note: No check is done for articles at the beginning of a tag; all articles
     will be lowercased.
     tag:        The single or multi-word tag to check
     '''
 
     new_words = []
     for word in tag.split():
         cleaned_word = word.replace('.', '').lower()
 
         #: Upper case specified words:
-        if cleaned_word.lower() in UPPERCASED_TAGS:
+        if cleaned_word.lower() in UPPERCASE_TAGS:
             new_words.append(cleaned_word.upper())
         #: Lower case articles/conjunctions
         elif cleaned_word.lower() in ARTICLES:
             new_words.append(cleaned_word.lower())
         #: Title case everything else
         else:
             new_words.append(cleaned_word.title())
```

### Comparing `agrc-sweeper-1.3.5/src/sweeper/tests/test_address_parser.py` & `agrc-sweeper-1.4.1/src/sweeper/tests/test_address_parser.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/tests/test_metadata.py` & `agrc-sweeper-1.4.1/src/sweeper/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.3.5/src/sweeper/workspace_info.py` & `agrc-sweeper-1.4.1/src/sweeper/workspace_info.py`

 * *Files identical despite different names*

