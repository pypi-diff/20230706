# Comparing `tmp/tencentcloud-sdk-python-mgobe-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-mgobe-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.927.tar", last modified: Tue Jul  4 00:25:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.928.tar", last modified: Wed Jul  5 00:29:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mgobe-3.0.927.tar` & `tencentcloud-sdk-python-mgobe-3.0.928.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud_sdk_python_mgobe.egg-info/
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20201014/
--rw-r--r--   0 root         (0) root         (0)    34111 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20201014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20430 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20201014/models.py
--rw-r--r--   0 root         (0) root         (0)     8244 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20201014/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20201014/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/
--rw-r--r--   0 root         (0) root         (0)    34005 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/models.py
--rw-r--r--   0 root         (0) root         (0)     1855 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:25:40.000000 tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud_sdk_python_mgobe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20201014/
+-rw-r--r--   0 root         (0) root         (0)    34111 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20201014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    32095 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20201014/models.py
+-rw-r--r--   0 root         (0) root         (0)     8244 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20201014/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20201014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:29:30.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/
+-rw-r--r--   0 root         (0) root         (0)    34005 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/models.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:29:29.000000 tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/setup.py` & `tencentcloud-sdk-python-mgobe-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.928/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/README.rst` & `tencentcloud-sdk-python-mgobe-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20201014/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20201014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20201014/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20201014/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/models.py` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,43 +21,68 @@
 class DismissRoomRequest(AbstractModel):
     """DismissRoom请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param GameId: 表示游戏资源唯一 ID, 由后台自动分配, 无法修改。
+        :param _GameId: 表示游戏资源唯一 ID, 由后台自动分配, 无法修改。
         :type GameId: str
-        :param RoomId: 表示游戏房间唯一ID。
+        :param _RoomId: 表示游戏房间唯一ID。
         :type RoomId: str
         """
-        self.GameId = None
-        self.RoomId = None
+        self._GameId = None
+        self._RoomId = None
+
+    @property
+    def GameId(self):
+        return self._GameId
+
+    @GameId.setter
+    def GameId(self, GameId):
+        self._GameId = GameId
+
+    @property
+    def RoomId(self):
+        return self._RoomId
+
+    @RoomId.setter
+    def RoomId(self, RoomId):
+        self._RoomId = RoomId
 
 
     def _deserialize(self, params):
-        self.GameId = params.get("GameId")
-        self.RoomId = params.get("RoomId")
+        self._GameId = params.get("GameId")
+        self._RoomId = params.get("RoomId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class DismissRoomResponse(AbstractModel):
     """DismissRoom返回参数结构体
 
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

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/mgobe/v20190929/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/mgobe/v20190929/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mgobe-3.0.928/tencentcloud/__init__.py`

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

