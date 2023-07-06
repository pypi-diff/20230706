# Comparing `tmp/tencentcloud-sdk-python-iotvideo-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-iotvideo-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.927.tar", last modified: Tue Jul  4 00:24:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.928.tar", last modified: Wed Jul  5 00:28:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotvideo-3.0.927.tar` & `tencentcloud-sdk-python-iotvideo-3.0.928.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud_sdk_python_iotvideo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      861 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20201215/
--rw-r--r--   0 root         (0) root         (0)    72251 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20201215/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20201215/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   188015 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20201215/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20201215/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20191126/
--rw-r--r--   0 root         (0) root         (0)    64459 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20191126/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20191126/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   149627 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20191126/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20191126/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20211125/
--rw-r--r--   0 root         (0) root         (0)    87013 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20211125/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20211125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   227341 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20211125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20211125/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:24:15.000000 tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud_sdk_python_iotvideo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      861 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20201215/
+-rw-r--r--   0 root         (0) root         (0)    72251 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20201215/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20201215/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   303767 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20201215/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20201215/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20191126/
+-rw-r--r--   0 root         (0) root         (0)    64459 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20191126/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20191126/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229605 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20191126/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20191126/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20211125/
+-rw-r--r--   0 root         (0) root         (0)    87013 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20211125/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20211125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   365162 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20211125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20211125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:28:14.000000 tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/setup.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.928/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/README.rst` & `tencentcloud-sdk-python-iotvideo-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20201215/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20201215/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20201215/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20201215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20191126/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20191126/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20191126/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20191126/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20211125/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20211125/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/iotvideo/v20211125/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/iotvideo/v20211125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotvideo-3.0.928/tencentcloud/__init__.py`

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

