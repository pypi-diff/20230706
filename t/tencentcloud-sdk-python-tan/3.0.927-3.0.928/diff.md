# Comparing `tmp/tencentcloud-sdk-python-tan-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-tan-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tan-3.0.927.tar", last modified: Tue Jul  4 00:29:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tan-3.0.928.tar", last modified: Wed Jul  5 00:33:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tan-3.0.927.tar` & `tencentcloud-sdk-python-tan-3.0.928.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud_sdk_python_tan.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud_sdk_python_tan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud_sdk_python_tan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud_sdk_python_tan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud_sdk_python_tan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/
--rw-r--r--   0 root         (0) root         (0)     2281 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2285 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/tan_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:29:31.000000 tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud_sdk_python_tan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud_sdk_python_tan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud_sdk_python_tan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud_sdk_python_tan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud_sdk_python_tan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/tan_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:33:27.000000 tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/__init__.py
```

### Comparing `tencentcloud-sdk-python-tan-3.0.927/setup.py` & `tencentcloud-sdk-python-tan-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-tan-3.0.928/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tan
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Tan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tan-3.0.927/tencentcloud_sdk_python_tan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tan-3.0.928/tencentcloud_sdk_python_tan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tan
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Tan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tan-3.0.927/README.rst` & `tencentcloud-sdk-python-tan-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tan-3.0.928/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/errorcodes.py` & `tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/models.py` & `tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,47 +21,80 @@
 class CreateBlockNodeRecordsRequest(AbstractModel):
     """CreateBlockNodeRecords请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param GroupId: 盘查组id，可在“盘查组概览”功能中获取。
+        :param _GroupId: 盘查组id，可在“盘查组概览”功能中获取。
         :type GroupId: str
-        :param NodeId: 节点id，可在“数据接入管理”中获取。
+        :param _NodeId: 节点id，可在“数据接入管理”中获取。
         :type NodeId: str
-        :param Records: 节点数据json，具体demo请参考输入示例，其中key为数据接入管理中节点内创建的属性变量名，value为期望的推送值。
+        :param _Records: 节点数据json，具体demo请参考输入示例，其中key为数据接入管理中节点内创建的属性变量名，value为期望的推送值。
         :type Records: str
         """
-        self.GroupId = None
-        self.NodeId = None
-        self.Records = None
+        self._GroupId = None
+        self._NodeId = None
+        self._Records = None
+
+    @property
+    def GroupId(self):
+        return self._GroupId
+
+    @GroupId.setter
+    def GroupId(self, GroupId):
+        self._GroupId = GroupId
+
+    @property
+    def NodeId(self):
+        return self._NodeId
+
+    @NodeId.setter
+    def NodeId(self, NodeId):
+        self._NodeId = NodeId
+
+    @property
+    def Records(self):
+        return self._Records
+
+    @Records.setter
+    def Records(self, Records):
+        self._Records = Records
 
 
     def _deserialize(self, params):
-        self.GroupId = params.get("GroupId")
-        self.NodeId = params.get("NodeId")
-        self.Records = params.get("Records")
+        self._GroupId = params.get("GroupId")
+        self._NodeId = params.get("NodeId")
+        self._Records = params.get("Records")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class CreateBlockNodeRecordsResponse(AbstractModel):
     """CreateBlockNodeRecords返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.RequestId = None
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self.RequestId = params.get("RequestId")
+        self._RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tan-3.0.927/tencentcloud/tan/v20220420/tan_client.py` & `tencentcloud-sdk-python-tan-3.0.928/tencentcloud/tan/v20220420/tan_client.py`

 * *Files identical despite different names*

