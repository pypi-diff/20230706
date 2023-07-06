# Comparing `tmp/yunhu-0.0.4.tar.gz` & `tmp/yunhu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunhu-0.0.4.tar", last modified: Mon May  8 11:30:17 2023, max compression
+gzip compressed data, was "yunhu-0.0.5.tar", last modified: Thu Jul  6 07:28:21 2023, max compression
```

## Comparing `yunhu-0.0.4.tar` & `yunhu-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.162910 yunhu-0.0.4/
--rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      610 2023-05-08 11:30:17.161938 yunhu-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.138483 yunhu-0.0.4/example_yunhu/
--rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.4/example_yunhu/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-05-08 08:56:14.000000 yunhu-0.0.4/example_yunhu/flask_demo.py
--rw-rw-rw-   0        0        0      426 2023-05-08 11:28:28.000000 yunhu-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 11:30:17.164423 yunhu-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-05-08 11:28:33.000000 yunhu-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.148935 yunhu-0.0.4/yunhu/
--rw-rw-rw-   0        0        0        0 2023-05-08 09:46:54.000000 yunhu-0.0.4/yunhu/__init__.py
--rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.4/yunhu/main.py
--rw-rw-rw-   0        0        0     2694 2023-04-25 08:55:43.000000 yunhu-0.0.4/yunhu/openapi.py
--rw-rw-rw-   0        0        0     2460 2023-05-08 11:27:24.000000 yunhu-0.0.4/yunhu/subscription.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.159909 yunhu-0.0.4/yunhu.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.212881 yunhu-0.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      610 2023-07-06 07:28:21.212881 yunhu-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.203725 yunhu-0.0.5/example_yunhu/
+-rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.5/example_yunhu/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-05-08 08:56:14.000000 yunhu-0.0.5/example_yunhu/flask_demo.py
+-rw-rw-rw-   0        0        0      316 2023-07-06 07:26:41.000000 yunhu-0.0.5/example_yunhu/set_board_demo.py
+-rw-rw-rw-   0        0        0      426 2023-07-06 07:25:02.000000 yunhu-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 07:28:21.213802 yunhu-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-07-06 07:24:55.000000 yunhu-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.207633 yunhu-0.0.5/yunhu/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:46:54.000000 yunhu-0.0.5/yunhu/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.5/yunhu/main.py
+-rw-rw-rw-   0        0        0     4551 2023-07-06 07:21:44.000000 yunhu-0.0.5/yunhu/openapi.py
+-rw-rw-rw-   0        0        0     2460 2023-05-08 11:27:24.000000 yunhu-0.0.5/yunhu/subscription.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.211854 yunhu-0.0.5/yunhu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/top_level.txt
```

### Comparing `yunhu-0.0.4/LICENSE.txt` & `yunhu-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.4/PKG-INFO` & `yunhu-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.4
+Version: 0.0.5
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yunhu-0.0.4/example_yunhu/flask_demo.py` & `yunhu-0.0.5/example_yunhu/flask_demo.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.4/setup.py` & `yunhu-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="yunhu", 
-    version="0.0.4", 
+    version="0.0.5", 
     author="yunhu",  
     description="云湖官方Python SDK", #包的简述
     author_email="1114110051@qq.com",    
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yunhu-0.0.4/yunhu/openapi.py` & `yunhu-0.0.5/yunhu/openapi.py`

 * *Files 19% similar despite different names*

```diff
@@ -70,8 +70,53 @@
             "msgId": msgId, 
             "recvId": recvId, 
             "recvType": recvType, 
             "contentType": contentType, 
             "content": content
          }
         headers = {'Content-Type': 'application/json'}
-        return requests.post(self.baseUrl + '/bot/edit?token=' + self.token,headers=headers, data=json.dumps(params))
+        return requests.post(self.baseUrl + '/bot/edit?token=' + self.token,headers=headers, data=json.dumps(params))
+    
+    def SetBotBoard(self, recvId: str, recvType: str, contentType: str, content: str):
+        """
+        @description: 机器人看板设置接口
+        机器人看板类型contentType取值: text、markdown、html
+        """
+        params = {
+            "recvId": recvId, 
+            "recvType": recvType, 
+            "contentType": contentType, 
+            "content": content
+         }
+        headers = {'Content-Type': 'application/json'}
+        return requests.post(self.baseUrl + '/bot/board?token=' + self.token,headers=headers, data=json.dumps(params))
+    
+    def SetBotBoardAll(self, contentType: str, content: str):
+        """
+        @description: 机器人看板批量设置接口
+        机器人看板类型contentType取值: text、markdown、html
+        """
+        params = {
+            "contentType": contentType, 
+            "content": content
+         }
+        headers = {'Content-Type': 'application/json'}
+        return requests.post(self.baseUrl + '/bot/board-all?token=' + self.token,headers=headers, data=json.dumps(params))
+    
+    def DismissBotBoard(self, recvId: str, recvType: str):
+        """
+        @description: 机器人看板取消接口
+        """
+        params = {
+            "recvId": recvId, 
+            "recvType": recvType, 
+         }
+        headers = {'Content-Type': 'application/json'}
+        return requests.post(self.baseUrl + '/bot/board-dismiss?token=' + self.token,headers=headers, data=json.dumps(params))
+    
+    def DismissBotBoardAll(self):
+        """
+        @description: 机器人看板取消接口
+        """
+        params = {}
+        headers = {'Content-Type': 'application/json'}
+        return requests.post(self.baseUrl + '/bot/board-all-dismiss?token=' + self.token,headers=headers, data=json.dumps(params))
```

### Comparing `yunhu-0.0.4/yunhu/subscription.py` & `yunhu-0.0.5/yunhu/subscription.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.4/yunhu.egg-info/PKG-INFO` & `yunhu-0.0.5/yunhu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.4
+Version: 0.0.5
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

