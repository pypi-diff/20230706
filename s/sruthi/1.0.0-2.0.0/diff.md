# Comparing `tmp/sruthi-1.0.0.tar.gz` & `tmp/sruthi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sruthi-1.0.0.tar", last modified: Mon Dec  6 14:08:34 2021, max compression
+gzip compressed data, was "sruthi-2.0.0.tar", last modified: Wed Jul  5 23:27:49 2023, max compression
```

## Comparing `sruthi-1.0.0.tar` & `sruthi-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 14:08:34.201871 sruthi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-12-06 14:08:20.000000 sruthi-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     8512 2021-12-06 14:08:34.201871 sruthi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6508 2021-12-06 14:08:20.000000 sruthi-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-06 14:08:34.201871 sruthi-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2021-12-06 14:08:20.000000 sruthi-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 14:08:34.201871 sruthi-1.0.0/sruthi/
--rw-r--r--   0 runner    (1001) docker     (121)      814 2021-12-06 14:08:20.000000 sruthi-1.0.0/sruthi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-12-06 14:08:20.000000 sruthi-1.0.0/sruthi/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2021-12-06 14:08:20.000000 sruthi-1.0.0/sruthi/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    11496 2021-12-06 14:08:20.000000 sruthi-1.0.0/sruthi/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3065 2021-12-06 14:08:20.000000 sruthi-1.0.0/sruthi/xmlparse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 14:08:34.201871 sruthi-1.0.0/sruthi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8512 2021-12-06 14:08:33.000000 sruthi-1.0.0/sruthi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-12-06 14:08:34.000000 sruthi-1.0.0/sruthi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-06 14:08:33.000000 sruthi-1.0.0/sruthi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-06 14:08:33.000000 sruthi-1.0.0/sruthi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-06 14:08:33.000000 sruthi-1.0.0/sruthi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:27:49.714792 sruthi-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-05 23:27:37.000000 sruthi-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-05 23:27:49.714792 sruthi-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-07-05 23:27:37.000000 sruthi-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 23:27:49.714792 sruthi-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-05 23:27:37.000000 sruthi-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:27:49.710792 sruthi-2.0.0/sruthi/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-05 23:27:37.000000 sruthi-2.0.0/sruthi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-05 23:27:37.000000 sruthi-2.0.0/sruthi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-05 23:27:37.000000 sruthi-2.0.0/sruthi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-05 23:27:37.000000 sruthi-2.0.0/sruthi/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-05 23:27:37.000000 sruthi-2.0.0/sruthi/xmlparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:27:49.714792 sruthi-2.0.0/sruthi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-05 23:27:49.000000 sruthi-2.0.0/sruthi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-05 23:27:49.000000 sruthi-2.0.0/sruthi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:27:49.000000 sruthi-2.0.0/sruthi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 23:27:49.000000 sruthi-2.0.0/sruthi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 23:27:49.000000 sruthi-2.0.0/sruthi.egg-info/top_level.txt
```

### Comparing `sruthi-1.0.0/LICENSE.md` & `sruthi-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sruthi-1.0.0/PKG-INFO` & `sruthi-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sruthi
-Version: 1.0.0
+Version: 2.0.0
 Summary: SRU client for Python
 Home-page: https://github.com/metaodi/sruthi
 Author: Stefan Oderbolz
 Author-email: odi@metaodi.ch
 Maintainer: Stefan Oderbolz
 Maintainer-email: odi@metaodi.ch
 License: MIT
-Download-URL: https://github.com/metaodi/sruthi/archive/v1.0.0.zip
+Download-URL: https://github.com/metaodi/sruthi/archive/v2.0.0.zip
 Description: [![PyPI Version](https://img.shields.io/pypi/v/sruthi)](https://pypi.org/project/sruthi/)
         [![Tests + Linting Python](https://github.com/metaodi/sruthi/actions/workflows/lint_python.yml/badge.svg)](https://github.com/metaodi/sruthi/actions/workflows/lint_python.yml)
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         # sruthi
         
         **sru**thi is a client for python to make [SRU requests (Search/Retrieve via URL)](http://www.loc.gov/standards/sru/).
         
         Currently only **SRU 1.1 and 1.2** is supported.
         
@@ -74,15 +75,16 @@
         https://suche.staatsarchiv.djiktzh.ch/detail.aspx?Id=4612939
         G I 1, Nr. 34
         Verordnung der Stadt Zürich betreffend die Erfüllung von Amtspflichten durch die Chorherren des Grossmünsterstifts
         24.09.1485
         https://suche.staatsarchiv.djiktzh.ch/detail.aspx?Id=3796980
         ```
         
-        The return value of `searchretrieve` is iterable, so you can easily loop over it. Or you can use indices to access elements, e.g. `records[1]` to get the second elemenet, or `records[-1]` to get the last one.
+        The return value of `searchretrieve` is iterable, so you can easily loop over it.
+        Or you can use indices to access records, e.g. `records[1]` to get the second record, or `records[-1]` to get the last one.
         
         Even [slicing](https://python-reference.readthedocs.io/en/latest/docs/brackets/slicing.html) is supported, so you can do things like only iterate over the first 5 elements using
         
         ```python
         for records in records[:5]:
            print(record)
         ```
@@ -129,29 +131,46 @@
         ...     record_schema='oai_dc',
         ...     sru_version='1.1'
         >>> )
         >>> records.count
         8985
         ```
         
+        ### Custom parameters and settings
+        
+        If an SRU endpoint needs additional (custom) parameters, you can create your own session object and pass it to the client.
+        This is useful for adding authentication (username, password), custom headers or parameters, SSL verification settings etc.
+        
+        ```python
+        >>> import sruthi
+        >>> import requests
+        >>> # customize session
+        >>> session = requests.Session()
+        >>> session.params = {"x-collection": "GGC"}
+        >>> # pass the customized session to sruthi
+        >>> records = sruthi.searchretrieve("https://jsru.kb.nl/sru", query="gruninger", session=session)
+        >>> records.count
+        4
+        ```
+        
         ## Schemas
         
         sruthi does not make any assumptions about the record data schema.
         The data is provided as-is (as a flattend dict).
         sruthi has been tested with the following schemas:
         
         * [Dublin Core Record Schema](http://www.loc.gov/standards/sru/recordSchemas/dc-schema.html) (dc)
         * [MARCXML: The MARC 21 XML Schema](http://www.loc.gov/standards/marcxml/schema/MARC21slim.xsd) (marcxml)
         * [ISAD(G): General International Standard Archival Description, Second edition](http://www.expertisecentrumdavid.be/xmlschemas/isad.xsd) (isad)
         
         ## Development
         
         To contribute to sruthi simply clone this repository and follow the instructions in [CONTRIBUTING.md](/CONTRIBUTING.md).
         
-        This project ha a Makefile with the most common commands.
+        This project has a `Makefile` with the most common commands.
         Type `make help` to get an overview.
         
         ## Release
         
         To create a new release, follow these steps (please respect [Semantic Versioning](http://semver.org/)):
         
         1. Adapt the version number in `sruthi/__init__.py`
@@ -162,12 +181,14 @@
         
 Keywords: sru,search,retrieve,archive,library
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `sruthi-1.0.0/README.md` & `sruthi-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![PyPI Version](https://img.shields.io/pypi/v/sruthi)](https://pypi.org/project/sruthi/)
 [![Tests + Linting Python](https://github.com/metaodi/sruthi/actions/workflows/lint_python.yml/badge.svg)](https://github.com/metaodi/sruthi/actions/workflows/lint_python.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # sruthi
 
 **sru**thi is a client for python to make [SRU requests (Search/Retrieve via URL)](http://www.loc.gov/standards/sru/).
 
 Currently only **SRU 1.1 and 1.2** is supported.
 
@@ -63,15 +64,16 @@
 https://suche.staatsarchiv.djiktzh.ch/detail.aspx?Id=4612939
 G I 1, Nr. 34
 Verordnung der Stadt Zürich betreffend die Erfüllung von Amtspflichten durch die Chorherren des Grossmünsterstifts
 24.09.1485
 https://suche.staatsarchiv.djiktzh.ch/detail.aspx?Id=3796980
 ```
 
-The return value of `searchretrieve` is iterable, so you can easily loop over it. Or you can use indices to access elements, e.g. `records[1]` to get the second elemenet, or `records[-1]` to get the last one.
+The return value of `searchretrieve` is iterable, so you can easily loop over it.
+Or you can use indices to access records, e.g. `records[1]` to get the second record, or `records[-1]` to get the last one.
 
 Even [slicing](https://python-reference.readthedocs.io/en/latest/docs/brackets/slicing.html) is supported, so you can do things like only iterate over the first 5 elements using
 
 ```python
 for records in records[:5]:
    print(record)
 ```
@@ -118,29 +120,46 @@
 ...     record_schema='oai_dc',
 ...     sru_version='1.1'
 >>> )
 >>> records.count
 8985
 ```
 
+### Custom parameters and settings
+
+If an SRU endpoint needs additional (custom) parameters, you can create your own session object and pass it to the client.
+This is useful for adding authentication (username, password), custom headers or parameters, SSL verification settings etc.
+
+```python
+>>> import sruthi
+>>> import requests
+>>> # customize session
+>>> session = requests.Session()
+>>> session.params = {"x-collection": "GGC"}
+>>> # pass the customized session to sruthi
+>>> records = sruthi.searchretrieve("https://jsru.kb.nl/sru", query="gruninger", session=session)
+>>> records.count
+4
+```
+
 ## Schemas
 
 sruthi does not make any assumptions about the record data schema.
 The data is provided as-is (as a flattend dict).
 sruthi has been tested with the following schemas:
 
 * [Dublin Core Record Schema](http://www.loc.gov/standards/sru/recordSchemas/dc-schema.html) (dc)
 * [MARCXML: The MARC 21 XML Schema](http://www.loc.gov/standards/marcxml/schema/MARC21slim.xsd) (marcxml)
 * [ISAD(G): General International Standard Archival Description, Second edition](http://www.expertisecentrumdavid.be/xmlschemas/isad.xsd) (isad)
 
 ## Development
 
 To contribute to sruthi simply clone this repository and follow the instructions in [CONTRIBUTING.md](/CONTRIBUTING.md).
 
-This project ha a Makefile with the most common commands.
+This project has a `Makefile` with the most common commands.
 Type `make help` to get an overview.
 
 ## Release
 
 To create a new release, follow these steps (please respect [Semantic Versioning](http://semver.org/)):
 
 1. Adapt the version number in `sruthi/__init__.py`
```

### Comparing `sruthi-1.0.0/setup.py` & `sruthi-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,13 +31,15 @@
     keywords=['sru', 'search', 'retrieve', 'archive', 'library'],
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
-    python_requires='>=3.6'
+    python_requires='>=3.7'
 )
```

### Comparing `sruthi-1.0.0/sruthi/__init__.py` & `sruthi-2.0.0/sruthi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-__version__ = '1.0.0'
-__all__ = ['client', 'errors', 'response', 'xmlparse']
+__version__ = "2.0.0"
+__all__ = ["client", "errors", "response", "xmlparse"]
 
-from .errors import SruthiError, ServerIncompatibleError, SruError, NoMoreRecordsError  # noqa
-from .errors import SruthiWarning, WrongNamespaceWarning # noqa
-from .client import Client # noqa
+from .errors import (  # noqa
+    SruthiError,
+    ServerIncompatibleError,
+    SruError,
+    NoMoreRecordsError,
+)
+from .errors import SruthiWarning, WrongNamespaceWarning  # noqa
+from .client import Client  # noqa
 
 
 def searchretrieve(url, query, **kwargs):
-    search_params = ['query', 'start_record', 'requests_kwargs']
+    search_params = ["query", "start_record"]
     search_kwargs = {k: v for k, v in kwargs.items() if k in search_params}
-    search_kwargs['query'] = query
+    search_kwargs["query"] = query
 
     # assume all others kwargs are for the client
     client_kwargs = {k: v for k, v in kwargs.items() if k not in search_params}
-    client_kwargs['url'] = url
+    client_kwargs["url"] = url
 
     c = Client(**client_kwargs)
     return c.searchretrieve(**search_kwargs)
 
 
 def explain(url, **kwargs):
     c = Client(url, **kwargs)
```

### Comparing `sruthi-1.0.0/sruthi/client.py` & `sruthi-2.0.0/sruthi/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,78 +3,78 @@
 import requests
 from . import errors
 from . import xmlparse
 from . import response
 
 
 class Client(object):
-    def __init__(self, url=None, maximum_records=10, record_schema=None, sru_version='1.2'):
+    def __init__(
+        self,
+        url=None,
+        maximum_records=10,
+        record_schema=None,
+        sru_version="1.2",
+        session=None,
+    ):
         self.url = url
         self.maximum_records = maximum_records
         self.sru_version = sru_version
         self.record_schema = record_schema
+        self.session = session or requests.Session()
 
-    def searchretrieve(self, query, start_record=1, requests_kwargs=None):
+    def searchretrieve(self, query, start_record=1):
         params = {
-            'operation': 'searchRetrieve',
-            'version': self.sru_version,
-            'query': query,
-            'startRecord': start_record,
-            'maximumRecords': self.maximum_records,
+            "operation": "searchRetrieve",
+            "version": self.sru_version,
+            "query": query,
+            "startRecord": start_record,
+            "maximumRecords": self.maximum_records,
         }
 
         if self.record_schema:
-            params['recordSchema'] = self.record_schema
+            params["recordSchema"] = self.record_schema
 
-        data_loader = DataLoader(self.url, params, requests_kwargs)
+        data_loader = DataLoader(self.url, self.session, params)
         return response.SearchRetrieveResponse(data_loader)
 
-    def explain(self, requests_kwargs=None):
+    def explain(self):
         params = {
-            'operation': 'explain',
-            'version': self.sru_version,
+            "operation": "explain",
+            "version": self.sru_version,
         }
-        data_loader = DataLoader(self.url, params, requests_kwargs)
+        data_loader = DataLoader(self.url, self.session, params)
         explain_response = response.ExplainResponse(data_loader)
         return explain_response.asdict()
 
 
 class DataLoader(object):
-    def __init__(self, url, params, requests_kwargs=None):
-        self.session = requests.Session()
+    def __init__(self, url, session, params):
+        self.session = session
         self.url = url
         self.params = params
         self.response = None
         self.xmlparser = xmlparse.XMLParser()
-        self.requests_kwargs = requests_kwargs or {}
 
     def load(self, **kwargs):
         self.params.update(kwargs)
         xml = self._get_content(self.url, self.params)
         self._check_errors(xml)
         return xml
 
     def _get_content(self, url, params):
         try:
-            res = self.session.get(
-                url,
-                params=params,
-                **self.requests_kwargs
-            )
+            res = self.session.get(url, params=params)
             res.raise_for_status()
         except requests.exceptions.HTTPError as e:
             raise errors.SruthiError("HTTP error: %s" % e)
         except requests.exceptions.RequestException as e:
             raise errors.SruthiError("Request error: %s" % e)
 
         return self.xmlparser.parse(res.content)
 
     def _check_errors(self, xml):
-        sru = '{http://www.loc.gov/zing/srw/}'
-        diag = '{http://www.loc.gov/zing/srw/diagnostic/}'
-        diagnostics = self.xmlparser.find(
-            xml,
-            f'{sru}diagnostics/{diag}diagnostic'
-        )
+        sru = "{http://www.loc.gov/zing/srw/}"
+        diag = "{http://www.loc.gov/zing/srw/diagnostic/}"
+        diagnostics = self.xmlparser.find(xml, f"{sru}diagnostics/{diag}diagnostic")
         if diagnostics:
             error_msg = ", ".join([d.text for d in diagnostics])
             raise errors.SruError(error_msg)
```

### Comparing `sruthi-1.0.0/sruthi/errors.py` & `sruthi-2.0.0/sruthi/errors.py`

 * *Files identical despite different names*

### Comparing `sruthi-1.0.0/sruthi/response.py` & `sruthi-2.0.0/sruthi/response.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,58 +19,60 @@
     def maybe_int(self, s):
         try:
             return int(s)
         except (ValueError, TypeError):
             return s
 
     def _check_response_tag(self, xml, tag):
-        sru = '{http://www.loc.gov/zing/srw/}'
+        sru = "{http://www.loc.gov/zing/srw/}"
         response = f"{sru}{tag}"
         if not xml.tag == response:
             # fix namespace for servers that provide the wrong namespace URI
             main_ns = self.xmlparser.namespace(xml)
-            if 'www.loc.gov/zing/srw' in main_ns:
+            if "www.loc.gov/zing/srw" in main_ns:
                 warnings.warn(
                     f"""
                     The server has the wrong namespace for SRU,
                     it should be {sru} but it's currently set to {{{main_ns}}}.
                     """,
-                    errors.WrongNamespaceWarning
+                    errors.WrongNamespaceWarning,
                 )
-                self.xmlparser.namespaces['sru'] = main_ns
+                self.xmlparser.namespaces["sru"] = main_ns
             else:
                 raise errors.ServerIncompatibleError(
                     f"Server response did not contain a {response} tag"
                 )
 
 
 class SearchRetrieveResponse(Response):
     def __repr__(self):
         try:
             return (
-                'SearchRetrieveResponse('
-                'sru_version=%r,'
-                'count=%r,'
-                'next_start_record=%r)'
-                ) % (
-                   self.sru_version,
-                   self.count,
-                   self.next_start_record,
-                )
+                "SearchRetrieveResponse("
+                "sru_version=%r,"
+                "count=%r,"
+                "next_start_record=%r)"
+            ) % (
+                self.sru_version,
+                self.count,
+                self.next_start_record,
+            )
         except AttributeError:
-            return 'SearchRetrieveResponse(empty)'
+            return "SearchRetrieveResponse(empty)"
 
     def _parse_content(self, xml):
-        self._check_response_tag(xml, 'searchRetrieveResponse')
+        self._check_response_tag(xml, "searchRetrieveResponse")
 
-        self.sru_version = self.xmlparser.find(xml, './sru:version').text
-        self.count = self.maybe_int(self.xmlparser.find(xml, './sru:numberOfRecords').text)
+        self.sru_version = self.xmlparser.find(xml, "./sru:version").text
+        self.count = self.maybe_int(
+            self.xmlparser.find(xml, "./sru:numberOfRecords").text
+        )
         self._extract_records(xml)
 
-        next_start_record = self.xmlparser.find(xml, './sru:nextRecordPosition').text
+        next_start_record = self.xmlparser.find(xml, "./sru:nextRecordPosition").text
         if next_start_record:
             self.next_start_record = self.maybe_int(next_start_record)
         else:
             self.next_start_record = None
 
     def __length_hint__(self):
         return self.count
@@ -117,23 +119,23 @@
             raise errors.NoMoreRecordsError()
         xml = self.data_loader.load(startRecord=self.next_start_record)
         self._parse_content(xml)
 
     def _extract_records(self, xml):
         new_records = []
 
-        xml_recs = self.xmlparser.findall(xml, './sru:records/sru:record')
+        xml_recs = self.xmlparser.findall(xml, "./sru:records/sru:record")
         for xml_rec in xml_recs:
             record = defaultdict()
-            record['schema'] = self.xmlparser.find(xml_rec, './sru:recordSchema').text
-            record_data = self.xmlparser.find(xml_rec, './sru:recordData')
-            extra_data = self.xmlparser.find(xml_rec, './sru:extraRecordData')
+            record["schema"] = self.xmlparser.find(xml_rec, "./sru:recordSchema").text
+            record_data = self.xmlparser.find(xml_rec, "./sru:recordData")
+            extra_data = self.xmlparser.find(xml_rec, "./sru:extraRecordData")
 
-            record.update(self._tag_data(record_data, 'sru:recordData') or {})
-            record['extra'] = self._tag_data(extra_data, 'sru:extraRecordData')
+            record.update(self._tag_data(record_data, "sru:recordData") or {})
+            record["extra"] = self._tag_data(extra_data, "sru:extraRecordData")
 
             record = dict(record)
             new_records.append(record)
         self.records.extend(new_records)
 
     def _tag_data(self, elem, parent):
         if not elem:
@@ -144,16 +146,16 @@
             return None
 
         # check if there is only one element on the top level
         keys = list(record_data.keys())
         if len(record_data) == 1 and len(keys) > 0 and len(record_data[keys[0]]) > 0:
             record_data = record_data[keys[0]]
 
-        record_data.pop('schemaLocation', None)
-        record_data.pop('xmlns', None)
+        record_data.pop("schemaLocation", None)
+        record_data.pop("xmlns", None)
 
         def leaf_reducer(k1, k2):
             # only use key of leaf element
             return k2
 
         try:
             record_data = flatten(record_data, reducer=leaf_reducer)
@@ -161,197 +163,189 @@
             # if the keys of the leaf elements are not unique
             # the dict will not be flattened
             pass
 
         return record_data
 
     def _remove_namespace(self, elem):
-        ns_pattern = re.compile('{.+}')
-        tag_name = ns_pattern.sub('', elem.tag)
+        ns_pattern = re.compile("{.+}")
+        tag_name = ns_pattern.sub("", elem.tag)
         return tag_name
 
 
 class ExplainResponse(Response):
     def __repr__(self):
         return (
-            'ExplainResponse('
-            'sru_version=%r,'
-            'server=%r,'
-            'database=%r'
-            'index=%r'
-            'schema=%r'
-            'config=%r)'
-            ) % (
-               self.sru_version,
-               self.server,
-               self.database,
-               self.index,
-               self.schema,
-               self.config,
-            )
+            "ExplainResponse("
+            "sru_version=%r,"
+            "server=%r,"
+            "database=%r"
+            "index=%r"
+            "schema=%r"
+            "config=%r)"
+        ) % (
+            self.sru_version,
+            self.server,
+            self.database,
+            self.index,
+            self.schema,
+            self.config,
+        )
 
     def asdict(self):
-        return AttributeDict({
-            'sru_version': self.sru_version,
-            'server': self.server,
-            'database': self.database,
-            'index': self.index,
-            'schema': self.schema,
-            'config': self.config,
-        })
+        return AttributeDict(
+            {
+                "sru_version": self.sru_version,
+                "server": self.server,
+                "database": self.database,
+                "index": self.index,
+                "schema": self.schema,
+                "config": self.config,
+            }
+        )
 
     def _parse_content(self, xml):
-        self._check_response_tag(xml, 'explainResponse')
+        self._check_response_tag(xml, "explainResponse")
 
-        record_schema = self.xmlparser.find(xml, './/sru:recordSchema').text
+        record_schema = self.xmlparser.find(xml, ".//sru:recordSchema").text
         if record_schema:
-            self.xmlparser.namespaces['zr'] = record_schema
+            self.xmlparser.namespaces["zr"] = record_schema
 
-        self.sru_version = self.xmlparser.find(xml, './sru:version').text
+        self.sru_version = self.xmlparser.find(xml, "./sru:version").text
 
         self.server = self._parse_server(xml)
         self.database = self._parse_database(xml)
         self.index = self._parse_index(xml)
         self.schema = self._parse_schema(xml)
         self.config = self._parse_config(xml)
 
     def _parse_server(self, xml):
         server_info = {
-            'host': self.xmlparser.find(
-                        xml,
-                        [
-                            './/zr:serverInfo/zr:host',
-                            './/zr2:serverInfo/zr:host'
-                        ]
-                    ).text,
-            'port': self.xmlparser.find(
-                        xml,
-                        [
-                            './/zr:serverInfo/zr:port',
-                            './/zr2:serverInfo/zr:port',
-                        ]
-                    ).text,
-            'database': self.xmlparser.find(
-                        xml,
-                        [
-                            './/zr:serverInfo/zr:database',
-                            './/zr2:serverInfo/zr:database',
-                        ]
-                    ).text,
+            "host": self.xmlparser.find(
+                xml, [".//zr:serverInfo/zr:host", ".//zr2:serverInfo/zr:host"]
+            ).text,
+            "port": self.xmlparser.find(
+                xml,
+                [
+                    ".//zr:serverInfo/zr:port",
+                    ".//zr2:serverInfo/zr:port",
+                ],
+            ).text,
+            "database": self.xmlparser.find(
+                xml,
+                [
+                    ".//zr:serverInfo/zr:database",
+                    ".//zr2:serverInfo/zr:database",
+                ],
+            ).text,
         }
-        server_info['port'] = self.maybe_int(server_info['port'])
+        server_info["port"] = self.maybe_int(server_info["port"])
         return server_info
 
     def _parse_schema(self, xml):
         def bool_or_none(v):
             if v is None:
                 return None
             return bool(v)
 
         def ident(a):
             return a
 
         attributes = {
-            'identifier': ident,
-            'name': ident,
-            'location': ident,
-            'sort': bool_or_none,
-            'retrieve': bool_or_none,
+            "identifier": ident,
+            "name": ident,
+            "location": ident,
+            "sort": bool_or_none,
+            "retrieve": bool_or_none,
         }
 
         schemas = {}
         xml_schemas = self.xmlparser.findall(
             xml,
             [
-                './/zr:schemaInfo/zr:schema',
-                './/zr2:schemaInfo/zr2:schema',
-            ]
+                ".//zr:schemaInfo/zr:schema",
+                ".//zr2:schemaInfo/zr2:schema",
+            ],
         )
         for schema in xml_schemas:
             schema_info = {}
             for attr, fn in attributes.items():
                 xml_attr = schema.attrib.get(attr)
                 if xml_attr:
                     schema_info[attr] = fn(xml_attr)
-            schema_info['title'] = self.xmlparser.find(schema, './zr:title').text
-            schemas[schema.attrib.get('name')] = schema_info
+            schema_info["title"] = self.xmlparser.find(schema, "./zr:title").text
+            schemas[schema.attrib.get("name")] = schema_info
         return schemas
 
     def _parse_config(self, xml):
         config = {}
         settings = self.xmlparser.findall(
             xml,
             [
-                './/zr:configInfo/zr:setting',
-                './/zr2:configInfo/zr:setting',
-            ]
+                ".//zr:configInfo/zr:setting",
+                ".//zr2:configInfo/zr:setting",
+            ],
         )
         for setting in settings:
-            t = setting.attrib['type']
+            t = setting.attrib["type"]
             config[t] = self.maybe_int(setting.text)
 
         # defaults
         xml_defaults = self.xmlparser.findall(
             xml,
             [
-                './/zr:configInfo/zr:default',
-                './/zr2:configInfo/zr:default',
-            ]
+                ".//zr:configInfo/zr:default",
+                ".//zr2:configInfo/zr:default",
+            ],
         )
         defaults = {}
         for default in xml_defaults:
-            t = default.attrib['type']
+            t = default.attrib["type"]
             defaults[t] = self.maybe_int(default.text)
-        config['defaults'] = defaults
+        config["defaults"] = defaults
         return config
 
     def _parse_database(self, xml):
-        db = self.xmlparser.find(xml, './/zr:databaseInfo')
+        db = self.xmlparser.find(xml, ".//zr:databaseInfo")
         if not db:
             return {}
         db_info = {
-            'title': self.xmlparser.find(db, ['./zr:title', './title']).text,
-            'description': self.xmlparser.find(db, ['./zr:description', './description']).text,
-            'contact': self.xmlparser.find(db, ['./zr:contact', './contact']).text,
+            "title": self.xmlparser.find(db, ["./zr:title", "./title"]).text,
+            "description": self.xmlparser.find(
+                db, ["./zr:description", "./description"]
+            ).text,
+            "contact": self.xmlparser.find(db, ["./zr:contact", "./contact"]).text,
         }
         db_info = {k: v.strip() if v else v for (k, v) in db_info.items()}
         return db_info
 
     def _parse_index(self, xml):
         index = defaultdict(defaultdict)
         index_sets = self.xmlparser.findall(
             xml,
             [
-                './/zr:indexInfo/zr:set',
-                './/zr2:indexInfo/zr2:set',
-            ]
+                ".//zr:indexInfo/zr:set",
+                ".//zr2:indexInfo/zr2:set",
+            ],
         )
         for index_set in index_sets:
-            index[index_set.attrib['name']] = defaultdict()
+            index[index_set.attrib["name"]] = defaultdict()
 
         index_fields = self.xmlparser.findall(
-            xml,
-            [
-                './/zr:indexInfo/zr:index',
-                './/zr2:indexInfo/zr2:index'
-            ]
+            xml, [".//zr:indexInfo/zr:index", ".//zr2:indexInfo/zr2:index"]
         )
         for index_field in index_fields:
-            title = self.xmlparser.find(index_field, ['./zr:title', './title']).text
+            title = self.xmlparser.find(index_field, ["./zr:title", "./title"]).text
             if title:
                 title = title.strip()
             names = self.xmlparser.findall(
-                index_field,
-                [
-                    './/zr:map/zr:name',
-                    './/zr2:map/zr2:name'
-                ]
+                index_field, [".//zr:map/zr:name", ".//zr2:map/zr2:name"]
             )
             for name in names:
-                index[name.attrib['set']][name.text.strip()] = title
+                index[name.attrib["set"]][name.text.strip()] = title
 
         return {k: dict(v) for k, v in dict(index).items()}
 
 
 class AttributeDict(dict):
     def __getattr__(self, attr):
         return self[attr]
```

### Comparing `sruthi-1.0.0/sruthi/xmlparse.py` & `sruthi-2.0.0/sruthi/xmlparse.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,35 +17,35 @@
 
     text = None
 
 
 class XMLParser(object):
     def __init__(self):
         self.namespaces = {
-            'sru': 'http://www.loc.gov/zing/srw/',
-            'isad': 'http://www.expertisecentrumdavid.be/xmlschemas/isad.xsd',
-            'rel': 'info:srw/extension/2/relevancy-1.0',
-            'ap': 'http://www.archivportal.ch/srw/extension/',
-            'zr': 'http://explain.z3950.org/dtd/2.1/',
-            'zr2': 'http://explain.z3950.org/dtd/2.0/',
+            "sru": "http://www.loc.gov/zing/srw/",
+            "isad": "http://www.expertisecentrumdavid.be/xmlschemas/isad.xsd",
+            "rel": "info:srw/extension/2/relevancy-1.0",
+            "ap": "http://www.archivportal.ch/srw/extension/",
+            "zr": "http://explain.z3950.org/dtd/2.1/",
+            "zr2": "http://explain.z3950.org/dtd/2.0/",
         }
         self.dict_namespaces = {
-            'http://www.loc.gov/zing/srw/': 'sru',
-            'http://explain.z3950.org/dtd/2.1/': 'zr',
-            'info:srw/extension/2/relevancy-1.0': None,
-            'http://www.archivportal.ch/srw/extension/': None,
-            'http://www.loc.gov/MARC21/slim': None,
-            'info:lc/xmlns/marcxchange-v1': None,
-            'http://www.loc.gov/mods/v3': None,
-            'http://www.loc.gov/standards/mods/v3/mods-3-6.xsd': None,
-            'http://www.loc.gov/standards/mods/v3/mods-3-6.xsd': None,
-            'http://purl.org/dc/elements/1.1/': None,
-            'http://www.expertisecentrumdavid.be/xmlschemas/isad.xsd': None,
-            'http://www.w3.org/2001/XMLSchema-instance': None,
-            'http://www.w3.org/XML/1998/namespace': None,
+            "http://www.loc.gov/zing/srw/": "sru",
+            "http://explain.z3950.org/dtd/2.1/": "zr",
+            "info:srw/extension/2/relevancy-1.0": None,
+            "http://www.archivportal.ch/srw/extension/": None,
+            "http://www.loc.gov/MARC21/slim": None,
+            "info:lc/xmlns/marcxchange-v1": None,
+            "http://www.loc.gov/mods/v3": None,
+            "http://www.loc.gov/standards/mods/v3/mods-3-6.xsd": None,
+            "http://www.loc.gov/standards/mods/v3/mods-3-6.xsd": None,
+            "http://purl.org/dc/elements/1.1/": None,
+            "http://www.expertisecentrumdavid.be/xmlschemas/isad.xsd": None,
+            "http://www.w3.org/2001/XMLSchema-instance": None,
+            "http://www.w3.org/XML/1998/namespace": None,
         }
 
     def parse(self, content):
         try:
             return etree.fromstring(content)
         except Exception as e:
             raise errors.SruError("Error while parsing XML: %s" % e)
@@ -77,19 +77,19 @@
     def todict(self, xml, **kwargs):
         if isinstance(xml, XMLNone):
             return None
         if isinstance(xml, Element):
             xml = self.tostring(xml)
 
         dict_args = {
-            'dict_constructor': dict,
-            'process_namespaces': True,
-            'namespaces': self.dict_namespaces,
-            'attr_prefix': '',
-            'cdata_key': 'text',
+            "dict_constructor": dict,
+            "process_namespaces": True,
+            "namespaces": self.dict_namespaces,
+            "attr_prefix": "",
+            "cdata_key": "text",
         }
         dict_args.update(kwargs)
         return dict(xmltodict.parse(xml, **dict_args))
 
     def namespace(self, element):
-        m = re.match(r'\{(.*)\}', element.tag)
-        return m.group(1) if m else ''
+        m = re.match(r"\{(.*)\}", element.tag)
+        return m.group(1) if m else ""
```

### Comparing `sruthi-1.0.0/sruthi.egg-info/PKG-INFO` & `sruthi-2.0.0/sruthi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sruthi
-Version: 1.0.0
+Version: 2.0.0
 Summary: SRU client for Python
 Home-page: https://github.com/metaodi/sruthi
 Author: Stefan Oderbolz
 Author-email: odi@metaodi.ch
 Maintainer: Stefan Oderbolz
 Maintainer-email: odi@metaodi.ch
 License: MIT
-Download-URL: https://github.com/metaodi/sruthi/archive/v1.0.0.zip
+Download-URL: https://github.com/metaodi/sruthi/archive/v2.0.0.zip
 Description: [![PyPI Version](https://img.shields.io/pypi/v/sruthi)](https://pypi.org/project/sruthi/)
         [![Tests + Linting Python](https://github.com/metaodi/sruthi/actions/workflows/lint_python.yml/badge.svg)](https://github.com/metaodi/sruthi/actions/workflows/lint_python.yml)
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         # sruthi
         
         **sru**thi is a client for python to make [SRU requests (Search/Retrieve via URL)](http://www.loc.gov/standards/sru/).
         
         Currently only **SRU 1.1 and 1.2** is supported.
         
@@ -74,15 +75,16 @@
         https://suche.staatsarchiv.djiktzh.ch/detail.aspx?Id=4612939
         G I 1, Nr. 34
         Verordnung der Stadt Zürich betreffend die Erfüllung von Amtspflichten durch die Chorherren des Grossmünsterstifts
         24.09.1485
         https://suche.staatsarchiv.djiktzh.ch/detail.aspx?Id=3796980
         ```
         
-        The return value of `searchretrieve` is iterable, so you can easily loop over it. Or you can use indices to access elements, e.g. `records[1]` to get the second elemenet, or `records[-1]` to get the last one.
+        The return value of `searchretrieve` is iterable, so you can easily loop over it.
+        Or you can use indices to access records, e.g. `records[1]` to get the second record, or `records[-1]` to get the last one.
         
         Even [slicing](https://python-reference.readthedocs.io/en/latest/docs/brackets/slicing.html) is supported, so you can do things like only iterate over the first 5 elements using
         
         ```python
         for records in records[:5]:
            print(record)
         ```
@@ -129,29 +131,46 @@
         ...     record_schema='oai_dc',
         ...     sru_version='1.1'
         >>> )
         >>> records.count
         8985
         ```
         
+        ### Custom parameters and settings
+        
+        If an SRU endpoint needs additional (custom) parameters, you can create your own session object and pass it to the client.
+        This is useful for adding authentication (username, password), custom headers or parameters, SSL verification settings etc.
+        
+        ```python
+        >>> import sruthi
+        >>> import requests
+        >>> # customize session
+        >>> session = requests.Session()
+        >>> session.params = {"x-collection": "GGC"}
+        >>> # pass the customized session to sruthi
+        >>> records = sruthi.searchretrieve("https://jsru.kb.nl/sru", query="gruninger", session=session)
+        >>> records.count
+        4
+        ```
+        
         ## Schemas
         
         sruthi does not make any assumptions about the record data schema.
         The data is provided as-is (as a flattend dict).
         sruthi has been tested with the following schemas:
         
         * [Dublin Core Record Schema](http://www.loc.gov/standards/sru/recordSchemas/dc-schema.html) (dc)
         * [MARCXML: The MARC 21 XML Schema](http://www.loc.gov/standards/marcxml/schema/MARC21slim.xsd) (marcxml)
         * [ISAD(G): General International Standard Archival Description, Second edition](http://www.expertisecentrumdavid.be/xmlschemas/isad.xsd) (isad)
         
         ## Development
         
         To contribute to sruthi simply clone this repository and follow the instructions in [CONTRIBUTING.md](/CONTRIBUTING.md).
         
-        This project ha a Makefile with the most common commands.
+        This project has a `Makefile` with the most common commands.
         Type `make help` to get an overview.
         
         ## Release
         
         To create a new release, follow these steps (please respect [Semantic Versioning](http://semver.org/)):
         
         1. Adapt the version number in `sruthi/__init__.py`
@@ -162,12 +181,14 @@
         
 Keywords: sru,search,retrieve,archive,library
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

