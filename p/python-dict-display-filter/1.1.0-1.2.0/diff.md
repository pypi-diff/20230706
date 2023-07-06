# Comparing `tmp/python-dict-display-filter-1.1.0.tar.gz` & `tmp/python-dict-display-filter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dict-display-filter-1.1.0.tar", last modified: Thu Jul  6 12:52:56 2023, max compression
+gzip compressed data, was "python-dict-display-filter-1.2.0.tar", last modified: Thu Jul  6 18:15:38 2023, max compression
```

## Comparing `python-dict-display-filter-1.1.0.tar` & `python-dict-display-filter-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.967988 python-dict-display-filter-1.1.0/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/LICENSE
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4365 2023-07-03 10:05:45.000000 python-dict-display-filter-1.1.0/README.md
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/pydictdisplayfilter/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    11102 2023-07-06 08:11:22.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/display_filters.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/exceptions.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/factories.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8801 2023-07-06 08:11:22.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/helpers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/models.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4265 2023-07-03 22:31:59.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7436 2023-07-06 07:21:25.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/pydictdisplayfilter/slicers.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1085 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      170 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/requires.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-06 12:52:56.000000 python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/top_level.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-06 12:52:56.967988 python-dict-display-filter-1.1.0/setup.cfg
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1185 2023-07-06 07:40:45.000000 python-dict-display-filter-1.1.0/setup.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 12:52:56.963988 python-dict-display-filter-1.1.0/tests/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/tests/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1753 2023-07-03 22:36:44.000000 python-dict-display-filter-1.1.0/tests/test_csv_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    12785 2023-07-06 08:11:22.000000 python-dict-display-filter-1.1.0/tests/test_dict_display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3237 2023-07-03 22:23:31.000000 python-dict-display-filter-1.1.0/tests/test_dict_display_filter_shell.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6331 2023-07-06 07:31:59.000000 python-dict-display-filter-1.1.0/tests/test_display_filter_parser.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1761 2023-07-03 13:37:42.000000 python-dict-display-filter-1.1.0/tests/test_json_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1762 2023-07-03 20:44:06.000000 python-dict-display-filter-1.1.0/tests/test_nmap_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-1.1.0/tests/test_slicers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7824 2023-07-06 07:33:28.000000 python-dict-display-filter-1.1.0/tests/test_sql_display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3911 2023-07-03 13:44:39.000000 python-dict-display-filter-1.1.0/tests/test_sqlite_display_filter_example.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3072 2023-07-03 22:27:07.000000 python-dict-display-filter-1.1.0/tests/test_table.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/LICENSE
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     5896 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     5441 2023-07-06 18:10:36.000000 python-dict-display-filter-1.2.0/README.md
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/pydictdisplayfilter/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      853 2023-07-06 15:55:44.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    12305 2023-07-06 18:10:36.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/display_filters.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/pydictdisplayfilter/evaluators/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/evaluators/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/evaluators/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/exceptions.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/factories.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8801 2023-07-06 08:11:22.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/helpers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/models.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/pydictdisplayfilter/parsers/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/parsers/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4265 2023-07-03 22:31:59.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/parsers/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7436 2023-07-06 07:21:25.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/parsers/display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/pydictdisplayfilter/slicers.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     5896 2023-07-06 18:15:38.000000 python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1121 2023-07-06 18:15:38.000000 python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-06 18:15:38.000000 python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      170 2023-07-06 18:15:38.000000 python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/requires.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-06 18:15:38.000000 python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/top_level.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/setup.cfg
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1185 2023-07-06 15:21:55.000000 python-dict-display-filter-1.2.0/setup.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-06 18:15:38.914869 python-dict-display-filter-1.2.0/tests/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/tests/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1753 2023-07-03 22:36:44.000000 python-dict-display-filter-1.2.0/tests/test_csv_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    12785 2023-07-06 08:11:22.000000 python-dict-display-filter-1.2.0/tests/test_dict_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3237 2023-07-03 22:23:31.000000 python-dict-display-filter-1.2.0/tests/test_dict_display_filter_shell.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6331 2023-07-06 07:31:59.000000 python-dict-display-filter-1.2.0/tests/test_display_filter_parser.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1761 2023-07-03 13:37:42.000000 python-dict-display-filter-1.2.0/tests/test_json_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1762 2023-07-03 20:44:06.000000 python-dict-display-filter-1.2.0/tests/test_nmap_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3385 2023-07-06 15:21:35.000000 python-dict-display-filter-1.2.0/tests/test_object_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-1.2.0/tests/test_slicers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7824 2023-07-06 07:33:28.000000 python-dict-display-filter-1.2.0/tests/test_sql_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3911 2023-07-03 13:44:39.000000 python-dict-display-filter-1.2.0/tests/test_sqlite_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3072 2023-07-03 22:27:07.000000 python-dict-display-filter-1.2.0/tests/test_table.py
```

### Comparing `python-dict-display-filter-1.1.0/LICENSE` & `python-dict-display-filter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/PKG-INFO` & `python-dict-display-filter-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,111 @@
-Metadata-Version: 2.1
-Name: python-dict-display-filter
-Version: 1.1.0
-Summary: A Wireshark-like display filter for dictionaries.
-Home-page: https://github.com/bytebutcher/python-dict-display-filter
-Author: bytebutcher
-Author-email: thomas.engel.web@gmail.com
-License: GPL-3.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <p align="center">
     <img src="https://github.com/bytebutcher/python-dict-display-filter/raw/main/images/python_dict_display_filter_logo.png" alt="python_dict_display_filter Logo"/>
 </p>
 <h1 align="center" style="margin-top: 0px;">Python Dictionary Display Filter</h1>
 <div align="center">
 
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
 ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-display-filter)
 ![Coverage](https://img.shields.io/codecov/c/github/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
-A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
-manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
-combining operators, membership operators, and more. 
+A Wireshark-like display filter for Python dictionaries and various other data 
+sources, including objects, lists, and SQL databases. 
 
 ## Table of Contents
 1. [Quick Start](#quick-start)
 2. [Features](#features)
 3. [Examples](#examples)
 4. [Acknowledgements](#acknowledgements)
 
 ## Quick Start
 
-Here's a simple example to get you started. First, install the package:
+To quickly get started with the python-dictionary-display-filter, follow the steps below:
+
+### Installation
+First, install the package using pip:
 
 ```commandline
 pip3 install python-dict-display-filter
 ```
 
-Then, use it to filter a list of dictionaries:
-```
+### Initialization
+Next, import the necessary module and initialize the ```DictDisplayFilter``` with a list of dictionaries:
+```python
 from pydictdisplayfilter import DictDisplayFilter
+
 actors = [
     {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
     {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
     {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"}, "gender": "male"},
     {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
 ]
+
 ddf = DictDisplayFilter(actors)
+```
+
+### Filtering Data
+Once the ```DictDisplayFilter``` is initialized, you can start filtering the data using the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#4-query-language">display filter query language</a>.
+For example, let's filter the actors whose birth year is after 1960:
+```python
+filter_query = "age.born > 1960"
+filtered_data = ddf.filter(filter_query)
+print(list(filtered_data))
+[
+    {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
+    {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
+    {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
+]
+```
+
+You can also use more complex queries to filter the data. 
+For example, let's filter male actors born between 1960 and 1964 whose names end with "e":
 
-# This will filter the list to show only male actors born between 1960 and 1965 whose names end with 'e'
-filtered_actors = ddf.filter("gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$")
+```python
+filter_query = "gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$"
+filtered_data = ddf.filter(filter_query)
+print(list(filtered_data))
+```
 
-print(list(filtered_actors))
+This will output the filtered data:
+```python
 [{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
 ```
 
-For more details, please refer to the 
+For more details and advanced usage, please refer to the 
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Features
 
 Python Dictionary Display Filter supports a wide range of features, including:
 * **Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```, ```~=```, ```~```, ```&```
 * **Combining Operators:** ```and```, ```or```, ```xor```, ```not``` 
 * **Membership Operators:** ```in```
 * **Types:** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Functions:** ```upper```, ```lower```, ```len```
-* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite```
+* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```Objects```, ```SQLite```
 
 For a detailed description of the individual features check out the
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Examples 
 
-For detailed examples of how the display filter can be utilized, please refer to the following:
+For detailed examples of how the display filter can be utilized, please refer to the following sections of the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>:
 
-* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-filter)
-* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter)
-* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#sqlite-display-filter)
-* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#nmap-display-filter)
+* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#51-csv-display-filter)
+* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#52-json-display-filter)
+* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#53-sqlite-display-filter)
+* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#54-nmap-display-filter)
 
 ## Acknowledgements
 
 This project wouldn't be possible without these awesome projects:
 
 * <a href="https://wiki.wireshark.org/DisplayFilters">wireshark display filter</a>: Display filter for filtering network packages
 * <a href="https://github.com/wolever/parameterized">parameterized</a>: Parameterized testing with any Python test framework
```

#### html2text {}

```diff
@@ -1,58 +1,62 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.1.0 Summary:
-A Wireshark-like display filter for dictionaries. Home-page: https://
-github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
-email: thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming
-Language :: Python :: 3 Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: test License-File:
-LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
   ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-
      display-filter) ![Coverage](https://img.shields.io/codecov/c/github/
                     bytebutcher/python-dict-display-filter)
 
-A Wireshark-like display filter for Python dictionaries. This tool allows you
-to easily filter, analyze, and manipulate data in Python dictionaries. It
-offers a range of features including comparison operators, combining operators,
-membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
-start) 2. [Features](#features) 3. [Examples](#examples) 4. [Acknowledgements]
-(#acknowledgements) ## Quick Start Here's a simple example to get you started.
-First, install the package: ```commandline pip3 install python-dict-display-
-filter ``` Then, use it to filter a list of dictionaries: ``` from
-pydictdisplayfilter import DictDisplayFilter actors = [ {"name": ["Laurence",
-"Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name": ["Keanu",
-"Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight",
-"bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"},
-"gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"},
-"gender": "female"} ] ddf = DictDisplayFilter(actors) # This will filter the
-list to show only male actors born between 1960 and 1965 whose names end with
-'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960 and
-age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [{'name':
-['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For
-more details, please refer to the User_Guide. ## Features Python Dictionary
-Display Filter supports a wide range of features, including: * **Comparison
-Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```,
-```~=```, ```~```, ```&``` * **Combining Operators:** ```and```, ```or```,
-```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:**
-```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+A Wireshark-like display filter for Python dictionaries and various other data
+sources, including objects, lists, and SQL databases. ## Table of Contents 1.
+[Quick Start](#quick-start) 2. [Features](#features) 3. [Examples](#examples)
+4. [Acknowledgements](#acknowledgements) ## Quick Start To quickly get started
+with the python-dictionary-display-filter, follow the steps below: ###
+Installation First, install the package using pip: ```commandline pip3 install
+python-dict-display-filter ``` ### Initialization Next, import the necessary
+module and initialize the ```DictDisplayFilter``` with a list of dictionaries:
+```python from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
+["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
+["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
+["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
+"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
+"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) ``` ###
+Filtering Data Once the ```DictDisplayFilter``` is initialized, you can start
+filtering the data using the display_filter_query_language. For example, let's
+filter the actors whose birth year is after 1960: ```python filter_query =
+"age.born > 1960" filtered_data = ddf.filter(filter_query) print(list
+(filtered_data)) [ {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"},
+"gender": "male"}, {"name": ["Keanu", "Reeves"], "age": {"born": "1964"},
+"gender": "male", "power": ["flight", "bullet-time"]}, {"name": ["Carrie-Anne",
+"Moss"], "age": {"born": "1967"}, "gender": "female"} ] ``` You can also use
+more complex queries to filter the data. For example, let's filter male actors
+born between 1960 and 1964 whose names end with "e": ```python filter_query =
+"gender == male and (age.born > 1960 and age.born < 1965) and name matches
+.*e$" filtered_data = ddf.filter(filter_query) print(list(filtered_data)) ```
+This will output the filtered data: ```python [{'name': ['Laurence',
+'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For more details
+and advanced usage, please refer to the User_Guide. ## Features Python
+Dictionary Display Filter supports a wide range of features, including: *
+**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
+```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
+```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
+** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
-**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
-detailed description of the individual features check out the User_Guide. ##
-Examples For detailed examples of how the display filter can be utilized,
-please refer to the following: * [CSV Display Filter](https://github.com/
-bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
-filter) * [JSON Display Filter](https://github.com/bytebutcher/python-dict-
-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter) * [SQLite
+**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```Objects```,
+```SQLite``` For a detailed description of the individual features check out
+the User_Guide. ## Examples For detailed examples of how the display filter can
+be utilized, please refer to the following sections of the User_Guide: * [CSV
 Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/
-main/docs/EXAMPLES.md#sqlite-display-filter) * [Nmap Display Filter](https://
+main/docs/USER_GUIDE.md#51-csv-display-filter) * [JSON Display Filter](https://
 github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
-EXAMPLES.md#nmap-display-filter) ## Acknowledgements This project wouldn't be
-possible without these awesome projects: * wireshark_display_filter: Display
+USER_GUIDE.md#52-json-display-filter) * [SQLite Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+USER_GUIDE.md#53-sqlite-display-filter) * [Nmap Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+USER_GUIDE.md#54-nmap-display-filter) ## Acknowledgements This project wouldn't
+be possible without these awesome projects: * wireshark_display_filter: Display
 filter for filtering network packages * parameterized: Parameterized testing
 with any Python test framework * pyparsing: Creating PEG-parsers made easy *
 ipranger: Parsing and matching IPv4-addresses * python-dateutil: Parsing and
 comparing dates
```

### Comparing `python-dict-display-filter-1.1.0/README.md` & `python-dict-display-filter-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,125 @@
+Metadata-Version: 2.1
+Name: python-dict-display-filter
+Version: 1.2.0
+Summary: A Wireshark-like display filter for dictionaries.
+Home-page: https://github.com/bytebutcher/python-dict-display-filter
+Author: bytebutcher
+Author-email: thomas.engel.web@gmail.com
+License: GPL-3.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 <p align="center">
     <img src="https://github.com/bytebutcher/python-dict-display-filter/raw/main/images/python_dict_display_filter_logo.png" alt="python_dict_display_filter Logo"/>
 </p>
 <h1 align="center" style="margin-top: 0px;">Python Dictionary Display Filter</h1>
 <div align="center">
 
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
 ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-display-filter)
 ![Coverage](https://img.shields.io/codecov/c/github/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
-A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
-manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
-combining operators, membership operators, and more. 
+A Wireshark-like display filter for Python dictionaries and various other data 
+sources, including objects, lists, and SQL databases. 
 
 ## Table of Contents
 1. [Quick Start](#quick-start)
 2. [Features](#features)
 3. [Examples](#examples)
 4. [Acknowledgements](#acknowledgements)
 
 ## Quick Start
 
-Here's a simple example to get you started. First, install the package:
+To quickly get started with the python-dictionary-display-filter, follow the steps below:
+
+### Installation
+First, install the package using pip:
 
 ```commandline
 pip3 install python-dict-display-filter
 ```
 
-Then, use it to filter a list of dictionaries:
-```
+### Initialization
+Next, import the necessary module and initialize the ```DictDisplayFilter``` with a list of dictionaries:
+```python
 from pydictdisplayfilter import DictDisplayFilter
+
 actors = [
     {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
     {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
     {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"}, "gender": "male"},
     {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
 ]
+
 ddf = DictDisplayFilter(actors)
+```
+
+### Filtering Data
+Once the ```DictDisplayFilter``` is initialized, you can start filtering the data using the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#4-query-language">display filter query language</a>.
+For example, let's filter the actors whose birth year is after 1960:
+```python
+filter_query = "age.born > 1960"
+filtered_data = ddf.filter(filter_query)
+print(list(filtered_data))
+[
+    {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
+    {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
+    {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
+]
+```
+
+You can also use more complex queries to filter the data. 
+For example, let's filter male actors born between 1960 and 1964 whose names end with "e":
 
-# This will filter the list to show only male actors born between 1960 and 1965 whose names end with 'e'
-filtered_actors = ddf.filter("gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$")
+```python
+filter_query = "gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$"
+filtered_data = ddf.filter(filter_query)
+print(list(filtered_data))
+```
 
-print(list(filtered_actors))
+This will output the filtered data:
+```python
 [{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
 ```
 
-For more details, please refer to the 
+For more details and advanced usage, please refer to the 
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Features
 
 Python Dictionary Display Filter supports a wide range of features, including:
 * **Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```, ```~=```, ```~```, ```&```
 * **Combining Operators:** ```and```, ```or```, ```xor```, ```not``` 
 * **Membership Operators:** ```in```
 * **Types:** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Functions:** ```upper```, ```lower```, ```len```
-* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite```
+* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```Objects```, ```SQLite```
 
 For a detailed description of the individual features check out the
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Examples 
 
-For detailed examples of how the display filter can be utilized, please refer to the following:
+For detailed examples of how the display filter can be utilized, please refer to the following sections of the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>:
 
-* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-filter)
-* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter)
-* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#sqlite-display-filter)
-* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#nmap-display-filter)
+* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#51-csv-display-filter)
+* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#52-json-display-filter)
+* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#53-sqlite-display-filter)
+* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#54-nmap-display-filter)
 
 ## Acknowledgements
 
 This project wouldn't be possible without these awesome projects:
 
 * <a href="https://wiki.wireshark.org/DisplayFilters">wireshark display filter</a>: Display filter for filtering network packages
 * <a href="https://github.com/wolever/parameterized">parameterized</a>: Parameterized testing with any Python test framework
```

#### html2text {}

```diff
@@ -1,51 +1,69 @@
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.2.0 Summary:
+A Wireshark-like display filter for dictionaries. Home-page: https://
+github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
+email: thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown Provides-Extra: test License-File:
+LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
   ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-
      display-filter) ![Coverage](https://img.shields.io/codecov/c/github/
                     bytebutcher/python-dict-display-filter)
 
-A Wireshark-like display filter for Python dictionaries. This tool allows you
-to easily filter, analyze, and manipulate data in Python dictionaries. It
-offers a range of features including comparison operators, combining operators,
-membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
-start) 2. [Features](#features) 3. [Examples](#examples) 4. [Acknowledgements]
-(#acknowledgements) ## Quick Start Here's a simple example to get you started.
-First, install the package: ```commandline pip3 install python-dict-display-
-filter ``` Then, use it to filter a list of dictionaries: ``` from
-pydictdisplayfilter import DictDisplayFilter actors = [ {"name": ["Laurence",
-"Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name": ["Keanu",
-"Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight",
-"bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"},
-"gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"},
-"gender": "female"} ] ddf = DictDisplayFilter(actors) # This will filter the
-list to show only male actors born between 1960 and 1965 whose names end with
-'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960 and
-age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [{'name':
-['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For
-more details, please refer to the User_Guide. ## Features Python Dictionary
-Display Filter supports a wide range of features, including: * **Comparison
-Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```,
-```~=```, ```~```, ```&``` * **Combining Operators:** ```and```, ```or```,
-```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:**
-```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+A Wireshark-like display filter for Python dictionaries and various other data
+sources, including objects, lists, and SQL databases. ## Table of Contents 1.
+[Quick Start](#quick-start) 2. [Features](#features) 3. [Examples](#examples)
+4. [Acknowledgements](#acknowledgements) ## Quick Start To quickly get started
+with the python-dictionary-display-filter, follow the steps below: ###
+Installation First, install the package using pip: ```commandline pip3 install
+python-dict-display-filter ``` ### Initialization Next, import the necessary
+module and initialize the ```DictDisplayFilter``` with a list of dictionaries:
+```python from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
+["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
+["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
+["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
+"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
+"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) ``` ###
+Filtering Data Once the ```DictDisplayFilter``` is initialized, you can start
+filtering the data using the display_filter_query_language. For example, let's
+filter the actors whose birth year is after 1960: ```python filter_query =
+"age.born > 1960" filtered_data = ddf.filter(filter_query) print(list
+(filtered_data)) [ {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"},
+"gender": "male"}, {"name": ["Keanu", "Reeves"], "age": {"born": "1964"},
+"gender": "male", "power": ["flight", "bullet-time"]}, {"name": ["Carrie-Anne",
+"Moss"], "age": {"born": "1967"}, "gender": "female"} ] ``` You can also use
+more complex queries to filter the data. For example, let's filter male actors
+born between 1960 and 1964 whose names end with "e": ```python filter_query =
+"gender == male and (age.born > 1960 and age.born < 1965) and name matches
+.*e$" filtered_data = ddf.filter(filter_query) print(list(filtered_data)) ```
+This will output the filtered data: ```python [{'name': ['Laurence',
+'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For more details
+and advanced usage, please refer to the User_Guide. ## Features Python
+Dictionary Display Filter supports a wide range of features, including: *
+**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
+```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
+```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
+** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
-**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
-detailed description of the individual features check out the User_Guide. ##
-Examples For detailed examples of how the display filter can be utilized,
-please refer to the following: * [CSV Display Filter](https://github.com/
-bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
-filter) * [JSON Display Filter](https://github.com/bytebutcher/python-dict-
-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter) * [SQLite
+**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```Objects```,
+```SQLite``` For a detailed description of the individual features check out
+the User_Guide. ## Examples For detailed examples of how the display filter can
+be utilized, please refer to the following sections of the User_Guide: * [CSV
 Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/
-main/docs/EXAMPLES.md#sqlite-display-filter) * [Nmap Display Filter](https://
+main/docs/USER_GUIDE.md#51-csv-display-filter) * [JSON Display Filter](https://
 github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
-EXAMPLES.md#nmap-display-filter) ## Acknowledgements This project wouldn't be
-possible without these awesome projects: * wireshark_display_filter: Display
+USER_GUIDE.md#52-json-display-filter) * [SQLite Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+USER_GUIDE.md#53-sqlite-display-filter) * [Nmap Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+USER_GUIDE.md#54-nmap-display-filter) ## Acknowledgements This project wouldn't
+be possible without these awesome projects: * wireshark_display_filter: Display
 filter for filtering network packages * parameterized: Parameterized testing
 with any Python test framework * pyparsing: Creating PEG-parsers made easy *
 ipranger: Parsing and matching IPv4-addresses * python-dateutil: Parsing and
 comparing dates
```

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/__init__.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/parsers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from pydictdisplayfilter.display_filters import DictDisplayFilter, ListDisplayFilter
+from pydictdisplayfilter.parsers.display_filter import DisplayFilterParser
```

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/display_filters.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/display_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     @abstractmethod
     def filter(self, display_filter: str):
         raise NotImplementedError()
 
 
 class DictDisplayFilter(BaseDisplayFilter):
-    """ Allows to filter a dictionary using a display filter. """
+    """ Allows to filter a list of dictionaries using a display filter. """
 
     def __init__(self,
                  data: List[dict],
                  field_names: List[str] = None,
                  functions: Dict[str, Callable] = None,
                  slicers: List[BasicSlicer] = None,
                  evaluator: Evaluator = None):
@@ -134,15 +134,15 @@
         Initializes the DictDisplayFilter.
         :param data: A list of dictionaries to filter on.
         """
         super().__init__(field_names=field_names, functions=functions, slicers=slicers, evaluator=evaluator)
         self._data = data
 
     def filter(self, display_filter: str):
-        """ Filters the data using the display filter. """
+        """ Filters the dictionaries using the display filter. """
         expressions = self._display_filter_parser.parse(display_filter)
         yield from self._filter_data(self._data, expressions)
 
 
 class ListDisplayFilter(DictDisplayFilter):
     """ Allows to filter a list of lists using a display filter. """
 
@@ -242,7 +242,37 @@
         self.field_names = column_names
 
     def filter(self, display_filter: str):
         """ Filters the data using the display filter. """
         expressions = self._display_filter_parser.parse(display_filter)
         table_data = self._get_table_data()
         yield from self._filter_data(table_data, expressions)
+
+
+class ObjectDisplayFilter(BaseDisplayFilter):
+    """ Allows to filter a list of objects using a display filter. """
+
+    def __init__(self,
+                 data: List[object],
+                 field_names: List[str] = None,
+                 functions: Dict[str, Callable] = None,
+                 slicers: List[BasicSlicer] = None,
+                 evaluator: Evaluator = None):
+        """
+        Initializes the DictDisplayFilter.
+        :param data: A list of dictionaries to filter on.
+        """
+        super().__init__(field_names=field_names, functions=functions, slicers=slicers, evaluator=evaluator)
+        self._data = data
+
+    def _filter_data(self, data: List[object], expressions: List[Union[Expression, str]]) -> List:
+        if expressions:
+            for item in data:
+                if self._evaluate_expressions(expressions, item.__dict__):
+                    yield item
+        else:
+            yield from data
+
+    def filter(self, display_filter: str):
+        """ Filters the objects using the display filter. """
+        expressions = self._display_filter_parser.parse(display_filter)
+        yield from self._filter_data(self._data, expressions)
```

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/__init__.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/evaluators/common.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/evaluators/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/exceptions.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/factories.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/factories.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/helpers.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/helpers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/models.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/models.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/__init__.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from pydictdisplayfilter.parsers.display_filter import DisplayFilterParser
+from pydictdisplayfilter.display_filters import \
+    DictDisplayFilter, ListDisplayFilter, ObjectDisplayFilter, SQLDisplayFilter
```

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/common.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/parsers/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/parsers/display_filter.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/parsers/display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/pydictdisplayfilter/slicers.py` & `python-dict-display-filter-1.2.0/pydictdisplayfilter/slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/PKG-INFO` & `python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -22,75 +22,104 @@
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
 ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-display-filter)
 ![Coverage](https://img.shields.io/codecov/c/github/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
-A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
-manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
-combining operators, membership operators, and more. 
+A Wireshark-like display filter for Python dictionaries and various other data 
+sources, including objects, lists, and SQL databases. 
 
 ## Table of Contents
 1. [Quick Start](#quick-start)
 2. [Features](#features)
 3. [Examples](#examples)
 4. [Acknowledgements](#acknowledgements)
 
 ## Quick Start
 
-Here's a simple example to get you started. First, install the package:
+To quickly get started with the python-dictionary-display-filter, follow the steps below:
+
+### Installation
+First, install the package using pip:
 
 ```commandline
 pip3 install python-dict-display-filter
 ```
 
-Then, use it to filter a list of dictionaries:
-```
+### Initialization
+Next, import the necessary module and initialize the ```DictDisplayFilter``` with a list of dictionaries:
+```python
 from pydictdisplayfilter import DictDisplayFilter
+
 actors = [
     {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
     {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
     {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"}, "gender": "male"},
     {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
 ]
+
 ddf = DictDisplayFilter(actors)
+```
 
-# This will filter the list to show only male actors born between 1960 and 1965 whose names end with 'e'
-filtered_actors = ddf.filter("gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$")
+### Filtering Data
+Once the ```DictDisplayFilter``` is initialized, you can start filtering the data using the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#4-query-language">display filter query language</a>.
+For example, let's filter the actors whose birth year is after 1960:
+```python
+filter_query = "age.born > 1960"
+filtered_data = ddf.filter(filter_query)
+print(list(filtered_data))
+[
+    {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"},
+    {"name": ["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight", "bullet-time"]},
+    {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"}, "gender": "female"}
+]
+```
+
+You can also use more complex queries to filter the data. 
+For example, let's filter male actors born between 1960 and 1964 whose names end with "e":
+
+```python
+filter_query = "gender == male and (age.born > 1960 and age.born < 1965) and name matches .*e$"
+filtered_data = ddf.filter(filter_query)
+print(list(filtered_data))
+```
 
-print(list(filtered_actors))
+This will output the filtered data:
+```python
 [{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
 ```
 
-For more details, please refer to the 
+For more details and advanced usage, please refer to the 
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Features
 
 Python Dictionary Display Filter supports a wide range of features, including:
 * **Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```, ```~=```, ```~```, ```&```
 * **Combining Operators:** ```and```, ```or```, ```xor```, ```not``` 
 * **Membership Operators:** ```in```
 * **Types:** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```, ```IPv6-Address```
 * **Functions:** ```upper```, ```lower```, ```len```
-* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite```
+* **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```Objects```, ```SQLite```
 
 For a detailed description of the individual features check out the
 <a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>.
 
 ## Examples 
 
-For detailed examples of how the display filter can be utilized, please refer to the following:
+For detailed examples of how the display filter can be utilized, please refer to the following sections of the 
+<a href="https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md">User Guide</a>:
 
-* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-filter)
-* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter)
-* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#sqlite-display-filter)
-* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#nmap-display-filter)
+* [CSV Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#51-csv-display-filter)
+* [JSON Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#52-json-display-filter)
+* [SQLite Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#53-sqlite-display-filter)
+* [Nmap Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/main/docs/USER_GUIDE.md#54-nmap-display-filter)
 
 ## Acknowledgements
 
 This project wouldn't be possible without these awesome projects:
 
 * <a href="https://wiki.wireshark.org/DisplayFilters">wireshark display filter</a>: Display filter for filtering network packages
 * <a href="https://github.com/wolever/parameterized">parameterized</a>: Parameterized testing with any Python test framework
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.2.0 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
 email: thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown Provides-Extra: test License-File:
 LICENSE
                        [python_dict_display_filter Logo]
@@ -10,49 +10,60 @@
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
   ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-
      display-filter) ![Coverage](https://img.shields.io/codecov/c/github/
                     bytebutcher/python-dict-display-filter)
 
-A Wireshark-like display filter for Python dictionaries. This tool allows you
-to easily filter, analyze, and manipulate data in Python dictionaries. It
-offers a range of features including comparison operators, combining operators,
-membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
-start) 2. [Features](#features) 3. [Examples](#examples) 4. [Acknowledgements]
-(#acknowledgements) ## Quick Start Here's a simple example to get you started.
-First, install the package: ```commandline pip3 install python-dict-display-
-filter ``` Then, use it to filter a list of dictionaries: ``` from
-pydictdisplayfilter import DictDisplayFilter actors = [ {"name": ["Laurence",
-"Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name": ["Keanu",
-"Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight",
-"bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"},
-"gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"},
-"gender": "female"} ] ddf = DictDisplayFilter(actors) # This will filter the
-list to show only male actors born between 1960 and 1965 whose names end with
-'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960 and
-age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [{'name':
-['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For
-more details, please refer to the User_Guide. ## Features Python Dictionary
-Display Filter supports a wide range of features, including: * **Comparison
-Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```,
-```~=```, ```~```, ```&``` * **Combining Operators:** ```and```, ```or```,
-```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:**
-```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+A Wireshark-like display filter for Python dictionaries and various other data
+sources, including objects, lists, and SQL databases. ## Table of Contents 1.
+[Quick Start](#quick-start) 2. [Features](#features) 3. [Examples](#examples)
+4. [Acknowledgements](#acknowledgements) ## Quick Start To quickly get started
+with the python-dictionary-display-filter, follow the steps below: ###
+Installation First, install the package using pip: ```commandline pip3 install
+python-dict-display-filter ``` ### Initialization Next, import the necessary
+module and initialize the ```DictDisplayFilter``` with a list of dictionaries:
+```python from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
+["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
+["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
+["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
+"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
+"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) ``` ###
+Filtering Data Once the ```DictDisplayFilter``` is initialized, you can start
+filtering the data using the display_filter_query_language. For example, let's
+filter the actors whose birth year is after 1960: ```python filter_query =
+"age.born > 1960" filtered_data = ddf.filter(filter_query) print(list
+(filtered_data)) [ {"name": ["Laurence", "Fishburne"], "age": {"born": "1961"},
+"gender": "male"}, {"name": ["Keanu", "Reeves"], "age": {"born": "1964"},
+"gender": "male", "power": ["flight", "bullet-time"]}, {"name": ["Carrie-Anne",
+"Moss"], "age": {"born": "1967"}, "gender": "female"} ] ``` You can also use
+more complex queries to filter the data. For example, let's filter male actors
+born between 1960 and 1964 whose names end with "e": ```python filter_query =
+"gender == male and (age.born > 1960 and age.born < 1965) and name matches
+.*e$" filtered_data = ddf.filter(filter_query) print(list(filtered_data)) ```
+This will output the filtered data: ```python [{'name': ['Laurence',
+'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For more details
+and advanced usage, please refer to the User_Guide. ## Features Python
+Dictionary Display Filter supports a wide range of features, including: *
+**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
+```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
+```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
+** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
-**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
-detailed description of the individual features check out the User_Guide. ##
-Examples For detailed examples of how the display filter can be utilized,
-please refer to the following: * [CSV Display Filter](https://github.com/
-bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
-filter) * [JSON Display Filter](https://github.com/bytebutcher/python-dict-
-display-filter/blob/main/docs/EXAMPLES.md#json-display-filter) * [SQLite
+**Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```Objects```,
+```SQLite``` For a detailed description of the individual features check out
+the User_Guide. ## Examples For detailed examples of how the display filter can
+be utilized, please refer to the following sections of the User_Guide: * [CSV
 Display Filter](https://github.com/bytebutcher/python-dict-display-filter/blob/
-main/docs/EXAMPLES.md#sqlite-display-filter) * [Nmap Display Filter](https://
+main/docs/USER_GUIDE.md#51-csv-display-filter) * [JSON Display Filter](https://
 github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
-EXAMPLES.md#nmap-display-filter) ## Acknowledgements This project wouldn't be
-possible without these awesome projects: * wireshark_display_filter: Display
+USER_GUIDE.md#52-json-display-filter) * [SQLite Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+USER_GUIDE.md#53-sqlite-display-filter) * [Nmap Display Filter](https://
+github.com/bytebutcher/python-dict-display-filter/blob/main/docs/
+USER_GUIDE.md#54-nmap-display-filter) ## Acknowledgements This project wouldn't
+be possible without these awesome projects: * wireshark_display_filter: Display
 filter for filtering network packages * parameterized: Parameterized testing
 with any Python test framework * pyparsing: Creating PEG-parsers made easy *
 ipranger: Parsing and matching IPv4-addresses * python-dateutil: Parsing and
 comparing dates
```

### Comparing `python-dict-display-filter-1.1.0/python_dict_display_filter.egg-info/SOURCES.txt` & `python-dict-display-filter-1.2.0/python_dict_display_filter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 tests/__init__.py
 tests/test_csv_display_filter_example.py
 tests/test_dict_display_filter.py
 tests/test_dict_display_filter_shell.py
 tests/test_display_filter_parser.py
 tests/test_json_display_filter_example.py
 tests/test_nmap_display_filter_example.py
+tests/test_object_display_filter.py
 tests/test_slicers.py
 tests/test_sql_display_filter.py
 tests/test_sqlite_display_filter_example.py
 tests/test_table.py
```

### Comparing `python-dict-display-filter-1.1.0/setup.py` & `python-dict-display-filter-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="python-dict-display-filter",
-    version="1.1.0",
+    version="1.2.0",
     description="A Wireshark-like display filter for dictionaries.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bytebutcher/python-dict-display-filter",
     author="bytebutcher",
     author_email="thomas.engel.web@gmail.com",
     license="GPL-3.0",
```

### Comparing `python-dict-display-filter-1.1.0/tests/__init__.py` & `python-dict-display-filter-1.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_csv_display_filter_example.py` & `python-dict-display-filter-1.2.0/tests/test_csv_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_dict_display_filter.py` & `python-dict-display-filter-1.2.0/tests/test_dict_display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_dict_display_filter_shell.py` & `python-dict-display-filter-1.2.0/tests/test_dict_display_filter_shell.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_display_filter_parser.py` & `python-dict-display-filter-1.2.0/tests/test_display_filter_parser.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_json_display_filter_example.py` & `python-dict-display-filter-1.2.0/tests/test_json_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_nmap_display_filter_example.py` & `python-dict-display-filter-1.2.0/tests/test_nmap_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_slicers.py` & `python-dict-display-filter-1.2.0/tests/test_slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_sql_display_filter.py` & `python-dict-display-filter-1.2.0/tests/test_sql_display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_sqlite_display_filter_example.py` & `python-dict-display-filter-1.2.0/tests/test_sqlite_display_filter_example.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-1.1.0/tests/test_table.py` & `python-dict-display-filter-1.2.0/tests/test_table.py`

 * *Files identical despite different names*

