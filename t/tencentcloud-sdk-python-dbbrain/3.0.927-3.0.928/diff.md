# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.927.tar", last modified: Tue Jul  4 00:20:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.928.tar", last modified: Wed Jul  5 00:24:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.927.tar` & `tencentcloud-sdk-python-dbbrain-3.0.928.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   185526 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20210527/models.py
--rw-r--r--   0 root         (0) root         (0)    48612 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20210527/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:20:00.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   114440 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)    27659 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:19:59.000000 tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20191016/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   299639 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20210527/models.py
+-rw-r--r--   0 root         (0) root         (0)    48612 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20210527/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   183920 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:24:08.000000 tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20191016/__init__.py
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.928/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.927'
+__version__ = '3.0.928'
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.927/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.928/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

