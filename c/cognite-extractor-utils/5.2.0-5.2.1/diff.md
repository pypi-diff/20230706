# Comparing `tmp/cognite_extractor_utils-5.2.0.tar.gz` & `tmp/cognite_extractor_utils-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-5.2.0.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-5.2.1.tar", max compression
```

## Comparing `cognite_extractor_utils-5.2.0.tar` & `cognite_extractor_utils-5.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10173 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/LICENSE
--rw-r--r--   0        0        0     4090 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/README.md
--rw-r--r--   0        0        0      739 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    15974 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     2861 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    19910 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0     9545 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1061 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    14929 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0     1108 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/middleware.py
--rw-r--r--   0        0        0        0 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    17829 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3054 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3865 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     6118 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    11674 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     7021 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26579 2023-06-28 07:09:15.525399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7476 2023-06-28 07:09:15.529399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1146 2023-06-28 07:09:15.529399 cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    14284 2023-06-28 07:09:15.529399 cognite_extractor_utils-5.2.0/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2066 2023-06-28 07:09:15.529399 cognite_extractor_utils-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     5406 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-07-06 06:33:06.189123 cognite_extractor_utils-5.2.1/LICENSE
+-rw-r--r--   0        0        0     4090 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/README.md
+-rw-r--r--   0        0        0      739 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    15974 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     2861 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    19910 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0     9545 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1061 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    14929 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0     1108 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    17829 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3054 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     4983 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3865 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     6118 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    11674 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     7021 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26582 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7476 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1146 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    14284 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2066 2023-07-06 06:33:06.193123 cognite_extractor_utils-5.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5406 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.2.1/PKG-INFO
```

### Comparing `cognite_extractor_utils-5.2.0/LICENSE` & `cognite_extractor_utils-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/README.md` & `cognite_extractor_utils-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "5.2.0"
+__version__ = "5.2.1"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/base.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/elements.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/middleware.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/middleware.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/statestore.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/_metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/events.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/files.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader/time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     TIMESERIES_UPLOADER_POINTS_DISCARDED,
     TIMESERIES_UPLOADER_POINTS_QUEUED,
     TIMESERIES_UPLOADER_POINTS_WRITTEN,
     TIMESERIES_UPLOADER_QUEUE_SIZE,
 )
 from cognite.extractorutils.util import EitherId, retry
 
-MIN_DATAPOINT_TIMESTAMP = 31536000000
+MIN_DATAPOINT_TIMESTAMP = -2208988800000
 MAX_DATAPOINT_STRING_LENGTH = 255
 MAX_DATAPOINT_VALUE = 1e100
 MIN_DATAPOINT_VALUE = -1e100
 
 DataPoint = Tuple[Union[int, float, datetime], Union[int, float, str]]
 DataPointList = List[DataPoint]
```

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/cognite/extractorutils/util.py` & `cognite_extractor_utils-5.2.1/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.2.0/pyproject.toml` & `cognite_extractor_utils-5.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "5.2.0"
+version = "5.2.1"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
@@ -69,16 +69,16 @@
 jq = [{version = "^1.3.0", platform = "macos"}, {version = "^1.3.0", platform = "linux"}]
 
 [tool.poetry.extras]
 experimental = ["cognite-sdk-experimental"]
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
-mypy = "1.2.0"
-ruff = "^0.0.274"
+mypy = "1.4.1"
+ruff = "^0.0.277"
 pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 sphinx = "^6.0.0"
 sphinx-rtd-theme = "^1.0.0"
 pre-commit = "^3.3.0"
 SecretStorage = "^3.1.2"
 twine = "^4.0.0"
```

### Comparing `cognite_extractor_utils-5.2.0/PKG-INFO` & `cognite_extractor_utils-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 5.2.0
+Version: 5.2.1
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.2.0 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.2.1 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

