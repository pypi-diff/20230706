# Comparing `tmp/python-dict-display-filter-1.0.0.tar.gz` & `tmp/python-dict-display-filter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dict-display-filter-1.0.0.tar", last modified: Tue Jul  4 10:03:02 2023, max compression
+gzip compressed data, was "python-dict-display-filter-1.1.0.tar", last modified: Thu Jul  6 12:52:56 2023, max compression
```

## Comparing `python-dict-display-filter-1.0.0.tar` & `python-dict-display-filter-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/LICENSE
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4365 2023-07-03 10:05:45.000000 python-dict-display-filter-1.0.0/README.md
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/pydictdisplayfilter/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    11024 2023-07-04 09:39:48.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/display_filters.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/exceptions.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/factories.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8801 2023-07-03 21:07:45.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/helpers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/models.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4265 2023-07-03 22:31:59.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7361 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/slicers.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1085 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      170 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/requires.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/top_level.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/setup.cfg
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1185 2023-07-04 10:01:31.000000 python-dict-display-filter-1.0.0/setup.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/tests/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/tests/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1753 2023-07-03 22:36:44.000000 python-dict-display-filter-1.0.0/tests/test_csv_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    12488 2023-07-04 09:44:24.000000 python-dict-display-filter-1.0.0/tests/test_dict_display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3237 2023-07-03 22:23:31.000000 python-dict-display-filter-1.0.0/tests/test_dict_display_filter_shell.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6105 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/tests/test_display_filter_parser.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1761 2023-07-03 13:37:42.000000 python-dict-display-filter-1.0.0/tests/test_json_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1762 2023-07-03 20:44:06.000000 python-dict-display-filter-1.0.0/tests/test_nmap_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/tests/test_slicers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7550 2023-07-02 14:04:11.000000 python-dict-display-filter-1.0.0/tests/test_sql_display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3911 2023-07-03 13:44:39.000000 python-dict-display-filter-1.0.0/tests/test_sqlite_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3072 2023-07-03 22:27:07.000000 python-dict-display-filter-1.0.0/tests/test_table.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.967988 python-dict-display-filter-1.1.0/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/LICENSE
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4365 2023-07-03 10:05:45.000000 python-dict-display-filter-1.1.0/README.md
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/pydictdisplayfilter/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    11102 2023-07-06 08:11:22.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/display_filters.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/exceptions.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/factories.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8801 2023-07-06 08:11:22.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/helpers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/models.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4265 2023-07-03 22:31:59.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7436 2023-07-06 07:21:25.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/slicers.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1085 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      170 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/requires.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/top_level.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-06 12:52:56.967988 python-dict-display-filter-1.1.0/setup.cfg
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1185 2023-07-06 07:40:45.000000 python-dict-display-filter-1.1.0/setup.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/tests/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/tests/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1753 2023-07-03 22:36:44.000000 python-dict-display-filter-1.1.0/tests/test_csv_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    12785 2023-07-06 08:11:22.000000 python-dict-display-filter-1.1.0/tests/test_dict_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3237 2023-07-03 22:23:31.000000 python-dict-display-filter-1.1.0/tests/test_dict_display_filter_shell.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6331 2023-07-06 07:31:59.000000 python-dict-display-filter-1.1.0/tests/test_display_filter_parser.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1761 2023-07-03 13:37:42.000000 python-dict-display-filter-1.1.0/tests/test_json_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1762 2023-07-03 20:44:06.000000 python-dict-display-filter-1.1.0/tests/test_nmap_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/tests/test_slicers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7824 2023-07-06 07:33:28.000000 python-dict-display-filter-1.1.0/tests/test_sql_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3911 2023-07-03 13:44:39.000000 python-dict-display-filter-1.1.0/tests/test_sqlite_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3072 2023-07-03 22:27:07.000000 python-dict-display-filter-1.1.0/tests/test_table.py
```

### Comparing `python-dict-display-filter-1.0.0/LICENSE` & `python-dict-display-filter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/PKG-INFO` & `python-dict-display-filter-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.1.0 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
 email: thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown Provides-Extra: test License-File:
 LICENSE
                        [python_dict_display_filter Logo]
```

### Comparing `python-dict-display-filter-1.0.0/README.md` & `python-dict-display-filter-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/__init__.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/display_filters.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/display_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,20 @@
                     result.append(expression)
             # Join list of booleans and operators and evaluate this expression (e.g. 'True or False and True').
             return bool(eval(' '.join(result)))
         except Exception as err:
             raise EvaluationError(err)
 
     def _filter_data(self, data: List, expressions: List[Union[Expression, str]]) -> List:
-        for item in data:
-            if self._evaluate_expressions(expressions, item):
-                yield item
+        if expressions:
+            for item in data:
+                if self._evaluate_expressions(expressions, item):
+                    yield item
+        else:
+            yield from data
 
     @property
     def field_names(self) -> List[str]:
         return self._field_names
 
     @field_names.setter
     def field_names(self, field_names: List[str] = None):
```

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/__init__.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/common.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/exceptions.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/factories.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/factories.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/helpers.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/helpers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/models.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/models.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/__init__.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/common.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/display_filter.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/display_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,13 +133,15 @@
         """
         Parses a display filter string.
         :param format: a display filter string. See class documentation for examples.
         :return a list of expressions and logical operators as string.
         :raises ParserError, when the given display filter could not be parsed correctly.
         """
         try:
+            if not format or not format.strip():
+                return []
             return self._display_filter_format.parseString(format, parseAll=True).asList()
         except Exception:
             # This error indicates that there is something wrong with the given display filter.
             # Especially if the given display filter is some kind of user input this error needs to be handled
             # accordingly.
             raise ParserError('Error parsing display filter!')
```

### Comparing `python-dict-display-filter-1.0.0/pydictdisplayfilter/slicers.py` & `python-dict-display-filter-1.1.0/pydictdisplayfilter/slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/PKG-INFO` & `python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.1.0 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
 email: thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown Provides-Extra: test License-File:
 LICENSE
                        [python_dict_display_filter Logo]
```

### Comparing `python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/SOURCES.txt` & `python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/setup.py` & `python-dict-display-filter-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="python-dict-display-filter",
-    version="1.0.0",
+    version="1.1.0",
     description="A Wireshark-like display filter for dictionaries.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bytebutcher/python-dict-display-filter",
     author="bytebutcher",
     author_email="thomas.engel.web@gmail.com",
     license="GPL-3.0",
```

### Comparing `python-dict-display-filter-1.0.0/tests/__init__.py` & `python-dict-display-filter-1.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/tests/test_csv_display_filter_example.py` & `python-dict-display-filter-1.1.0/tests/test_csv_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/tests/test_dict_display_filter.py` & `python-dict-display-filter-1.1.0/tests/test_dict_display_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,23 @@
         {"value": True},
         {"value": "True"},
         {"value": False},
         {"value": "False"},
     ]
 
     @parameterized.expand([
+        [None],
+        [''],
+        [' ']
+    ])
+    def test_empty_display_filter_return_all_items(self, display_filter):
+        actual_result = list(DictDisplayFilter(self.data).filter(display_filter))
+        self.assertEqual(len(actual_result), len(self.data))
+
+    @parameterized.expand([
         # Field existence
         ['name', 4],
         ['power', 1],
         ['not power', 3],
         # Comparison operators
         ['name == Neo', 1],
         ['name == \x4e\x65\x6f', 1],
```

### Comparing `python-dict-display-filter-1.0.0/tests/test_dict_display_filter_shell.py` & `python-dict-display-filter-1.1.0/tests/test_dict_display_filter_shell.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/tests/test_display_filter_parser.py` & `python-dict-display-filter-1.1.0/tests/test_display_filter_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 
 
 class TestFilterStringParser(TestCase):
     display_filter_parser = DisplayFilterParser(['address', 'port', 'protocol', 'banner'])
     generic_display_filter_parser = DisplayFilterParser()
 
     @parameterized.expand([
+        [None],
+        [''],
+        [' ']
+    ])
+    def test_empty_query_returns_empty_list(self, display_filter):
+        self.assertEqual(self.display_filter_parser.parse(display_filter), [])
+
+    @parameterized.expand([
         ['127.0.0.1'],
         ['127.0.0.1/24'],
         ['127.0.0.?'],
         ['127.*'],
         ['^asd$'],
         ['*asd*'],
         ['.asd.'],
```

### Comparing `python-dict-display-filter-1.0.0/tests/test_json_display_filter_example.py` & `python-dict-display-filter-1.1.0/tests/test_json_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/tests/test_nmap_display_filter_example.py` & `python-dict-display-filter-1.1.0/tests/test_nmap_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/tests/test_slicers.py` & `python-dict-display-filter-1.1.0/tests/test_slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/tests/test_sql_display_filter.py` & `python-dict-display-filter-1.1.0/tests/test_sql_display_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,22 @@
         connection.execute(create_table_command)
         insert_table_data_command = _build_insert_table_data_command()
         for table_data_row in table_data:
             data = tuple(table_data_row.values())
             connection.execute(insert_table_data_command, data)
 
     @parameterized.expand([
+        [None],
+        [''],
+        [' ']
+    ])
+    def test_empty_display_filter_returns_all_items(self, display_filter):
+        self.assertEqual(len(list(SQLDisplayFilter(self._connection, 'data').filter(display_filter))), len(self.data))
+
+    @parameterized.expand([
         # Field existence
         ['name', 4],
         ['power', 1],
         ['not power', 3],
         # Comparison operators
         ['name == Neo', 1],
         ['name == \x4e\x65\x6f', 1],
```

### Comparing `python-dict-display-filter-1.0.0/tests/test_sqlite_display_filter_example.py` & `python-dict-display-filter-1.1.0/tests/test_sqlite_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.0.0/tests/test_table.py` & `python-dict-display-filter-1.1.0/tests/test_table.py`

 * *Files identical despite different names*

