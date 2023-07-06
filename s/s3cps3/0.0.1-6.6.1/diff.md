# Comparing `tmp/s3cps3-0.0.1.tar.gz` & `tmp/s3cps3-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/PJLAB/qinwenkai/PycharmProjects/s3cps3/dist/.tmp-d6hau35a/s3cps3-0.0.1.tar", last modified: Mon Jul  3 10:51:18 2023, max compression
+gzip compressed data, was "dist/s3cps3-6.6.1.tar", last modified: Thu Jul  6 06:55:33 2023, max compression
```

## Comparing `s3cps3-0.0.1.tar` & `s3cps3-6.6.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-03 10:51:18.000000 s3cps3-0.0.1/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1069 2023-07-03 09:25:58.000000 s3cps3-0.0.1/LICENSE
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       72 2023-07-03 10:51:18.000000 s3cps3-0.0.1/PKG-INFO
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       96 2023-07-03 10:40:00.000000 s3cps3-0.0.1/pyproject.toml
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-03 10:51:18.000000 s3cps3-0.0.1/s3cps3/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-05-29 11:05:45.000000 s3cps3-0.0.1/s3cps3/__init__.py
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1210 2023-06-26 09:37:27.000000 s3cps3-0.0.1/s3cps3/commons.py
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2217 2023-07-03 10:47:21.000000 s3cps3-0.0.1/s3cps3/listbucket.py
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     4150 2023-07-03 10:47:21.000000 s3cps3-0.0.1/s3cps3/s3cps3.py
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-03 10:51:18.000000 s3cps3-0.0.1/s3cps3.egg-info/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       72 2023-07-03 10:51:18.000000 s3cps3-0.0.1/s3cps3.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      246 2023-07-03 10:51:18.000000 s3cps3-0.0.1/s3cps3.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        1 2023-07-03 10:51:18.000000 s3cps3-0.0.1/s3cps3.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       19 2023-07-03 10:51:18.000000 s3cps3-0.0.1/s3cps3.egg-info/requires.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        7 2023-07-03 10:51:18.000000 s3cps3-0.0.1/s3cps3.egg-info/top_level.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       38 2023-07-03 10:51:18.000000 s3cps3-0.0.1/setup.cfg
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 06:55:33.000000 s3cps3-6.6.1/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1069 2023-07-03 09:25:58.000000 s3cps3-6.6.1/LICENSE
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       80 2023-07-05 10:09:29.000000 s3cps3-6.6.1/MANIFEST.in
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       72 2023-07-06 06:55:33.000000 s3cps3-6.6.1/PKG-INFO
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-05-29 11:05:45.000000 s3cps3-6.6.1/s3cps3/__init__.py
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1210 2023-06-26 09:37:27.000000 s3cps3-6.6.1/s3cps3/commons.py
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2212 2023-07-06 02:46:29.000000 s3cps3-6.6.1/s3cps3/listbucket.py
+-rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)    10400 2023-07-06 02:25:10.000000 s3cps3-6.6.1/s3cps3/main.xsh
+-rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       45 2023-07-05 10:52:13.000000 s3cps3-6.6.1/s3cps3/s32s3
+-rwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      437 2023-05-29 13:19:00.000000 s3cps3-6.6.1/s3cps3/s3bigcp.sh
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     4119 2023-07-06 02:43:40.000000 s3cps3-6.6.1/s3cps3/s3cps3.py
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       72 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      299 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        1 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      165 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/requires.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        7 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/top_level.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       38 2023-07-06 06:55:33.000000 s3cps3-6.6.1/setup.cfg
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      646 2023-07-06 06:26:53.000000 s3cps3-6.6.1/setup.py
```

### Comparing `s3cps3-0.0.1/LICENSE` & `s3cps3-6.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s3cps3-0.0.1/s3cps3/commons.py` & `s3cps3-6.6.1/s3cps3/commons.py`

 * *Files identical despite different names*

### Comparing `s3cps3-0.0.1/s3cps3/listbucket.py` & `s3cps3-6.6.1/s3cps3/listbucket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import boto3
 import json
 from botocore.config import Config
-import sys, re
+import sys, re, os
 from loguru import logger
-from s3cps3.commons import parse_aws_param
+from commons import parse_aws_param
 
 #保存传递给脚本的第一个参数
 profile_s3path = sys.argv[1]
 if not profile_s3path or not profile_s3path.endswith("/"):
     print("参数需要以/结尾，代表s3上的目录")
     exit(-1)
 
@@ -16,15 +16,14 @@
     logger.error(f"{profile_s3path} format ERROR")
     exit(-1)
 
 aws_profile = s3info[0][0]
 bucket = s3info[0][1]
 path = s3info[0][2]
 
-
 ak, sk, end_point, addressing_style = parse_aws_param(aws_profile)
 
 try:
     cli = boto3.client(service_name="s3", aws_access_key_id=ak, aws_secret_access_key=sk, endpoint_url=end_point,
                                     config=Config(s3={'addressing_style': addressing_style}))
 
     def list_obj_scluster():
@@ -38,15 +37,14 @@
             response = cli.list_objects(**list_kwargs)
             contents = response.get("Contents", [])#获取桶内该路径下的对象列表
             yield from contents#一个个返回contents中的值
             if not response.get("IsTruncated") or len(contents)==0:
                 break
             marker = contents[-1]['Key']
 
-
     for info in list_obj_scluster():
         file_path = info['Key']
         size = info['Size']
         f_info = {"size": size, "path": file_path}
 
         if path!="":
             f_info['path']=file_path[len(path):]
```

### Comparing `s3cps3-0.0.1/s3cps3/s3cps3.py` & `s3cps3-6.6.1/s3cps3/s3cps3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import sys, boto3, json
+import sys, boto3, json, os
 from botocore.config import Config
 import queue, threading
 from concurrent import futures
 from loguru import logger
-from s3cps3.commons import parse_aws_param
-
+from commons import parse_aws_param
 
 input_path = sys.argv[1] # 内含jsonl
 src_profile = sys.argv[2]
 dest_profile = sys.argv[3]
 thread_cnt = int(sys.argv[4])
 
 src_ak, src_sk, src_end_point, src_addressing_style = parse_aws_param(src_profile)
@@ -34,22 +33,19 @@
             "s3": {
                 "addressing_style": dest_addressing_style,
             },
             "retries": {
                 "max_attempts": 3,
             }
         })
-#print(src_cli_config)
 
 src_cli =  boto3.session.Session().client("s3", aws_access_key_id=src_ak,  aws_secret_access_key=src_sk,  endpoint_url=src_end_point, region_name='', config=src_cli_config)
 dest_cli = boto3.session.Session().client("s3", aws_access_key_id=dest_ak, aws_secret_access_key=dest_sk, endpoint_url=dest_end_point, region_name='', config=dest_cli_config)
-
 cur_thread_id = threading.get_ident()
 
-
 # 接下来开启线程，开始copy
 class ThreadPoolExecutorWithQueueSizeLimit(futures.ThreadPoolExecutor):
     def __init__(self, max_workers=10, *args, **kwargs):
         """
         param: max_workers 最多并发执行数
         param: len_queue  队列长队 至少为 1
         """
@@ -87,24 +83,22 @@
             exit(-1)
     
 src_buckets = []
 src_paths = []
 dest_buckets = []
 dest_paths = []
 
-
 with open(input_path, "r", encoding='utf-8') as f:
     for l in f:
         o = json.loads(l)
         src_buckets.append(o["src_bucket"])
         src_paths.append(o["src_path"])
         dest_buckets.append(o["dst_bucket"])
         dest_paths.append(o["dst_path"])
 
 total_files = len(src_buckets)
 with ThreadPoolExecutorWithQueueSizeLimit(max_workers=thread_cnt) as thread_pooll:
     thread_pooll.total_files = total_files
     thread_pooll.map(thread_pooll.do_copy, src_buckets, src_paths, dest_buckets, dest_paths, chunksize=20)
 
-
 logger.info(f"线程 {cur_thread_id} copy {total_files} 个文件成功")
 exit(0)
```

