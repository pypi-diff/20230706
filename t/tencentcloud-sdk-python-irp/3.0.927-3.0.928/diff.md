# Comparing `tmp/tencentcloud-sdk-python-irp-3.0.927.tar.gz` & `tmp/tencentcloud-sdk-python-irp-3.0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-irp-3.0.927.tar", last modified: Tue Jul  4 00:24:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-irp-3.0.928.tar", last modified: Wed Jul  5 00:28:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-irp-3.0.927.tar` & `tencentcloud-sdk-python-irp-3.0.928.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud_sdk_python_irp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud_sdk_python_irp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud_sdk_python_irp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud_sdk_python_irp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220324/
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    33284 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220324/models.py
--rw-r--r--   0 root         (0) root         (0)     4373 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220324/irp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220324/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:24:33.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53358 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/models.py
--rw-r--r--   0 root         (0) root         (0)     7337 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/irp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:24:32.000000 tencentcloud-sdk-python-irp-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud_sdk_python_irp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud_sdk_python_irp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud_sdk_python_irp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud_sdk_python_irp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54088 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/models.py
+-rw-r--r--   0 root         (0) root         (0)     4373 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/irp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220805/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220805/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    81404 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220805/models.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220805/irp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220805/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:28:25.000000 tencentcloud-sdk-python-irp-3.0.928/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-irp-3.0.927/setup.py` & `tencentcloud-sdk-python-irp-3.0.928/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.927/PKG-INFO` & `tencentcloud-sdk-python-irp-3.0.928/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-irp
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Irp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud_sdk_python_irp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud_sdk_python_irp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud_sdk_python_irp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-irp
-Version: 3.0.927
+Version: 3.0.928
 Summary: Tencent Cloud Irp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-irp-3.0.927/README.rst` & `tencentcloud-sdk-python-irp-3.0.928/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220324/errorcodes.py` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220324/irp_client.py` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/irp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/errorcodes.py` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220805/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/models.py` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220324/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,1153 +14,1832 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
-class DescribeGoodsRecommendRequest(AbstractModel):
-    """DescribeGoodsRecommend请求参数结构体
+class AuthorInfo(AbstractModel):
+    """作者信息
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID，在控制台获取
-        :type InstanceId: str
-        :param SceneId: 场景ID，在控制台创建场景后获取
-        :type SceneId: str
-        :param UserId: 用户唯一ID，客户自定义用户ID，作为一个用户的唯一标识，需和行为数据上报接口中的UserId一致，否则影响特征关联
-        :type UserId: str
-        :param UserIdList: 用户设备ID数组，可传入用户的多个类型ID，用于关联画像信息
-        :type UserIdList: list of StrUserIdInfo
-        :param GoodsCnt: 推荐返回数量，默认10个，最多支持50个的内容返回。如果有更多数量要求，<a href="https://console.cloud.tencent.com/workorder/category" target="_blank">提单</a>沟通解决
-        :type GoodsCnt: int
-        :param CurrentGoodsId: 当场景是相关推荐时该值必填，场景是非相关推荐时该值无效
-        :type CurrentGoodsId: str
-        :param UserPortraitInfo: 用户的实时特征信息，用作特征
-        :type UserPortraitInfo: :class:`tencentcloud.irp.v20220805.models.UserPortraitInfo`
-        :param BlackGoodsList: 本次请求针对该用户需要过滤的物品列表(不超过100个)
-        :type BlackGoodsList: list of str
-        :param Extension: json字符串，扩展字段
-        :type Extension: str
+        :param _Id: 作者id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _Name: 作者名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _SourceId: 作者来源
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SourceId: int
+        :param _FollowType: 关注类型：1-关注，2-取关
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FollowType: int
+        :param _IconUrl: 作者头像icon地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IconUrl: str
         """
-        self.InstanceId = None
-        self.SceneId = None
-        self.UserId = None
-        self.UserIdList = None
-        self.GoodsCnt = None
-        self.CurrentGoodsId = None
-        self.UserPortraitInfo = None
-        self.BlackGoodsList = None
-        self.Extension = None
+        self._Id = None
+        self._Name = None
+        self._SourceId = None
+        self._FollowType = None
+        self._IconUrl = None
 
+    @property
+    def Id(self):
+        return self._Id
 
-    def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        self.SceneId = params.get("SceneId")
-        self.UserId = params.get("UserId")
-        if params.get("UserIdList") is not None:
-            self.UserIdList = []
-            for item in params.get("UserIdList"):
-                obj = StrUserIdInfo()
-                obj._deserialize(item)
-                self.UserIdList.append(obj)
-        self.GoodsCnt = params.get("GoodsCnt")
-        self.CurrentGoodsId = params.get("CurrentGoodsId")
-        if params.get("UserPortraitInfo") is not None:
-            self.UserPortraitInfo = UserPortraitInfo()
-            self.UserPortraitInfo._deserialize(params.get("UserPortraitInfo"))
-        self.BlackGoodsList = params.get("BlackGoodsList")
-        self.Extension = params.get("Extension")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
 
+    @property
+    def Name(self):
+        return self._Name
 
-class DescribeGoodsRecommendResponse(AbstractModel):
-    """DescribeGoodsRecommend返回参数结构体
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
 
-    """
+    @property
+    def SourceId(self):
+        return self._SourceId
 
-    def __init__(self):
-        r"""
-        :param DataList: 推荐返回的商品信息列表
-        :type DataList: list of RecGoodsData
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.DataList = None
-        self.RequestId = None
+    @SourceId.setter
+    def SourceId(self, SourceId):
+        self._SourceId = SourceId
 
+    @property
+    def FollowType(self):
+        return self._FollowType
 
-    def _deserialize(self, params):
-        if params.get("DataList") is not None:
-            self.DataList = []
-            for item in params.get("DataList"):
-                obj = RecGoodsData()
-                obj._deserialize(item)
-                self.DataList.append(obj)
-        self.RequestId = params.get("RequestId")
+    @FollowType.setter
+    def FollowType(self, FollowType):
+        self._FollowType = FollowType
 
+    @property
+    def IconUrl(self):
+        return self._IconUrl
 
-class DislikeInfo(AbstractModel):
-    """不喜欢信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Type: 过滤的类别：<br>● author 作者名<br/>（如当前类型不满足，请<a href="https://console.cloud.tencent.com/workorder/category" target="_blank">提单</a>沟通解决方案）
-        :type Type: str
-        :param Value: Type对应字段名的值，如：需要过滤的作者名
-        :type Value: str
-        """
-        self.Type = None
-        self.Value = None
+    @IconUrl.setter
+    def IconUrl(self, IconUrl):
+        self._IconUrl = IconUrl
 
 
     def _deserialize(self, params):
-        self.Type = params.get("Type")
-        self.Value = params.get("Value")
+        self._Id = params.get("Id")
+        self._Name = params.get("Name")
+        self._SourceId = params.get("SourceId")
+        self._FollowType = params.get("FollowType")
+        self._IconUrl = params.get("IconUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DocItem(AbstractModel):
-    """信息流内容
+class DislikeInfo(AbstractModel):
+    """不喜欢信息
 
     """
 
     def __init__(self):
         r"""
-        :param ItemId: 内容唯一id，建议限制在128字符以内
-        :type ItemId: str
-        :param ItemType: 内容类型：<br/>● article -图文<br>● text -纯文本<br/>● video -视频<br/>● short_video -时长15秒以内的视频<br/>● mini_video -竖屏视频<br/>● image -纯图片<br/>（如当前类型不满足，请登录控制台进入对应项目，在<b>物料管理->物料类型管理</b>中添加）
-        :type ItemType: str
-        :param Status: 内容状态：
-● 1 - 上架 
-● 2 - 下架 
-Status=2的内容不会在推荐结果中出现 
-需要下架内容时，把Status的值修改为2即可
-        :type Status: int
-        :param PublishTimestamp: 内容生成时间，秒级时间戳（1639624786），需大于0，<b>用作特征和物料管理</b>
-        :type PublishTimestamp: int
-        :param ExpireTimestamp: 内容过期时间，秒级时间戳（1639624786），如未填，则默认PublishTimestamp往后延一年，用作特征，过期则不会被推荐，<b>强烈建议</b>
-        :type ExpireTimestamp: int
-        :param CategoryLevel: 类目层级数，例如3级类目，则填3，和CategoryPath字段的类数据匹配，<b>强烈建议</b>
-        :type CategoryLevel: int
-        :param CategoryPath: 类目路径，一级二级三级等依次用英文冒号联接，和CategoryLevel字段值匹配，如体育：“足球:巴塞罗那”。<b>用于物料池管理，强烈建议</b>
-        :type CategoryPath: str
-        :param Tags: 内容标签，多个标签用英文冒号联接，<b>用作特征，强烈建议</b>
-        :type Tags: str
-        :param Author: 作者名，需保证作者名唯一，若有重名需要加编号区分。<b>用于召回过滤、规则打散，强烈建议</b>
-        :type Author: str
-        :param SourceId: 内容来源类型，客户自定义，<b>用于物料池管理</b>
-        :type SourceId: str
-        :param Title: 内容标题，<b>主要用于语义分析</b>
-        :type Title: str
-        :param Content: 正文关键片段，建议控制在500字符以内，<b>主要用于语义分析</b>
-        :type Content: str
-        :param ContentUrl: 正文详情，主要用于语义分析，当内容过大时建议用ContentUrl传递，<b>与Content可二选一</b>
-        :type ContentUrl: str
-        :param VideoDuration: 视频时长，时间秒，大于等于0，小于 3600 * 10。<b>视频内容必填，其它内容非必填，用作特征</b>
-        :type VideoDuration: int
-        :param Country: 国家，ISO 3166-1 alpha-2编码，参考<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2" target="_blank">ISO 3166-1 alpha-2</a>，中国：“CN”，<b>用作特征</b>
-        :type Country: str
-        :param Province: 省份，ISO 3166-2行政区编码，如中国参考<a href="https://zh.wikipedia.org/wiki/ISO_3166-2:CN" target="_blank">ISO_3166-2:CN</a>，广东省：“CN-GD”，<b>用作特征</b>
-        :type Province: str
-        :param City: 城市地区，统一用国家最新标准地区行政编码，如：<a href="https://www.mca.gov.cn/article/sj/xzqh/2020/" target="_blank">2020年行政区编码</a>，其他国家统一用国际公认城市简称或者城市编码，<b>用作特征</b>
-        :type City: str
-        :param AuthorFans: 作者粉丝数，<b>用作特征</b>
-        :type AuthorFans: int
-        :param AuthorLevel: 作者评级，<b>用作特征</b>
-        :type AuthorLevel: str
-        :param CollectCnt: 内容累计收藏次数，<b>用作特征</b>
-        :type CollectCnt: int
-        :param PraiseCnt: 内容累积点赞次数，<b>用作特征</b>
-        :type PraiseCnt: int
-        :param CommentCnt: 内容累计评论次数，<b>用作特征</b>
-        :type CommentCnt: int
-        :param ShareCnt: 内容累计分享次数，<b>用作特征</b>
-        :type ShareCnt: int
-        :param RewardCnt: 内容累积打赏数，<b>用作特征</b>
-        :type RewardCnt: int
-        :param Score: 内容质量评分，<b>用作特征</b>
-        :type Score: float
-        :param Extension: json字符串，<b>用于物料池管理的自定义扩展</b>，需要base64加密
-        :type Extension: str
+        :param _Type: 不喜欢的物料类别，对应物料上传协议中的字段名，如authorId，keyword，topic等
+        :type Type: str
+        :param _Value: type对应字段名的值，如具体的topic名，作者id等
+        :type Value: str
         """
-        self.ItemId = None
-        self.ItemType = None
-        self.Status = None
-        self.PublishTimestamp = None
-        self.ExpireTimestamp = None
-        self.CategoryLevel = None
-        self.CategoryPath = None
-        self.Tags = None
-        self.Author = None
-        self.SourceId = None
-        self.Title = None
-        self.Content = None
-        self.ContentUrl = None
-        self.VideoDuration = None
-        self.Country = None
-        self.Province = None
-        self.City = None
-        self.AuthorFans = None
-        self.AuthorLevel = None
-        self.CollectCnt = None
-        self.PraiseCnt = None
-        self.CommentCnt = None
-        self.ShareCnt = None
-        self.RewardCnt = None
-        self.Score = None
-        self.Extension = None
+        self._Type = None
+        self._Value = None
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def Value(self):
+        return self._Value
+
+    @Value.setter
+    def Value(self, Value):
+        self._Value = Value
 
 
     def _deserialize(self, params):
-        self.ItemId = params.get("ItemId")
-        self.ItemType = params.get("ItemType")
-        self.Status = params.get("Status")
-        self.PublishTimestamp = params.get("PublishTimestamp")
-        self.ExpireTimestamp = params.get("ExpireTimestamp")
-        self.CategoryLevel = params.get("CategoryLevel")
-        self.CategoryPath = params.get("CategoryPath")
-        self.Tags = params.get("Tags")
-        self.Author = params.get("Author")
-        self.SourceId = params.get("SourceId")
-        self.Title = params.get("Title")
-        self.Content = params.get("Content")
-        self.ContentUrl = params.get("ContentUrl")
-        self.VideoDuration = params.get("VideoDuration")
-        self.Country = params.get("Country")
-        self.Province = params.get("Province")
-        self.City = params.get("City")
-        self.AuthorFans = params.get("AuthorFans")
-        self.AuthorLevel = params.get("AuthorLevel")
-        self.CollectCnt = params.get("CollectCnt")
-        self.PraiseCnt = params.get("PraiseCnt")
-        self.CommentCnt = params.get("CommentCnt")
-        self.ShareCnt = params.get("ShareCnt")
-        self.RewardCnt = params.get("RewardCnt")
-        self.Score = params.get("Score")
-        self.Extension = params.get("Extension")
+        self._Type = params.get("Type")
+        self._Value = params.get("Value")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class FeedBehaviorInfo(AbstractModel):
-    """信息流行为
+class DocBehavior(AbstractModel):
+    """行为数据
 
     """
 
     def __init__(self):
         r"""
-        :param UserId: 用户唯一ID，客户自定义用户ID，作为一个用户的唯一标识
-        :type UserId: str
-        :param ItemId: 内容唯一id
+        :param _ItemId: 内容唯一ID，如 2824324234
         :type ItemId: str
-        :param BehaviorType: 行为类型：<br> ● expose - 曝光，<b>必须</b><br> ● click - 点击，<b>必须</b><br/>  ● stay - 详情页停留时长，<b>强烈建议</b><br/>  ● videoover - 视频播放时长，<b>强烈建议</b><br/> ●  like - 点赞&喜欢，<b>正效果</b><br/> ● collect - 收藏，<b>正效果</b><br/> ●  share - 转发&分享，<b>正效果</b><br/> ● reward - 打赏，<b>正效果</b><br/> ● unlike - 踩&不喜欢，<b>负效果</b><br/> ●  comment - 评论<br/> 不支持的行为类型，可以映射到未被使用的其他行为类型。如实际业务数据中有私信行为，没有收藏行为，可以将私信行为映射到收藏行为
-        :type BehaviorType: str
-        :param BehaviorValue: 行为类型对应的行为值：<br/> ● expose - 曝光，固定填1<br/> ● click - 点击，固定填1<br/>  ● stay - 详情页停留时长，填停留秒数，取值[1-86400]<br/>  ● videoover - 视频播放时长，填播放结束的秒数，取值[1-86400]<br/> ●  like - 点赞&喜欢，固定填1<br/> ● collect - 收藏，固定填1<br/> ●  share - 转发&分享，固定填1<br/> ● reward - 打赏，填打赏金额，没有则填1<br/> ● unlike - 踩&不喜欢，填不喜欢的原因，没有则填1<br/> ●  comment - 评论，填评论内容，如“上海加油”
+        :param _BehaviorType: 行为类型
+        :type BehaviorType: int
+        :param _BehaviorValue: 行为值
         :type BehaviorValue: str
-        :param BehaviorTimestamp: 行为发生的时间戳： 秒级时间戳，尽量实时上报，最长不超过半小时否则会影响推荐结果的准确性
+        :param _BehaviorTimestamp: 行为时间戳： 秒级时间戳（默认为当前时间）,不能延迟太久，尽量实时上报，否则会影响推荐结果的准确性。
         :type BehaviorTimestamp: int
-        :param SceneId: 行为发生的场景ID，在控制台创建场景后获取
+        :param _SceneId: 场景id，在控制台创建场景后获取。
         :type SceneId: str
-        :param ItemTraceId: 推荐追踪ID，使用推荐结果中返回的ItemTraceId填入。 
-注意：如果和推荐结果中的ItemTraceId不同，会影响行为特征归因，影响推荐算法效果
-        :type ItemTraceId: str
-        :param ItemType: 内容类型，跟内容上报类型一致，用于效果分析，不做内容校验，<b>强烈建议</b>
-        :type ItemType: str
-        :param ReferrerItemId: 相关推荐场景点击进入详情页的内容id，该字段用来注明行为发生于哪个内容的详情页推荐中，<b>相关推荐场景强烈建议</b>
-        :type ReferrerItemId: str
-        :param UserIdList: 用户设备ID数组，可传入用户的多个类型ID，详见UserIdInfo结构体，建议补齐，<b>用于构建用户画像信息</b>
+        :param _UserIdList: 用户id列表
         :type UserIdList: list of UserIdInfo
-        :param Source: 算法来源： <br>● business 业务自己的算法对照组<br/> ● tencent 腾讯算法<br/> ● other 其他算法<br/>默认为tencent，区分行为来源于哪个算法，<b>用于Poc阶段的效果对比验证</b>
+        :param _RecTraceId: 会话id，使用获取推荐结果中返回的RecTraceId填入。<br>注意：如果和在线推荐请求中的traceId不同，会影响行为特征归因，影响推荐算法效果
+        :type RecTraceId: str
+        :param _Source: 算法来源：用来区分行为来源于哪个算法。值为**business，tencent，other** 三者之一<br>● business 表示业务自己的算法对照组<br>● tencent 为腾讯算法<br>● other 为其他算法
         :type Source: str
-        :param Country: 行为发生时的国家，ISO 3166-1 alpha-2编码，参考<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2" target="_blank">ISO 3166-1 alpha-2</a>，中国：“CN”，<b>用作特征</b>
+        :param _ItemType: 物料类型
+        :type ItemType: int
+        :param _AppId: 微信开放平台上查看appId
+        :type AppId: str
+        :param _VideoPlayDuration: 回传video_over事件的时候，回传的用户播放视频的总时长（真正播放的，拖动不算，单位为秒）
+        :type VideoPlayDuration: int
+        :param _ReferrerItemId: 来源物料内容：用来标识在指定内容页面产生的行为，如需要统计用户在A内容详情页里，对推荐内容B点击等行为，则ReferrerItemId代表内容A，ItemId代表内容B
+        :type ReferrerItemId: str
+        :param _Country: 国家，统一用简写，比如中国则填写CN
         :type Country: str
-        :param Province: 行为发生时的省份，ISO 3166-2行政区编码，如中国参考<a href="https://zh.wikipedia.org/wiki/ISO_3166-2:CN" target="_blank">ISO_3166-2:CN</a>，广东省：“CN-GD”，<b>用作特征</b>
+        :param _Province: 省
         :type Province: str
-        :param City: 行为发生时的城市地区，统一用国家最新标准地区行政编码，如：<a href="https://www.mca.gov.cn/article/sj/xzqh/2020/" target="_blank">2020年行政区编码</a>，其他国家统一用国际公认城市简称或者城市编码，<b>用作特征</b>
+        :param _City: 城市
         :type City: str
-        :param IP: 行为发生时的客户端ip，<b>用作特征</b>
+        :param _District: 区县
+        :type District: str
+        :param _IP: 客户端ip
         :type IP: str
-        :param Network: 行为发生时的客户端网络类型，<b>用作特征</b>
+        :param _Network: 客户端网络类型
         :type Network: str
-        :param Platform: 行为发生时的客户端平台，ios/android/h5，<b>用作特征</b>
+        :param _Platform: 客户端平台，ios/android/h5
         :type Platform: str
-        :param AppVersion: 行为发生时的客户端app版本，<b>用作特征</b>
+        :param _AppVersion: 客户端app版本
         :type AppVersion: str
-        :param OsVersion: 行为发生时的操作系统版本，<b>用作特征</b>
+        :param _OsVersion: 操作系统版本
         :type OsVersion: str
-        :param DeviceModel: 行为发生时的机型，<b>用作特征</b>
+        :param _DeviceModel: 机型
         :type DeviceModel: str
-        :param Extension: json字符串，<b>用于行为数据的扩展</b>，需要base64加密
+        :param _Extension: json字符串，用于行为数据的扩展
         :type Extension: str
         """
-        self.UserId = None
-        self.ItemId = None
-        self.BehaviorType = None
-        self.BehaviorValue = None
-        self.BehaviorTimestamp = None
-        self.SceneId = None
-        self.ItemTraceId = None
-        self.ItemType = None
-        self.ReferrerItemId = None
-        self.UserIdList = None
-        self.Source = None
-        self.Country = None
-        self.Province = None
-        self.City = None
-        self.IP = None
-        self.Network = None
-        self.Platform = None
-        self.AppVersion = None
-        self.OsVersion = None
-        self.DeviceModel = None
-        self.Extension = None
-
-
-    def _deserialize(self, params):
-        self.UserId = params.get("UserId")
-        self.ItemId = params.get("ItemId")
-        self.BehaviorType = params.get("BehaviorType")
-        self.BehaviorValue = params.get("BehaviorValue")
-        self.BehaviorTimestamp = params.get("BehaviorTimestamp")
-        self.SceneId = params.get("SceneId")
-        self.ItemTraceId = params.get("ItemTraceId")
-        self.ItemType = params.get("ItemType")
-        self.ReferrerItemId = params.get("ReferrerItemId")
+        self._ItemId = None
+        self._BehaviorType = None
+        self._BehaviorValue = None
+        self._BehaviorTimestamp = None
+        self._SceneId = None
+        self._UserIdList = None
+        self._RecTraceId = None
+        self._Source = None
+        self._ItemType = None
+        self._AppId = None
+        self._VideoPlayDuration = None
+        self._ReferrerItemId = None
+        self._Country = None
+        self._Province = None
+        self._City = None
+        self._District = None
+        self._IP = None
+        self._Network = None
+        self._Platform = None
+        self._AppVersion = None
+        self._OsVersion = None
+        self._DeviceModel = None
+        self._Extension = None
+
+    @property
+    def ItemId(self):
+        return self._ItemId
+
+    @ItemId.setter
+    def ItemId(self, ItemId):
+        self._ItemId = ItemId
+
+    @property
+    def BehaviorType(self):
+        return self._BehaviorType
+
+    @BehaviorType.setter
+    def BehaviorType(self, BehaviorType):
+        self._BehaviorType = BehaviorType
+
+    @property
+    def BehaviorValue(self):
+        return self._BehaviorValue
+
+    @BehaviorValue.setter
+    def BehaviorValue(self, BehaviorValue):
+        self._BehaviorValue = BehaviorValue
+
+    @property
+    def BehaviorTimestamp(self):
+        return self._BehaviorTimestamp
+
+    @BehaviorTimestamp.setter
+    def BehaviorTimestamp(self, BehaviorTimestamp):
+        self._BehaviorTimestamp = BehaviorTimestamp
+
+    @property
+    def SceneId(self):
+        return self._SceneId
+
+    @SceneId.setter
+    def SceneId(self, SceneId):
+        self._SceneId = SceneId
+
+    @property
+    def UserIdList(self):
+        return self._UserIdList
+
+    @UserIdList.setter
+    def UserIdList(self, UserIdList):
+        self._UserIdList = UserIdList
+
+    @property
+    def RecTraceId(self):
+        return self._RecTraceId
+
+    @RecTraceId.setter
+    def RecTraceId(self, RecTraceId):
+        self._RecTraceId = RecTraceId
+
+    @property
+    def Source(self):
+        return self._Source
+
+    @Source.setter
+    def Source(self, Source):
+        self._Source = Source
+
+    @property
+    def ItemType(self):
+        return self._ItemType
+
+    @ItemType.setter
+    def ItemType(self, ItemType):
+        self._ItemType = ItemType
+
+    @property
+    def AppId(self):
+        return self._AppId
+
+    @AppId.setter
+    def AppId(self, AppId):
+        self._AppId = AppId
+
+    @property
+    def VideoPlayDuration(self):
+        return self._VideoPlayDuration
+
+    @VideoPlayDuration.setter
+    def VideoPlayDuration(self, VideoPlayDuration):
+        self._VideoPlayDuration = VideoPlayDuration
+
+    @property
+    def ReferrerItemId(self):
+        return self._ReferrerItemId
+
+    @ReferrerItemId.setter
+    def ReferrerItemId(self, ReferrerItemId):
+        self._ReferrerItemId = ReferrerItemId
+
+    @property
+    def Country(self):
+        return self._Country
+
+    @Country.setter
+    def Country(self, Country):
+        self._Country = Country
+
+    @property
+    def Province(self):
+        return self._Province
+
+    @Province.setter
+    def Province(self, Province):
+        self._Province = Province
+
+    @property
+    def City(self):
+        return self._City
+
+    @City.setter
+    def City(self, City):
+        self._City = City
+
+    @property
+    def District(self):
+        return self._District
+
+    @District.setter
+    def District(self, District):
+        self._District = District
+
+    @property
+    def IP(self):
+        return self._IP
+
+    @IP.setter
+    def IP(self, IP):
+        self._IP = IP
+
+    @property
+    def Network(self):
+        return self._Network
+
+    @Network.setter
+    def Network(self, Network):
+        self._Network = Network
+
+    @property
+    def Platform(self):
+        return self._Platform
+
+    @Platform.setter
+    def Platform(self, Platform):
+        self._Platform = Platform
+
+    @property
+    def AppVersion(self):
+        return self._AppVersion
+
+    @AppVersion.setter
+    def AppVersion(self, AppVersion):
+        self._AppVersion = AppVersion
+
+    @property
+    def OsVersion(self):
+        return self._OsVersion
+
+    @OsVersion.setter
+    def OsVersion(self, OsVersion):
+        self._OsVersion = OsVersion
+
+    @property
+    def DeviceModel(self):
+        return self._DeviceModel
+
+    @DeviceModel.setter
+    def DeviceModel(self, DeviceModel):
+        self._DeviceModel = DeviceModel
+
+    @property
+    def Extension(self):
+        return self._Extension
+
+    @Extension.setter
+    def Extension(self, Extension):
+        self._Extension = Extension
+
+
+    def _deserialize(self, params):
+        self._ItemId = params.get("ItemId")
+        self._BehaviorType = params.get("BehaviorType")
+        self._BehaviorValue = params.get("BehaviorValue")
+        self._BehaviorTimestamp = params.get("BehaviorTimestamp")
+        self._SceneId = params.get("SceneId")
         if params.get("UserIdList") is not None:
-            self.UserIdList = []
+            self._UserIdList = []
             for item in params.get("UserIdList"):
                 obj = UserIdInfo()
                 obj._deserialize(item)
-                self.UserIdList.append(obj)
-        self.Source = params.get("Source")
-        self.Country = params.get("Country")
-        self.Province = params.get("Province")
-        self.City = params.get("City")
-        self.IP = params.get("IP")
-        self.Network = params.get("Network")
-        self.Platform = params.get("Platform")
-        self.AppVersion = params.get("AppVersion")
-        self.OsVersion = params.get("OsVersion")
-        self.DeviceModel = params.get("DeviceModel")
-        self.Extension = params.get("Extension")
+                self._UserIdList.append(obj)
+        self._RecTraceId = params.get("RecTraceId")
+        self._Source = params.get("Source")
+        self._ItemType = params.get("ItemType")
+        self._AppId = params.get("AppId")
+        self._VideoPlayDuration = params.get("VideoPlayDuration")
+        self._ReferrerItemId = params.get("ReferrerItemId")
+        self._Country = params.get("Country")
+        self._Province = params.get("Province")
+        self._City = params.get("City")
+        self._District = params.get("District")
+        self._IP = params.get("IP")
+        self._Network = params.get("Network")
+        self._Platform = params.get("Platform")
+        self._AppVersion = params.get("AppVersion")
+        self._OsVersion = params.get("OsVersion")
+        self._DeviceModel = params.get("DeviceModel")
+        self._Extension = params.get("Extension")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class FeedRecommendRequest(AbstractModel):
-    """FeedRecommend请求参数结构体
+class DocItem(AbstractModel):
+    """推荐物料信息
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID，在控制台获取
-        :type InstanceId: str
-        :param SceneId: 场景ID，在控制台创建场景后获取
-        :type SceneId: str
-        :param UserId: 用户唯一ID，客户自定义用户ID，作为一个用户的唯一标识
-        :type UserId: str
-        :param UserIdList: 用户设备ID数组，可传入用户的多个类型ID，用于关联画像信息
-        :type UserIdList: list of UserIdInfo
-        :param ItemCnt: 推荐返回数量，默认10个，最多支持50个的内容返回。如果有更多数量要求，<a href="https://console.cloud.tencent.com/workorder/category" target="_blank">提单</a>沟通解决
-        :type ItemCnt: int
-        :param CurrentItemId: 当场景是相关推荐时该值必填，场景是非相关推荐时该值无效
-        :type CurrentItemId: str
+        :param _ItemId: 内容唯一id
+        :type ItemId: str
+        :param _ItemType: 内容类型
+        :type ItemType: int
+        :param _Status: 内容状态：1 - 上架， 2 - 下架
+        :type Status: int
+        :param _PublishTimestamp: 内容生成时间，秒级时间戳（1639624786），需大于0
+        :type PublishTimestamp: int
+        :param _SourceId: 物料来源ID
+        :type SourceId: int
+        :param _Title: 标题名称
+        :type Title: str
+        :param _Content: 内容正文
+        :type Content: str
+        :param _Author: 作者
+        :type Author: str
+        :param _AuthorId: 作者id
+        :type AuthorId: str
+        :param _Keyword: 标签关键词，多个用英文分号分割
+        :type Keyword: str
+        :param _Desc: 内容物料描述：物料的描述信息，推荐系统会对内容的描述信息，使用否LP技术，进行分词、提取关键词，作为news的特征使用。
+        :type Desc: str
+        :param _PicUrlList: 图片url
+        :type PicUrlList: list of str
+        :param _VideoUrlList: 视频url
+        :type VideoUrlList: list of str
+        :param _VideoDuration: 视频时长，时间秒
+        :type VideoDuration: int
+        :param _CategoryLevel: 类目层级数，例如3级类目，则填3，和CategoryPath字段的类数据匹配
+        :type CategoryLevel: int
+        :param _CategoryPath: 类目路径，一级二级三级等依次用英文冒号联接，如体育：“足球:巴塞罗那”
+        :type CategoryPath: str
+        :param _Country: 国家，统一用简写，比如中国则填写CN
+        :type Country: str
+        :param _Province: 省
+        :type Province: str
+        :param _City: 城市
+        :type City: str
+        :param _District: 区县
+        :type District: str
+        :param _ExpireTimestamp: 内容过期时间，秒级时间戳（1639624786），如未填，则默认PublishTimestamp往后延一年
+        :type ExpireTimestamp: int
+        :param _Topic: 所属话题
+        :type Topic: str
+        :param _AuthorFans: 作者粉丝数
+        :type AuthorFans: int
+        :param _AuthorLevel: 作者评级
+        :type AuthorLevel: str
+        :param _CollectCnt: 内容累计收藏次数
+        :type CollectCnt: int
+        :param _PraiseCnt: 内容累积点赞次数
+        :type PraiseCnt: int
+        :param _CommentCnt: 内容累计评论次数
+        :type CommentCnt: int
+        :param _ShareCnt: 内容累计分享次数
+        :type ShareCnt: int
+        :param _RewardCnt: 内容累积打赏数
+        :type RewardCnt: int
+        :param _Score: 内容质量评分，类似豆瓣电影的评分，这里为100分制，比如97分，满分100分，最低0分，范围外的将会被拦截
+        :type Score: float
+        :param _PoolIdList: 内容池id，用于分内容池召回，一个内容支持指定一个或多个内容池， 内容池id不建议使用0（0表示不区分内容池）
+        :type PoolIdList: list of str
+        :param _TagInfoList: 描述用户标签
+        :type TagInfoList: list of TagInfo
+        :param _Extension: json字符串，用于物料数据的扩展
+        :type Extension: str
         """
-        self.InstanceId = None
-        self.SceneId = None
-        self.UserId = None
-        self.UserIdList = None
-        self.ItemCnt = None
-        self.CurrentItemId = None
-
-
-    def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        self.SceneId = params.get("SceneId")
-        self.UserId = params.get("UserId")
-        if params.get("UserIdList") is not None:
-            self.UserIdList = []
-            for item in params.get("UserIdList"):
-                obj = UserIdInfo()
+        self._ItemId = None
+        self._ItemType = None
+        self._Status = None
+        self._PublishTimestamp = None
+        self._SourceId = None
+        self._Title = None
+        self._Content = None
+        self._Author = None
+        self._AuthorId = None
+        self._Keyword = None
+        self._Desc = None
+        self._PicUrlList = None
+        self._VideoUrlList = None
+        self._VideoDuration = None
+        self._CategoryLevel = None
+        self._CategoryPath = None
+        self._Country = None
+        self._Province = None
+        self._City = None
+        self._District = None
+        self._ExpireTimestamp = None
+        self._Topic = None
+        self._AuthorFans = None
+        self._AuthorLevel = None
+        self._CollectCnt = None
+        self._PraiseCnt = None
+        self._CommentCnt = None
+        self._ShareCnt = None
+        self._RewardCnt = None
+        self._Score = None
+        self._PoolIdList = None
+        self._TagInfoList = None
+        self._Extension = None
+
+    @property
+    def ItemId(self):
+        return self._ItemId
+
+    @ItemId.setter
+    def ItemId(self, ItemId):
+        self._ItemId = ItemId
+
+    @property
+    def ItemType(self):
+        return self._ItemType
+
+    @ItemType.setter
+    def ItemType(self, ItemType):
+        self._ItemType = ItemType
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def PublishTimestamp(self):
+        return self._PublishTimestamp
+
+    @PublishTimestamp.setter
+    def PublishTimestamp(self, PublishTimestamp):
+        self._PublishTimestamp = PublishTimestamp
+
+    @property
+    def SourceId(self):
+        return self._SourceId
+
+    @SourceId.setter
+    def SourceId(self, SourceId):
+        self._SourceId = SourceId
+
+    @property
+    def Title(self):
+        return self._Title
+
+    @Title.setter
+    def Title(self, Title):
+        self._Title = Title
+
+    @property
+    def Content(self):
+        return self._Content
+
+    @Content.setter
+    def Content(self, Content):
+        self._Content = Content
+
+    @property
+    def Author(self):
+        return self._Author
+
+    @Author.setter
+    def Author(self, Author):
+        self._Author = Author
+
+    @property
+    def AuthorId(self):
+        return self._AuthorId
+
+    @AuthorId.setter
+    def AuthorId(self, AuthorId):
+        self._AuthorId = AuthorId
+
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
+    @property
+    def Desc(self):
+        return self._Desc
+
+    @Desc.setter
+    def Desc(self, Desc):
+        self._Desc = Desc
+
+    @property
+    def PicUrlList(self):
+        return self._PicUrlList
+
+    @PicUrlList.setter
+    def PicUrlList(self, PicUrlList):
+        self._PicUrlList = PicUrlList
+
+    @property
+    def VideoUrlList(self):
+        return self._VideoUrlList
+
+    @VideoUrlList.setter
+    def VideoUrlList(self, VideoUrlList):
+        self._VideoUrlList = VideoUrlList
+
+    @property
+    def VideoDuration(self):
+        return self._VideoDuration
+
+    @VideoDuration.setter
+    def VideoDuration(self, VideoDuration):
+        self._VideoDuration = VideoDuration
+
+    @property
+    def CategoryLevel(self):
+        return self._CategoryLevel
+
+    @CategoryLevel.setter
+    def CategoryLevel(self, CategoryLevel):
+        self._CategoryLevel = CategoryLevel
+
+    @property
+    def CategoryPath(self):
+        return self._CategoryPath
+
+    @CategoryPath.setter
+    def CategoryPath(self, CategoryPath):
+        self._CategoryPath = CategoryPath
+
+    @property
+    def Country(self):
+        return self._Country
+
+    @Country.setter
+    def Country(self, Country):
+        self._Country = Country
+
+    @property
+    def Province(self):
+        return self._Province
+
+    @Province.setter
+    def Province(self, Province):
+        self._Province = Province
+
+    @property
+    def City(self):
+        return self._City
+
+    @City.setter
+    def City(self, City):
+        self._City = City
+
+    @property
+    def District(self):
+        return self._District
+
+    @District.setter
+    def District(self, District):
+        self._District = District
+
+    @property
+    def ExpireTimestamp(self):
+        return self._ExpireTimestamp
+
+    @ExpireTimestamp.setter
+    def ExpireTimestamp(self, ExpireTimestamp):
+        self._ExpireTimestamp = ExpireTimestamp
+
+    @property
+    def Topic(self):
+        return self._Topic
+
+    @Topic.setter
+    def Topic(self, Topic):
+        self._Topic = Topic
+
+    @property
+    def AuthorFans(self):
+        return self._AuthorFans
+
+    @AuthorFans.setter
+    def AuthorFans(self, AuthorFans):
+        self._AuthorFans = AuthorFans
+
+    @property
+    def AuthorLevel(self):
+        return self._AuthorLevel
+
+    @AuthorLevel.setter
+    def AuthorLevel(self, AuthorLevel):
+        self._AuthorLevel = AuthorLevel
+
+    @property
+    def CollectCnt(self):
+        return self._CollectCnt
+
+    @CollectCnt.setter
+    def CollectCnt(self, CollectCnt):
+        self._CollectCnt = CollectCnt
+
+    @property
+    def PraiseCnt(self):
+        return self._PraiseCnt
+
+    @PraiseCnt.setter
+    def PraiseCnt(self, PraiseCnt):
+        self._PraiseCnt = PraiseCnt
+
+    @property
+    def CommentCnt(self):
+        return self._CommentCnt
+
+    @CommentCnt.setter
+    def CommentCnt(self, CommentCnt):
+        self._CommentCnt = CommentCnt
+
+    @property
+    def ShareCnt(self):
+        return self._ShareCnt
+
+    @ShareCnt.setter
+    def ShareCnt(self, ShareCnt):
+        self._ShareCnt = ShareCnt
+
+    @property
+    def RewardCnt(self):
+        return self._RewardCnt
+
+    @RewardCnt.setter
+    def RewardCnt(self, RewardCnt):
+        self._RewardCnt = RewardCnt
+
+    @property
+    def Score(self):
+        return self._Score
+
+    @Score.setter
+    def Score(self, Score):
+        self._Score = Score
+
+    @property
+    def PoolIdList(self):
+        return self._PoolIdList
+
+    @PoolIdList.setter
+    def PoolIdList(self, PoolIdList):
+        self._PoolIdList = PoolIdList
+
+    @property
+    def TagInfoList(self):
+        return self._TagInfoList
+
+    @TagInfoList.setter
+    def TagInfoList(self, TagInfoList):
+        self._TagInfoList = TagInfoList
+
+    @property
+    def Extension(self):
+        return self._Extension
+
+    @Extension.setter
+    def Extension(self, Extension):
+        self._Extension = Extension
+
+
+    def _deserialize(self, params):
+        self._ItemId = params.get("ItemId")
+        self._ItemType = params.get("ItemType")
+        self._Status = params.get("Status")
+        self._PublishTimestamp = params.get("PublishTimestamp")
+        self._SourceId = params.get("SourceId")
+        self._Title = params.get("Title")
+        self._Content = params.get("Content")
+        self._Author = params.get("Author")
+        self._AuthorId = params.get("AuthorId")
+        self._Keyword = params.get("Keyword")
+        self._Desc = params.get("Desc")
+        self._PicUrlList = params.get("PicUrlList")
+        self._VideoUrlList = params.get("VideoUrlList")
+        self._VideoDuration = params.get("VideoDuration")
+        self._CategoryLevel = params.get("CategoryLevel")
+        self._CategoryPath = params.get("CategoryPath")
+        self._Country = params.get("Country")
+        self._Province = params.get("Province")
+        self._City = params.get("City")
+        self._District = params.get("District")
+        self._ExpireTimestamp = params.get("ExpireTimestamp")
+        self._Topic = params.get("Topic")
+        self._AuthorFans = params.get("AuthorFans")
+        self._AuthorLevel = params.get("AuthorLevel")
+        self._CollectCnt = params.get("CollectCnt")
+        self._PraiseCnt = params.get("PraiseCnt")
+        self._CommentCnt = params.get("CommentCnt")
+        self._ShareCnt = params.get("ShareCnt")
+        self._RewardCnt = params.get("RewardCnt")
+        self._Score = params.get("Score")
+        self._PoolIdList = params.get("PoolIdList")
+        if params.get("TagInfoList") is not None:
+            self._TagInfoList = []
+            for item in params.get("TagInfoList"):
+                obj = TagInfo()
                 obj._deserialize(item)
-                self.UserIdList.append(obj)
-        self.ItemCnt = params.get("ItemCnt")
-        self.CurrentItemId = params.get("CurrentItemId")
+                self._TagInfoList.append(obj)
+        self._Extension = params.get("Extension")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class FeedRecommendResponse(AbstractModel):
-    """FeedRecommend返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param DataList: 推荐返回的内容信息列表
-        :type DataList: list of RecItemData
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.DataList = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        if params.get("DataList") is not None:
-            self.DataList = []
-            for item in params.get("DataList"):
-                obj = RecItemData()
-                obj._deserialize(item)
-                self.DataList.append(obj)
-        self.RequestId = params.get("RequestId")
-
-
-class FeedUserInfo(AbstractModel):
-    """信息流用户信息
+class PortraitInfo(AbstractModel):
+    """画像信息
 
     """
 
     def __init__(self):
         r"""
-        :param UserId: 用户唯一ID，客户自定义用户ID，作为一个用户的唯一标识
-        :type UserId: str
-        :param UserIdList: 用户设备ID数组，可传入用户的多个类型ID，详见UserIdInfo结构体，建议补齐，<b>用于构建用户画像信息</b>
+        :param _UserIdList: 用户id列表
         :type UserIdList: list of UserIdInfo
-        :param Tags: 用户标签，多个标签用英文冒号联接，<b>用作特征，强烈建议</b>
-        :type Tags: str
-        :param DislikeInfoList: 过滤列表，<b>会在推荐结果里过滤掉这类内容</b>
-        :type DislikeInfoList: list of DislikeInfo
-        :param Age: 用户年龄
+        :param _AppId: 如果"userIdType"是10则必传，在微信开放平台上查看appId
+        :type AppId: str
+        :param _Age: 用户年龄，值域在 0-200
         :type Age: int
-        :param Gender: 用户性别： 0 - 未知 1 - 男 2 - 女
+        :param _Gender: 用户性别：0-未知，1-男， 2-女
         :type Gender: int
-        :param Degree: 用户学历 ：小学，初中，高中，大专，本科，硕士，博士
+        :param _Degree: 用户学历 ：小学，初中，高中，大专，本科，硕士，博士
         :type Degree: str
-        :param School: 用户毕业学校全称
+        :param _School: 用户毕业学校全称
         :type School: str
-        :param Occupation: 用户职业
+        :param _Occupation: 用户职业，保证业务的唯一性
         :type Occupation: str
-        :param Industry: 用户所属行业
+        :param _Industry: 用户所属行业，保证业务的唯一性
         :type Industry: str
-        :param ResidentCountry: 用户常驻国家，ISO 3166-1 alpha-2编码，参考<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2" target="_blank">ISO 3166-1 alpha-2</a>，中国：“CN”
+        :param _ResidentCountry: 用户常驻国家，统一用简写，比如中国则填写CN
         :type ResidentCountry: str
-        :param ResidentProvince: 用户常驻省份，ISO 3166-2行政区编码，如中国参考<a href="https://zh.wikipedia.org/wiki/ISO_3166-2:CN" target="_blank">ISO_3166-2:CN</a>，广东省：“CN-GD”
+        :param _ResidentProvince: 用户常驻省份
         :type ResidentProvince: str
-        :param ResidentCity: 用户常驻城市，统一用国家最新标准地区行政编码，如：<a href="https://www.mca.gov.cn/article/sj/xzqh/2020/" target="_blank">2020年行政区编码</a>，
+        :param _ResidentCity: 用户常驻城市
         :type ResidentCity: str
-        :param RegisterTimestamp: 用户注册时间，秒级时间戳（1639624786）
+        :param _ResidentDistrict: 用户常驻区县
+        :type ResidentDistrict: str
+        :param _PhoneMd5: 用户手机的MD5值
+        :type PhoneMd5: str
+        :param _PhoneImei: 用户手机的IMEI号
+        :type PhoneImei: str
+        :param _Idfa: 设备idfa信息
+        :type Idfa: str
+        :param _RegisterTimestamp: 用户注册时间，秒级时间戳（1639624786）
         :type RegisterTimestamp: int
-        :param MembershipLevel: 用户会员等级
+        :param _MembershipLevel: 用户会员等级
         :type MembershipLevel: str
-        :param LastLoginTimestamp: 用户上一次登录时间，秒级时间戳（1639624786）
+        :param _LastLoginTimestamp: 用户上一次登录时间，秒级时间戳（1639624786）
         :type LastLoginTimestamp: int
-        :param LastLoginIp: 用户上一次登录的ip
+        :param _LastLoginIp: 用户上一次登录的ip
         :type LastLoginIp: str
-        :param LastModifyTimestamp: 用户信息的最后修改时间戳，秒级时间戳（1639624786）
+        :param _LastModifyTimestamp: 用户信息的最后修改时间戳，秒级时间戳（1639624786）
         :type LastModifyTimestamp: int
-        :param Extension: json字符串，用于画像数据的扩展，需要base64加密
+        :param _TagInfoList: 用户标签
+        :type TagInfoList: list of TagInfo
+        :param _AuthorInfoList: 用户关注作者列表
+        :type AuthorInfoList: list of AuthorInfo
+        :param _DislikeInfoList: 用户不喜欢列表
+        :type DislikeInfoList: list of DislikeInfo
+        :param _Extension: json字符串，用于画像数据的扩展
         :type Extension: str
-        """
-        self.UserId = None
-        self.UserIdList = None
-        self.Tags = None
-        self.DislikeInfoList = None
-        self.Age = None
-        self.Gender = None
-        self.Degree = None
-        self.School = None
-        self.Occupation = None
-        self.Industry = None
-        self.ResidentCountry = None
-        self.ResidentProvince = None
-        self.ResidentCity = None
-        self.RegisterTimestamp = None
-        self.MembershipLevel = None
-        self.LastLoginTimestamp = None
-        self.LastLoginIp = None
-        self.LastModifyTimestamp = None
-        self.Extension = None
+        :param _Oaid: 设备oaid信息
+        :type Oaid: str
+        :param _AndroidId: 设备AndroidId信息
+        :type AndroidId: str
+        """
+        self._UserIdList = None
+        self._AppId = None
+        self._Age = None
+        self._Gender = None
+        self._Degree = None
+        self._School = None
+        self._Occupation = None
+        self._Industry = None
+        self._ResidentCountry = None
+        self._ResidentProvince = None
+        self._ResidentCity = None
+        self._ResidentDistrict = None
+        self._PhoneMd5 = None
+        self._PhoneImei = None
+        self._Idfa = None
+        self._RegisterTimestamp = None
+        self._MembershipLevel = None
+        self._LastLoginTimestamp = None
+        self._LastLoginIp = None
+        self._LastModifyTimestamp = None
+        self._TagInfoList = None
+        self._AuthorInfoList = None
+        self._DislikeInfoList = None
+        self._Extension = None
+        self._Oaid = None
+        self._AndroidId = None
+
+    @property
+    def UserIdList(self):
+        return self._UserIdList
+
+    @UserIdList.setter
+    def UserIdList(self, UserIdList):
+        self._UserIdList = UserIdList
+
+    @property
+    def AppId(self):
+        return self._AppId
+
+    @AppId.setter
+    def AppId(self, AppId):
+        self._AppId = AppId
+
+    @property
+    def Age(self):
+        return self._Age
+
+    @Age.setter
+    def Age(self, Age):
+        self._Age = Age
+
+    @property
+    def Gender(self):
+        return self._Gender
+
+    @Gender.setter
+    def Gender(self, Gender):
+        self._Gender = Gender
+
+    @property
+    def Degree(self):
+        return self._Degree
+
+    @Degree.setter
+    def Degree(self, Degree):
+        self._Degree = Degree
+
+    @property
+    def School(self):
+        return self._School
+
+    @School.setter
+    def School(self, School):
+        self._School = School
+
+    @property
+    def Occupation(self):
+        return self._Occupation
+
+    @Occupation.setter
+    def Occupation(self, Occupation):
+        self._Occupation = Occupation
+
+    @property
+    def Industry(self):
+        return self._Industry
+
+    @Industry.setter
+    def Industry(self, Industry):
+        self._Industry = Industry
+
+    @property
+    def ResidentCountry(self):
+        return self._ResidentCountry
+
+    @ResidentCountry.setter
+    def ResidentCountry(self, ResidentCountry):
+        self._ResidentCountry = ResidentCountry
+
+    @property
+    def ResidentProvince(self):
+        return self._ResidentProvince
+
+    @ResidentProvince.setter
+    def ResidentProvince(self, ResidentProvince):
+        self._ResidentProvince = ResidentProvince
+
+    @property
+    def ResidentCity(self):
+        return self._ResidentCity
+
+    @ResidentCity.setter
+    def ResidentCity(self, ResidentCity):
+        self._ResidentCity = ResidentCity
+
+    @property
+    def ResidentDistrict(self):
+        return self._ResidentDistrict
+
+    @ResidentDistrict.setter
+    def ResidentDistrict(self, ResidentDistrict):
+        self._ResidentDistrict = ResidentDistrict
+
+    @property
+    def PhoneMd5(self):
+        return self._PhoneMd5
+
+    @PhoneMd5.setter
+    def PhoneMd5(self, PhoneMd5):
+        self._PhoneMd5 = PhoneMd5
+
+    @property
+    def PhoneImei(self):
+        return self._PhoneImei
+
+    @PhoneImei.setter
+    def PhoneImei(self, PhoneImei):
+        self._PhoneImei = PhoneImei
+
+    @property
+    def Idfa(self):
+        return self._Idfa
+
+    @Idfa.setter
+    def Idfa(self, Idfa):
+        self._Idfa = Idfa
+
+    @property
+    def RegisterTimestamp(self):
+        return self._RegisterTimestamp
+
+    @RegisterTimestamp.setter
+    def RegisterTimestamp(self, RegisterTimestamp):
+        self._RegisterTimestamp = RegisterTimestamp
+
+    @property
+    def MembershipLevel(self):
+        return self._MembershipLevel
+
+    @MembershipLevel.setter
+    def MembershipLevel(self, MembershipLevel):
+        self._MembershipLevel = MembershipLevel
+
+    @property
+    def LastLoginTimestamp(self):
+        return self._LastLoginTimestamp
+
+    @LastLoginTimestamp.setter
+    def LastLoginTimestamp(self, LastLoginTimestamp):
+        self._LastLoginTimestamp = LastLoginTimestamp
+
+    @property
+    def LastLoginIp(self):
+        return self._LastLoginIp
+
+    @LastLoginIp.setter
+    def LastLoginIp(self, LastLoginIp):
+        self._LastLoginIp = LastLoginIp
+
+    @property
+    def LastModifyTimestamp(self):
+        return self._LastModifyTimestamp
+
+    @LastModifyTimestamp.setter
+    def LastModifyTimestamp(self, LastModifyTimestamp):
+        self._LastModifyTimestamp = LastModifyTimestamp
+
+    @property
+    def TagInfoList(self):
+        return self._TagInfoList
+
+    @TagInfoList.setter
+    def TagInfoList(self, TagInfoList):
+        self._TagInfoList = TagInfoList
+
+    @property
+    def AuthorInfoList(self):
+        return self._AuthorInfoList
+
+    @AuthorInfoList.setter
+    def AuthorInfoList(self, AuthorInfoList):
+        self._AuthorInfoList = AuthorInfoList
+
+    @property
+    def DislikeInfoList(self):
+        return self._DislikeInfoList
+
+    @DislikeInfoList.setter
+    def DislikeInfoList(self, DislikeInfoList):
+        self._DislikeInfoList = DislikeInfoList
+
+    @property
+    def Extension(self):
+        return self._Extension
+
+    @Extension.setter
+    def Extension(self, Extension):
+        self._Extension = Extension
+
+    @property
+    def Oaid(self):
+        return self._Oaid
+
+    @Oaid.setter
+    def Oaid(self, Oaid):
+        self._Oaid = Oaid
+
+    @property
+    def AndroidId(self):
+        return self._AndroidId
+
+    @AndroidId.setter
+    def AndroidId(self, AndroidId):
+        self._AndroidId = AndroidId
 
 
     def _deserialize(self, params):
-        self.UserId = params.get("UserId")
         if params.get("UserIdList") is not None:
-            self.UserIdList = []
+            self._UserIdList = []
             for item in params.get("UserIdList"):
                 obj = UserIdInfo()
                 obj._deserialize(item)
-                self.UserIdList.append(obj)
-        self.Tags = params.get("Tags")
+                self._UserIdList.append(obj)
+        self._AppId = params.get("AppId")
+        self._Age = params.get("Age")
+        self._Gender = params.get("Gender")
+        self._Degree = params.get("Degree")
+        self._School = params.get("School")
+        self._Occupation = params.get("Occupation")
+        self._Industry = params.get("Industry")
+        self._ResidentCountry = params.get("ResidentCountry")
+        self._ResidentProvince = params.get("ResidentProvince")
+        self._ResidentCity = params.get("ResidentCity")
+        self._ResidentDistrict = params.get("ResidentDistrict")
+        self._PhoneMd5 = params.get("PhoneMd5")
+        self._PhoneImei = params.get("PhoneImei")
+        self._Idfa = params.get("Idfa")
+        self._RegisterTimestamp = params.get("RegisterTimestamp")
+        self._MembershipLevel = params.get("MembershipLevel")
+        self._LastLoginTimestamp = params.get("LastLoginTimestamp")
+        self._LastLoginIp = params.get("LastLoginIp")
+        self._LastModifyTimestamp = params.get("LastModifyTimestamp")
+        if params.get("TagInfoList") is not None:
+            self._TagInfoList = []
+            for item in params.get("TagInfoList"):
+                obj = TagInfo()
+                obj._deserialize(item)
+                self._TagInfoList.append(obj)
+        if params.get("AuthorInfoList") is not None:
+            self._AuthorInfoList = []
+            for item in params.get("AuthorInfoList"):
+                obj = AuthorInfo()
+                obj._deserialize(item)
+                self._AuthorInfoList.append(obj)
         if params.get("DislikeInfoList") is not None:
-            self.DislikeInfoList = []
+            self._DislikeInfoList = []
             for item in params.get("DislikeInfoList"):
                 obj = DislikeInfo()
                 obj._deserialize(item)
-                self.DislikeInfoList.append(obj)
-        self.Age = params.get("Age")
-        self.Gender = params.get("Gender")
-        self.Degree = params.get("Degree")
-        self.School = params.get("School")
-        self.Occupation = params.get("Occupation")
-        self.Industry = params.get("Industry")
-        self.ResidentCountry = params.get("ResidentCountry")
-        self.ResidentProvince = params.get("ResidentProvince")
-        self.ResidentCity = params.get("ResidentCity")
-        self.RegisterTimestamp = params.get("RegisterTimestamp")
-        self.MembershipLevel = params.get("MembershipLevel")
-        self.LastLoginTimestamp = params.get("LastLoginTimestamp")
-        self.LastLoginIp = params.get("LastLoginIp")
-        self.LastModifyTimestamp = params.get("LastModifyTimestamp")
-        self.Extension = params.get("Extension")
+                self._DislikeInfoList.append(obj)
+        self._Extension = params.get("Extension")
+        self._Oaid = params.get("Oaid")
+        self._AndroidId = params.get("AndroidId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class GoodsBehaviorInfo(AbstractModel):
-    """电商行为
+class RecItemData(AbstractModel):
+    """推荐内容信息
 
     """
 
     def __init__(self):
         r"""
-        :param UserId: 用户唯一ID，客户自定义用户ID，作为一个用户的唯一标识
-        :type UserId: str
-        :param GoodsId: 商品唯一ID，skuId或spuId，客户根据需求自行决定商品主键粒度
-        :type GoodsId: str
-        :param BehaviorType: 行为类型：<br> ● expose - 曝光，<b>必须</b><br> ● click - 点击，<b>必须</b><br/>  ● stay - 详情页停留时长，<b>强烈建议</b><br/>  ● videoover - 视频播放时长，<b>强烈建议</b><br/> ●  like - 点赞&喜欢，<b>正效果</b><br/> ● collect - 收藏，<b>正效果</b><br/> ●  share - 转发&分享，<b>正效果</b><br/> ● reward - 打赏，<b>正效果</b><br/> ● unlike - 踩&不喜欢，<b>负效果</b><br/> ●  comment - 评论<br/> ●  order - 下单<br/> ●  buy - 购买成功<br/> ●  addcart - 加入购物车<br/>   
-不支持的行为类型，可以映射到未被使用的其他行为类型。如实际业务数据中有私信行为，没有收藏行为，可以将私信行为映射到收藏行为
-        :type BehaviorType: str
-        :param BehaviorValue: 行为类型对应的行为值：<br/> ● expose - 曝光，固定填1<br/> ● click - 点击，固定填1<br/>  ● stay - 详情页停留时长，填停留秒数，取值[1-86400]<br/>  ● videoover - 视频播放时长，填播放结束的秒数，取值[1-86400]<br/> ●  like - 点赞&喜欢，固定填1<br/> ● collect - 收藏，固定填1<br/> ●  share - 转发&分享，固定填1<br/> ● reward - 打赏，填打赏金额，没有则填1<br/> ● unlike - 踩&不喜欢，填不喜欢的原因，没有则填1<br/> ●  comment - 评论，填评论内容，如“上海加油”<br/> ●  order - 下单，固定填1<br/> ●  buy - 购买成功，固定填1<br/> ●  addcart - 加入购物车，固定填1
-        :type BehaviorValue: str
-        :param BehaviorTimestamp: 行为发生的时间戳： 秒级时间戳，尽量实时上报，最长不超过半小时否则会影响推荐结果的准确性
-        :type BehaviorTimestamp: int
-        :param SceneId: 行为发生的场景ID，在控制台创建场景后获取
-        :type SceneId: str
-        :param Source: 算法来源： <br>● business 业务自己的算法对照组<br/> ● tencent 腾讯算法<br/> ● other 其他算法<br/>默认为tencent，区分行为来源于哪个算法，<b>用于Poc阶段的效果对比验证</b>
-        :type Source: str
-        :param Page: 标识行为发生在app内哪个页面，取值客户自定，可以是明文或id，建议传明文便于理解、分析，如首页，发现页，用户中心等
-<b>用作上下文特征，刻画不同场景用户行为分布的差异</b>
-        :type Page: str
-        :param Module: 标识行为发生在页面的哪一区块，取值客户自定，可以是明文或id，建议传明文便于理解、分析，如横幅、广告位、猜你喜欢等
-<b>用作上下文特征，刻画不同模块用户行为分布的差异</b>
-        :type Module: str
-        :param GoodsTraceId: 推荐追踪ID，使用推荐结果中返回的GoodsTraceId填入。 
-注意：如果和推荐结果中的GoodsTraceId不同，会影响行为特征归因，影响推荐算法效果。<b>强烈建议</b>
-        :type GoodsTraceId: str
-        :param ReferrerGoodsId: 相关推荐场景点击进入详情页的内容id，该字段用来注明行为发生于哪个内容的详情页推荐中，<b>相关推荐场景强烈建议</b>
-        :type ReferrerGoodsId: str
-        :param OrderGoodsCnt: 订单商品购买个数，当behaviorType=order，buy或addcart时有值，<b>用作特征</b>
-        :type OrderGoodsCnt: int
-        :param OrderAmount: 订单总金额，当behaviorType=order或buy时有值（单位：元，统一货币体系，如统一为RMB，美元等），<b>用作特征</b>
-        :type OrderAmount: float
-        :param UserIdList: 用户设备ID数组，可传入用户的多个类型ID，详见UserIdInfo结构体，建议补齐，<b>用于构建用户画像信息</b>
-        :type UserIdList: list of StrUserIdInfo
-        :param UserPortraitInfo: 行为发生时用户基础特征信息，<b>用作特征</b>
-        :type UserPortraitInfo: :class:`tencentcloud.irp.v20220805.models.UserPortraitInfo`
-        :param Position: 标识行为发生在模块内的具体位置，如1、2、...
-<b>用作上下文特征，刻画不同位置用户行为分布的差异</b>
-        :type Position: int
-        :param Extension: json字符串，<b>用于行为数据的扩展</b>
-        :type Extension: str
+        :param _ItemId: 推荐的内容id，即用户行为上报中的itemId
+        :type ItemId: str
+        :param _ItemType: 物料子类型，包括如下： 1-图文、2-长视频（横视频）、3-短视频（横视频）、4-小说、5-小视频（竖视频）、6-纯文本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ItemType: int
+        :param _Weight: 推荐内容的权重，取值范围[0,1000000]
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Weight: int
+        :param _Score: 推荐预测分
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Score: float
+        :param _Keyword: 关键词，多个用英文分号分割，和物料上传的keyword一致
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Keyword: str
         """
-        self.UserId = None
-        self.GoodsId = None
-        self.BehaviorType = None
-        self.BehaviorValue = None
-        self.BehaviorTimestamp = None
-        self.SceneId = None
-        self.Source = None
-        self.Page = None
-        self.Module = None
-        self.GoodsTraceId = None
-        self.ReferrerGoodsId = None
-        self.OrderGoodsCnt = None
-        self.OrderAmount = None
-        self.UserIdList = None
-        self.UserPortraitInfo = None
-        self.Position = None
-        self.Extension = None
+        self._ItemId = None
+        self._ItemType = None
+        self._Weight = None
+        self._Score = None
+        self._Keyword = None
 
+    @property
+    def ItemId(self):
+        return self._ItemId
 
-    def _deserialize(self, params):
-        self.UserId = params.get("UserId")
-        self.GoodsId = params.get("GoodsId")
-        self.BehaviorType = params.get("BehaviorType")
-        self.BehaviorValue = params.get("BehaviorValue")
-        self.BehaviorTimestamp = params.get("BehaviorTimestamp")
-        self.SceneId = params.get("SceneId")
-        self.Source = params.get("Source")
-        self.Page = params.get("Page")
-        self.Module = params.get("Module")
-        self.GoodsTraceId = params.get("GoodsTraceId")
-        self.ReferrerGoodsId = params.get("ReferrerGoodsId")
-        self.OrderGoodsCnt = params.get("OrderGoodsCnt")
-        self.OrderAmount = params.get("OrderAmount")
-        if params.get("UserIdList") is not None:
-            self.UserIdList = []
-            for item in params.get("UserIdList"):
-                obj = StrUserIdInfo()
-                obj._deserialize(item)
-                self.UserIdList.append(obj)
-        if params.get("UserPortraitInfo") is not None:
-            self.UserPortraitInfo = UserPortraitInfo()
-            self.UserPortraitInfo._deserialize(params.get("UserPortraitInfo"))
-        self.Position = params.get("Position")
-        self.Extension = params.get("Extension")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+    @ItemId.setter
+    def ItemId(self, ItemId):
+        self._ItemId = ItemId
 
+    @property
+    def ItemType(self):
+        return self._ItemType
 
-class GoodsInfo(AbstractModel):
-    """电商物料内容
+    @ItemType.setter
+    def ItemType(self, ItemType):
+        self._ItemType = ItemType
 
-    """
+    @property
+    def Weight(self):
+        return self._Weight
 
-    def __init__(self):
-        r"""
-        :param GoodsId: 商品唯一ID，skuId或spuId，客户根据需求自行决定商品主键粒度。建议限制在128字符以内
-        :type GoodsId: str
-        :param GoodsType: 商品物料展示类型：<br/>● article -图文<br>● text -纯文本<br/>● video -视频<br/>● short_video -时长15秒以内的视频<br/>● mini_video -竖屏视频<br/>● image -纯图片<br/>（如当前类型不满足，请<a href="https://console.cloud.tencent.com/workorder/category" target="_blank">提单</a>沟通解决方案）
-        :type GoodsType: str
-        :param Status: 商品状态：
-● 1 - 上架 
-● 2 - 下架 
-Status=2的内容不会在推荐结果中出现 
-需要下架内容时，把Status的值修改为2即可
-        :type Status: int
-        :param PublishTimestamp: 商品生成时间，秒级时间戳（1639624786），需大于0，<b>用作特征和物料管理</b>
-        :type PublishTimestamp: int
-        :param ExpireTimestamp: 商品过期时间，秒级时间戳（1639624786），如未填，则默认PublishTimestamp往后延一年，<b>用作特征</b>，过期则不会被推荐，<b>强烈建议</b>
-        :type ExpireTimestamp: int
-        :param SpuId: spu((Standard Product Unit))维度id，商品聚合信息的最小单位，<b>强烈建议</b>
-        :type SpuId: str
-        :param CategoryLevel: 类目层级数，例如3级类目，则填3，和CategoryPath字段的类数据匹配，<b>强烈建议</b>
-        :type CategoryLevel: int
-        :param CategoryPath: 类目路径，一级二级三级等依次用英文冒号联接，和CategoryLevel字段值匹配，如体育：“女装:裙子:半身裙”。<b>用于物料池管理，强烈建议</b>
-        :type CategoryPath: str
-        :param Title: 商品标题，<b>主要用于语义分析</b>，<b>强烈建议</b>
-        :type Title: str
-        :param Tags: 商品标签，多个标签用英文冒号联接，<b>用作特征，强烈建议</b>
-        :type Tags: str
-        :param Brand: 商品对应的品牌，取值用户自定义，可以是品牌id或品牌明文，<b>用作特征以及打散/过滤规则，强烈建议</b>
-        :type Brand: str
-        :param ShopId: 商品所属店铺ID，取值客户自定义，<b>用作特征，强烈建议</b>
-        :type ShopId: str
-        :param OrgPrice: 商品原始价格（单位：元，统一货币体系，如统一为RMB或美元等），<b>用作特征，强烈建议</b>
-        :type OrgPrice: float
-        :param CurPrice: 商品当前价格（单位：元，统一货币体系，如统一为RMB或美元等），<b>用作特征，强烈建议</b>
-        :type CurPrice: float
-        :param SourceId: 商品来源类型，客户自定义，<b>用于物料池管理</b>
-        :type SourceId: str
-        :param Content: 商品正文关键片段，建议控制在500字符以内，<b>主要用于语义分析</b>
-        :type Content: str
-        :param ContentUrl: 商品正文详情，主要用于语义分析，当内容过大时建议用ContentUrl传递，<b>与Content可二选一</b>
-        :type ContentUrl: str
-        :param PicUrlList: 商品封面url，不超过10个，<b>用作特征</b>
-        :type PicUrlList: list of str
-        :param Country: 卖家所在国家，ISO 3166-1 alpha-2编码，参考<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2" target="_blank">ISO 3166-1 alpha-2</a>，中国：“CN”，<b>用作特征</b>
-        :type Country: str
-        :param Province: 卖家所在省份，ISO 3166-2行政区编码，如中国参考<a href="https://zh.wikipedia.org/wiki/ISO_3166-2:CN" target="_blank">ISO_3166-2:CN</a>，广东省：“CN-GD”，<b>用作特征</b>
-        :type Province: str
-        :param City: 卖家所在城市地区，统一用国家最新标准地区行政编码，如：<a href="https://www.mca.gov.cn/article/sj/xzqh/2020/" target="_blank">2020年行政区编码</a>，其他国家统一用国际公认城市简称或者城市编码，<b>用作特征</b>
-        :type City: str
-        :param FreeShipping: 商品是否包邮；1:包邮；2:不包邮；3:满足条件包邮，<b>用作特征</b>
-        :type FreeShipping: int
-        :param ShippingPrice: 商品邮费（单位：元，统一货币体系，如统一为RMB或美元等），<b>用作特征</b>
-        :type ShippingPrice: float
-        :param PraiseCnt: 商品累计好评次数，<b>用作特征</b>
-        :type PraiseCnt: int
-        :param CommentCnt: 商品累计评论次数，<b>用作特征</b>
-        :type CommentCnt: int
-        :param ShareCnt: 商品累计分享次数，<b>用作特征</b>
-        :type ShareCnt: int
-        :param CollectCnt: 商品累计收藏次数，<b>用作特征</b>
-        :type CollectCnt: int
-        :param OrderCnt: 商品累积成交次数，<b>用作特征</b>
-        :type OrderCnt: int
-        :param Score: 商品平均客户评分，取值范围用户自定，<b>用作特征</b>
-        :type Score: float
-        :param Extension: json字符串，<b>用于物料池管理的自定义扩展</b>
-        :type Extension: str
-        """
-        self.GoodsId = None
-        self.GoodsType = None
-        self.Status = None
-        self.PublishTimestamp = None
-        self.ExpireTimestamp = None
-        self.SpuId = None
-        self.CategoryLevel = None
-        self.CategoryPath = None
-        self.Title = None
-        self.Tags = None
-        self.Brand = None
-        self.ShopId = None
-        self.OrgPrice = None
-        self.CurPrice = None
-        self.SourceId = None
-        self.Content = None
-        self.ContentUrl = None
-        self.PicUrlList = None
-        self.Country = None
-        self.Province = None
-        self.City = None
-        self.FreeShipping = None
-        self.ShippingPrice = None
-        self.PraiseCnt = None
-        self.CommentCnt = None
-        self.ShareCnt = None
-        self.CollectCnt = None
-        self.OrderCnt = None
-        self.Score = None
-        self.Extension = None
+    @Weight.setter
+    def Weight(self, Weight):
+        self._Weight = Weight
+
+    @property
+    def Score(self):
+        return self._Score
+
+    @Score.setter
+    def Score(self, Score):
+        self._Score = Score
+
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
 
 
     def _deserialize(self, params):
-        self.GoodsId = params.get("GoodsId")
-        self.GoodsType = params.get("GoodsType")
-        self.Status = params.get("Status")
-        self.PublishTimestamp = params.get("PublishTimestamp")
-        self.ExpireTimestamp = params.get("ExpireTimestamp")
-        self.SpuId = params.get("SpuId")
-        self.CategoryLevel = params.get("CategoryLevel")
-        self.CategoryPath = params.get("CategoryPath")
-        self.Title = params.get("Title")
-        self.Tags = params.get("Tags")
-        self.Brand = params.get("Brand")
-        self.ShopId = params.get("ShopId")
-        self.OrgPrice = params.get("OrgPrice")
-        self.CurPrice = params.get("CurPrice")
-        self.SourceId = params.get("SourceId")
-        self.Content = params.get("Content")
-        self.ContentUrl = params.get("ContentUrl")
-        self.PicUrlList = params.get("PicUrlList")
-        self.Country = params.get("Country")
-        self.Province = params.get("Province")
-        self.City = params.get("City")
-        self.FreeShipping = params.get("FreeShipping")
-        self.ShippingPrice = params.get("ShippingPrice")
-        self.PraiseCnt = params.get("PraiseCnt")
-        self.CommentCnt = params.get("CommentCnt")
-        self.ShareCnt = params.get("ShareCnt")
-        self.CollectCnt = params.get("CollectCnt")
-        self.OrderCnt = params.get("OrderCnt")
-        self.Score = params.get("Score")
-        self.Extension = params.get("Extension")
+        self._ItemId = params.get("ItemId")
+        self._ItemType = params.get("ItemType")
+        self._Weight = params.get("Weight")
+        self._Score = params.get("Score")
+        self._Keyword = params.get("Keyword")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class RecGoodsData(AbstractModel):
-    """推荐返回的内容信息
+class RecommendContentRequest(AbstractModel):
+    """RecommendContent请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param GoodsId: 推荐返回的商品ID
-        :type GoodsId: str
-        :param Score: 推荐结果分，取值范围[0,1000000]
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Score: float
-        :param GoodsTraceId: 推荐追踪id，本次推荐内容产生的后续行为上报均要用该GoodsTraceId上报。每次接口调用返回的GoodsTraceId不同
-注意：此字段可能返回 null，表示取不到有效值。
-        :type GoodsTraceId: str
-        :param Position: 商品所在位置
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Position: int
-        """
-        self.GoodsId = None
-        self.Score = None
-        self.GoodsTraceId = None
-        self.Position = None
+        :param _Bid: 业务id
+        :type Bid: str
+        :param _SceneId: 场景id：比如有“猜你喜欢”，“热门内容”等推荐模块，每一个模块都有一个scene_id来表示。 在控制台创建场景后获取。需要跟行为上报时的id一致
+        :type SceneId: str
+        :param _UserIdList: 用户唯一ID数组，每个数组元素详见userId结构体，若不填，则接口返回热门结果
+        :type UserIdList: list of UserIdInfo
+        :param _RecTraceId: 会话id：必须和行为数据上报时所填写的traceId相同，用于行为数据来自于那次在线推荐请求的归因。**注意：此处如果没传，则响应会返回一个全局唯一ID返回给客户，并需客户透传给行为日志上报接口**
+        :type RecTraceId: str
+        :param _ItemCnt: 推荐数量：物料优选的结果， 默认50个，目前最多支持200个的内容返回，如果返回个数更多，会影响性能，容易超时。
+        :type ItemCnt: int
+        :param _PoolId: 物料池id，用于召回该pool_id下的商品，如果有多个，用英文;分割。**注意：此处poolId需和物料上报时的poolIdList对应上**
+        :type PoolId: str
+        :param _CurrentItemId: 来源物料id，即用户当前浏览的物料id，用于在内容详情页获取关联推荐内容
+        :type CurrentItemId: str
+        :param _ResponseTimeout: 请求响应超时时间，单位ms，默认300ms，数值设置的过小，会影响推荐效果，最小支持250ms
+        :type ResponseTimeout: int
+        :param _ItemTypeRatio: 返回结果中不同物料类型的比例，比例顺序需严格按照（图文，长视频，短视频，小视频）进行。只允许传[0,100]数字，多个请用**英文冒号**分割，且加起来不能超过100，以及比例数量不能超过**场景绑定的物料类型**（图文，长视频，短视频，小视频）数。**示例：**图文和短视频比例为40%:60%时，则填40:60图文和短视频比例为0%:100%时，则填0:100图文，长视频和短视频的比例为，图文占20%，剩余80%由长视频和短视频随机返回，则填20:80或仅填20均可
+        :type ItemTypeRatio: str
+        """
+        self._Bid = None
+        self._SceneId = None
+        self._UserIdList = None
+        self._RecTraceId = None
+        self._ItemCnt = None
+        self._PoolId = None
+        self._CurrentItemId = None
+        self._ResponseTimeout = None
+        self._ItemTypeRatio = None
+
+    @property
+    def Bid(self):
+        return self._Bid
+
+    @Bid.setter
+    def Bid(self, Bid):
+        self._Bid = Bid
+
+    @property
+    def SceneId(self):
+        return self._SceneId
+
+    @SceneId.setter
+    def SceneId(self, SceneId):
+        self._SceneId = SceneId
+
+    @property
+    def UserIdList(self):
+        return self._UserIdList
+
+    @UserIdList.setter
+    def UserIdList(self, UserIdList):
+        self._UserIdList = UserIdList
+
+    @property
+    def RecTraceId(self):
+        return self._RecTraceId
+
+    @RecTraceId.setter
+    def RecTraceId(self, RecTraceId):
+        self._RecTraceId = RecTraceId
+
+    @property
+    def ItemCnt(self):
+        return self._ItemCnt
+
+    @ItemCnt.setter
+    def ItemCnt(self, ItemCnt):
+        self._ItemCnt = ItemCnt
+
+    @property
+    def PoolId(self):
+        return self._PoolId
+
+    @PoolId.setter
+    def PoolId(self, PoolId):
+        self._PoolId = PoolId
+
+    @property
+    def CurrentItemId(self):
+        return self._CurrentItemId
+
+    @CurrentItemId.setter
+    def CurrentItemId(self, CurrentItemId):
+        self._CurrentItemId = CurrentItemId
+
+    @property
+    def ResponseTimeout(self):
+        return self._ResponseTimeout
+
+    @ResponseTimeout.setter
+    def ResponseTimeout(self, ResponseTimeout):
+        self._ResponseTimeout = ResponseTimeout
+
+    @property
+    def ItemTypeRatio(self):
+        return self._ItemTypeRatio
+
+    @ItemTypeRatio.setter
+    def ItemTypeRatio(self, ItemTypeRatio):
+        self._ItemTypeRatio = ItemTypeRatio
 
 
     def _deserialize(self, params):
-        self.GoodsId = params.get("GoodsId")
-        self.Score = params.get("Score")
-        self.GoodsTraceId = params.get("GoodsTraceId")
-        self.Position = params.get("Position")
+        self._Bid = params.get("Bid")
+        self._SceneId = params.get("SceneId")
+        if params.get("UserIdList") is not None:
+            self._UserIdList = []
+            for item in params.get("UserIdList"):
+                obj = UserIdInfo()
+                obj._deserialize(item)
+                self._UserIdList.append(obj)
+        self._RecTraceId = params.get("RecTraceId")
+        self._ItemCnt = params.get("ItemCnt")
+        self._PoolId = params.get("PoolId")
+        self._CurrentItemId = params.get("CurrentItemId")
+        self._ResponseTimeout = params.get("ResponseTimeout")
+        self._ItemTypeRatio = params.get("ItemTypeRatio")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class RecItemData(AbstractModel):
-    """推荐返回的内容信息
+class RecommendContentResponse(AbstractModel):
+    """RecommendContent返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ItemId: 推荐的内容ID
-        :type ItemId: str
-        :param ItemType: 内容类型，同内容上报类型一致
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ItemType: str
-        :param ItemTraceId: 推荐追踪id，本次推荐内容产生的后续行为上报均要用该ItemTraceId上报。每次接口调用返回的ItemTraceId不同
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ItemTraceId: str
-        :param Score: 推荐预测分，分值越高被推荐的理由越充分，取值范围[0,1000000]，用于做二次排序的参考
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Score: float
+        :param _RecTraceId: 推荐追踪id，用于行为上报。每次接口调用返回的traceId不同
+        :type RecTraceId: str
+        :param _DataList: 标识具体的物料信息
+        :type DataList: list of RecItemData
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self.ItemId = None
-        self.ItemType = None
-        self.ItemTraceId = None
-        self.Score = None
+        self._RecTraceId = None
+        self._DataList = None
+        self._RequestId = None
 
+    @property
+    def RecTraceId(self):
+        return self._RecTraceId
 
-    def _deserialize(self, params):
-        self.ItemId = params.get("ItemId")
-        self.ItemType = params.get("ItemType")
-        self.ItemTraceId = params.get("ItemTraceId")
-        self.Score = params.get("Score")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+    @RecTraceId.setter
+    def RecTraceId(self, RecTraceId):
+        self._RecTraceId = RecTraceId
 
+    @property
+    def DataList(self):
+        return self._DataList
 
-class ReportFeedBehaviorRequest(AbstractModel):
-    """ReportFeedBehavior请求参数结构体
+    @DataList.setter
+    def DataList(self, DataList):
+        self._DataList = DataList
 
-    """
+    @property
+    def RequestId(self):
+        return self._RequestId
 
-    def __init__(self):
-        r"""
-        :param InstanceId: 实例ID，在控制台获取
-        :type InstanceId: str
-        :param FeedBehaviorList: 上报的行为数据数组，数量不超过50
-        :type FeedBehaviorList: list of FeedBehaviorInfo
-        """
-        self.InstanceId = None
-        self.FeedBehaviorList = None
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        if params.get("FeedBehaviorList") is not None:
-            self.FeedBehaviorList = []
-            for item in params.get("FeedBehaviorList"):
-                obj = FeedBehaviorInfo()
+        self._RecTraceId = params.get("RecTraceId")
+        if params.get("DataList") is not None:
+            self._DataList = []
+            for item in params.get("DataList"):
+                obj = RecItemData()
                 obj._deserialize(item)
-                self.FeedBehaviorList.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+                self._DataList.append(obj)
+        self._RequestId = params.get("RequestId")
 
 
-class ReportFeedBehaviorResponse(AbstractModel):
-    """ReportFeedBehavior返回参数结构体
+class ReportActionRequest(AbstractModel):
+    """ReportAction请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
+        :param _Bid: 业务id
+        :type Bid: str
+        :param _DocBehaviorList: 上报的行为对象数组，数量不超过50
+        :type DocBehaviorList: list of DocBehavior
         """
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.RequestId = params.get("RequestId")
+        self._Bid = None
+        self._DocBehaviorList = None
 
+    @property
+    def Bid(self):
+        return self._Bid
 
-class ReportFeedItemRequest(AbstractModel):
-    """ReportFeedItem请求参数结构体
+    @Bid.setter
+    def Bid(self, Bid):
+        self._Bid = Bid
 
-    """
+    @property
+    def DocBehaviorList(self):
+        return self._DocBehaviorList
 
-    def __init__(self):
-        r"""
-        :param InstanceId: 实例ID，在控制台获取
-        :type InstanceId: str
-        :param FeedItemList: 上报的信息流内容数组，一次数量不超过50
-        :type FeedItemList: list of DocItem
-        """
-        self.InstanceId = None
-        self.FeedItemList = None
+    @DocBehaviorList.setter
+    def DocBehaviorList(self, DocBehaviorList):
+        self._DocBehaviorList = DocBehaviorList
 
 
     def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        if params.get("FeedItemList") is not None:
-            self.FeedItemList = []
-            for item in params.get("FeedItemList"):
-                obj = DocItem()
+        self._Bid = params.get("Bid")
+        if params.get("DocBehaviorList") is not None:
+            self._DocBehaviorList = []
+            for item in params.get("DocBehaviorList"):
+                obj = DocBehavior()
                 obj._deserialize(item)
-                self.FeedItemList.append(obj)
+                self._DocBehaviorList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ReportFeedItemResponse(AbstractModel):
-    """ReportFeedItem返回参数结构体
+class ReportActionResponse(AbstractModel):
+    """ReportAction返回参数结构体
 
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
 
 
-class ReportFeedUserRequest(AbstractModel):
-    """ReportFeedUser请求参数结构体
+class ReportMaterialRequest(AbstractModel):
+    """ReportMaterial请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID，在控制台获取
-        :type InstanceId: str
-        :param FeedUserList: 上报的用户信息数组，数量不超过50
-        :type FeedUserList: list of FeedUserInfo
+        :param _Bid: 业务id
+        :type Bid: str
+        :param _DocItemList: 上报的信息流数组，一次数量不超过50
+        :type DocItemList: list of DocItem
         """
-        self.InstanceId = None
-        self.FeedUserList = None
+        self._Bid = None
+        self._DocItemList = None
+
+    @property
+    def Bid(self):
+        return self._Bid
+
+    @Bid.setter
+    def Bid(self, Bid):
+        self._Bid = Bid
+
+    @property
+    def DocItemList(self):
+        return self._DocItemList
+
+    @DocItemList.setter
+    def DocItemList(self, DocItemList):
+        self._DocItemList = DocItemList
 
 
     def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        if params.get("FeedUserList") is not None:
-            self.FeedUserList = []
-            for item in params.get("FeedUserList"):
-                obj = FeedUserInfo()
+        self._Bid = params.get("Bid")
+        if params.get("DocItemList") is not None:
+            self._DocItemList = []
+            for item in params.get("DocItemList"):
+                obj = DocItem()
                 obj._deserialize(item)
-                self.FeedUserList.append(obj)
+                self._DocItemList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ReportFeedUserResponse(AbstractModel):
-    """ReportFeedUser返回参数结构体
+class ReportMaterialResponse(AbstractModel):
+    """ReportMaterial返回参数结构体
 
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
 
 
-class ReportGoodsBehaviorRequest(AbstractModel):
-    """ReportGoodsBehavior请求参数结构体
+class ReportPortraitRequest(AbstractModel):
+    """ReportPortrait请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID，在控制台获取
-        :type InstanceId: str
-        :param GoodsBehaviorList: 上报的商品对应的用户行为数据数组，数量不超过50
-        :type GoodsBehaviorList: list of GoodsBehaviorInfo
+        :param _Bid: 推荐平台上的业务id
+        :type Bid: str
+        :param _PortraitList: 上报的用户画像数组，数量不超过50
+        :type PortraitList: list of PortraitInfo
         """
-        self.InstanceId = None
-        self.GoodsBehaviorList = None
+        self._Bid = None
+        self._PortraitList = None
+
+    @property
+    def Bid(self):
+        return self._Bid
+
+    @Bid.setter
+    def Bid(self, Bid):
+        self._Bid = Bid
+
+    @property
+    def PortraitList(self):
+        return self._PortraitList
+
+    @PortraitList.setter
+    def PortraitList(self, PortraitList):
+        self._PortraitList = PortraitList
 
 
     def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        if params.get("GoodsBehaviorList") is not None:
-            self.GoodsBehaviorList = []
-            for item in params.get("GoodsBehaviorList"):
-                obj = GoodsBehaviorInfo()
+        self._Bid = params.get("Bid")
+        if params.get("PortraitList") is not None:
+            self._PortraitList = []
+            for item in params.get("PortraitList"):
+                obj = PortraitInfo()
                 obj._deserialize(item)
-                self.GoodsBehaviorList.append(obj)
+                self._PortraitList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ReportGoodsBehaviorResponse(AbstractModel):
-    """ReportGoodsBehavior返回参数结构体
+class ReportPortraitResponse(AbstractModel):
+    """ReportPortrait返回参数结构体
 
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
 
 
-class ReportGoodsInfoRequest(AbstractModel):
-    """ReportGoodsInfo请求参数结构体
+class TagInfo(AbstractModel):
+    """标题信息
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID，在控制台获取
-        :type InstanceId: str
-        :param GoodsList: 上报的商品数组，一次数量不超过50
-        :type GoodsList: list of GoodsInfo
+        :param _Id: 标签id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _Name: 标签名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _Weight: 推荐权重
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Weight: float
         """
-        self.InstanceId = None
-        self.GoodsList = None
+        self._Id = None
+        self._Name = None
+        self._Weight = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Weight(self):
+        return self._Weight
+
+    @Weight.setter
+    def Weight(self, Weight):
+        self._Weight = Weight
 
 
     def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        if params.get("GoodsList") is not None:
-            self.GoodsList = []
-            for item in params.get("GoodsList"):
-                obj = GoodsInfo()
-                obj._deserialize(item)
-                self.GoodsList.append(obj)
+        self._Id = params.get("Id")
+        self._Name = params.get("Name")
+        self._Weight = params.get("Weight")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ReportGoodsInfoResponse(AbstractModel):
-    """ReportGoodsInfo返回参数结构体
+class UserIdInfo(AbstractModel):
+    """用户信息
 
     """
 
     def __init__(self):
         r"""
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
+        :param _UserIdType: 用户ID类型：
+1 - qq
+2 - qq_md5：md5后的qq
+3 - imei：设备imei（安卓10之后不会再授权imei，安卓10之后的imei映射关系可能拿不到，故安卓10之后的设备建议用oaid）
+4 - imei_md5：md5后的imei
+5 - idfa: Apple 向用户设备随机分配的设备标识符
+6 - idfa_md5：md5之后的idfa
+7 - gdt_openid：广点通生成的openid
+8 - oaid：安卓10之后一种非永久性设备标识符
+9 - oaid_md5：md5后的oaid
+10 - wx_openid：微信openid
+11 - qq_openid：QQ的openid
+12 - phone：电话号码
+13 - phone_md5：md5后的电话号码
+14 - phone_sha256：SHA256加密的手机号
+15 - phone_sm3：国密SM3加密的手机号
+1000 - 客户自定义id
+        :type UserIdType: int
+        :param _UserId: 用户id
+        :type UserId: str
         """
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.RequestId = params.get("RequestId")
+        self._UserIdType = None
+        self._UserId = None
 
+    @property
+    def UserIdType(self):
+        return self._UserIdType
 
-class StrUserIdInfo(AbstractModel):
-    """用户信息
+    @UserIdType.setter
+    def UserIdType(self, UserIdType):
+        self._UserIdType = UserIdType
 
-    """
+    @property
+    def UserId(self):
+        return self._UserId
 
-
-class UserIdInfo(AbstractModel):
-    """用户ID信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Type: 用户ID类型： <br/>● qq: qq号码 <br/>● qq_md5：qq的md5值 <br/>● imei：设备imei <br/>● imei_md5：imei的md5值 <br/>● idfa: Apple 向用户设备随机分配的设备标识符 <br/>● idfa_md5：idfa的md5值 <br/>● oaid：安卓10之后一种非永久性设备标识符 <br/>● oaid_md5：md5后的oaid <br/>● wx_openid：微信openid <br/>● qq_openid：QQ的openid <br/>● phone：电话号码 <br/>● phone_md5：md5后的电话号码 <br/>● phone_sha256：SHA256加密的手机号 <br/>● phone_sm3：国密SM3加密的手机号 <br/>（如当前类型不满足，请<a href="https://console.cloud.tencent.com/workorder/category" target="_blank">提单</a>沟通解决方案）
-        :type Type: str
-        :param Value: 用户ID值
-        :type Value: str
-        """
-        self.Type = None
-        self.Value = None
+    @UserId.setter
+    def UserId(self, UserId):
+        self._UserId = UserId
 
 
     def _deserialize(self, params):
-        self.Type = params.get("Type")
-        self.Value = params.get("Value")
+        self._UserIdType = params.get("UserIdType")
+        self._UserId = params.get("UserId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class UserPortraitInfo(AbstractModel):
-    """用户基础画像
-
-    """
+
```

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud/irp/v20220805/irp_client.py` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud/irp/v20220805/irp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-irp-3.0.927/tencentcloud/__init__.py` & `tencentcloud-sdk-python-irp-3.0.928/tencentcloud/__init__.py`

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

