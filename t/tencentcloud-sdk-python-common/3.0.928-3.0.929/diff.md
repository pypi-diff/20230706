# Comparing `tmp/tencentcloud-sdk-python-common-3.0.928.tar.gz` & `tmp/tencentcloud-sdk-python-common-3.0.929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.928.tar", last modified: Wed Jul  5 00:23:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.929.tar", last modified: Thu Jul  6 00:23:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-common-3.0.928.tar` & `tencentcloud-sdk-python-common-3.0.929.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1055 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/setup.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/
--rw-r--r--   0 root         (0) root         (0)    15666 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/credential.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/abstract_model.py
--rw-r--r--   0 root         (0) root         (0)     4301 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/circuit_breaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/exception/
--rw-r--r--   0 root         (0) root         (0)      760 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/exception/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/profile/
--rw-r--r--   0 root         (0) root         (0)     4534 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/profile/http_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/http/
--rw-r--r--   0 root         (0) root         (0)     5120 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/http/request.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20283 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/abstract_client.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/common_client.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/sign.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      876 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:23:05.000000 tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/
+-rw-r--r--   0 root         (0) root         (0)    15666 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/credential.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 root         (0) root         (0)     4301 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/circuit_breaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/exception/
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/exception/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/profile/
+-rw-r--r--   0 root         (0) root         (0)     4534 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/profile/http_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/http/
+-rw-r--r--   0 root         (0) root         (0)     5120 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/http/request.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20283 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/common_client.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/sign.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:23:17.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      876 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:23:18.000000 tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-common-3.0.928/setup.py` & `tencentcloud-sdk-python-common-3.0.929/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.929/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-common-3.0.928/README.rst` & `tencentcloud-sdk-python-common-3.0.929/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/credential.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/abstract_model.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/circuit_breaker.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/exception/__init__.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/profile/client_profile.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/profile/http_profile.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/http/request.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/abstract_client.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/common_client.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/common/sign.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud/__init__.py` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.928'
+__version__ = '3.0.929'
```

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.928/tencentcloud_sdk_python_common.egg-info/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.929/tencentcloud_sdk_python_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

