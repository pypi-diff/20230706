# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.927.tar", last modified: Tue Jul  4 00:21:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.928.tar", last modified: Wed Jul  5 00:25:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.927.tar` & `tencentcloud-sdk-python-emr-3.0.928.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud_sdk_python_emr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:21:35.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    14329 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   262188 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27334 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:21:34.000000 tencentcloud-sdk-python-emr-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    14329 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   455303 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30020 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:25:42.000000 tencentcloud-sdk-python-emr-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-emr-3.0.927/setup.py` & `tencentcloud-sdk-python-emr-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.928/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.927/README.rst` & `tencentcloud-sdk-python-emr-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.927/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.928/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.927/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.928/tencentcloud/emr/v20190103/emr_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,14 +184,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeHiveQueries(self, request):
+        """获取hive查询信息
+
+        :param request: Request instance for DescribeHiveQueries.
+        :type request: :class:`tencentcloud.emr.v20190103.models.DescribeHiveQueriesRequest`
+        :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeHiveQueriesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeHiveQueries", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeHiveQueriesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeImpalaQueries(self, request):
+        """DescribeImpalaQueries
+
+        :param request: Request instance for DescribeImpalaQueries.
+        :type request: :class:`tencentcloud.emr.v20190103.models.DescribeImpalaQueriesRequest`
+        :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeImpalaQueriesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeImpalaQueries", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeImpalaQueriesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeInstanceRenewNodes(self, request):
         """查询待续费节点信息
 
         :param request: Request instance for DescribeInstanceRenewNodes.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeInstanceRenewNodesRequest`
         :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeInstanceRenewNodesResponse`
 
@@ -321,14 +367,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeYarnApplications(self, request):
+        """DescribeYarnApplications
+
+        :param request: Request instance for DescribeYarnApplications.
+        :type request: :class:`tencentcloud.emr.v20190103.models.DescribeYarnApplicationsRequest`
+        :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeYarnApplicationsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeYarnApplications", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeYarnApplicationsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def InquirePriceRenewEmr(self, request):
         """集群续费询价。
 
         :param request: Request instance for InquirePriceRenewEmr.
         :type request: :class:`tencentcloud.emr.v20190103.models.InquirePriceRenewEmrRequest`
```

### Comparing `tencentcloud-sdk-python-emr-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.928/tencentcloud/__init__.py`

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

