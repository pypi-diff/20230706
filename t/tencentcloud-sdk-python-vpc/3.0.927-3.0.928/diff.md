# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.927.tar", last modified: Tue Jul  4 00:33:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.928.tar", last modified: Wed Jul  5 00:37:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.927.tar` & `tencentcloud-sdk-python-vpc-3.0.928.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:50.000000 tencentcloud-sdk-python-vpc-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:33:50.000000 tencentcloud-sdk-python-vpc-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:33:50.000000 tencentcloud-sdk-python-vpc-3.0.927/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:50.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:50.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:50.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:50.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)    42398 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   852411 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   332318 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:33:49.000000 tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    42398 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1310476 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   332321 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:37:35.000000 tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.927/setup.py` & `tencentcloud-sdk-python-vpc-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.928/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.927/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.928/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.927/README.rst` & `tencentcloud-sdk-python-vpc-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def AttachCcnInstances(self, request):
         """本接口（AttachCcnInstances）用于将网络实例加载到云联网实例中，网络实例包括VPC和专线网关。<br />
-        每个云联网能够关联的网络实例个数是有限的，详请参考产品文档。如果需要扩充请联系在线客服。
+        每个云联网能够关联的网络实例个数是有限的，详情请参考产品文档。如果需要扩充请联系在线客服。
 
         :param request: Request instance for AttachCcnInstances.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AttachCcnInstancesRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.AttachCcnInstancesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.928/tencentcloud/__init__.py`

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
