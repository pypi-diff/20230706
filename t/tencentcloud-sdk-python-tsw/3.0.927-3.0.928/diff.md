# Comparing `tmp/tencentcloud-sdk-python-tsw-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-tsw-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsw-3.0.927.tar", last modified: Tue Jul  4 00:33:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsw-3.0.928.tar", last modified: Wed Jul  5 00:37:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsw-3.0.927.tar` & `tencentcloud-sdk-python-tsw-3.0.928.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud_sdk_python_tsw.egg-info/
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud_sdk_python_tsw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud_sdk_python_tsw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud_sdk_python_tsw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud_sdk_python_tsw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20210412/
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20210412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3032 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20210412/models.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20210412/tsw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20210412/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3837 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/models.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/tsw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:33:15.000000 tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud_sdk_python_tsw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud_sdk_python_tsw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud_sdk_python_tsw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud_sdk_python_tsw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud_sdk_python_tsw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20210412/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20210412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20210412/models.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20210412/tsw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20210412/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5590 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/models.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/tsw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:37:01.000000 tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud_sdk_python_tsw.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud_sdk_python_tsw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud_sdk_python_tsw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud_sdk_python_tsw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsw
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Tsw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/setup.py` & `tencentcloud-sdk-python-tsw-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-tsw-3.0.928/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsw
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Tsw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/README.rst` & `tencentcloud-sdk-python-tsw-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20210412/errorcodes.py` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20210412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20210412/tsw_client.py` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20210412/tsw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/errorcodes.py` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/models.py` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,62 +21,127 @@
 class AgentShell(AbstractModel):
     """agent安装脚本串
 
     """
 
     def __init__(self):
         r"""
-        :param Token: 鉴权token
+        :param _Token: 鉴权token
 注意：此字段可能返回 null，表示取不到有效值。
         :type Token: str
-        :param EtlIp: 数据接收Ip
+        :param _EtlIp: 数据接收Ip
 注意：此字段可能返回 null，表示取不到有效值。
         :type EtlIp: str
-        :param EtlPort: 数据接收port
+        :param _EtlPort: 数据接收port
 注意：此字段可能返回 null，表示取不到有效值。
         :type EtlPort: str
-        :param ByHandAccess: 手动接入脚本串
+        :param _ByHandAccess: 手动接入脚本串
 注意：此字段可能返回 null，表示取不到有效值。
         :type ByHandAccess: str
-        :param ByShellAccess: 自动接入脚本串
+        :param _ByShellAccess: 自动接入脚本串
 注意：此字段可能返回 null，表示取不到有效值。
         :type ByShellAccess: str
-        :param SkyWalkingPort: SkyWalking数据接收port
+        :param _SkyWalkingPort: SkyWalking数据接收port
 注意：此字段可能返回 null，表示取不到有效值。
         :type SkyWalkingPort: str
-        :param ZipkinPort: Zipkin数据接收port
+        :param _ZipkinPort: Zipkin数据接收port
 注意：此字段可能返回 null，表示取不到有效值。
         :type ZipkinPort: str
-        :param JaegerPort: Jaeger数据接收port
+        :param _JaegerPort: Jaeger数据接收port
 注意：此字段可能返回 null，表示取不到有效值。
         :type JaegerPort: str
         """
-        self.Token = None
-        self.EtlIp = None
-        self.EtlPort = None
-        self.ByHandAccess = None
-        self.ByShellAccess = None
-        self.SkyWalkingPort = None
-        self.ZipkinPort = None
-        self.JaegerPort = None
+        self._Token = None
+        self._EtlIp = None
+        self._EtlPort = None
+        self._ByHandAccess = None
+        self._ByShellAccess = None
+        self._SkyWalkingPort = None
+        self._ZipkinPort = None
+        self._JaegerPort = None
+
+    @property
+    def Token(self):
+        return self._Token
+
+    @Token.setter
+    def Token(self, Token):
+        self._Token = Token
+
+    @property
+    def EtlIp(self):
+        return self._EtlIp
+
+    @EtlIp.setter
+    def EtlIp(self, EtlIp):
+        self._EtlIp = EtlIp
+
+    @property
+    def EtlPort(self):
+        return self._EtlPort
+
+    @EtlPort.setter
+    def EtlPort(self, EtlPort):
+        self._EtlPort = EtlPort
+
+    @property
+    def ByHandAccess(self):
+        return self._ByHandAccess
+
+    @ByHandAccess.setter
+    def ByHandAccess(self, ByHandAccess):
+        self._ByHandAccess = ByHandAccess
+
+    @property
+    def ByShellAccess(self):
+        return self._ByShellAccess
+
+    @ByShellAccess.setter
+    def ByShellAccess(self, ByShellAccess):
+        self._ByShellAccess = ByShellAccess
+
+    @property
+    def SkyWalkingPort(self):
+        return self._SkyWalkingPort
+
+    @SkyWalkingPort.setter
+    def SkyWalkingPort(self, SkyWalkingPort):
+        self._SkyWalkingPort = SkyWalkingPort
+
+    @property
+    def ZipkinPort(self):
+        return self._ZipkinPort
+
+    @ZipkinPort.setter
+    def ZipkinPort(self, ZipkinPort):
+        self._ZipkinPort = ZipkinPort
+
+    @property
+    def JaegerPort(self):
+        return self._JaegerPort
+
+    @JaegerPort.setter
+    def JaegerPort(self, JaegerPort):
+        self._JaegerPort = JaegerPort
 
 
     def _deserialize(self, params):
-        self.Token = params.get("Token")
-        self.EtlIp = params.get("EtlIp")
-        self.EtlPort = params.get("EtlPort")
-        self.ByHandAccess = params.get("ByHandAccess")
-        self.ByShellAccess = params.get("ByShellAccess")
-        self.SkyWalkingPort = params.get("SkyWalkingPort")
-        self.ZipkinPort = params.get("ZipkinPort")
-        self.JaegerPort = params.get("JaegerPort")
+        self._Token = params.get("Token")
+        self._EtlIp = params.get("EtlIp")
+        self._EtlPort = params.get("EtlPort")
+        self._ByHandAccess = params.get("ByHandAccess")
+        self._ByShellAccess = params.get("ByShellAccess")
+        self._SkyWalkingPort = params.get("SkyWalkingPort")
+        self._ZipkinPort = params.get("ZipkinPort")
+        self._JaegerPort = params.get("JaegerPort")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class DescribeAgentShellRequest(AbstractModel):
     """DescribeAgentShell请求参数结构体
@@ -87,22 +152,38 @@
 class DescribeAgentShellResponse(AbstractModel):
     """DescribeAgentShell返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Result: 接入信息
+        :param _Result: 接入信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type Result: :class:`tencentcloud.tsw.v20200924.models.AgentShell`
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.Result = None
-        self.RequestId = None
+        self._Result = None
+        self._RequestId = None
+
+    @property
+    def Result(self):
+        return self._Result
+
+    @Result.setter
+    def Result(self, Result):
+        self._Result = Result
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Result") is not None:
-            self.Result = AgentShell()
-            self.Result._deserialize(params.get("Result"))
-        self.RequestId = params.get("RequestId")
+            self._Result = AgentShell()
+            self._Result._deserialize(params.get("Result"))
+        self._RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/tsw/v20200924/tsw_client.py` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/tsw/v20200924/tsw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsw-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsw-3.0.928/tencentcloud/__init__.py`

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

