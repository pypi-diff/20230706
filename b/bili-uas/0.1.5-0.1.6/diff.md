# Comparing `tmp/bili-uas-0.1.5.tar.gz` & `tmp/bili-uas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili-uas-0.1.5.tar", last modified: Wed Jul  5 11:40:30 2023, max compression
+gzip compressed data, was "bili-uas-0.1.6.tar", last modified: Thu Jul  6 12:29:24 2023, max compression
```

## Comparing `bili-uas-0.1.5.tar` & `bili-uas-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-05 11:40:30.309592 bili-uas-0.1.5/
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-05 11:40:30.304941 bili-uas-0.1.5/Bili_UAS/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.5/Bili_UAS/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1903 2023-07-03 09:43:52.000000 bili-uas-0.1.5/Bili_UAS/bili_config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5309 2023-07-03 09:35:16.000000 bili-uas-0.1.5/Bili_UAS/bili_live.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-03 09:35:16.000000 bili-uas-0.1.5/Bili_UAS/bili_login.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-07-03 09:35:16.000000 bili-uas-0.1.5/Bili_UAS/bili_user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2510 2023-07-03 09:35:16.000000 bili-uas-0.1.5/Bili_UAS/bili_video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-05 11:40:30.306184 bili-uas-0.1.5/Bili_UAS/scripts/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.5/Bili_UAS/scripts/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.5/Bili_UAS/scripts/config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4271 2023-06-30 11:45:34.000000 bili-uas-0.1.5/Bili_UAS/scripts/live.py
--rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.5/Bili_UAS/scripts/log_in.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.5/Bili_UAS/scripts/user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.5/Bili_UAS/scripts/video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-05 11:40:30.307969 bili-uas-0.1.5/Bili_UAS/utils/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.5/Bili_UAS/utils/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)    50101 2023-06-30 11:57:40.000000 bili-uas-0.1.5/Bili_UAS/utils/live_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.5/Bili_UAS/utils/search_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.5/Bili_UAS/utils/train_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.5/Bili_UAS/utils/user_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.5/Bili_UAS/utils/utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.5/Bili_UAS/utils/video_utils.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-05 11:40:30.308601 bili-uas-0.1.5/Bili_UAS/writer/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.5/Bili_UAS/writer/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.5/Bili_UAS/writer/abnormal_monitor.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3575 2023-07-03 09:41:05.000000 bili-uas-0.1.5/Bili_UAS/writer/log_writer.py
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.5/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-05 11:40:30.309455 bili-uas-0.1.5/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)     3880 2023-07-02 23:09:01.000000 bili-uas-0.1.5/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-05 11:40:30.309278 bili-uas-0.1.5/bili_uas.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-05 11:40:30.000000 bili-uas-0.1.5/bili_uas.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-05 11:40:30.000000 bili-uas-0.1.5/bili_uas.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-05 11:40:30.000000 bili-uas-0.1.5/bili_uas.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-05 11:40:30.000000 bili-uas-0.1.5/bili_uas.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      229 2023-07-05 11:40:30.000000 bili-uas-0.1.5/bili_uas.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-05 11:40:30.000000 bili-uas-0.1.5/bili_uas.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-05 11:40:30.309637 bili-uas-0.1.5/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     1978 2023-07-05 11:39:12.000000 bili-uas-0.1.5/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-06 12:29:24.455019 bili-uas-0.1.6/
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-06 12:29:24.448926 bili-uas-0.1.6/Bili_UAS/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.6/Bili_UAS/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1903 2023-07-03 09:43:52.000000 bili-uas-0.1.6/Bili_UAS/bili_config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5309 2023-07-03 09:35:16.000000 bili-uas-0.1.6/Bili_UAS/bili_live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-03 09:35:16.000000 bili-uas-0.1.6/Bili_UAS/bili_login.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-07-03 09:35:16.000000 bili-uas-0.1.6/Bili_UAS/bili_user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2510 2023-07-03 09:35:16.000000 bili-uas-0.1.6/Bili_UAS/bili_video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-06 12:29:24.450439 bili-uas-0.1.6/Bili_UAS/scripts/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.6/Bili_UAS/scripts/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.6/Bili_UAS/scripts/config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4271 2023-06-30 11:45:34.000000 bili-uas-0.1.6/Bili_UAS/scripts/live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.6/Bili_UAS/scripts/log_in.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.6/Bili_UAS/scripts/user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.6/Bili_UAS/scripts/video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-06 12:29:24.452888 bili-uas-0.1.6/Bili_UAS/utils/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.6/Bili_UAS/utils/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    50103 2023-07-06 12:19:35.000000 bili-uas-0.1.6/Bili_UAS/utils/live_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.6/Bili_UAS/utils/search_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.6/Bili_UAS/utils/train_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.6/Bili_UAS/utils/user_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.6/Bili_UAS/utils/utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.6/Bili_UAS/utils/video_utils.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-06 12:29:24.453832 bili-uas-0.1.6/Bili_UAS/writer/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.6/Bili_UAS/writer/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.6/Bili_UAS/writer/abnormal_monitor.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3575 2023-07-03 09:41:05.000000 bili-uas-0.1.6/Bili_UAS/writer/log_writer.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.6/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-06 12:29:24.454886 bili-uas-0.1.6/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)     3880 2023-07-02 23:09:01.000000 bili-uas-0.1.6/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-06 12:29:24.454711 bili-uas-0.1.6/bili_uas.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-06 12:29:24.000000 bili-uas-0.1.6/bili_uas.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-06 12:29:24.000000 bili-uas-0.1.6/bili_uas.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-06 12:29:24.000000 bili-uas-0.1.6/bili_uas.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-06 12:29:24.000000 bili-uas-0.1.6/bili_uas.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      229 2023-07-06 12:29:24.000000 bili-uas-0.1.6/bili_uas.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-06 12:29:24.000000 bili-uas-0.1.6/bili_uas.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-06 12:29:24.455062 bili-uas-0.1.6/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     1978 2023-07-06 12:20:36.000000 bili-uas-0.1.6/setup.py
```

### Comparing `bili-uas-0.1.5/Bili_UAS/bili_config.py` & `bili-uas-0.1.6/Bili_UAS/bili_config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/bili_live.py` & `bili-uas-0.1.6/Bili_UAS/bili_live.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/bili_login.py` & `bili-uas-0.1.6/Bili_UAS/bili_login.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/bili_user.py` & `bili-uas-0.1.6/Bili_UAS/bili_user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/bili_video.py` & `bili-uas-0.1.6/Bili_UAS/bili_video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/scripts/config.py` & `bili-uas-0.1.6/Bili_UAS/scripts/config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/scripts/live.py` & `bili-uas-0.1.6/Bili_UAS/scripts/live.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/scripts/log_in.py` & `bili-uas-0.1.6/Bili_UAS/scripts/log_in.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/scripts/user.py` & `bili-uas-0.1.6/Bili_UAS/scripts/user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/scripts/video.py` & `bili-uas-0.1.6/Bili_UAS/scripts/video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/utils/live_utils.py` & `bili-uas-0.1.6/Bili_UAS/utils/live_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1074,15 +1074,15 @@
         Analyze revenue from live-streaming rooms.
 
         Args:
             interval: the minute interval for revenue analysis
             live_dir: directory for storing single live-streaming data
         """
         await self.__revenue_stat_by_time(interval, live_dir)
-        await self._revenue_stat_by_price()
+        # await self._revenue_stat_by_price()
         await self.__revenue_stat_by_type()
 
     async def __view_stat(self, live_dir: str) -> None:
         """
         Analyze the number of viewers in live-streaming rooms.
 
         Args:
```

### Comparing `bili-uas-0.1.5/Bili_UAS/utils/search_utils.py` & `bili-uas-0.1.6/Bili_UAS/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/utils/user_utils.py` & `bili-uas-0.1.6/Bili_UAS/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/utils/utils.py` & `bili-uas-0.1.6/Bili_UAS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/utils/video_utils.py` & `bili-uas-0.1.6/Bili_UAS/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/Bili_UAS/writer/log_writer.py` & `bili-uas-0.1.6/Bili_UAS/writer/log_writer.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/LICENSE` & `bili-uas-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/PKG-INFO` & `bili-uas-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.5
+Version: 0.1.6
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.1.5/README.md` & `bili-uas-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/bili_uas.egg-info/PKG-INFO` & `bili-uas-0.1.6/bili_uas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.5
+Version: 0.1.6
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.1.5/bili_uas.egg-info/SOURCES.txt` & `bili-uas-0.1.6/bili_uas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.5/setup.py` & `bili-uas-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'asyncio~=3.4.3',
     'apscheduler~=3.10.1',
     'requests~=2.31.0',
     'httpx~=0.24.1']
 
 setup(
     name='bili-uas',
-    version='0.1.5',
+    version='0.1.6',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     url='https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System',
     description='Assist up in personal, live, and video data analysis and prediction.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

