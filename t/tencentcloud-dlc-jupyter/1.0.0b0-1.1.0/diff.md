# Comparing `tmp/tencentcloud-dlc-jupyter-1.0.0b0.tar.gz` & `tmp/tencentcloud-dlc-jupyter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tencentcloud-dlc-jupyter-1.0.0b0.tar", last modified: Mon Oct 24 06:50:51 2022, max compression
+gzip compressed data, was "tencentcloud-dlc-jupyter-1.1.0.tar", last modified: Thu Jul  6 09:24:38 2023, max compression
```

## Comparing `tencentcloud-dlc-jupyter-1.0.0b0.tar` & `tencentcloud-dlc-jupyter-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.695230 tencentcloud-dlc-jupyter-1.0.0b0/
--rw-r--r--   0 valux      (501) staff       (20)      308 2022-10-24 06:50:51.694982 tencentcloud-dlc-jupyter-1.0.0b0/PKG-INFO
--rw-r--r--   0 valux      (501) staff       (20)       38 2022-10-24 06:50:51.695293 tencentcloud-dlc-jupyter-1.0.0b0/setup.cfg
--rw-r--r--   0 valux      (501) staff       (20)     1458 2022-10-18 14:12:38.000000 tencentcloud-dlc-jupyter-1.0.0b0/setup.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.669882 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/
--rw-r--r--   0 valux      (501) staff       (20)       22 2022-09-28 12:14:40.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/__init__.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.671586 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-08-22 14:04:50.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     5753 2022-10-18 14:22:45.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/cloudapi.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.673887 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/
--rw-r--r--   0 valux      (501) staff       (20)      202 2022-09-05 09:16:24.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     3491 2022-10-18 02:48:06.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/command.py
--rw-r--r--   0 valux      (501) staff       (20)     2379 2022-09-28 09:06:36.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/pandas2spark.py
--rw-r--r--   0 valux      (501) staff       (20)     1667 2022-09-26 12:28:54.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/sqlcommand.py
--rw-r--r--   0 valux      (501) staff       (20)     2634 2022-09-27 02:22:03.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/storecommand.py
--rw-r--r--   0 valux      (501) staff       (20)     1122 2022-09-26 12:54:58.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/string2spark.py
--rw-r--r--   0 valux      (501) staff       (20)     1039 2022-09-23 06:41:03.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/var2spark.py
--rw-r--r--   0 valux      (501) staff       (20)     5375 2022-10-20 08:53:35.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/controllers.py
--rw-r--r--   0 valux      (501) staff       (20)     1485 2022-10-18 14:22:55.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/qclient.py
--rw-r--r--   0 valux      (501) staff       (20)     9080 2022-10-24 02:12:39.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/sessions.py
--rw-r--r--   0 valux      (501) staff       (20)     4530 2022-10-18 12:40:38.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/exceptions.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.674944 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/
--rw-r--r--   0 valux      (501) staff       (20)       39 2022-09-20 03:53:04.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/__init__.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.675493 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcpysparkkernel/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-20 03:26:39.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcpysparkkernel/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)      736 2022-09-22 08:11:56.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcpysparkkernel/pysparkkernel.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.676076 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcsparkkernel/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-20 02:51:37.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcsparkkernel/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)      715 2022-09-20 04:02:37.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcsparkkernel/sparkkernel.py
--rw-r--r--   0 valux      (501) staff       (20)     5720 2022-10-18 14:19:21.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/kernelbase.py
--rw-r--r--   0 valux      (501) staff       (20)     3170 2022-10-18 11:30:36.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/kernelmagics.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.677117 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/magics/
--rw-r--r--   0 valux      (501) staff       (20)       38 2022-09-15 15:38:31.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/magics/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     4154 2022-10-18 12:50:45.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/magics/basemagics.py
--rw-r--r--   0 valux      (501) staff       (20)    12215 2022-10-18 08:04:45.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/magics/remotemagics.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.677505 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/
--rw-r--r--   0 valux      (501) staff       (20)      630 2022-09-28 07:00:46.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/__init__.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.679428 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-28 06:37:11.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)    16453 2022-09-28 07:01:13.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/abstract_client.py
--rw-r--r--   0 valux      (501) staff       (20)     2337 2022-09-28 06:37:11.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/abstract_model.py
--rw-r--r--   0 valux      (501) staff       (20)     1997 2022-09-28 06:48:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/common_client.py
--rw-r--r--   0 valux      (501) staff       (20)    12336 2022-09-28 06:48:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/credential.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.680057 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/exception/
--rw-r--r--   0 valux      (501) staff       (20)      740 2022-09-28 06:48:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)      760 2022-09-28 06:37:11.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.680584 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/http/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-28 06:37:11.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/http/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     5070 2022-09-28 06:48:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/http/request.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.681534 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/profile/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-28 06:37:11.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     1655 2022-09-28 06:48:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 valux      (501) staff       (20)     1857 2022-09-28 06:37:11.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 valux      (501) staff       (20)     1573 2022-09-28 06:48:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/sign.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.681875 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-28 06:37:41.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.684042 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-28 06:37:41.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)   340988 2022-09-28 07:02:56.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 valux      (501) staff       (20)    14039 2022-09-28 06:37:41.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 valux      (501) staff       (20)   787410 2022-09-28 06:48:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/models.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.691522 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-08-22 14:15:50.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     2231 2022-10-18 11:05:47.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/common.py
--rw-r--r--   0 valux      (501) staff       (20)     4292 2022-10-20 06:38:59.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/configurations.py
--rw-r--r--   0 valux      (501) staff       (20)     2783 2022-10-18 14:19:48.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/constants.py
--rw-r--r--   0 valux      (501) staff       (20)     1850 2022-10-18 14:19:53.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/log.py
--rw-r--r--   0 valux      (501) staff       (20)      606 2022-10-18 14:19:56.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/render.py
--rw-r--r--   0 valux      (501) staff       (20)     1039 2022-10-18 14:20:02.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/validators.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.693182 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/widgets/
--rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-27 06:43:04.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/widgets/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)      981 2022-10-18 14:20:09.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/widgets/configuiwidget.py
--rw-r--r--   0 valux      (501) staff       (20)     5733 2022-10-18 03:26:54.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/widgets/createsessionwidget.py
--rw-r--r--   0 valux      (501) staff       (20)      506 2022-09-21 11:38:19.000000 tencentcloud-dlc-jupyter-1.0.0b0/tdlc/widgets/managesessionwidget.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2022-10-24 06:50:51.694756 tencentcloud-dlc-jupyter-1.0.0b0/tencentcloud_dlc_jupyter.egg-info/
--rw-r--r--   0 valux      (501) staff       (20)      308 2022-10-24 06:50:51.000000 tencentcloud-dlc-jupyter-1.0.0b0/tencentcloud_dlc_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 valux      (501) staff       (20)     2103 2022-10-24 06:50:51.000000 tencentcloud-dlc-jupyter-1.0.0b0/tencentcloud_dlc_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 valux      (501) staff       (20)        1 2022-10-24 06:50:51.000000 tencentcloud-dlc-jupyter-1.0.0b0/tencentcloud_dlc_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 valux      (501) staff       (20)       94 2022-10-24 06:50:51.000000 tencentcloud-dlc-jupyter-1.0.0b0/tencentcloud_dlc_jupyter.egg-info/requires.txt
--rw-r--r--   0 valux      (501) staff       (20)        5 2022-10-24 06:50:51.000000 tencentcloud-dlc-jupyter-1.0.0b0/tencentcloud_dlc_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.188691 tencentcloud-dlc-jupyter-1.1.0/
+-rw-r--r--   0 valux      (501) staff       (20)      306 2023-07-06 09:24:38.188382 tencentcloud-dlc-jupyter-1.1.0/PKG-INFO
+-rw-r--r--   0 valux      (501) staff       (20)       38 2023-07-06 09:24:38.188767 tencentcloud-dlc-jupyter-1.1.0/setup.cfg
+-rw-r--r--   0 valux      (501) staff       (20)     1480 2023-02-16 06:56:13.000000 tencentcloud-dlc-jupyter-1.1.0/setup.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.169069 tencentcloud-dlc-jupyter-1.1.0/tdlc/
+-rw-r--r--   0 valux      (501) staff       (20)       17 2023-06-27 07:06:14.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/__init__.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.171018 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2022-08-22 14:04:50.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     5935 2023-06-30 05:55:23.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/cloudapi.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.173463 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/
+-rw-r--r--   0 valux      (501) staff       (20)      202 2022-09-05 09:16:24.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     3795 2023-04-28 18:19:12.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/command.py
+-rw-r--r--   0 valux      (501) staff       (20)     2379 2022-09-28 09:06:36.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/pandas2spark.py
+-rw-r--r--   0 valux      (501) staff       (20)     1667 2022-09-26 12:28:54.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/sqlcommand.py
+-rw-r--r--   0 valux      (501) staff       (20)     2634 2023-04-28 17:38:14.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/storecommand.py
+-rw-r--r--   0 valux      (501) staff       (20)     1122 2022-09-26 12:54:58.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/string2spark.py
+-rw-r--r--   0 valux      (501) staff       (20)     1039 2022-09-23 06:41:03.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/var2spark.py
+-rw-r--r--   0 valux      (501) staff       (20)     5375 2022-10-20 08:53:35.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/controllers.py
+-rw-r--r--   0 valux      (501) staff       (20)     1601 2023-06-30 06:50:13.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/qclient.py
+-rw-r--r--   0 valux      (501) staff       (20)     9460 2023-07-06 09:21:47.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/sessions.py
+-rw-r--r--   0 valux      (501) staff       (20)     4618 2023-06-30 06:20:18.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/exceptions.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.174594 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/
+-rw-r--r--   0 valux      (501) staff       (20)       39 2022-09-20 03:53:04.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/__init__.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.175023 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcpysparkkernel/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-20 03:26:39.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcpysparkkernel/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)      736 2022-09-22 08:11:56.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcpysparkkernel/pysparkkernel.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.175500 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcsparkkernel/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-20 02:51:37.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcsparkkernel/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)      715 2022-09-20 04:02:37.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcsparkkernel/sparkkernel.py
+-rw-r--r--   0 valux      (501) staff       (20)     5720 2022-10-18 14:19:21.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/kernelbase.py
+-rw-r--r--   0 valux      (501) staff       (20)     3170 2022-10-18 11:30:36.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/kernelmagics.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.176429 tencentcloud-dlc-jupyter-1.1.0/tdlc/magics/
+-rw-r--r--   0 valux      (501) staff       (20)       38 2022-09-15 15:38:31.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/magics/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     4154 2022-12-28 03:55:10.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/magics/basemagics.py
+-rw-r--r--   0 valux      (501) staff       (20)    13163 2023-06-30 06:40:11.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/magics/remotemagics.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.176769 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/
+-rw-r--r--   0 valux      (501) staff       (20)      630 2022-09-28 07:00:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/__init__.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.178518 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2023-06-30 06:50:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)    18589 2023-06-30 06:51:47.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 valux      (501) staff       (20)     2337 2023-06-30 06:50:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 valux      (501) staff       (20)     1968 2023-06-30 06:51:20.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/common_client.py
+-rw-r--r--   0 valux      (501) staff       (20)    15676 2023-06-30 06:51:13.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/credential.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.179142 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/exception/
+-rw-r--r--   0 valux      (501) staff       (20)      735 2023-06-30 06:50:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)      760 2023-06-30 06:50:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.179509 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/http/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2023-06-30 06:50:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     4998 2023-06-30 06:52:09.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/http/request.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.180563 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/profile/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2023-06-30 06:50:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     1655 2023-06-30 06:52:01.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 valux      (501) staff       (20)     1857 2023-06-30 06:50:46.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 valux      (501) staff       (20)     1573 2023-06-30 06:51:02.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/sign.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.180823 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2023-06-27 07:01:45.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.182378 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2023-06-27 07:01:45.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)   314526 2023-06-27 07:02:41.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 valux      (501) staff       (20)    14774 2023-06-27 07:01:45.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 valux      (501) staff       (20)   999665 2023-06-27 07:02:52.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/models.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.186031 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2022-08-22 14:15:50.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     2231 2022-10-18 11:05:47.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/common.py
+-rw-r--r--   0 valux      (501) staff       (20)     4534 2023-06-27 07:17:20.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/configurations.py
+-rw-r--r--   0 valux      (501) staff       (20)     2863 2023-06-30 06:26:45.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/constants.py
+-rw-r--r--   0 valux      (501) staff       (20)     1850 2022-10-18 14:19:53.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/log.py
+-rw-r--r--   0 valux      (501) staff       (20)      606 2022-10-18 14:19:56.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/render.py
+-rw-r--r--   0 valux      (501) staff       (20)     1039 2022-10-18 14:20:02.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/validators.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.187109 tencentcloud-dlc-jupyter-1.1.0/tdlc/widgets/
+-rw-r--r--   0 valux      (501) staff       (20)        0 2022-09-27 06:43:04.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/widgets/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)      981 2022-10-18 14:20:09.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/widgets/configuiwidget.py
+-rw-r--r--   0 valux      (501) staff       (20)     5733 2022-10-18 03:26:54.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/widgets/createsessionwidget.py
+-rw-r--r--   0 valux      (501) staff       (20)      506 2022-09-21 11:38:19.000000 tencentcloud-dlc-jupyter-1.1.0/tdlc/widgets/managesessionwidget.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-06 09:24:38.188056 tencentcloud-dlc-jupyter-1.1.0/tencentcloud_dlc_jupyter.egg-info/
+-rw-r--r--   0 valux      (501) staff       (20)      306 2023-07-06 09:24:38.000000 tencentcloud-dlc-jupyter-1.1.0/tencentcloud_dlc_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 valux      (501) staff       (20)     2103 2023-07-06 09:24:38.000000 tencentcloud-dlc-jupyter-1.1.0/tencentcloud_dlc_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 valux      (501) staff       (20)        1 2023-07-06 09:24:38.000000 tencentcloud-dlc-jupyter-1.1.0/tencentcloud_dlc_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 valux      (501) staff       (20)      105 2023-07-06 09:24:38.000000 tencentcloud-dlc-jupyter-1.1.0/tencentcloud_dlc_jupyter.egg-info/requires.txt
+-rw-r--r--   0 valux      (501) staff       (20)        5 2023-07-06 09:24:38.000000 tencentcloud-dlc-jupyter-1.1.0/tencentcloud_dlc_jupyter.egg-info/top_level.txt
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/setup.py` & `tencentcloud-dlc-jupyter-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,19 @@
     # package_data={
     # 	'tdlc': {
 
     # 	}
 
     # },
     install_requires=[
-        "ipython==7.8.0",
+        "ipython>=7.8.0",
         "numpy",
         "tornado>=4",
         "notebook>=4.2",
         "ipykernel>=4.2.2"
         "nose",
         "pandas",
         "requests",
         "ipywidgets",
+        "matplotlib",
     ]
 )
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/cloudapi.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/cloudapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tdlc.tencentcloud.common import credential
 from tdlc.tencentcloud.common.profile import http_profile, client_profile
 from tdlc.tencentcloud.dlc.v20210125 import models
 from tdlc.utils import log, configurations
 from tdlc.engines import qclient
+import base64
 
 LOG = log.getLogger('QCloud')
 
 
 def toSession(dto: models.NotebookSessionInfo) -> dict:
     session = {
         'name': dto.Name,
@@ -116,15 +117,16 @@
                     executor_size,
                     executor_num,
                     files=[],
                     jars=[],
                     pyfiles=[],
                     archives=[],
                     timeout=3600,
-                    arguments={}):
+                    arguments={},
+                    image=None):
 
         request = models.CreateNotebookSessionRequest()
         request.Name = name
         request.DataEngineName = engine
         request.Kind = kind
         request.DriverSize = driver_size
         request.ExecutorSize = executor_size
@@ -132,14 +134,15 @@
         request.ProgramDependentFiles = files
         request.ProgramDependentJars = jars
         request.ProgramDependentPython = pyfiles
         request.ProgramArchives = archives
         request.ProxyUser = configurations.PROXY_USER.get()
         request.TimeoutInSecond = timeout
         request.Arguments = []
+        request.SparkImage = image
 
         for k, v in arguments.items():
             o = models.KVPair()
             o.Key, o.Value = k, str(v)
             request.Arguments.append(o)
 
         response = self._client.CreateNotebookSession(request)
@@ -160,15 +163,17 @@
 
 
     def submit_statement(self, session_id, kind, statement):
 
         request = models.CreateNotebookSessionStatementRequest()
         request.SessionId = session_id
         request.Kind = kind
-        request.Code = statement
+        if not statement:
+            statement = ""
+        request.Code = base64.b64encode(statement.encode('utf8')).decode('utf8')
 
         response = self._client.CreateNotebookSessionStatement(request)
 
         return toStatement(response.NotebookSessionStatement)
 
 
     def get_statement(self, session_id, statement_id):
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/command.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         )
         render.render(progress)
 
         retries = 1
 
         while True:
             statement = session.get_statement(statement_id)
+            LOG.debug("The statement is :", statement)
             status = statement['status'].lower()
 
             if status not in constants.STATEMENT_STATUS_AVAILABLE:
                 progress.value = statement.get("progress", 0.0)
                 session.sleep(1)
                 retries += 1
             else:
@@ -84,16 +85,19 @@
                     if constants.MIMETYPE_IMAGE_PNG in data:
                         image = Image(base64.b64decode(data[constants.MIMETYPE_IMAGE_PNG]))
                         return (True, image, constants.MIMETYPE_IMAGE_PNG)
                     
                     elif constants.MIMETYPE_TEXT_HTML in data:
                         return (True, data[constants.MIMETYPE_TEXT_HTML], constants.MIMETYPE_TEXT_HTML)
                     
+                    # elif constants.MIMETYPE_TEXT_PLAIN in data:
+                    #     return (True, data[constants.MIMETYPE_TEXT_PLAIN], constants.MIMETYPE_TEXT_PLAIN)
                     else:
                         return (True, data[constants.MIMETYPE_TEXT_PLAIN], constants.MIMETYPE_TEXT_PLAIN)
+                        # return (True, "", constants.MIMETYPE_TEXT_PLAIN)
 
                 elif output['status'] == constants.OUTPUT_STATUS_ERROR:
                     error = output['error']
                     error_message =f'{error.get("name", "")}: {error.get("value", "")}\n {error.get("message", "")}'
                     return (False, f'{error_message}', constants.MIMETYPE_TEXT_PLAIN)
                 
                 else:
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/pandas2spark.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/pandas2spark.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/sqlcommand.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/sqlcommand.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/storecommand.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/storecommand.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         sample_fraction=None, 
         max_rows=None, 
         coerce=None) -> None:
         super().__init__("")
 
         self.output_var = output_var
         self.sample_method = sample_method or configurations.RESULT_SAMPLE_METHOD.get()
-        self.max_rows = max_rows or configurations.RESULT_MAX_ROWS.get()
         self.sample_fraction = sample_fraction or configurations.RESULT_SAMPLE_FRACTION.get()
         self.coerce = coerce
+        self.max_rows = max_rows or configurations.RESULT_MAX_ROWS.get()
 
 
     def _scala_command(self, output_var_context):
 
         code = f"{output_var_context}.toJSON"
         
         if self.sample_method == "sample":
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/string2spark.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/string2spark.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/commands/var2spark.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/commands/var2spark.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/controllers.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/controllers.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/qclient.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/qclient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from tdlc.tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tdlc.tencentcloud.dlc.v20210125 import dlc_client
 from tdlc.utils import log
 
 import tdlc
 import json
 
 
@@ -24,14 +24,15 @@
         if headers is None:
             headers = {}
 
         headers.setdefault('_v_', f'nb-{tdlc.VERSION}')
 
         err = None
 
+        # 网络异常
         while retry < self.RETRY_TIMES:
             LOG.debug(f"Calling (retry={retry}) {action} with  args: {params}")
             retry += 1
             try:
                 body = super().call(action, params, options, headers)
                 LOG.debug(f"Calling {action} with response: {body}")
 
@@ -40,18 +41,18 @@
                 if 'Error' in r['Response'] and 'Detail' in r['Response']['Error']:
 
                     try:
                         o = json.loads(r['Response']['Error']['Detail'])
                         r['Response']['Error']['Message'] = o['errMsg']
                         return json.dumps(r)
                     except Exception as e:
-                        LOG.error(e)
+                        LOG.warning(e)
+                    
                 return body
             except Exception as e:
-                LOG.error(e)
                 err = e
 
         if err is not None:
             raise err
 
         return body
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/engines/sessions.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/engines/sessions.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,49 +7,52 @@
 
 
 LOG = log.getLogger("Session")
 
 ''' 处理已知业务问题 '''
 def _handle_known_errors(e, *args):
 
-    LOG.error(e)
-
     ''' 引擎不存在问题 '''
-    if common.contains_all_keywords(e.message, ['Get House', 'fail']):
+    if common.contains_all_keywords(e.message, ['Find no house', 'fail']):
         raise exceptions.EngineNotExistException(*args)
     
     ''' RoleArn 不存在问题 '''
     if common.contains_all_keywords(e.message, ['Get role', 'fail']):
         raise exceptions.RoleArnNotFoundException(*args)
 
     ''' 远程 Session 不存在问题 '''
     if common.contains_all_keywords(e.message, ["Get session", "fail"]):
         raise exceptions.SessionNotFoundException(*args)
     
     ''' 集群 不在运行状态 '''
-    if common.contains_all_keywords(e.message, ["Cluster is not ready"]):
+    if common.contains_all_keywords(e.message, ["Cluster is not ready"]) or common.contains_all_keywords(e.message, ["not running"]):
         raise exceptions.EngineNotReadyException
     
     ''' 集群资源不足 '''
     if common.contains_all_keywords(e.message, ["Cluster resources insufficient"]):
         raise exceptions.EngineInsufficientException
+    
+    ''' 镜像不存在 '''
+    if common.contains_all_keywords(e.message, ["Spark images nonuniquen"]):
+        raise exceptions.ImageNotExistsException
 
     raise e
 
 class Session(object):
 
     def __init__(self, gateway, 
                        engine, 
                        name, 
                        kind,
                        roleArn=None,
                        timeout=None, 
                        driverSize=None, 
                        executorSize=None, 
                        executorNum=None, 
+                       image=None,
                        jars=[], 
                        pyfiles=[], 
                        archives=[], 
                        files=[],
                        conf={}) -> None:
 
         self._gateway :cloudapi.QCloudInteractiveApi= gateway
@@ -71,14 +74,15 @@
         self.name = name
         self.remote_name = self._build_session_name()
         self.kind = kind
         self.timeout = timeout or configurations.SESSION_TIMEOUT.get()
         self.driver_size = driverSize or configurations.DRIVER_SIZE.get()
         self.executor_size = executorSize or configurations.EXECUTOR_SIZE.get()
         self.executor_num = executorNum or configurations.EXECUTOR_NUM.get()
+        self.image = image
 
         self.spark_or_sql_context_var_name = None
     
     def _build_session_name(self):
         r = random.randint(0, 1000)
         return f'session-{int(time.time())}'
 
@@ -102,28 +106,29 @@
                 executor_size=self.executor_size,
                 executor_num=self.executor_num,
                 files=self._files,
                 jars=self._jars,
                 pyfiles=self._pyfiles,
                 archives=self._archives,
                 timeout=self.timeout,
-                arguments=arguments)
+                arguments=arguments,
+                image=self.image)
 
             self.id = r['sessionId']
             self.spark_app_id = r['sparkAppId']
             self.status = r['status']
             # self.spark_ui_url = r['appInfo']['sparkUiUrl']
 
         except Exception as e:
             _handle_known_errors(e)
 
         try:
             r = self.wait_for_idle()
         except exceptions.SessionTimeoutException as e:
-            raise exceptions.SessionTimeoutException(post=f"{self} did not start up in {configurations.WAIT_IDLE_TIMEOUT}s.")
+            raise exceptions.SessionTimeoutException(post=f"{self} did not start up in {configurations.WAIT_IDLE_TIMEOUT.get()}s.")
         except KeyboardInterrupt:
             # 不判断那状态 直接 kill
             # if self.status != constants.SESSION_STATUS_NOT_STARTED:
             # 处理 EOS 超时问题
             try:
                 self.stop()
             except Exception as e:
@@ -134,15 +139,18 @@
         
         self.render_as_table(True)
      
     def stop(self):
 
         render.toStdout(f"Closing the {self}...\n")
 
-        self._gateway.delete_session(self.id)
+        try:
+            self._gateway.delete_session(self.id)
+        except Exception as e:
+            LOG.error(e)
 
         starts = time.time()
 
         while time.time() - starts <= 60:
             self.refresh_status()
             if self.status in constants.SESSION_FINAL_STATUS:
                 render.toStdout(f"Successfully close the {self}.\n")
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/exceptions.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 
         
         msg = f'[{self.__class__.__name__}] {message}'
         if self.stack_message:
             msg += '\n\n' + self.stack_message
         return msg
 
+class ImageNotExistsException(tdlcException):
+    message = "The image is not exists."
 
 class EngineNotReadyException(tdlcException):
     message = "The engine is not ready, please check engines in DLC console. "
 
 class EngineNotExistException(tdlcException):
     message = "The engine is not found, please check engines in DLC console. "
 
@@ -166,7 +168,8 @@
     message = 'Parse dataframe error.'
 
 class InternalErrorException(tdlcException):
     message = "Internal Error. "
 
 
 
+
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcpysparkkernel/pysparkkernel.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcpysparkkernel/pysparkkernel.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/dlcsparkkernel/sparkkernel.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/dlcsparkkernel/sparkkernel.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/kernelbase.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/kernelbase.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/kernels/kernelmagics.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/kernels/kernelmagics.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/magics/basemagics.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/magics/basemagics.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/magics/remotemagics.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/magics/remotemagics.py`

 * *Files 14% similar despite different names*

```diff
@@ -209,14 +209,20 @@
     )
     @magic_arguments.argument(
         "--var-name",
         type=str,
         default=None,
         help="The variable name to store the data being sended. ",
     )
+    @magic_arguments.argument(
+        "--image",
+        type=str,
+        default=None,
+        help="The spark image to be used. ",
+    )
     @needs_local_scope
     @line_cell_magic
     @exceptions.wrap_magic_exceptions
     def spark(self, line, cell=None, local_ns=None):
         '''Magic to communicate with DLC spark cluster.
 
         The maigc is used to communicate a DLC spark cluster remotely. 
@@ -224,15 +230,15 @@
 
         Subcommand
         ----------
         ui
             Create session using GUI.
         config
             Config current kernel or globally if --save is provided.
-            e.g. `%%spark cohnfig --save
+            e.g. `%%spark config --save
                 {
                     region: <REGION>,
                     secret-id: <SECRETID>,
                     secret-key: <SECRETKEY>
                 }`
         start
             Create a new session.
@@ -259,15 +265,15 @@
             e.g. `%%spark --var-output var1 --max-rows 1000` will execute code and store the 1000 rows result typed pandas dataframe in 'var1'
         sql
             Execute SQL for a given session
             e.g. `%%spark sql --quiet` will execute SQL with no result.
             e.g. `%%spark sql --sample-method sample --sample-fraction 0.1 --max-rows 1000`
         send
             Sending local data to cluster.
-            e.g. `%spark send --var-intput localVar --var-type str --var-name remoteVar`
+            e.g. `%spark send --var-intput localVar --var-type str --var-output remoteVar`
         '''
         args = magic_arguments.parse_argstring(self.spark, line)
 
         qclouds_args = {
             'region': args.region or configurations.REGION.get(),
             'secretId': args.secret_id or configurations.SECRET_ID.get(),
             'secretKey': args.secret_key or configurations.SECRET_KEY.get(),
@@ -277,19 +283,37 @@
 
         properties_args = {
             'timeout': args.timeout or configurations.SESSION_TIMEOUT.get(),
             'roleArn': args.role_arn or configurations.ROLE_ARN.get(),
             'driverSize': args.driver_size or configurations.DRIVER_SIZE.get(),
             'executorSize': args.executor_size or configurations.EXECUTOR_SIZE.get(),
             'executorNum': args.executor_num or configurations.EXECUTOR_NUM.get(),
-            'jars': args.jars,
-            'pyfiles': args.py_files,
-            'archives': args.archives
+            'jars': args.jars or configurations.JARS.get(),
+            'pyfiles': args.py_files or configurations.PYFILES.get(),
+            'archives': args.archives or configurations.ARCHIVES.get(),
+            'image': args.image or configurations.IMAGE.get(),
         }
 
+        if properties_args['image']:
+            properties_args['image'] = properties_args['image'].strip("'").strip('"')
+
+        if properties_args['jars']:
+            properties_args['jars'] = properties_args['jars'].split(',')
+        else:
+            properties_args['jars'] = []
+
+        if properties_args['pyfiles']:
+            properties_args['pyfiles'] = properties_args['pyfiles'].split(',')
+        else:
+            properties_args['pyfiles'] = []
+
+        if properties_args['archives']:
+            properties_args['archives'] = properties_args['archives'].split(',')
+        else:
+            properties_args['archives'] = []
 
         engine = args.engine or configurations.ENGINE.get()
         if args.language is not None:
             validators.range(args.language, constants.LANGUAGES_SUPPORTED, f"The language is not supported, should be one of {', '.join(constants.LANGUAGES_SUPPORTED)}")
         
         sparkConf = configurations.SPARK_CONF.get()
         if args.conf:
@@ -347,15 +371,15 @@
         elif subcommand == 'logs':
             self.controller.render_logs(args.name, args.reverse)
 
         elif subcommand == 'sql':
             return self.execute_sqlquery(args.name, cell, args.var_output, args.sample_method, args.sample_fraction, args.max_rows, args.coerce, args.quiet)
         
         elif subcommand == "send":
-            return self.var_to_spark(args.name, args.var_input, args.var_type, args.var_name, args.max_rows)
+            return self.var_to_spark(args.name, args.var_input, args.var_type, args.var_output, args.max_rows)
 
         elif subcommand == "exec":
             return self.execute_spark(args.name, cell, args.var_output, args.sample_method, args.sample_fraction, args.max_rows, args.coerce, args.language)
         else:
             raise exceptions.CommandNotFoundException
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/__init__.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/abstract_client.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/abstract_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import logging.handlers
 
 try:
     from urllib.parse import urlencode
 except ImportError:
     from urllib import urlencode
 
-import tdlc
+from tdlc import tencentcloud
 from tdlc.tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tdlc.tencentcloud.common.exception import TencentCloudSDKException as SDKError
 from tdlc.tencentcloud.common.http.request import ApiRequest
 from tdlc.tencentcloud.common.http.request import RequestInternal
 from tdlc.tencentcloud.common.profile.client_profile import ClientProfile
 from tdlc.tencentcloud.common.sign import Sign
 
@@ -59,22 +59,19 @@
 
 class AbstractClient(object):
     _requestPath = '/'
     _params = {}
     _apiVersion = ''
     _endpoint = ''
     _service = ''
-    _sdkVersion = 'SDK_PYTHON_%s' % tdlc.tencentcloud.__version__
+    _sdkVersion = 'SDK_PYTHON_%s' % tencentcloud.__version__
     _default_content_type = _form_urlencoded_content
     FMT = '%(asctime)s %(process)d %(filename)s L%(lineno)s %(levelname)s %(message)s'
 
     def __init__(self, credential, region, profile=None):
-        if credential is None:
-            raise TencentCloudSDKException(
-                "InvalidCredential", "Credential is None or invalid")
         self.credential = credential
         self.region = region
         self.profile = ClientProfile() if profile is None else profile
         is_http = True if self.profile.httpProfile.scheme == "http" else False
         self.request = ApiRequest(self._get_endpoint(),
                                   req_timeout=self.profile.httpProfile.reqTimeout,
                                   proxy=self.profile.httpProfile.proxy,
@@ -115,15 +112,17 @@
                 d.update(self._format_params(key, v))
             return d
 
         raise TencentCloudSDKException("ClientParamsError", "some params type error")
 
     def _build_req_inter(self, action, params, req_inter, options=None):
         options = options or {}
-        if self.profile.signMethod == "TC3-HMAC-SHA256" or options.get("IsMultipart") is True:
+        if options.get('SkipSign'):
+            self._build_req_without_signature(action, params, req_inter, options)
+        elif self.profile.signMethod == "TC3-HMAC-SHA256" or options.get("IsMultipart") is True:
             self._build_req_with_tc3_signature(action, params, req_inter, options)
         elif self.profile.signMethod in ("HmacSHA1", "HmacSHA256"):
             self._build_req_with_old_signature(action, params, req_inter)
         else:
             raise TencentCloudSDKException("ClientError", "Invalid signature method.")
 
     def _build_req_with_old_signature(self, action, params, req):
@@ -196,15 +195,15 @@
         elif content_type == _json_content:
             req.data = json.dumps(params)
         elif content_type == _multipart_content:
             boundary = uuid.uuid4().hex
             req.header["Content-Type"] = content_type + "; boundary=" + boundary
             req.data = self._get_multipart_body(params, boundary, options)
 
-        service = endpoint.split('.')[0]
+        service = self._service
         date = datetime.utcfromtimestamp(timestamp).strftime('%Y-%m-%d')
         signature = self._get_tc3_signature(params, req, date, service, options)
 
         auth = "TC3-HMAC-SHA256 Credential=%s/%s/%s/tc3_request, SignedHeaders=content-type;host, Signature=%s" % (
             self.credential.secret_id, date, service, signature)
         req.header["Authorization"] = auth
 
@@ -244,14 +243,57 @@
         string2sign = '%s\n%s\n%s\n%s' % (algorithm,
                                           req.header["X-TC-Timestamp"],
                                           credential_scope,
                                           digest)
 
         return Sign.sign_tc3(self.credential.secret_key, date, service, string2sign)
 
+    def _build_req_without_signature(self, action, params, req, options=None):
+        content_type = self._default_content_type
+        if req.method == 'GET':
+            content_type = _form_urlencoded_content
+        elif req.method == 'POST':
+            content_type = _json_content
+        options = options or {}
+        if options.get("IsMultipart"):
+            content_type = _multipart_content
+        if options.get("IsOctetStream"):
+            content_type = _octet_stream
+        req.header["Content-Type"] = content_type
+
+        if req.method == "GET" and content_type == _multipart_content:
+            raise SDKError("ClientError",
+                           "Invalid request method GET for multipart.")
+
+        endpoint = self._get_endpoint()
+        timestamp = int(time.time())
+        req.header["Host"] = endpoint
+        req.header["X-TC-Action"] = action[0].upper() + action[1:]
+        req.header["X-TC-RequestClient"] = self._sdkVersion
+        req.header["X-TC-Timestamp"] = str(timestamp)
+        req.header["X-TC-Version"] = self._apiVersion
+        if self.profile.unsignedPayload is True:
+            req.header["X-TC-Content-SHA256"] = "UNSIGNED-PAYLOAD"
+        if self.region:
+            req.header['X-TC-Region'] = self.region
+        if self.profile.language:
+            req.header['X-TC-Language'] = self.profile.language
+
+        if req.method == 'GET':
+            params = copy.deepcopy(self._fix_params(params))
+            req.data = urlencode(params)
+        elif content_type == _json_content:
+            req.data = json.dumps(params)
+        elif content_type == _multipart_content:
+            boundary = uuid.uuid4().hex
+            req.header["Content-Type"] = content_type + "; boundary=" + boundary
+            req.data = self._get_multipart_body(params, boundary, options)
+
+        req.header["Authorization"] = "SKIP"
+
     # it must return bytes instead of string
     def _get_multipart_body(self, params, boundary, options=None):
         if options is None:
             options = {}
         # boundary and params key will never contain unicode characters
         boundary = boundary.encode()
         binparas = options.get("BinaryParams", [])
@@ -292,24 +334,38 @@
 
     def _get_endpoint(self):
         endpoint = self.profile.httpProfile.endpoint
         if endpoint is None:
             endpoint = self._get_service_domain()
         return endpoint
 
+    def _handle_response(self, data):
+        resp = json.loads(data)
+        if "Error" in resp["Response"]:
+            code = resp["Response"]["Error"]["Code"]
+            message = resp["Response"]["Error"]["Message"]
+            reqid = resp["Response"]["RequestId"]
+            raise TencentCloudSDKException(code, message, reqid)
+        if "DeprecatedWarning" in resp["Response"]:
+            import warnings
+            warnings.filterwarnings("default")
+            warnings.warn("This action is deprecated, detail: %s" % resp["Response"]["DeprecatedWarning"],
+                          DeprecationWarning)
+
     def call(self, action, params, options=None, headers=None):
         req = RequestInternal(self._get_endpoint(),
                               self.profile.httpProfile.reqMethod,
                               self._requestPath,
                               header=headers)
         self._build_req_inter(action, params, req, options)
 
         resp_inter = self.request.send_request(req)
         self._check_status(resp_inter)
         data = resp_inter.data
+        self._handle_response(data)
         return data
 
     def call_octet_stream(self, action, headers, body):
         """
         Invoke API with application/ocet-stream content-type.
 
         Note:
@@ -337,43 +393,35 @@
         req.data = body
         options = {"IsOctetStream": True}
         self._build_req_inter(action, None, req, options)
 
         resp = self.request.send_request(req)
         self._check_status(resp)
         data = resp.data
+        self._handle_response(data)
 
         json_rsp = json.loads(data)
-        if "Error" in json_rsp["Response"]:
-            code = json_rsp["Response"]["Error"]["Code"]
-            message = json_rsp["Response"]["Error"]["Message"]
-            reqid = json_rsp["Response"]["RequestId"]
-            raise TencentCloudSDKException(code, message, reqid)
         return json_rsp
 
-    def call_json(self, action, params, headers=None):
+    def call_json(self, action, params, headers=None, options=None):
         """
         Call api with json object and return with json object.
 
         :type action: str
         :param action: api name e.g. ``DescribeInstances``
         :type params: dict
         :param params: params with this action
-        :type header: dict
-        :param header: request header, like {"X-TC-TraceId": "ffe0c072-8a5d-4e17-8887-a8a60252abca"}
+        :type headers: dict
+        :param headers: request header, like {"X-TC-TraceId": "ffe0c072-8a5d-4e17-8887-a8a60252abca"}
+        :type options: dict
+        :param options: request options, like {"SkipSign": False, "IsMultipart": False, "IsOctetStream": False, "BinaryParams": []}
         """
-        body = self.call(action, params, headers=headers)
+        body = self.call(action, params, options, headers)
         response = json.loads(body)
-        if "Error" not in response["Response"]:
-            return response
-        else:
-            code = response["Response"]["Error"]["Code"]
-            message = response["Response"]["Error"]["Message"]
-            reqid = response["Response"]["RequestId"]
-            raise TencentCloudSDKException(code, message, reqid)
+        return response
 
     def set_stream_logger(self, stream=None, level=logging.DEBUG, log_format=None):
         """
         Add a stream handler
 
         :type stream: IO[str]
         :param stream: e.g. ``sys.stdout`` ``sys.stdin`` ``sys.stderr``
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/abstract_model.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/common_client.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/common_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     使用详情见github示例
 
     """
 
     def __init__(self, service, version, credential, region, profile=None):
         """
         :param credential: 接口调用凭证
-        :type credential: tdlc.tencentcloud.common.credential.Credential or tdlc.tencentcloud.common.credential.STSAssumeRoleCredential
+        :type credential: tencentcloud.common.credential.Credential or tencentcloud.common.credential.STSAssumeRoleCredential or None
         :param region: 接口调用地域
         :type region: str
         :param version: 接口版本
         :type version: str
         :param service: 接口产品
         :type service: str
         :param profile: 请求网络信息
-        :type profile: tdlc.tencentcloud.common.profile.client_profile.ClientProfile
+        :type profile: tencentcloud.common.profile.client_profile.ClientProfile
         """
-        if credential is None or region is None or version is None or service is None:
+        if region is None or version is None or service is None:
             raise TencentCloudSDKException("CommonClient Parameter Error, "
                                            "credential region version service all required.")
         self._apiVersion = version
         self._service = service
         super(CommonClient, self).__init__(credential, region, profile)
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/credential.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/credential.py`

 * *Files 12% similar despite different names*

```diff
@@ -345,7 +345,106 @@
             return self.cred
 
         self.cred = CVMRoleCredential().get_credential()
         if self.cred is not None:
             return self.cred
 
         raise TencentCloudSDKException("ClientSideError", "no valid credentail.")
+
+
+class DefaultTkeOIDCRoleArnProvider(object):
+    default_session_name = 'tencentcloud-python-sdk-'
+
+    def __init__(self):
+        self.region = os.getenv('TKE_REGION')
+        if not self.region:
+            raise EnvironmentError("TKE_REGION not exist")
+
+        self.provider_id = os.getenv('TKE_PROVIDER_ID')
+        if not self.provider_id:
+            raise EnvironmentError("TKE_PROVIDER_ID not exist")
+
+        token_file = os.getenv('TKE_IDENTITY_TOKEN_FILE')
+        if not token_file:
+            raise EnvironmentError("TKE_IDENTITY_TOKEN_FILE not exist")
+
+        with open(token_file) as f:
+            self.web_identity_token = f.read()
+
+        self.role_arn = os.getenv('TKE_ROLE_ARN')
+        if not self.role_arn:
+            raise EnvironmentError("TKE_ROLE_ARN not exist")
+
+        self.role_session_name = self.default_session_name + str(time.time() * 1e6)  # time in microseconds
+
+    def get_credentials(self):
+        return OIDCRoleArnCredential(self.region, self.provider_id, self.web_identity_token, self.role_arn,
+                                     self.role_session_name)
+
+
+class OIDCRoleArnCredential(object):
+    _version = '2018-08-13'
+    _service = "sts"
+    _action = 'AssumeRoleWithWebIdentity'
+
+    def __init__(self, region, provider_id, web_identity_token, role_arn, role_session_name, duration_seconds=7200):
+        self._region = region
+        self._provider_id = provider_id
+        self._web_identity_token = web_identity_token
+        self._role_arn = role_arn
+        self._role_session_name = role_session_name
+        self._duration_seconds = duration_seconds
+
+        self._token = None
+        self._tmp_secret_id = None
+        self._tmp_secret_key = None
+        self._expired_time = 0
+
+        self._last_role_arn = None
+        self._tmp_credential = None
+
+    @property
+    def secretId(self):
+        self._keep_fresh()
+        return self._tmp_secret_id
+
+    @property
+    def secretKey(self):
+        self._keep_fresh()
+        return self._tmp_secret_key
+
+    @property
+    def secret_id(self):
+        self._keep_fresh()
+        return self._tmp_secret_id
+
+    @property
+    def secret_key(self):
+        self._keep_fresh()
+        return self._tmp_secret_key
+
+    @property
+    def token(self):
+        self._keep_fresh()
+        return self._token
+
+    def _keep_fresh(self):
+        if None in [self._token, self._tmp_secret_key, self._tmp_secret_id] or self._expired_time < int(time.time()):
+            self.refresh()
+
+    def refresh(self):
+        common_client = CommonClient(credential=None, region=self._region, version=self._version, service=self._service)
+        params = {
+            "ProviderId": self._provider_id,
+            "WebIdentityToken": self._web_identity_token,
+            "RoleArn": self._role_arn,
+            "RoleSessionName": self._role_session_name,
+            "DurationSeconds": self._duration_seconds,
+        }
+
+        options = {'SkipSign': True}
+
+        rsp = common_client.call_json(self._action, params, options=options)
+        self._token = rsp["Response"]["Credentials"]["Token"]
+        self._tmp_secret_id = rsp["Response"]["Credentials"]["TmpSecretId"]
+        self._tmp_secret_key = rsp["Response"]["Credentials"]["TmpSecretKey"]
+        self._expired_time = rsp["Response"]["ExpiredTime"] - self._duration_seconds * 0.9
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/exception/__init__.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/exception/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from tdlc.tencentcloud.common.exception.tencent_cloud_sdk_exception import *
+from tencentcloud.common.exception.tencent_cloud_sdk_exception import *
 
 __all__ = ("TencentCloudSDKException")
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/http/request.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/http/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,27 +25,24 @@
     return os.environ.get(varname.lower()) or os.environ.get(varname.upper())
 
 
 class ProxyConnection(object):
     def __init__(self, host, timeout=60, proxy=None, certification=None, is_http=False):
         self.request_host = host
         self.certification = certification
-        if not certification:
+        if certification is None:
             self.certification = certifi.where()
         self.timeout = timeout
         self.proxy = None
         if is_http:
             proxy = proxy or _get_proxy_from_env(host, varname="HTTP_PROXY")
         else:
             proxy = proxy or _get_proxy_from_env(host, varname="HTTPS_PROXY")
         if proxy:
-            if is_http:
-                self.proxy = {"http": proxy}
-            else:
-                self.proxy = {"https": proxy}
+            self.proxy = {"http": proxy, "https": proxy}
         self.request_length = 0
 
     def request(self, method, url, body=None, headers={}):
         self.request_length = 0
         headers.setdefault("Host", self.request_host)
         return requests.request(method=method,
                                 url=url,
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/profile/client_profile.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/profile/http_profile.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/common/sign.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,23 +35,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddColumnAfter", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddColumnAfterResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddColumnAfterResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -64,23 +58,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddColumns", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddColumnsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddColumnsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -93,23 +81,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddDMSPartitions", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddDMSPartitionsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddDMSPartitionsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def AddLakeFsChdfsBinding(self, request):
+        """本接口（AddLakeFsChdfsBinding）用于添加chdfs权限组
+
+        :param request: Request instance for AddLakeFsChdfsBinding.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.AddLakeFsChdfsBindingRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.AddLakeFsChdfsBindingResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AddLakeFsChdfsBinding", params, headers=headers)
+            response = json.loads(body)
+            model = models.AddLakeFsChdfsBindingResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -122,23 +127,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddPartitionField", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddPartitionFieldResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddPartitionFieldResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -151,23 +150,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddSparkImage", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddSparkImageResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddSparkImageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -180,23 +173,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddSparkImageUserRecords", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddSparkImageUserRecordsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddSparkImageUserRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -209,23 +196,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -238,23 +219,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddUsersToWorkGroup", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddUsersToWorkGroupResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddUsersToWorkGroupResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -267,23 +242,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AddWhiteStrategy", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AddWhiteStrategyResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AddWhiteStrategyResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -296,23 +265,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterDMSDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterDMSDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterDMSDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -325,23 +288,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterDMSPartition", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterDMSPartitionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterDMSPartitionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -354,23 +311,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterDMSPartitionColumnStatistic", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterDMSPartitionColumnStatisticResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterDMSPartitionColumnStatisticResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -383,23 +334,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterDMSTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterDMSTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterDMSTableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -412,23 +357,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterDMSTableColumnStatistic", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterDMSTableColumnStatisticResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterDMSTableColumnStatisticResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -441,23 +380,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterMetaKeyConstraint", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterMetaKeyConstraintResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterMetaKeyConstraintResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -470,23 +403,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterTableColumns", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterTableColumnsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterTableColumnsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -499,23 +426,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterTableComment", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterTableCommentResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterTableCommentResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -528,23 +449,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AlterTableProperties", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AlterTablePropertiesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AlterTablePropertiesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -557,23 +472,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AssociateCHDFSAccessGroups", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AssociateCHDFSAccessGroupsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AssociateCHDFSAccessGroupsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -586,23 +495,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AssociateDatasourceHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AssociateDatasourceHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AssociateDatasourceHouseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -615,23 +518,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AttachUserPolicy", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AttachUserPolicyResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AttachUserPolicyResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -644,23 +541,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("AttachWorkGroupPolicy", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.AttachWorkGroupPolicyResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.AttachWorkGroupPolicyResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -673,23 +564,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("BindDefaultSharedEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.BindDefaultSharedEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.BindDefaultSharedEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -702,23 +587,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("BindTagsToDataEngines", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.BindTagsToDataEnginesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.BindTagsToDataEnginesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -731,81 +610,155 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("BindWorkGroupsToUser", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.BindWorkGroupsToUserResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.BindWorkGroupsToUserResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CancelNotebookSessionStatement(self, request):
-        """本接口（CancelNotebookSessionStatement）用于取消session statement
+        """本接口（CancelNotebookSessionStatement）用于取消session中执行的任务
 
         :param request: Request instance for CancelNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CancelNotebookSessionStatement", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CancelNotebookSessionStatementResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CancelNotebookSessionStatementResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CancelNotebookSessionStatementBatch(self, request):
+        """本接口（CancelNotebookSessionStatementBatch）用于批量取消Session 中执行的任务
+
+        :param request: Request instance for CancelNotebookSessionStatementBatch.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementBatchRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementBatchResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelNotebookSessionStatementBatch", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelNotebookSessionStatementBatchResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CancelSparkSessionBatchSQL(self, request):
+        """本接口（CancelSparkSessionBatchSQL）用于取消Spark SQL批任务。
+
+        :param request: Request instance for CancelSparkSessionBatchSQL.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CancelSparkSessionBatchSQLRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelSparkSessionBatchSQLResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelSparkSessionBatchSQL", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelSparkSessionBatchSQLResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CancelTableProperties(self, request):
+        """本接口（CancelTableProperties）用于删除表属性
+
+        :param request: Request instance for CancelTableProperties.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CancelTablePropertiesRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelTablePropertiesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelTableProperties", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelTablePropertiesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CancelTask(self, request):
-        """本接口（CancelTask），用于取消任务执行
+        """本接口（CancelTask），用于取消任务
 
         :param request: Request instance for CancelTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelTaskRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CancelTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CancelTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CancelTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CancelTasks(self, request):
+        """批量取消任务
+
+        :param request: Request instance for CancelTasks.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CancelTasksRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelTasksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelTasks", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -818,23 +771,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ChangeColumn", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ChangeColumnResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ChangeColumnResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -847,23 +794,86 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckDLCResourceRole", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckDLCResourceRoleResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckDLCResourceRoleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CheckDataEngineConfigPairsValidity(self, request):
+        """本接口（CheckDataEngineConfigPairsValidity）用于检查引擎用户自定义参数的有效性
+
+        :param request: Request instance for CheckDataEngineConfigPairsValidity.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CheckDataEngineConfigPairsValidityRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CheckDataEngineConfigPairsValidityResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CheckDataEngineConfigPairsValidity", params, headers=headers)
+            response = json.loads(body)
+            model = models.CheckDataEngineConfigPairsValidityResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CheckDataEngineImageCanBeRollback(self, request):
+        """本接口（CheckDataEngineImageCanBeRollback）用于查看集群是否能回滚。
+
+        :param request: Request instance for CheckDataEngineImageCanBeRollback.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CheckDataEngineImageCanBeRollbackRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CheckDataEngineImageCanBeRollbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CheckDataEngineImageCanBeRollback", params, headers=headers)
+            response = json.loads(body)
+            model = models.CheckDataEngineImageCanBeRollbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CheckDataEngineImageCanBeUpgrade(self, request):
+        """本接口（CheckDataEngineImageCanBeUpgrade）用于查看集群镜像是否能够升级。
+
+        :param request: Request instance for CheckDataEngineImageCanBeUpgrade.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CheckDataEngineImageCanBeUpgradeRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CheckDataEngineImageCanBeUpgradeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CheckDataEngineImageCanBeUpgrade", params, headers=headers)
+            response = json.loads(body)
+            model = models.CheckDataEngineImageCanBeUpgradeResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -876,23 +886,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckDatabaseExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckDatabaseExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckDatabaseExistsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -905,23 +909,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckDatabaseUDFExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckDatabaseUDFExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckDatabaseUDFExistsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -934,23 +932,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckDatasourceConnectivity", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckDatasourceConnectivityResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckDatasourceConnectivityResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -963,23 +955,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckInstanceName", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckInstanceNameResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckInstanceNameResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -992,23 +978,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckLakeFsChdfsEnable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckLakeFsChdfsEnableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckLakeFsChdfsEnableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1021,23 +1001,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckLakeFsExist", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckLakeFsExistResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckLakeFsExistResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1050,23 +1024,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckLockMetaData", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckLockMetaDataResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckLockMetaDataResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CheckRegionCHDFSEnable(self, request):
+        """此接口（CheckRegionCHDFSEnable）用于检查当前地域是否支持元数据加速桶能力
+
+        :param request: Request instance for CheckRegionCHDFSEnable.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CheckRegionCHDFSEnableRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CheckRegionCHDFSEnableResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CheckRegionCHDFSEnable", params, headers=headers)
+            response = json.loads(body)
+            model = models.CheckRegionCHDFSEnableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1079,23 +1070,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckSQLSessionCatalogNameExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckSQLSessionCatalogNameExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckSQLSessionCatalogNameExistsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1108,23 +1093,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckScheduleScriptExist", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckScheduleScriptExistResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckScheduleScriptExistResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1137,23 +1116,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckScheduleTaskNameExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckScheduleTaskNameExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckScheduleTaskNameExistsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1166,23 +1139,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckSparkImageExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckSparkImageExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckSparkImageExistsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1195,23 +1162,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckSparkImageUserRecordExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckSparkImageUserRecordExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckSparkImageUserRecordExistsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1224,23 +1185,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckTableExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckTableExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckTableExistsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1253,23 +1208,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CheckViewExists", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CheckViewExistsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CheckViewExistsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CheckVpcCidrBlock(self, request):
+        """检查vpc的cidrblock是否符合要求
+
+        :param request: Request instance for CheckVpcCidrBlock.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CheckVpcCidrBlockRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CheckVpcCidrBlockResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CheckVpcCidrBlock", params, headers=headers)
+            response = json.loads(body)
+            model = models.CheckVpcCidrBlockResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1282,23 +1254,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CleanImportStorage", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CleanImportStorageResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CleanImportStorageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1311,23 +1277,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CloseOrOpenSQLSessionSnapshot", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CloseOrOpenSQLSessionSnapshotResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CloseOrOpenSQLSessionSnapshotResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1340,23 +1300,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateAdministrator", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateAdministratorResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateAdministratorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateCHDFSBindingProduct(self, request):
+        """此接口（CreateCHDFSBindingProduct）用于创建元数据加速桶和产品绑定关系
+
+        :param request: Request instance for CreateCHDFSBindingProduct.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateCHDFSBindingProductRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateCHDFSBindingProductResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateCHDFSBindingProduct", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateCHDFSBindingProductResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateCHDFSProduct(self, request):
+        """此接口（CreateCHDFSProduct）创建元数据加速桶绑定产品
+
+        :param request: Request instance for CreateCHDFSProduct.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateCHDFSProductRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateCHDFSProductResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateCHDFSProduct", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateCHDFSProductResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1369,23 +1369,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateDMSDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateDMSDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateDMSDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1398,52 +1392,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateDMSTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateDMSTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateDMSTableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateDataEngine(self, request):
-        """为用户创建默认数据连接
+        """为用户创建数据引擎
 
         :param request: Request instance for CreateDataEngine.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateDataEngineRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateDataEngineResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1456,23 +1438,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateDataQuery", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateDataQueryResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateDataQueryResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1485,23 +1461,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1514,23 +1484,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateDatasourceConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateDatasourceConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateDatasourceConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1543,23 +1507,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateDefaultDatasourceConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateDefaultDatasourceConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateDefaultDatasourceConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1572,23 +1530,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateExportResultTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateExportResultTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateExportResultTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1601,23 +1553,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateExportTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateExportTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateExportTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1630,23 +1576,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateHouseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1659,52 +1599,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateImportTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateImportTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateImportTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateInternalTable(self, request):
-        """创建托管存储内表
+        """创建托管存储内表（该接口已废弃）
 
         :param request: Request instance for CreateInternalTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateInternalTableRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateInternalTableResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateInternalTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateInternalTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateInternalTableResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateKyuubiTask(self, request):
+        """创建Kyuubi任务
+
+        :param request: Request instance for CreateKyuubiTask.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateKyuubiTaskRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateKyuubiTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateKyuubiTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateKyuubiTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1717,23 +1668,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateLakeFs", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateLakeFsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateLakeFsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1746,23 +1691,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateLakeFsChdfsBinding", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateLakeFsChdfsBindingResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateLakeFsChdfsBindingResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1775,23 +1714,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateLink", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateLinkResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateLinkResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1804,81 +1737,109 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateMetaDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateMetaDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateMetaDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateNotebookSession(self, request):
-        """本接口（CreateNotebookSession）用于创建notebook livy session
+        """本接口（CreateNotebookSession）用于创建交互式session（notebook）
 
         :param request: Request instance for CreateNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateNotebookSession", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateNotebookSessionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateNotebookSessionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateNotebookSessionStatement(self, request):
-        """本接口（CreateNotebookSessionStatement）用于创建session statement
+        """本接口（CreateNotebookSessionStatement）用于在session中执行代码片段
 
         :param request: Request instance for CreateNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateNotebookSessionStatement", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateNotebookSessionStatementResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateNotebookSessionStatementResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateNotebookSessionStatementSupportBatchSQL(self, request):
+        """本接口（CreateNotebookSessionStatementSupportBatchSQL）用于创建交互式session并执行SQL任务
+
+        :param request: Request instance for CreateNotebookSessionStatementSupportBatchSQL.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementSupportBatchSQLRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementSupportBatchSQLResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateNotebookSessionStatementSupportBatchSQL", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateNotebookSessionStatementSupportBatchSQLResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateOrModifyCHDFSProduct(self, request):
+        """此接口（CreateOrModifyCHDFSProduct）创建或修改元数据加速桶绑定产品
+
+        :param request: Request instance for CreateOrModifyCHDFSProduct.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateOrModifyCHDFSProductRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateOrModifyCHDFSProductResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateOrModifyCHDFSProduct", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateOrModifyCHDFSProductResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1891,52 +1852,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateQueryDir", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateQueryDirResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateQueryDirResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateResultDownload(self, request):
+        """创建查询结果下载任务
+
+        :param request: Request instance for CreateResultDownload.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateResultDownloadRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateResultDownloadResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateResultDownload", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateResultDownloadResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateSQLSessionCatalog(self, request):
-        """本接口（CreateSQLSessionCatalog）用于数据探索创建目录
+        """本接口（CreateSQLSessionCatalog）用于数据探索创建目录。
 
         :param request: Request instance for CreateSQLSessionCatalog.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSQLSessionCatalogRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSQLSessionCatalogResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateSQLSessionCatalog", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateSQLSessionCatalogResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateSQLSessionCatalogResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1949,23 +1921,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateSQLSessionSnapshot", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateSQLSessionSnapshotResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateSQLSessionSnapshotResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -1978,23 +1944,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateSQLSessionSubmitRecord", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateSQLSessionSubmitRecordResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateSQLSessionSubmitRecordResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2007,23 +1967,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateScheduleTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateScheduleTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateScheduleTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2036,81 +1990,109 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateScript", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateScriptResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateScriptResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateSparkApp(self, request):
-        """创建spark应用
+        """创建spark作业
 
         :param request: Request instance for CreateSparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateSparkApp", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateSparkAppResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateSparkAppResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateSparkAppForSQL(self, request):
+        """本接口（CreateSparkAppForSQL）用于创建Spark Batch任务运行SQL。
+
+        :param request: Request instance for CreateSparkAppForSQL.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppForSQLRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppForSQLResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateSparkAppForSQL", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateSparkAppForSQLResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateSparkAppTask(self, request):
-        """创建spark任务
+        """启动Spark作业
 
         :param request: Request instance for CreateSparkAppTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppTaskRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateSparkAppTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateSparkAppTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateSparkAppTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateSparkSessionBatchSQL(self, request):
+        """本接口（CreateSparkSessionBatchSQL）用于向Spark作业引擎提交Spark SQL批任务。
+
+        :param request: Request instance for CreateSparkSessionBatchSQL.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkSessionBatchSQLRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSparkSessionBatchSQLResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateSparkSessionBatchSQL", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateSparkSessionBatchSQLResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2123,23 +2105,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateStoreLocation", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateStoreLocationResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateStoreLocationResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2152,81 +2128,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateTableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTask(self, request):
-        """本接口（CreateTask）用于创建sql查询任务。（推荐使用CreateTasks接口）
+        """本接口（CreateTask）用于创建并执行SQL任务。（推荐使用CreateTasks接口）
 
         :param request: Request instance for CreateTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTaskRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTasks(self, request):
-        """本接口（CreateTasks），用于批量创建任务
+        """本接口（CreateTasks），用于批量创建并执行SQL任务
 
         :param request: Request instance for CreateTasks.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTasksRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateTasksResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2239,23 +2197,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateTasksInOrder", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateTasksInOrderResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateTasksInOrderResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2268,23 +2220,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateUser", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateUserResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateUserResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2297,23 +2243,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateUserRole", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateUserRoleResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateUserRoleResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2326,23 +2266,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateWorkGroup", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateWorkGroupResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateWorkGroupResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2355,23 +2289,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateWorkflow", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.CreateWorkflowResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.CreateWorkflowResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteCHDFSBindingProduct(self, request):
+        """此接口（DeleteCHDFSBindingProduct）用于删除元数据加速桶和产品绑定关系
+
+        :param request: Request instance for DeleteCHDFSBindingProduct.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteCHDFSBindingProductRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DeleteCHDFSBindingProductResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteCHDFSBindingProduct", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteCHDFSBindingProductResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteCHDFSProduct(self, request):
+        """此接口（DeleteCHDFSProduct）用于删除元数据加速桶绑定产品
+
+        :param request: Request instance for DeleteCHDFSProduct.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteCHDFSProductRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DeleteCHDFSProductResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteCHDFSProduct", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteCHDFSProductResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2384,23 +2358,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteColumns", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteColumnsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteColumnsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2413,23 +2381,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2442,23 +2404,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteDataQuery", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteDataQueryResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteDataQueryResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2471,23 +2427,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteDatabaseUDF", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteDatabaseUDFResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteDatabaseUDFResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2500,23 +2450,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteDatasourceConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteDatasourceConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteDatasourceConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2529,23 +2473,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteHouseResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteLakeFs(self, request):
+        """删除托管存储
+
+        :param request: Request instance for DeleteLakeFs.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteLakeFsRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DeleteLakeFsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteLakeFs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteLakeFsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2558,23 +2519,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteLakeFsChdfsBinding", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteLakeFsChdfsBindingResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteLakeFsChdfsBindingResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2587,23 +2542,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteLink", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteLinkResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteLinkResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2616,52 +2565,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteMetaDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteMetaDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteMetaDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteNotebookSession(self, request):
-        """本接口（DeleteNotebookSession）用于删除notebook livy session
+        """本接口（DeleteNotebookSession）用于删除交互式session（notebook）
 
         :param request: Request instance for DeleteNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteNotebookSessionRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DeleteNotebookSessionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteNotebookSession", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteNotebookSessionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteNotebookSessionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2674,23 +2611,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeletePartitionField", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeletePartitionFieldResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeletePartitionFieldResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2703,23 +2634,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteQueryDir", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteQueryDirResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteQueryDirResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2732,23 +2657,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteSQLSessionCatalog", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteSQLSessionCatalogResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteSQLSessionCatalogResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2761,23 +2680,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteSQLSessionSnapshot", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteSQLSessionSnapshotResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteSQLSessionSnapshotResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2790,23 +2703,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteScheduleTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteScheduleTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteScheduleTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2819,52 +2726,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteScript", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteScriptResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteScriptResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteSparkApp(self, request):
-        """删除spark应用
+        """删除spark作业
 
         :param request: Request instance for DeleteSparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteSparkAppRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DeleteSparkAppResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteSparkApp", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteSparkAppResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteSparkAppResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2877,23 +2772,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteSparkImage", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteSparkImageResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteSparkImageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2906,23 +2795,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteSparkImageUserRecords", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteSparkImageUserRecordsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteSparkImageUserRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2935,23 +2818,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteTableResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteTableBatch(self, request):
+        """本接口（DeleteTableBatch）用于批量删除表
+
+        :param request: Request instance for DeleteTableBatch.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteTableBatchRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DeleteTableBatchResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteTableBatch", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteTableBatchResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2964,23 +2864,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteUser", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteUserResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteUserResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -2993,23 +2887,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteUserRole", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteUserRoleResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteUserRoleResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3022,23 +2910,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteUsersFromWorkGroup", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteUsersFromWorkGroupResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteUsersFromWorkGroupResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3051,23 +2933,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteView", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteViewResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteViewResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3080,23 +2956,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteWorkGroup", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteWorkGroupResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteWorkGroupResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3109,23 +2979,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DeleteWorkflow", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DeleteWorkflowResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DeleteWorkflowResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3138,23 +3002,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeAdvancedStoreLocation", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeAdvancedStoreLocationResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeAdvancedStoreLocationResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3167,23 +3025,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeAllColumns", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeAllColumnsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeAllColumnsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3196,23 +3048,86 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeAuditEvents", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeAuditEventsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeAuditEventsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeAvailableVpc(self, request):
+        """获取可用的vpc信息
+
+        :param request: Request instance for DescribeAvailableVpc.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeAvailableVpcRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeAvailableVpcResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAvailableVpc", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAvailableVpcResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeBucketType(self, request):
+        """此接口（DescribeBucketType）用于查询当前桶类型
+
+        :param request: Request instance for DescribeBucketType.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeBucketTypeRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeBucketTypeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBucketType", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBucketTypeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeCHDFSAccessInfos(self, request):
+        """此接口（DescribeCHDFSAccessInfos）用于查询元数据加速桶访问权限配置（托管桶和用户桶）
+
+        :param request: Request instance for DescribeCHDFSAccessInfos.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeCHDFSAccessInfosRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeCHDFSAccessInfosResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCHDFSAccessInfos", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCHDFSAccessInfosResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3225,23 +3140,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeCHDFSMountPointAssociateInfos", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeCHDFSMountPointAssociateInfosResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeCHDFSMountPointAssociateInfosResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeCHDFSMountPointSuperuser(self, request):
+        """此接口（DescribeCHDFSMountPointSuperuser）用于查询桶Superuser
+
+        :param request: Request instance for DescribeCHDFSMountPointSuperuser.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeCHDFSMountPointSuperuserRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeCHDFSMountPointSuperuserResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCHDFSMountPointSuperuser", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCHDFSMountPointSuperuserResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3254,23 +3186,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeCHDFSMountPoints", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeCHDFSMountPointsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeCHDFSMountPointsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeCHDFSProducts(self, request):
+        """此接口（DescribeCHDFSProducts）用于查询元数据加速桶绑定产品
+
+        :param request: Request instance for DescribeCHDFSProducts.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeCHDFSProductsRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeCHDFSProductsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCHDFSProducts", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCHDFSProductsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3283,23 +3232,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeColumns", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeColumnsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeColumnsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeDLCCHDFSBindingList(self, request):
+        """此接口（DescribeDLCCHDFSBindingList）用于查询DLC元数据加速桶绑定列表
+
+        :param request: Request instance for DescribeDLCCHDFSBindingList.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDLCCHDFSBindingListRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDLCCHDFSBindingListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDLCCHDFSBindingList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDLCCHDFSBindingListResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3312,23 +3278,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDMSDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDMSDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDMSDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3341,23 +3301,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDMSPartitionColumnStatisticList", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDMSPartitionColumnStatisticListResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDMSPartitionColumnStatisticListResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3370,23 +3324,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDMSPartitions", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDMSPartitionsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDMSPartitionsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3399,23 +3347,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDMSTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDMSTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDMSTableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3428,23 +3370,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDMSTableColumnStatisticList", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDMSTableColumnStatisticListResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDMSTableColumnStatisticListResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3457,23 +3393,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDMSTables", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDMSTablesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDMSTablesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3486,23 +3416,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3515,23 +3439,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDataEngineEvents", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDataEngineEventsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDataEngineEventsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeDataEngineImageOperateRecords(self, request):
+        """本接口（DescribeDataEngineImageOperateRecords）用于获取引擎镜像操作日志列表。
+
+        :param request: Request instance for DescribeDataEngineImageOperateRecords.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEngineImageOperateRecordsRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEngineImageOperateRecordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDataEngineImageOperateRecords", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDataEngineImageOperateRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeDataEngineImageVersions(self, request):
+        """本接口（DescribeDataEngineImageVersions）用于获取独享集群大版本镜像列表。
+
+        :param request: Request instance for DescribeDataEngineImageVersions.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEngineImageVersionsRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEngineImageVersionsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDataEngineImageVersions", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDataEngineImageVersionsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3544,52 +3508,86 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDataEngineParameters", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDataEngineParametersResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDataEngineParametersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeDataEnginePythonSparkImages(self, request):
+        """本接口（DescribeDataEnginePythonSparkImages）用于获取PYSPARK镜像列表
+
+        :param request: Request instance for DescribeDataEnginePythonSparkImages.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEnginePythonSparkImagesRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEnginePythonSparkImagesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDataEnginePythonSparkImages", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDataEnginePythonSparkImagesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeDataEngineSessionParameters(self, request):
+        """本接口（DescribeDataEngineSessionParameters）用于获取指定小版本下的Session配置。
+
+        :param request: Request instance for DescribeDataEngineSessionParameters.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEngineSessionParametersRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEngineSessionParametersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDataEngineSessionParameters", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDataEngineSessionParametersResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDataEngines(self, request):
-        """本接口（DescribeDataEngines）用于获取DataEngines信息列表
+        """本接口（DescribeDataEngines）用于查询DataEngines信息列表
 
         :param request: Request instance for DescribeDataEngines.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEnginesRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEnginesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDataEngines", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDataEnginesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDataEnginesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3602,23 +3600,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDataQueries", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDataQueriesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDataQueriesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3631,23 +3623,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDataQuery", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDataQueryResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDataQueryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeDataTaskAlarmFiled(self, request):
+        """该接口（DescribeDataTaskAlarmFiled）用于云监控查询数据任务告警字段
+
+        :param request: Request instance for DescribeDataTaskAlarmFiled.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataTaskAlarmFiledRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDataTaskAlarmFiledResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDataTaskAlarmFiled", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDataTaskAlarmFiledResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3660,23 +3669,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3689,23 +3692,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDatabaseUDFList", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDatabaseUDFListResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDatabaseUDFListResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3718,23 +3715,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDatabases", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDatabasesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDatabasesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3747,23 +3738,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDatasourceConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDatasourceConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDatasourceConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3776,23 +3761,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDefaultEngineConfig", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeDefaultEngineConfigResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeDefaultEngineConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeEngineUsageInfo(self, request):
+        """本接口根据引擎ID查询数据引擎资源使用情况
+
+        :param request: Request instance for DescribeEngineUsageInfo.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeEngineUsageInfoRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeEngineUsageInfoResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeEngineUsageInfo", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeEngineUsageInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3805,23 +3807,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeExportResultTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeExportResultTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeExportResultTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3834,23 +3830,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeFatherAndSonTaskInstances", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeFatherAndSonTaskInstancesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeFatherAndSonTaskInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3863,23 +3853,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeFatherAndSonTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeFatherAndSonTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeFatherAndSonTasksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeForbiddenTablePro(self, request):
+        """本接口（DescribeForbiddenTablePro）用于查询被禁用的表属性列表（新）
+
+        :param request: Request instance for DescribeForbiddenTablePro.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeForbiddenTableProRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeForbiddenTableProResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeForbiddenTablePro", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeForbiddenTableProResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeForbiddenTableProperties(self, request):
+        """本接口（DescribeForbiddenTableProperties）用于获取被禁用的表属性列表
+
+        :param request: Request instance for DescribeForbiddenTableProperties.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeForbiddenTablePropertiesRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeForbiddenTablePropertiesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeForbiddenTableProperties", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeForbiddenTablePropertiesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3892,23 +3922,86 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeFunctions", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeFunctionsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeFunctionsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeGovernDefaultPolicy(self, request):
+        """查询数据治理规则默认值
+
+        :param request: Request instance for DescribeGovernDefaultPolicy.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeGovernDefaultPolicyRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeGovernDefaultPolicyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeGovernDefaultPolicy", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeGovernDefaultPolicyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeGovernEventRule(self, request):
+        """查询数据治理事件阈值
+
+        :param request: Request instance for DescribeGovernEventRule.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeGovernEventRuleRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeGovernEventRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeGovernEventRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeGovernEventRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeGovernMetaInfo(self, request):
+        """查询数据治理元信息
+
+        :param request: Request instance for DescribeGovernMetaInfo.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeGovernMetaInfoRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeGovernMetaInfoResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeGovernMetaInfo", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeGovernMetaInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3921,23 +4014,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeHouseEvents", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeHouseEventsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeHouseEventsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3950,23 +4037,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeInstanceLogList", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeInstanceLogListResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeInstanceLogListResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -3979,23 +4060,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeLakeFsAccess", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeLakeFsAccessResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeLakeFsAccessResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4008,23 +4083,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeLakeFsChdfsBindings", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeLakeFsChdfsBindingsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeLakeFsChdfsBindingsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4037,23 +4106,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeLakeFsChdfsNames", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeLakeFsChdfsNamesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeLakeFsChdfsNamesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeLakeFsDirSummary(self, request):
+        """查询托管存储指定目录的Summary
+
+        :param request: Request instance for DescribeLakeFsDirSummary.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsDirSummaryRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsDirSummaryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLakeFsDirSummary", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLakeFsDirSummaryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeLakeFsInfo(self, request):
+        """查询用户的托管存储信息
+
+        :param request: Request instance for DescribeLakeFsInfo.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsInfoRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsInfoResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLakeFsInfo", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLakeFsInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4066,23 +4175,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeLakeFsPath", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeLakeFsPathResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeLakeFsPathResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeLakeFsWarehouseAccess(self, request):
+        """查询托管存储warehouse目录的访问权限
+
+        :param request: Request instance for DescribeLakeFsWarehouseAccess.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsWarehouseAccessRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsWarehouseAccessResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLakeFsWarehouseAccess", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLakeFsWarehouseAccessResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4095,23 +4221,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMainDataDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMainDataDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMainDataDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4124,23 +4244,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMainDataOverview", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMainDataOverviewResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMainDataOverviewResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4153,23 +4267,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMainDataOverviewLine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMainDataOverviewLineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMainDataOverviewLineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4182,23 +4290,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMainDataPrivateEngineLine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMainDataPrivateEngineLineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMainDataPrivateEngineLineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4211,23 +4313,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMainDataShareEngineLine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMainDataShareEngineLineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMainDataShareEngineLineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4240,23 +4336,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMainDataTaskLine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMainDataTaskLineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMainDataTaskLineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4269,23 +4359,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMetaDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMetaDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMetaDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4298,23 +4382,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMetaDatabases", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMetaDatabasesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMetaDatabasesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4327,23 +4405,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMetaKeyConstraint", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMetaKeyConstraintResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMetaKeyConstraintResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4356,23 +4428,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMetaTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMetaTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMetaTableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4385,23 +4451,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMetaTableInternal", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMetaTableInternalResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMetaTableInternalResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4414,23 +4474,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMetaTables", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMetaTablesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMetaTablesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4443,23 +4497,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeMonitorObjects", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeMonitorObjectsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeMonitorObjectsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4472,139 +4520,155 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeNetworkConnections", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeNetworkConnectionsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeNetworkConnectionsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSession(self, request):
-        """本接口（DescribeNotebookSession）用于获取notebook livy session详情信息
+        """本接口（DescribeNotebookSession）用于查询交互式 session详情信息
 
         :param request: Request instance for DescribeNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeNotebookSession", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeNotebookSessionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeNotebookSessionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSessionLog(self, request):
-        """本接口（DescribeNotebookSessionLog）用于获取notebook livy session日志
+        """本接口（DescribeNotebookSessionLog）用于查询交互式 session日志
 
         :param request: Request instance for DescribeNotebookSessionLog.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionLogRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionLogResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeNotebookSessionLog", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeNotebookSessionLogResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeNotebookSessionLogResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSessionStatement(self, request):
-        """本接口（DescribeNotebookSessionStatement）用于获取session statement信息
+        """本接口（DescribeNotebookSessionStatement）用于查询session 中执行任务的详情
 
         :param request: Request instance for DescribeNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeNotebookSessionStatement", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeNotebookSessionStatementResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeNotebookSessionStatementResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeNotebookSessionStatementSqlResult(self, request):
+        """本接口（DescribeNotebookSessionStatementSqlResult）用于获取statement运行结果。
+
+        :param request: Request instance for DescribeNotebookSessionStatementSqlResult.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementSqlResultRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementSqlResultResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeNotebookSessionStatementSqlResult", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeNotebookSessionStatementSqlResultResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeNotebookSessionStatements(self, request):
+        """本接口（DescribeNotebookSessionStatements）用于查询Session中执行的任务列表
+
+        :param request: Request instance for DescribeNotebookSessionStatements.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementsRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeNotebookSessionStatements", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeNotebookSessionStatementsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSessions(self, request):
-        """本接口（DescribeNotebookSessions）用于获取notebook livy session列表
+        """本接口（DescribeNotebookSessions）用于查询交互式 session列表
 
         :param request: Request instance for DescribeNotebookSessions.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionsRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeNotebookSessions", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeNotebookSessionsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeNotebookSessionsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4617,23 +4681,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeOrCreateCHDFSAccessGroups", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeOrCreateCHDFSAccessGroupsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeOrCreateCHDFSAccessGroupsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeOtherCHDFSBindingList(self, request):
+        """此接口（DescribeOtherCHDFSBindingList）用于查询其他产品元数据加速桶绑定列表
+
+        :param request: Request instance for DescribeOtherCHDFSBindingList.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeOtherCHDFSBindingListRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeOtherCHDFSBindingListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOtherCHDFSBindingList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOtherCHDFSBindingListResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4646,23 +4727,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeQueryDir", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeQueryDirResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeQueryDirResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4675,23 +4750,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeQueryDirs", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeQueryDirsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeQueryDirsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4704,23 +4773,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeQueue", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeQueueResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeQueueResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4733,23 +4796,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeRegion", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeRegionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeRegionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeResultDownload(self, request):
+        """查询结果下载任务
+
+        :param request: Request instance for DescribeResultDownload.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeResultDownloadRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeResultDownloadResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeResultDownload", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeResultDownloadResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4762,23 +4842,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeResultDownloadInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeResultDownloadInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeResultDownloadInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4791,23 +4865,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeResultSize", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeResultSizeResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeResultSizeResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4820,23 +4888,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSQLSessionCatalog", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSQLSessionCatalogResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSQLSessionCatalogResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4849,23 +4911,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSQLSessionSnapshot", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSQLSessionSnapshotResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSQLSessionSnapshotResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4878,23 +4934,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSQLSessionSnapshots", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSQLSessionSnapshotsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSQLSessionSnapshotsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4907,23 +4957,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSQLSessionSubmitRecords", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSQLSessionSubmitRecordsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSQLSessionSubmitRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4936,23 +4980,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeScheduleExecutionInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeScheduleExecutionInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeScheduleExecutionInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4965,23 +5003,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeScheduleTaskInstances", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeScheduleTaskInstancesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeScheduleTaskInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -4994,81 +5026,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeScheduleTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeScheduleTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeScheduleTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeScripts(self, request):
-        """该接口（DescribeScripts）用于获取所有SQL查询。
+        """该接口（DescribeScripts）用于查询SQL脚本列表
 
         :param request: Request instance for DescribeScripts.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeScriptsRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeScriptsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeScripts", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeScriptsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeScriptsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSparkAppJob(self, request):
-        """查询具体的spark应用
+        """查询spark作业信息
 
         :param request: Request instance for DescribeSparkAppJob.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSparkAppJob", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSparkAppJobResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSparkAppJobResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5081,23 +5095,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSparkAppJobImages", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSparkAppJobImagesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSparkAppJobImagesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5110,81 +5118,109 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSparkAppJobUserInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSparkAppJobUserInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSparkAppJobUserInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSparkAppJobs(self, request):
-        """获取spark应用列表
+        """查询spark作业列表
 
         :param request: Request instance for DescribeSparkAppJobs.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobsRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSparkAppJobs", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSparkAppJobsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSparkAppJobsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSparkAppTasks(self, request):
-        """查询spark应用的运行任务实例列表
+        """查询Spark作业的运行任务列表
 
         :param request: Request instance for DescribeSparkAppTasks.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppTasksRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppTasksResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSparkAppTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSparkAppTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSparkAppTasksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeSparkSessionBatchSqlLog(self, request):
+        """本接口（DescribeSparkSessionBatchSqlLog）用于查询Spark SQL批任务日志
+
+        :param request: Request instance for DescribeSparkSessionBatchSqlLog.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkSessionBatchSqlLogRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkSessionBatchSqlLogResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeSparkSessionBatchSqlLog", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeSparkSessionBatchSqlLogResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeSparkSessionBatchSqlTasks(self, request):
+        """本接口（DescribeSparkSessionBatchSqlTasks）用于获取SparkSQL批任务运行列表。
+
+        :param request: Request instance for DescribeSparkSessionBatchSqlTasks.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkSessionBatchSqlTasksRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkSessionBatchSqlTasksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeSparkSessionBatchSqlTasks", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeSparkSessionBatchSqlTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5197,23 +5233,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSparkTaskLogDownloadInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSparkTaskLogDownloadInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSparkTaskLogDownloadInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5226,23 +5256,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSparkUiUrl", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSparkUiUrlResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSparkUiUrlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeStandbyDataEngine(self, request):
+        """查询备用集群
+
+        :param request: Request instance for DescribeStandbyDataEngine.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeStandbyDataEngineRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeStandbyDataEngineResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeStandbyDataEngine", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeStandbyDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5255,23 +5302,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeStoreLocation", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeStoreLocationResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeStoreLocationResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5284,23 +5325,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSubUsers", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSubUsersResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSubUsersResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5313,23 +5348,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSubuins", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSubuinsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSubuinsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5342,23 +5371,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeSystemStorage", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeSystemStorageResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeSystemStorageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5371,23 +5394,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeTableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5400,23 +5417,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTables", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeTablesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeTablesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5429,23 +5440,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTablesExtend", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeTablesExtendResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeTablesExtendResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeTaskMetrics(self, request):
+        """此接口（DescribeTaskMetrics）用于查询任务统计指标
+
+        :param request: Request instance for DescribeTaskMetrics.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeTaskMetricsRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeTaskMetricsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeTaskMetrics", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeTaskMetricsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5458,23 +5486,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTaskResult", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeTaskResultResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeTaskResultResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5487,23 +5509,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5516,23 +5532,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeTasksOverview", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeTasksOverviewResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeTasksOverviewResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeUpdatableDataEngines(self, request):
+        """查询可更新配置的引擎列表
+
+        :param request: Request instance for DescribeUpdatableDataEngines.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeUpdatableDataEnginesRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeUpdatableDataEnginesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeUpdatableDataEngines", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeUpdatableDataEnginesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeUserDataEngineConfig(self, request):
+        """查询用户自定义引擎参数
+
+        :param request: Request instance for DescribeUserDataEngineConfig.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeUserDataEngineConfigRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeUserDataEngineConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeUserDataEngineConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeUserDataEngineConfigResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5545,23 +5601,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeUserInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeUserInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeUserInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5574,23 +5624,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeUserRoles", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeUserRolesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeUserRolesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5603,23 +5647,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeUserType", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeUserTypeResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeUserTypeResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5632,23 +5670,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeUserUseScene", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeUserUseSceneResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeUserUseSceneResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5661,23 +5693,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeUsers", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeUsersResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeUsersResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5690,23 +5716,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeView", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeViewResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeViewResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5719,23 +5739,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeViews", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeViewsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeViewsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5748,23 +5762,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeWhitelist", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeWhitelistResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeWhitelistResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5777,23 +5785,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeWorkGroupInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeWorkGroupInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeWorkGroupInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5806,23 +5808,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeWorkGroups", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeWorkGroupsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeWorkGroupsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5835,23 +5831,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeWorkloadStat", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DescribeWorkloadStatResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DescribeWorkloadStatResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeYuntiUser(self, request):
+        """判断用户是否是云梯接口
+
+        :param request: Request instance for DescribeYuntiUser.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeYuntiUserRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeYuntiUserResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeYuntiUser", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeYuntiUserResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5864,23 +5877,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DetachUserPolicy", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DetachUserPolicyResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DetachUserPolicyResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5893,23 +5900,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DetachWorkGroupPolicy", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DetachWorkGroupPolicyResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DetachWorkGroupPolicyResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5922,23 +5923,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DisassociateCHDFSAccessGroups", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DisassociateCHDFSAccessGroupsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DisassociateCHDFSAccessGroupsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5951,23 +5946,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DownloadResult", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DownloadResultResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DownloadResultResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -5980,23 +5969,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DownloadSparkTaskLog", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DownloadSparkTaskLogResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DownloadSparkTaskLogResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6009,23 +5992,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DropDMSDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DropDMSDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DropDMSDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6038,23 +6015,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DropDMSPartitionColumnStatistic", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DropDMSPartitionColumnStatisticResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DropDMSPartitionColumnStatisticResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6067,23 +6038,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DropDMSPartitions", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DropDMSPartitionsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DropDMSPartitionsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6096,23 +6061,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DropDMSTable", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DropDMSTableResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DropDMSTableResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6125,23 +6084,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DropDMSTableColumnStatistic", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.DropDMSTableColumnStatisticResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.DropDMSTableColumnStatisticResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6154,23 +6107,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ExportResult", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ExportResultResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ExportResultResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6183,23 +6130,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ForceSuccessScheduleTaskInstances", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ForceSuccessScheduleTaskInstancesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ForceSuccessScheduleTaskInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6212,23 +6153,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("FreezeScheduleTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.FreezeScheduleTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.FreezeScheduleTasksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def GenerateCreateMangedTableSql(self, request):
+        """生成创建托管表语句
+
+        :param request: Request instance for GenerateCreateMangedTableSql.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.GenerateCreateMangedTableSqlRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.GenerateCreateMangedTableSqlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GenerateCreateMangedTableSql", params, headers=headers)
+            response = json.loads(body)
+            model = models.GenerateCreateMangedTableSqlResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6241,23 +6199,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("GetWorkflowCanvas", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.GetWorkflowCanvasResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.GetWorkflowCanvasResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6270,23 +6222,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("GetWorkflowInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.GetWorkflowInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.GetWorkflowInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6299,23 +6245,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("InferInternalTableSchema", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.InferInternalTableSchemaResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.InferInternalTableSchemaResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6328,23 +6268,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("InferSchema", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.InferSchemaResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.InferSchemaResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6357,23 +6291,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("InquireCreateDataEnginePrice", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.InquireCreateDataEnginePriceResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.InquireCreateDataEnginePriceResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6386,23 +6314,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("InquirePriceCreateDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.InquirePriceCreateDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.InquirePriceCreateDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6415,23 +6337,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("InquirePriceModifyDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.InquirePriceModifyDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.InquirePriceModifyDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6444,23 +6360,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("InquirePriceTerminateDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.InquirePriceTerminateDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.InquirePriceTerminateDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6473,23 +6383,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("KillScheduleTaskInstances", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.KillScheduleTaskInstancesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.KillScheduleTaskInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6502,23 +6406,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ListDataEngines", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ListDataEnginesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ListDataEnginesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6531,52 +6429,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ListHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ListHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ListHouseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ListTaskJobLogDetail(self, request):
-        """本接口（ListTaskJobLogDetail）用于获取spark-jar日志列表
+        """本接口（ListTaskJobLogDetail）用于获取spark 作业任务日志详情
 
         :param request: Request instance for ListTaskJobLogDetail.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ListTaskJobLogDetailRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.ListTaskJobLogDetailResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ListTaskJobLogDetail", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ListTaskJobLogDetailResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ListTaskJobLogDetailResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6589,23 +6475,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ListTaskJobLogName", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ListTaskJobLogNameResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ListTaskJobLogNameResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6618,23 +6498,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ListWorkflow", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ListWorkflowResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ListWorkflowResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6647,23 +6521,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("LockMetaData", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.LockMetaDataResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.LockMetaDataResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6676,23 +6544,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("MigrateDatasourceConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.MigrateDatasourceConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.MigrateDatasourceConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6705,23 +6567,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyAdvancedStoreLocation", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyAdvancedStoreLocationResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyAdvancedStoreLocationResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6734,23 +6590,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyCHDFSMountPointAssociateInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyCHDFSMountPointAssociateInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyCHDFSMountPointAssociateInfoResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyCHDFSMountPointSuperuser(self, request):
+        """此接口（ModifyCHDFSMountPointSuperuser）用于修改Superuser
+
+        :param request: Request instance for ModifyCHDFSMountPointSuperuser.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.ModifyCHDFSMountPointSuperuserRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifyCHDFSMountPointSuperuserResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyCHDFSMountPointSuperuser", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyCHDFSMountPointSuperuserResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyCHDFSProduct(self, request):
+        """此接口（ModifyCHDFSProduct）修改元数据加速桶绑定产品
+
+        :param request: Request instance for ModifyCHDFSProduct.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.ModifyCHDFSProductRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifyCHDFSProductResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyCHDFSProduct", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyCHDFSProductResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6763,23 +6659,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyDataEngineDescription", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyDataEngineDescriptionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyDataEngineDescriptionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6792,23 +6682,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyDatabaseUDF", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyDatabaseUDFResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyDatabaseUDFResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6821,23 +6705,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyDatasourceConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyDatasourceConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyDatasourceConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyGovernEventRule(self, request):
+        """修改数据治理事件阈值
+
+        :param request: Request instance for ModifyGovernEventRule.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.ModifyGovernEventRuleRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifyGovernEventRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyGovernEventRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyGovernEventRuleResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6850,23 +6751,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyMetaDatabase", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyMetaDatabaseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyMetaDatabaseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6879,23 +6774,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifySQLSessionCatalog", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifySQLSessionCatalogResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifySQLSessionCatalogResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6908,23 +6797,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifySQLSessionSnapshot", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifySQLSessionSnapshotResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifySQLSessionSnapshotResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6937,23 +6820,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyScheduleTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyScheduleTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyScheduleTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -6966,52 +6843,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyScheduleTaskExecuteInfo", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyScheduleTaskExecuteInfoResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyScheduleTaskExecuteInfoResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifySparkApp(self, request):
-        """更新spark应用
+        """更新spark作业
 
         :param request: Request instance for ModifySparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifySparkApp", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifySparkAppResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifySparkAppResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifySparkAppBatch(self, request):
+        """本接口（ModifySparkAppBatch）用于批量修改Spark作业参数配置
+
+        :param request: Request instance for ModifySparkAppBatch.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppBatchRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppBatchResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifySparkAppBatch", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifySparkAppBatchResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7024,23 +6912,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifySparkImage", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifySparkImageResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifySparkImageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7053,23 +6935,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyUser", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyUserResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyUserResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7082,23 +6958,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyUserAlias", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyUserAliasResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyUserAliasResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7111,23 +6981,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyUserType", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyUserTypeResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyUserTypeResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7140,23 +7004,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyUserUseScene", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyUserUseSceneResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyUserUseSceneResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7169,23 +7027,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyWorkGroup", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ModifyWorkGroupResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ModifyWorkGroupResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def QueryInternalTableWarehouse(self, request):
+        """本接口（QueryInternalTableWarehouse）用于获取原生表warehouse路径
+
+        :param request: Request instance for QueryInternalTableWarehouse.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.QueryInternalTableWarehouseRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.QueryInternalTableWarehouseResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("QueryInternalTableWarehouse", params, headers=headers)
+            response = json.loads(body)
+            model = models.QueryInternalTableWarehouseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7198,23 +7073,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("QueryResult", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.QueryResultResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.QueryResultResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7227,23 +7096,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("QuerySparkImageUserRecords", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.QuerySparkImageUserRecordsResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.QuerySparkImageUserRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7256,23 +7119,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("QuerySparkImages", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.QuerySparkImagesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.QuerySparkImagesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7285,23 +7142,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("QuerySystemStorage", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.QuerySystemStorageResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.QuerySystemStorageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7314,23 +7165,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("QueryTaskResult", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.QueryTaskResultResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.QueryTaskResultResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7343,23 +7188,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("RemoveTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.RemoveTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.RemoveTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7372,23 +7211,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("RenewDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.RenewDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.RenewDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7401,23 +7234,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("RenewHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.RenewHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.RenewHouseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7430,23 +7257,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ReportHeartbeatMetaData", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ReportHeartbeatMetaDataResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ReportHeartbeatMetaDataResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7459,23 +7280,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("RerunScheduleTaskInstances", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.RerunScheduleTaskInstancesResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.RerunScheduleTaskInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def RestartDataEngine(self, request):
+        """重启引擎
+
+        :param request: Request instance for RestartDataEngine.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.RestartDataEngineRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.RestartDataEngineResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RestartDataEngine", params, headers=headers)
+            response = json.loads(body)
+            model = models.RestartDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def RollbackDataEngineImage(self, request):
+        """回滚引擎镜像版本
+
+        :param request: Request instance for RollbackDataEngineImage.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.RollbackDataEngineImageRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.RollbackDataEngineImageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RollbackDataEngineImage", params, headers=headers)
+            response = json.loads(body)
+            model = models.RollbackDataEngineImageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7488,23 +7349,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("RunScheduleTask", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.RunScheduleTaskResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.RunScheduleTaskResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7517,23 +7372,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("SavePosition", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.SavePositionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.SavePositionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SetTableProperties(self, request):
+        """本接口（SetTableProperties）用于增加或修改表属性批量删除表
+
+        :param request: Request instance for SetTableProperties.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.SetTablePropertiesRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.SetTablePropertiesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SetTableProperties", params, headers=headers)
+            response = json.loads(body)
+            model = models.SetTablePropertiesResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7546,23 +7418,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("StopScheduleTasks", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.StopScheduleTasksResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.StopScheduleTasksResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7575,52 +7441,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("SupplementData", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.SupplementDataResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.SupplementDataResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SuspendResumeDataEngine(self, request):
-        """本接口用于控制暂停或恢复数据引擎
+        """本接口用于控制挂起或启动数据引擎
 
         :param request: Request instance for SuspendResumeDataEngine.
         :type request: :class:`tencentcloud.dlc.v20210125.models.SuspendResumeDataEngineRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.SuspendResumeDataEngineResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("SuspendResumeDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.SuspendResumeDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.SuspendResumeDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7633,23 +7487,63 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("SuspendResumeHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.SuspendResumeHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.SuspendResumeHouseResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SwitchDataEngine(self, request):
+        """切换主备集群
+
+        :param request: Request instance for SwitchDataEngine.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.SwitchDataEngineRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.SwitchDataEngineResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SwitchDataEngine", params, headers=headers)
+            response = json.loads(body)
+            model = models.SwitchDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SwitchDataEngineImage(self, request):
+        """切换引擎镜像版本
+
+        :param request: Request instance for SwitchDataEngineImage.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.SwitchDataEngineImageRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.SwitchDataEngineImageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SwitchDataEngineImage", params, headers=headers)
+            response = json.loads(body)
+            model = models.SwitchDataEngineImageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7662,23 +7556,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UnbindWorkGroupsFromUser", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UnbindWorkGroupsFromUserResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UnbindWorkGroupsFromUserResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7691,23 +7579,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UnboundDatasourceHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UnboundDatasourceHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UnboundDatasourceHouseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7720,23 +7602,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UnlockMetaData", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UnlockMetaDataResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UnlockMetaDataResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7749,23 +7625,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UpdateDataEngine", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UpdateDataEngineResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UpdateDataEngineResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateDataEngineConfig(self, request):
+        """用户某种操作，触发引擎配置修改
+
+        :param request: Request instance for UpdateDataEngineConfig.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.UpdateDataEngineConfigRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.UpdateDataEngineConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateDataEngineConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateDataEngineConfigResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7778,23 +7671,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UpdateDataQuery", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UpdateDataQueryResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UpdateDataQueryResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7807,23 +7694,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UpdateDatasourceConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UpdateDatasourceConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UpdateDatasourceConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7836,23 +7717,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UpdateHouse", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UpdateHouseResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UpdateHouseResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7865,23 +7740,86 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UpdateNetworkConnection", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UpdateNetworkConnectionResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UpdateNetworkConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateRowFilter(self, request):
+        """此接口用于更新行过滤规则。注意只能更新过滤规则，不能更新规格对象catalog，database和table。
+
+        :param request: Request instance for UpdateRowFilter.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.UpdateRowFilterRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.UpdateRowFilterResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateRowFilter", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateRowFilterResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateTaskStatus(self, request):
+        """更新任务
+
+        :param request: Request instance for UpdateTaskStatus.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.UpdateTaskStatusRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.UpdateTaskStatusResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateTaskStatus", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateTaskStatusResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateUserDataEngineConfig(self, request):
+        """修改用户引擎自定义配置
+
+        :param request: Request instance for UpdateUserDataEngineConfig.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.UpdateUserDataEngineConfigRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.UpdateUserDataEngineConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateUserDataEngineConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateUserDataEngineConfigResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7894,23 +7832,17 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UpdateUserRole", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UpdateUserRoleResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UpdateUserRoleResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7923,23 +7855,40 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("UpdateWorkflow", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.UpdateWorkflowResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.UpdateWorkflowResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpgradeDataEngineImage(self, request):
+        """升级引擎镜像
+
+        :param request: Request instance for UpgradeDataEngineImage.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.UpgradeDataEngineImageRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.UpgradeDataEngineImageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpgradeDataEngineImage", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpgradeDataEngineImageResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
@@ -7952,21 +7901,15 @@
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ValidateWorkflowName", params, headers=headers)
             response = json.loads(body)
-            if "Error" not in response["Response"]:
-                model = models.ValidateWorkflowNameResponse()
-                model._deserialize(response["Response"])
-                return model
-            else:
-                code = response["Response"]["Error"]["Code"]
-                message = response["Response"]["Error"]["Message"]
-                reqid = response["Response"]["RequestId"]
-                raise TencentCloudSDKException(code, message, reqid)
+            model = models.ValidateWorkflowNameResponse()
+            model._deserialize(response["Response"])
+            return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -103,14 +103,17 @@
 
 # 参数校验失败。
 FAILEDOPERATION_PARAMETERVALIDATIONFAILED = 'FailedOperation.ParameterValidationFailed'
 
 # 退押金失败。
 FAILEDOPERATION_REFUNDDEPOSITFAILED = 'FailedOperation.RefundDepositFailed'
 
+# 重复绑定chdfs。
+FAILEDOPERATION_REPEATBINDCHDFS = 'FailedOperation.RepeatBindChdfs'
+
 # 取消授权失败。
 FAILEDOPERATION_REVOKEPOLICYFAILED = 'FailedOperation.RevokePolicyFailed'
 
 # 资源已经绑定了同名标签键。
 FAILEDOPERATION_TAGALREADYATTACHED = 'FailedOperation.TagAlreadyAttached'
 
 # 标签键长度超过限制。
@@ -181,29 +184,38 @@
 
 # 无效的默认数据引擎参数。
 INVALIDPARAMETER_INVALIDDEFAULTDATAENGINE = 'InvalidParameter.InvalidDefaultDataEngine'
 
 # 无效的描述信息。
 INVALIDPARAMETER_INVALIDDESCRIPTION = 'InvalidParameter.InvalidDescription'
 
+# 无效的引擎执行类别。
+INVALIDPARAMETER_INVALIDENGINEEXECTYPE = 'InvalidParameter.InvalidEngineExecType'
+
 # 无效的引擎类型。
 INVALIDPARAMETER_INVALIDENGINETYPE = 'InvalidParameter.InvalidEngineType'
 
 # 无效的容错策略。
 INVALIDPARAMETER_INVALIDFAILURETOLERANCE = 'InvalidParameter.InvalidFailureTolerance'
 
 # 无效的过滤条件。
 INVALIDPARAMETER_INVALIDFILTERKEY = 'InvalidParameter.InvalidFilterKey'
 
 # 无效的工作组Id。
 INVALIDPARAMETER_INVALIDGROUPID = 'InvalidParameter.InvalidGroupId'
 
+# 不支持的Hive版本。
+INVALIDPARAMETER_INVALIDHIVEVERSION = 'InvalidParameter.InvalidHiveVersion'
+
 # 请求的消息类型无效。
 INVALIDPARAMETER_INVALIDINFOTYPE = 'InvalidParameter.InvalidInfoType'
 
+# 无效的最大结果数。
+INVALIDPARAMETER_INVALIDMAXRESULTS = 'InvalidParameter.InvalidMaxResults'
+
 # 无效的最小集群数量。
 INVALIDPARAMETER_INVALIDMINCLUSTERS = 'InvalidParameter.InvalidMinClusters'
 
 # 无效的Offset值。
 INVALIDPARAMETER_INVALIDOFFSET = 'InvalidParameter.InvalidOffset'
 
 # 无效的计费模式。
@@ -277,26 +289,32 @@
 
 # 请求的次数超过了频率限制。
 REQUESTLIMITEXCEEDED = 'RequestLimitExceeded'
 
 # 资源被占用。
 RESOURCEINUSE = 'ResourceInUse'
 
+# 有SQL任务尚未执行完成。
+RESOURCEINUSE_UNFINISHEDSQLS = 'ResourceInUse.UnfinishedSQLs'
+
 # 资源不足。
 RESOURCEINSUFFICIENT = 'ResourceInsufficient'
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
 # 指定数据源连接没有找到。
 RESOURCENOTFOUND_DATASOURCENOTFOUND = 'ResourceNotFound.DatasourceNotFound'
 
 # Eks计算集群初始化或迁移中，请稍后再试。
 RESOURCENOTFOUND_EKSRESOURCENOTFOUND = 'ResourceNotFound.EksResourceNotFound'
 
+# 当前无资源创建session，请稍后重试或使用包年包月集群。
+RESOURCENOTFOUND_RESOURCENOTFOUNDCODE_SESSIONINSUFFICIENTRESOURCES = 'ResourceNotFound.ResourceNotFoundCode_SessionInsufficientResources'
+
 # 未找到结果路径。
 RESOURCENOTFOUND_RESULTOUTPUTPATHNOTFOUND = 'ResourceNotFound.ResultOutputPathNotFound'
 
 # session不存在。
 RESOURCENOTFOUND_SESSIONNOTFOUND = 'ResourceNotFound.SessionNotFound'
 
 # session已消亡。
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/tencentcloud/dlc/v20210125/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,63 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AccessGroup(AbstractModel):
+    """权限组
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AccessGroupId: 权限组ID
+        :type AccessGroupId: str
+        :param AccessGroupName: 权限组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AccessGroupName: str
+        :param Description: 权限组描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param VpcId: VPC网络ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param VpcType: VPC网络类型（1：CVM；2：黑石1.0）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcType: int
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        """
+        self.AccessGroupId = None
+        self.AccessGroupName = None
+        self.Description = None
+        self.VpcId = None
+        self.VpcType = None
+        self.CreateTime = None
+
+
+    def _deserialize(self, params):
+        self.AccessGroupId = params.get("AccessGroupId")
+        self.AccessGroupName = params.get("AccessGroupName")
+        self.Description = params.get("Description")
+        self.VpcId = params.get("VpcId")
+        self.VpcType = params.get("VpcType")
+        self.CreateTime = params.get("CreateTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AddColumnAfterRequest(AbstractModel):
     """AddColumnAfter请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -234,14 +283,68 @@
             for item in params.get("Partitions"):
                 obj = DMSPartition()
                 obj._deserialize(item)
                 self.Partitions.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class AddLakeFsChdfsBindingRequest(AbstractModel):
+    """AddLakeFsChdfsBinding请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MountPoint: 挂载点ID
+        :type MountPoint: str
+        :param AccessGroups: 权限组列表
+        :type AccessGroups: list of AccessGroup
+        :param SupperUsers: 超级用户列表
+        :type SupperUsers: list of str
+        """
+        self.MountPoint = None
+        self.AccessGroups = None
+        self.SupperUsers = None
+
+
+    def _deserialize(self, params):
+        self.MountPoint = params.get("MountPoint")
+        if params.get("AccessGroups") is not None:
+            self.AccessGroups = []
+            for item in params.get("AccessGroups"):
+                obj = AccessGroup()
+                obj._deserialize(item)
+                self.AccessGroups.append(obj)
+        self.SupperUsers = params.get("SupperUsers")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AddLakeFsChdfsBindingResponse(AbstractModel):
+    """AddLakeFsChdfsBinding返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class AddPartitionFieldRequest(AbstractModel):
     """AddPartitionField请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -314,26 +417,34 @@
         :type ImageVersion: str
         :param ImageTag: 镜像tag
         :type ImageTag: str
         :param IsPublic: 是否为公共镜像：0：非公共；1：公共
         :type IsPublic: int
         :param Description: 镜像描述
         :type Description: str
+        :param ImageVersionId: 镜像唯一id
+        :type ImageVersionId: str
+        :param Operator: 操作者
+        :type Operator: str
         """
         self.ImageVersion = None
         self.ImageTag = None
         self.IsPublic = None
         self.Description = None
+        self.ImageVersionId = None
+        self.Operator = None
 
 
     def _deserialize(self, params):
         self.ImageVersion = params.get("ImageVersion")
         self.ImageTag = params.get("ImageTag")
         self.IsPublic = params.get("IsPublic")
         self.Description = params.get("Description")
+        self.ImageVersionId = params.get("ImageVersionId")
+        self.Operator = params.get("Operator")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -369,24 +480,28 @@
         r"""
         :param ImageId: 镜像编码
         :type ImageId: str
         :param UserAppId: 用户APPID
         :type UserAppId: int
         :param UserUin: 用户UIN
         :type UserUin: str
+        :param ImageType: ImageType：1（父版本）、2（子版本）、3（pyspark镜像）；
+        :type ImageType: int
         """
         self.ImageId = None
         self.UserAppId = None
         self.UserUin = None
+        self.ImageType = None
 
 
     def _deserialize(self, params):
         self.ImageId = params.get("ImageId")
         self.UserAppId = params.get("UserAppId")
         self.UserUin = params.get("UserUin")
+        self.ImageType = params.get("ImageType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -395,21 +510,25 @@
 class AddSparkImageUserRecordsResponse(AbstractModel):
     """AddSparkImageUserRecords返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param RecordId: 记录id
+        :type RecordId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self.RecordId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
+        self.RecordId = params.get("RecordId")
         self.RequestId = params.get("RequestId")
 
 
 class AddTasksRequest(AbstractModel):
     """AddTasks请求参数结构体
 
     """
@@ -1841,30 +1960,171 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CHDFSAccessInfo(AbstractModel):
+    """元数据加速桶访问权限配置列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BucketId: 桶名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BucketId: str
+        :param BucketType: 桶类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BucketType: str
+        :param BindProNum: 已绑定的产品数量（该字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BindProNum: int
+        :param ProNum: 产品总数（该字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProNum: int
+        :param BindProNameList: 已绑定产品名称列表（该字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BindProNameList: list of str
+        :param BindEngineNum: 已绑定的引擎数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BindEngineNum: int
+        :param EngineNum: 引擎数量
+
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EngineNum: int
+        """
+        self.BucketId = None
+        self.BucketType = None
+        self.BindProNum = None
+        self.ProNum = None
+        self.BindProNameList = None
+        self.BindEngineNum = None
+        self.EngineNum = None
+
+
+    def _deserialize(self, params):
+        self.BucketId = params.get("BucketId")
+        self.BucketType = params.get("BucketType")
+        self.BindProNum = params.get("BindProNum")
+        self.ProNum = params.get("ProNum")
+        self.BindProNameList = params.get("BindProNameList")
+        self.BindEngineNum = params.get("BindEngineNum")
+        self.EngineNum = params.get("EngineNum")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CHDFSProductInfo(AbstractModel):
+    """chdfs产品信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductName: 产品名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProductName: str
+        :param SuperUser: 用户名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SuperUser: list of str
+        :param VpcInfo: vpc配置信息
+
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcInfo: list of CHDFSProductVpcInfo
+        :param CanBeDeleted: 能够被删除
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CanBeDeleted: bool
+        """
+        self.ProductName = None
+        self.SuperUser = None
+        self.VpcInfo = None
+        self.CanBeDeleted = None
+
+
+    def _deserialize(self, params):
+        self.ProductName = params.get("ProductName")
+        self.SuperUser = params.get("SuperUser")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = CHDFSProductVpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        self.CanBeDeleted = params.get("CanBeDeleted")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CHDFSProductVpcInfo(AbstractModel):
+    """chdfs产品vpc信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcId: vpc id
+
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param VpcName: vpc名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcName: str
+        :param VpcCidrBlock: vpc子网信息列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcCidrBlock: list of VpcCidrBlock
+        """
+        self.VpcId = None
+        self.VpcName = None
+        self.VpcCidrBlock = None
+
+
+    def _deserialize(self, params):
+        self.VpcId = params.get("VpcId")
+        self.VpcName = params.get("VpcName")
+        if params.get("VpcCidrBlock") is not None:
+            self.VpcCidrBlock = []
+            for item in params.get("VpcCidrBlock"):
+                obj = VpcCidrBlock()
+                obj._deserialize(item)
+                self.VpcCidrBlock.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CSV(AbstractModel):
     """CSV类型数据格式
 
     """
 
     def __init__(self):
         r"""
         :param CodeCompress: 压缩格式，["Snappy", "Gzip", "None"选一]。
         :type CodeCompress: str
         :param CSVSerde: CSV序列化及反序列化数据结构。
         :type CSVSerde: :class:`tencentcloud.dlc.v20210125.models.CSVSerde`
         :param HeadLines: 标题行，默认为0。
-注意：此字段可能返回 null，表示取不到有效值。
         :type HeadLines: int
         :param Format: 格式，默认值为CSV
-注意：此字段可能返回 null，表示取不到有效值。
         :type Format: str
         """
         self.CodeCompress = None
         self.CSVSerde = None
         self.HeadLines = None
         self.Format = None
 
@@ -1889,26 +2149,22 @@
     """CSV类型文件
 
     """
 
     def __init__(self):
         r"""
         :param Format: 文本类型，本参数取值为CSV
-注意：此字段可能返回 null，表示取不到有效值。
         :type Format: str
         :param CodeCompress: 压缩格式，["Snappy", "Gzip", "None"选一]。
         :type CodeCompress: str
         :param HeaderLine: 标题行，默认为False。
-注意：此字段可能返回 null，表示取不到有效值。
         :type HeaderLine: bool
         :param NewLineSymbol: 数据行分隔符。
-注意：此字段可能返回 null，表示取不到有效值。
         :type NewLineSymbol: str
         :param CSVSerde: CSV序列化及反序列化数据结构。
-注意：此字段可能返回 null，表示取不到有效值。
         :type CSVSerde: :class:`tencentcloud.dlc.v20210125.models.CSVSerde`
         """
         self.Format = None
         self.CodeCompress = None
         self.HeaderLine = None
         self.NewLineSymbol = None
         self.CSVSerde = None
@@ -1959,14 +2215,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CancelNotebookSessionStatementBatchRequest(AbstractModel):
+    """CancelNotebookSessionStatementBatch请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SessionId: Session唯一标识
+        :type SessionId: str
+        :param BatchId: 批任务唯一标识
+        :type BatchId: str
+        """
+        self.SessionId = None
+        self.BatchId = None
+
+
+    def _deserialize(self, params):
+        self.SessionId = params.get("SessionId")
+        self.BatchId = params.get("BatchId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelNotebookSessionStatementBatchResponse(AbstractModel):
+    """CancelNotebookSessionStatementBatch返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CancelNotebookSessionStatementRequest(AbstractModel):
     """CancelNotebookSessionStatement请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2004,14 +2305,116 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CancelSparkSessionBatchSQLRequest(AbstractModel):
+    """CancelSparkSessionBatchSQL请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务唯一标识
+        :type BatchId: str
+        """
+        self.BatchId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelSparkSessionBatchSQLResponse(AbstractModel):
+    """CancelSparkSessionBatchSQL返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class CancelTablePropertiesRequest(AbstractModel):
+    """CancelTableProperties请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DatasourceConnectionName: Catalog名称
+        :type DatasourceConnectionName: str
+        :param DatabaseName: 库名
+        :type DatabaseName: str
+        :param TableName: 表名
+        :type TableName: str
+        :param Properties: 属性列表
+        :type Properties: list of str
+        """
+        self.DatasourceConnectionName = None
+        self.DatabaseName = None
+        self.TableName = None
+        self.Properties = None
+
+
+    def _deserialize(self, params):
+        self.DatasourceConnectionName = params.get("DatasourceConnectionName")
+        self.DatabaseName = params.get("DatabaseName")
+        self.TableName = params.get("TableName")
+        self.Properties = params.get("Properties")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelTablePropertiesResponse(AbstractModel):
+    """CancelTableProperties返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务Id
+        :type BatchId: str
+        :param TaskIdSet: TaskId列表
+        :type TaskIdSet: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BatchId = None
+        self.TaskIdSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        self.TaskIdSet = params.get("TaskIdSet")
+        self.RequestId = params.get("RequestId")
+
+
 class CancelTaskRequest(AbstractModel):
     """CancelTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2054,14 +2457,64 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CancelTasksRequest(AbstractModel):
+    """CancelTasks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务Id数组，全局唯一
+        :type TaskId: list of str
+        :param Config: 配置信息，key-value数组，对外不可见。key1：AuthorityRole（鉴权角色，默认传SubUin，base64加密，仅在jdbc提交任务时使用）
+        :type Config: list of KVPair
+        """
+        self.TaskId = None
+        self.Config = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        if params.get("Config") is not None:
+            self.Config = []
+            for item in params.get("Config"):
+                obj = KVPair()
+                obj._deserialize(item)
+                self.Config.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelTasksResponse(AbstractModel):
+    """CancelTasks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CanvasInfo(AbstractModel):
     """画布数据
 
     """
 
     def __init__(self):
         r"""
@@ -2224,14 +2677,179 @@
 
 
     def _deserialize(self, params):
         self.Granted = params.get("Granted")
         self.RequestId = params.get("RequestId")
 
 
+class CheckDataEngineConfigPairsValidityRequest(AbstractModel):
+    """CheckDataEngineConfigPairsValidity请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ChildImageVersionId: 引擎小版本ID
+        :type ChildImageVersionId: str
+        :param DataEngineConfigPairs: 用户自定义参数
+        :type DataEngineConfigPairs: list of DataEngineConfigPair
+        :param ImageVersionId: 引擎大版本ID，存在小版本ID时仅需传入小版本ID，不存在时会获取当前大版本下最新的小版本ID。
+        :type ImageVersionId: str
+        """
+        self.ChildImageVersionId = None
+        self.DataEngineConfigPairs = None
+        self.ImageVersionId = None
+
+
+    def _deserialize(self, params):
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        if params.get("DataEngineConfigPairs") is not None:
+            self.DataEngineConfigPairs = []
+            for item in params.get("DataEngineConfigPairs"):
+                obj = DataEngineConfigPair()
+                obj._deserialize(item)
+                self.DataEngineConfigPairs.append(obj)
+        self.ImageVersionId = params.get("ImageVersionId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CheckDataEngineConfigPairsValidityResponse(AbstractModel):
+    """CheckDataEngineConfigPairsValidity返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param IsAvailable: 参数有效性：ture:有效，false:至少存在一个无效参数；
+        :type IsAvailable: bool
+        :param UnavailableConfig: 无效参数集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UnavailableConfig: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.IsAvailable = None
+        self.UnavailableConfig = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.IsAvailable = params.get("IsAvailable")
+        self.UnavailableConfig = params.get("UnavailableConfig")
+        self.RequestId = params.get("RequestId")
+
+
+class CheckDataEngineImageCanBeRollbackRequest(AbstractModel):
+    """CheckDataEngineImageCanBeRollback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎唯一id
+        :type DataEngineId: str
+        """
+        self.DataEngineId = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CheckDataEngineImageCanBeRollbackResponse(AbstractModel):
+    """CheckDataEngineImageCanBeRollback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ToRecordId: 回滚后日志记录id
+        :type ToRecordId: str
+        :param FromRecordId: 回滚前日志记录id
+        :type FromRecordId: str
+        :param IsRollback: 是否能够回滚
+        :type IsRollback: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ToRecordId = None
+        self.FromRecordId = None
+        self.IsRollback = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.ToRecordId = params.get("ToRecordId")
+        self.FromRecordId = params.get("FromRecordId")
+        self.IsRollback = params.get("IsRollback")
+        self.RequestId = params.get("RequestId")
+
+
+class CheckDataEngineImageCanBeUpgradeRequest(AbstractModel):
+    """CheckDataEngineImageCanBeUpgrade请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 集群id
+        :type DataEngineId: str
+        """
+        self.DataEngineId = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CheckDataEngineImageCanBeUpgradeResponse(AbstractModel):
+    """CheckDataEngineImageCanBeUpgrade返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ChildImageVersionId: 当前大版本下，可升级的集群镜像小版本id
+        :type ChildImageVersionId: str
+        :param IsUpgrade: 是否能够升级
+        :type IsUpgrade: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ChildImageVersionId = None
+        self.IsUpgrade = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        self.IsUpgrade = params.get("IsUpgrade")
+        self.RequestId = params.get("RequestId")
+
+
 class CheckDatabaseExistsRequest(AbstractModel):
     """CheckDatabaseExists请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2549,14 +3167,41 @@
 
     def _deserialize(self, params):
         self.LockId = params.get("LockId")
         self.LockState = params.get("LockState")
         self.RequestId = params.get("RequestId")
 
 
+class CheckRegionCHDFSEnableRequest(AbstractModel):
+    """CheckRegionCHDFSEnable请求参数结构体
+
+    """
+
+
+class CheckRegionCHDFSEnableResponse(AbstractModel):
+    """CheckRegionCHDFSEnable返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CHDFSEnable: 是否支持元数据加速能力
+        :type CHDFSEnable: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.CHDFSEnable = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.CHDFSEnable = params.get("CHDFSEnable")
+        self.RequestId = params.get("RequestId")
+
+
 class CheckSQLSessionCatalogNameExistsRequest(AbstractModel):
     """CheckSQLSessionCatalogNameExists请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2714,20 +3359,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param ImageVersion: 镜像version
         :type ImageVersion: str
+        :param ImageVersionId: imageId
+        :type ImageVersionId: str
         """
         self.ImageVersion = None
+        self.ImageVersionId = None
 
 
     def _deserialize(self, params):
         self.ImageVersion = params.get("ImageVersion")
+        self.ImageVersionId = params.get("ImageVersionId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2761,22 +3410,26 @@
 
     def __init__(self):
         r"""
         :param ImageId: 镜像编码
         :type ImageId: str
         :param UserAppId: 用户APPID
         :type UserAppId: int
+        :param ImageType: 枚举值：1（父版本）、2（子版本）、3（pyspark）
+        :type ImageType: int
         """
         self.ImageId = None
         self.UserAppId = None
+        self.ImageType = None
 
 
     def _deserialize(self, params):
         self.ImageId = params.get("ImageId")
         self.UserAppId = params.get("UserAppId")
+        self.ImageType = params.get("ImageType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2905,14 +3558,59 @@
 
 
     def _deserialize(self, params):
         self.IsExists = params.get("IsExists")
         self.RequestId = params.get("RequestId")
 
 
+class CheckVpcCidrBlockRequest(AbstractModel):
+    """CheckVpcCidrBlock请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcCidrBlock: vpc的cidrblock
+        :type VpcCidrBlock: str
+        """
+        self.VpcCidrBlock = None
+
+
+    def _deserialize(self, params):
+        self.VpcCidrBlock = params.get("VpcCidrBlock")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CheckVpcCidrBlockResponse(AbstractModel):
+    """CheckVpcCidrBlock返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CidrBlockValid: cidrblock是否符合预期，false不符合，true符合
+        :type CidrBlockValid: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.CidrBlockValid = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.CidrBlockValid = params.get("CidrBlockValid")
+        self.RequestId = params.get("RequestId")
+
+
 class CleanImportStorageRequest(AbstractModel):
     """CleanImportStorage请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3073,43 +3771,128 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CommonMetrics(AbstractModel):
+    """任务公共指标
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CreateTaskTime: 创建任务时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTaskTime: float
+        :param ProcessTime: 预处理总时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcessTime: float
+        :param QueueTime: 排队时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QueueTime: float
+        :param ExecutionTime: 执行时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutionTime: float
+        :param IsResultCacheHit: 是否命中结果缓存
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsResultCacheHit: bool
+        :param MatchedMVBytes: 匹配物化视图数据量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MatchedMVBytes: int
+        :param MatchedMVs: 匹配物化视图列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MatchedMVs: str
+        :param AffectedBytes: 结果数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AffectedBytes: str
+        :param AffectedRows: 	结果行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AffectedRows: int
+        :param ProcessedBytes: 扫描数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcessedBytes: int
+        :param ProcessedRows: 	扫描行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcessedRows: int
+        """
+        self.CreateTaskTime = None
+        self.ProcessTime = None
+        self.QueueTime = None
+        self.ExecutionTime = None
+        self.IsResultCacheHit = None
+        self.MatchedMVBytes = None
+        self.MatchedMVs = None
+        self.AffectedBytes = None
+        self.AffectedRows = None
+        self.ProcessedBytes = None
+        self.ProcessedRows = None
+
+
+    def _deserialize(self, params):
+        self.CreateTaskTime = params.get("CreateTaskTime")
+        self.ProcessTime = params.get("ProcessTime")
+        self.QueueTime = params.get("QueueTime")
+        self.ExecutionTime = params.get("ExecutionTime")
+        self.IsResultCacheHit = params.get("IsResultCacheHit")
+        self.MatchedMVBytes = params.get("MatchedMVBytes")
+        self.MatchedMVs = params.get("MatchedMVs")
+        self.AffectedBytes = params.get("AffectedBytes")
+        self.AffectedRows = params.get("AffectedRows")
+        self.ProcessedBytes = params.get("ProcessedBytes")
+        self.ProcessedRows = params.get("ProcessedRows")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ComputerResource(AbstractModel):
     """计算资源配置。
 
     """
 
     def __init__(self):
         r"""
         :param Resource: 计算资源
         :type Resource: str
         :param Engine: 计算引擎
         :type Engine: str
         :param Config: 计算配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type Config: list of Config
+        :param ChildImageVersionId: 集群小版本ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChildImageVersionId: str
+        :param ImageVersionName: 集群大版本名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageVersionName: str
         """
         self.Resource = None
         self.Engine = None
         self.Config = None
+        self.ChildImageVersionId = None
+        self.ImageVersionName = None
 
 
     def _deserialize(self, params):
         self.Resource = params.get("Resource")
         self.Engine = params.get("Engine")
         if params.get("Config") is not None:
             self.Config = []
             for item in params.get("Config"):
                 obj = Config()
                 obj._deserialize(item)
                 self.Config.append(obj)
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        self.ImageVersionName = params.get("ImageVersionName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3194,14 +3977,130 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CreateCHDFSBindingProductRequest(AbstractModel):
+    """CreateCHDFSBindingProduct请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MountPoint: 需要绑定的元数据加速桶名
+        :type MountPoint: str
+        :param BucketType: 桶的类型，分为cos和lakefs
+        :type BucketType: str
+        :param ProductName: 产品名称
+        :type ProductName: str
+        :param EngineName: 引擎名称，ProductName选择DLC产品时，必传此参数。其他产品可不传
+        :type EngineName: str
+        :param VpcInfo: vpc信息，产品名称为other时必传此参数
+        :type VpcInfo: list of VpcInfo
+        """
+        self.MountPoint = None
+        self.BucketType = None
+        self.ProductName = None
+        self.EngineName = None
+        self.VpcInfo = None
+
+
+    def _deserialize(self, params):
+        self.MountPoint = params.get("MountPoint")
+        self.BucketType = params.get("BucketType")
+        self.ProductName = params.get("ProductName")
+        self.EngineName = params.get("EngineName")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = VpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateCHDFSBindingProductResponse(AbstractModel):
+    """CreateCHDFSBindingProduct返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class CreateCHDFSProductRequest(AbstractModel):
+    """CreateCHDFSProduct请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductName: 产品名称
+        :type ProductName: str
+        :param SuperUser: 超级用户名称数组
+        :type SuperUser: list of str
+        :param VpcInfo: vpc配置信息数组
+        :type VpcInfo: list of CHDFSProductVpcInfo
+        """
+        self.ProductName = None
+        self.SuperUser = None
+        self.VpcInfo = None
+
+
+    def _deserialize(self, params):
+        self.ProductName = params.get("ProductName")
+        self.SuperUser = params.get("SuperUser")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = CHDFSProductVpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateCHDFSProductResponse(AbstractModel):
+    """CreateCHDFSProduct返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CreateDMSDatabaseRequest(AbstractModel):
     """CreateDMSDatabase请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3414,22 +4313,38 @@
         :type Tags: list of TagInfo
         :param AutoSuspend: 是否自定挂起集群：false（默认）：不自动挂起、true：自动挂起
         :type AutoSuspend: bool
         :param CrontabResumeSuspend: 定时启停集群策略：0（默认）：关闭定时策略、1：开启定时策略（注：定时启停策略与自动挂起策略互斥）
         :type CrontabResumeSuspend: int
         :param CrontabResumeSuspendStrategy: 定时启停策略，复杂类型：包含启停时间、挂起集群策略
         :type CrontabResumeSuspendStrategy: :class:`tencentcloud.dlc.v20210125.models.CrontabResumeSuspendStrategy`
-        :param EngineExecType: 引擎执行任务类型，默认为SQL
+        :param EngineExecType: 引擎执行任务类型，有效值：SQL/BATCH，默认为SQL
         :type EngineExecType: str
         :param MaxConcurrency: 单个集群最大并发任务数，默认5
         :type MaxConcurrency: int
         :param TolerableQueueTime: 可容忍的排队时间，默认0。当任务排队的时间超过可容忍的时间时可能会触发扩容。如果该参数为0，则表示一旦有任务排队就可能立即触发扩容。
         :type TolerableQueueTime: int
         :param AutoSuspendTime: 集群自动挂起时间，默认10分钟
         :type AutoSuspendTime: int
+        :param ResourceType: 资源类型。Standard_CU：标准型；Memory_CU：内存型
+        :type ResourceType: str
+        :param DataEngineConfigPairs: 集群高级配置
+        :type DataEngineConfigPairs: list of DataEngineConfigPair
+        :param ImageVersionName: 集群镜像版本名字。如SuperSQL-P 1.1;SuperSQL-S 3.2等,不传，默认创建最新镜像版本的集群
+        :type ImageVersionName: str
+        :param MainClusterName: 主集群名称
+        :type MainClusterName: str
+        :param ElasticSwitch: spark jar 包年包月集群是否开启弹性
+        :type ElasticSwitch: bool
+        :param ElasticLimit: spark jar 包年包月集群弹性上限
+        :type ElasticLimit: int
+        :param EmrLivyInfo: spark on emr-livy类型集群所需参数，包含emr集群和livy服务的信息
+        :type EmrLivyInfo: str
+        :param SessionResourceTemplate: spark作业集群session资源配置模板
+        :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
         """
         self.EngineType = None
         self.DataEngineName = None
         self.ClusterType = None
         self.Mode = None
         self.AutoResume = None
         self.MinClusters = None
@@ -3446,14 +4361,22 @@
         self.AutoSuspend = None
         self.CrontabResumeSuspend = None
         self.CrontabResumeSuspendStrategy = None
         self.EngineExecType = None
         self.MaxConcurrency = None
         self.TolerableQueueTime = None
         self.AutoSuspendTime = None
+        self.ResourceType = None
+        self.DataEngineConfigPairs = None
+        self.ImageVersionName = None
+        self.MainClusterName = None
+        self.ElasticSwitch = None
+        self.ElasticLimit = None
+        self.EmrLivyInfo = None
+        self.SessionResourceTemplate = None
 
 
     def _deserialize(self, params):
         self.EngineType = params.get("EngineType")
         self.DataEngineName = params.get("DataEngineName")
         self.ClusterType = params.get("ClusterType")
         self.Mode = params.get("Mode")
@@ -3479,14 +4402,29 @@
         if params.get("CrontabResumeSuspendStrategy") is not None:
             self.CrontabResumeSuspendStrategy = CrontabResumeSuspendStrategy()
             self.CrontabResumeSuspendStrategy._deserialize(params.get("CrontabResumeSuspendStrategy"))
         self.EngineExecType = params.get("EngineExecType")
         self.MaxConcurrency = params.get("MaxConcurrency")
         self.TolerableQueueTime = params.get("TolerableQueueTime")
         self.AutoSuspendTime = params.get("AutoSuspendTime")
+        self.ResourceType = params.get("ResourceType")
+        if params.get("DataEngineConfigPairs") is not None:
+            self.DataEngineConfigPairs = []
+            for item in params.get("DataEngineConfigPairs"):
+                obj = DataEngineConfigPair()
+                obj._deserialize(item)
+                self.DataEngineConfigPairs.append(obj)
+        self.ImageVersionName = params.get("ImageVersionName")
+        self.MainClusterName = params.get("MainClusterName")
+        self.ElasticSwitch = params.get("ElasticSwitch")
+        self.ElasticLimit = params.get("ElasticLimit")
+        self.EmrLivyInfo = params.get("EmrLivyInfo")
+        if params.get("SessionResourceTemplate") is not None:
+            self.SessionResourceTemplate = SessionResourceTemplate()
+            self.SessionResourceTemplate._deserialize(params.get("SessionResourceTemplate"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4020,18 +4958,21 @@
         r"""
         :param TableBaseInfo: 表基本信息
         :type TableBaseInfo: :class:`tencentcloud.dlc.v20210125.models.TableBaseInfo`
         :param Columns: 表字段信息
         :type Columns: list of TColumn
         :param Partitions: 表分区信息
         :type Partitions: list of TPartition
+        :param Properties: 表属性信息
+        :type Properties: list of Property
         """
         self.TableBaseInfo = None
         self.Columns = None
         self.Partitions = None
+        self.Properties = None
 
 
     def _deserialize(self, params):
         if params.get("TableBaseInfo") is not None:
             self.TableBaseInfo = TableBaseInfo()
             self.TableBaseInfo._deserialize(params.get("TableBaseInfo"))
         if params.get("Columns") is not None:
@@ -4042,14 +4983,20 @@
                 self.Columns.append(obj)
         if params.get("Partitions") is not None:
             self.Partitions = []
             for item in params.get("Partitions"):
                 obj = TPartition()
                 obj._deserialize(item)
                 self.Partitions.append(obj)
+        if params.get("Properties") is not None:
+            self.Properties = []
+            for item in params.get("Properties"):
+                obj = Property()
+                obj._deserialize(item)
+                self.Properties.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4072,14 +5019,97 @@
 
 
     def _deserialize(self, params):
         self.Execution = params.get("Execution")
         self.RequestId = params.get("RequestId")
 
 
+class CreateKyuubiTaskRequest(AbstractModel):
+    """CreateKyuubiTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineName: 计算引擎名称，不填任务提交到默认集群	官
+        :type DataEngineName: str
+        :param DatasourceConnectionName: 数据源名称，默认为DataLakeCatalog
+        :type DatasourceConnectionName: str
+        :param DatabaseName: 数据库名称。如果SQL语句中有数据库名称，优先使用SQL语句中的数据库，否则使用该参数指定的数据库（注：当提交建库sql时，该字段传空字符串）。
+        :type DatabaseName: str
+        :param Task: SQL任务信息
+        :type Task: :class:`tencentcloud.dlc.v20210125.models.Task`
+        """
+        self.DataEngineName = None
+        self.DatasourceConnectionName = None
+        self.DatabaseName = None
+        self.Task = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineName = params.get("DataEngineName")
+        self.DatasourceConnectionName = params.get("DatasourceConnectionName")
+        self.DatabaseName = params.get("DatabaseName")
+        if params.get("Task") is not None:
+            self.Task = Task()
+            self.Task._deserialize(params.get("Task"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateKyuubiTaskResponse(AbstractModel):
+    """CreateKyuubiTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserAppID: 用户AppID
+        :type UserAppID: int
+        :param UserUin: 用户uin
+        :type UserUin: str
+        :param UserSubAccountUin: 用户SubAccountUin
+        :type UserSubAccountUin: str
+        :param TaskId: TaskId
+        :type TaskId: str
+        :param Vip: PrivateLink vpi
+        :type Vip: str
+        :param CoordinatorIp: CoordinatorIp
+        :type CoordinatorIp: str
+        :param DataEngineStatus: 集群状态 0-初始化 1-暂停 2-运行中
+        :type DataEngineStatus: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.UserAppID = None
+        self.UserUin = None
+        self.UserSubAccountUin = None
+        self.TaskId = None
+        self.Vip = None
+        self.CoordinatorIp = None
+        self.DataEngineStatus = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.UserAppID = params.get("UserAppID")
+        self.UserUin = params.get("UserUin")
+        self.UserSubAccountUin = params.get("UserSubAccountUin")
+        self.TaskId = params.get("TaskId")
+        self.Vip = params.get("Vip")
+        self.CoordinatorIp = params.get("CoordinatorIp")
+        self.DataEngineStatus = params.get("DataEngineStatus")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateLakeFsChdfsBindingRequest(AbstractModel):
     """CreateLakeFsChdfsBinding请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4126,14 +5156,36 @@
 
 
 class CreateLakeFsRequest(AbstractModel):
     """CreateLakeFs请求参数结构体
 
     """
 
+    def __init__(self):
+        r"""
+        :param Mode: 计费模式
+        :type Mode: str
+        :param BucketType: 桶类型，cos/chdfs
+        :type BucketType: str
+        """
+        self.Mode = None
+        self.BucketType = None
+
+
+    def _deserialize(self, params):
+        self.Mode = params.get("Mode")
+        self.BucketType = params.get("BucketType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class CreateLakeFsResponse(AbstractModel):
     """CreateLakeFs返回参数结构体
 
     """
 
     def __init__(self):
@@ -4202,24 +5254,30 @@
 
     def __init__(self):
         r"""
         :param DatasourceConnectionName: 数据源名称，默认DataLakeCatalog
         :type DatasourceConnectionName: str
         :param MetaDatabaseInfo: 元数据库基本信息
         :type MetaDatabaseInfo: :class:`tencentcloud.dlc.v20210125.models.MetaDatabaseInfo`
+        :param GovernPolicy: 数据治理配置项
+        :type GovernPolicy: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
         """
         self.DatasourceConnectionName = None
         self.MetaDatabaseInfo = None
+        self.GovernPolicy = None
 
 
     def _deserialize(self, params):
         self.DatasourceConnectionName = params.get("DatasourceConnectionName")
         if params.get("MetaDatabaseInfo") is not None:
             self.MetaDatabaseInfo = MetaDatabaseInfo()
             self.MetaDatabaseInfo._deserialize(params.get("MetaDatabaseInfo"))
+        if params.get("GovernPolicy") is not None:
+            self.GovernPolicy = DataGovernPolicy()
+            self.GovernPolicy._deserialize(params.get("GovernPolicy"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4273,34 +5331,40 @@
         :type ProgramArchives: list of str
         :param DriverSize: 指定的Driver规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type DriverSize: str
         :param ExecutorSize: 指定的Executor规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type ExecutorSize: str
         :param ExecutorNumbers: 指定的Executor数量，默认为1
         :type ExecutorNumbers: int
-        :param Arguments: Session相关配置，当前支持：eni、roleArn以及用户指定的配置
+        :param Arguments: Session相关配置，当前支持：dlc.eni、dlc.role.arn、dlc.sql.set.config以及用户指定的配置，注：roleArn必填；
         :type Arguments: list of KVPair
         :param ProxyUser: 代理用户，默认为root
         :type ProxyUser: str
         :param TimeoutInSecond: 指定的Session超时时间，单位秒，默认3600秒
         :type TimeoutInSecond: int
+        :param ExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于ExecutorNumbers
+        :type ExecutorMaxNumbers: int
+        :param SparkImage: 指定spark版本名称，当前任务使用该spark镜像运行
+        :type SparkImage: str
         """
         self.Name = None
         self.Kind = None
         self.DataEngineName = None
         self.ProgramDependentFiles = None
         self.ProgramDependentJars = None
         self.ProgramDependentPython = None
         self.ProgramArchives = None
         self.DriverSize = None
         self.ExecutorSize = None
         self.ExecutorNumbers = None
         self.Arguments = None
         self.ProxyUser = None
         self.TimeoutInSecond = None
+        self.ExecutorMaxNumbers = None
+        self.SparkImage = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Kind = params.get("Kind")
         self.DataEngineName = params.get("DataEngineName")
         self.ProgramDependentFiles = params.get("ProgramDependentFiles")
@@ -4314,14 +5378,16 @@
             self.Arguments = []
             for item in params.get("Arguments"):
                 obj = KVPair()
                 obj._deserialize(item)
                 self.Arguments.append(obj)
         self.ProxyUser = params.get("ProxyUser")
         self.TimeoutInSecond = params.get("TimeoutInSecond")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        self.SparkImage = params.get("SparkImage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4408,14 +5474,127 @@
     def _deserialize(self, params):
         if params.get("NotebookSessionStatement") is not None:
             self.NotebookSessionStatement = NotebookSessionStatementInfo()
             self.NotebookSessionStatement._deserialize(params.get("NotebookSessionStatement"))
         self.RequestId = params.get("RequestId")
 
 
+class CreateNotebookSessionStatementSupportBatchSQLRequest(AbstractModel):
+    """CreateNotebookSessionStatementSupportBatchSQL请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SessionId: Session唯一标识
+        :type SessionId: str
+        :param Code: 执行的代码
+        :type Code: str
+        :param Kind: 类型，当前支持：sql
+        :type Kind: str
+        :param SaveResult: 是否保存运行结果
+        :type SaveResult: bool
+        """
+        self.SessionId = None
+        self.Code = None
+        self.Kind = None
+        self.SaveResult = None
+
+
+    def _deserialize(self, params):
+        self.SessionId = params.get("SessionId")
+        self.Code = params.get("Code")
+        self.Kind = params.get("Kind")
+        self.SaveResult = params.get("SaveResult")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateNotebookSessionStatementSupportBatchSQLResponse(AbstractModel):
+    """CreateNotebookSessionStatementSupportBatchSQL返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NotebookSessionStatementBatches: Session Statement详情
+        :type NotebookSessionStatementBatches: :class:`tencentcloud.dlc.v20210125.models.NotebookSessionStatementBatchInformation`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.NotebookSessionStatementBatches = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("NotebookSessionStatementBatches") is not None:
+            self.NotebookSessionStatementBatches = NotebookSessionStatementBatchInformation()
+            self.NotebookSessionStatementBatches._deserialize(params.get("NotebookSessionStatementBatches"))
+        self.RequestId = params.get("RequestId")
+
+
+class CreateOrModifyCHDFSProductRequest(AbstractModel):
+    """CreateOrModifyCHDFSProduct请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductName: 产品名称
+        :type ProductName: str
+        :param SuperUser: 超级用户名称数组
+        :type SuperUser: list of str
+        :param VpcInfo: vpc配置信息数组
+        :type VpcInfo: list of CHDFSProductVpcInfo
+        """
+        self.ProductName = None
+        self.SuperUser = None
+        self.VpcInfo = None
+
+
+    def _deserialize(self, params):
+        self.ProductName = params.get("ProductName")
+        self.SuperUser = params.get("SuperUser")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = CHDFSProductVpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateOrModifyCHDFSProductResponse(AbstractModel):
+    """CreateOrModifyCHDFSProduct返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CreateQueryDirRequest(AbstractModel):
     """CreateQueryDir请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4449,37 +5628,112 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CreateResultDownloadRequest(AbstractModel):
+    """CreateResultDownload请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 查询结果任务Id
+        :type TaskId: str
+        :param Format: 下载格式
+        :type Format: str
+        :param Options: 下载选项
+        :type Options: list of KVPair
+        :param Force: 是否重新生成下载文件，仅当之前任务状态为 timeout | error 时有效
+        :type Force: bool
+        """
+        self.TaskId = None
+        self.Format = None
+        self.Options = None
+        self.Force = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.Format = params.get("Format")
+        if params.get("Options") is not None:
+            self.Options = []
+            for item in params.get("Options"):
+                obj = KVPair()
+                obj._deserialize(item)
+                self.Options.append(obj)
+        self.Force = params.get("Force")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateResultDownloadResponse(AbstractModel):
+    """CreateResultDownload返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DownloadId: 下载任务Id
+        :type DownloadId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DownloadId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DownloadId = params.get("DownloadId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateSQLSessionCatalogRequest(AbstractModel):
     """CreateSQLSessionCatalog请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Name: 目录名称
         :type Name: str
         :param Operator: 操作者
         :type Operator: str
         :param Path: 父目录名称
         :type Path: str
+        :param UserVisibility: 授权的子用户，空为自己和管理员可见
+        :type UserVisibility: str
+        :param PurviewInfoSet: 权限信息
+        :type PurviewInfoSet: list of PurviewInfo
         """
         self.Name = None
         self.Operator = None
         self.Path = None
+        self.UserVisibility = None
+        self.PurviewInfoSet = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Operator = params.get("Operator")
         self.Path = params.get("Path")
+        self.UserVisibility = params.get("UserVisibility")
+        if params.get("PurviewInfoSet") is not None:
+            self.PurviewInfoSet = []
+            for item in params.get("PurviewInfoSet"):
+                obj = PurviewInfo()
+                obj._deserialize(item)
+                self.PurviewInfoSet.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4739,69 +5993,150 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CreateSparkAppForSQLRequest(AbstractModel):
+    """CreateSparkAppForSQL请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AppName: spark应用名
+        :type AppName: str
+        :param DataEngine: 执行spark作业的数据引擎
+        :type DataEngine: str
+        :param AppDriverSize: spark作业driver资源规格大小, 可取small,medium,large,xlarge
+        :type AppDriverSize: str
+        :param AppExecutorSize: spark作业executor资源规格大小, 可取small,medium,large,xlarge
+        :type AppExecutorSize: str
+        :param AppExecutorNums: spark作业executor个数
+        :type AppExecutorNums: int
+        :param SQL: spark作业命令行参数
+        :type SQL: str
+        :param ENI: 该字段已下线，请使用字段Datasource
+        :type ENI: str
+        :param AppExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于AppExecutorNums
+        :type AppExecutorMaxNumbers: int
+        """
+        self.AppName = None
+        self.DataEngine = None
+        self.AppDriverSize = None
+        self.AppExecutorSize = None
+        self.AppExecutorNums = None
+        self.SQL = None
+        self.ENI = None
+        self.AppExecutorMaxNumbers = None
+
+
+    def _deserialize(self, params):
+        self.AppName = params.get("AppName")
+        self.DataEngine = params.get("DataEngine")
+        self.AppDriverSize = params.get("AppDriverSize")
+        self.AppExecutorSize = params.get("AppExecutorSize")
+        self.AppExecutorNums = params.get("AppExecutorNums")
+        self.SQL = params.get("SQL")
+        self.ENI = params.get("ENI")
+        self.AppExecutorMaxNumbers = params.get("AppExecutorMaxNumbers")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateSparkAppForSQLResponse(AbstractModel):
+    """CreateSparkAppForSQL返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SparkAppId: Job id
+        :type SparkAppId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.SparkAppId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.SparkAppId = params.get("SparkAppId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateSparkAppRequest(AbstractModel):
     """CreateSparkApp请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AppName: spark应用名
+        :param AppName: spark作业名
         :type AppName: str
-        :param AppType: 1代表spark jar应用，2代表spark streaming应用
+        :param AppType: spark作业类型，1代表spark jar作业，2代表spark streaming作业
         :type AppType: int
-        :param DataEngine: 执行spark作业的数据引擎
+        :param DataEngine: 执行spark作业的数据引擎名称
         :type DataEngine: str
-        :param AppFile: spark应用的执行入口
+        :param AppFile: spark作业程序包文件路径
         :type AppFile: str
-        :param RoleArn: 执行spark作业的角色ID
+        :param RoleArn: 数据访问策略，CAM Role arn
         :type RoleArn: int
-        :param AppDriverSize: spark作业driver资源规格大小, 可取small,medium,large,xlarge
+        :param AppDriverSize: 指定的Driver规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppDriverSize: str
-        :param AppExecutorSize: spark作业executor资源规格大小, 可取small,medium,large,xlarge
+        :param AppExecutorSize: 指定的Executor规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppExecutorSize: str
         :param AppExecutorNums: spark作业executor个数
         :type AppExecutorNums: int
         :param Eni: 该字段已下线，请使用字段Datasource
         :type Eni: str
-        :param IsLocal: 是否本地上传，可去cos,lakefs
+        :param IsLocal: spark作业程序包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocal: str
-        :param MainClass: spark jar作业时的主类
+        :param MainClass: spark作业主类
         :type MainClass: str
         :param AppConf: spark配置，以换行符分隔
         :type AppConf: str
-        :param IsLocalJars: 是否本地上传，包含cos,lakefs
+        :param IsLocalJars: spark 作业依赖jar包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalJars: str
-        :param AppJars: spark jar作业依赖jars，以逗号分隔
+        :param AppJars: spark 作业依赖jar包（--jars），以逗号分隔
         :type AppJars: str
-        :param IsLocalFiles: 是否本地上传，包含cos,lakefs
+        :param IsLocalFiles: spark作业依赖文件资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalFiles: str
-        :param AppFiles: spark作业依赖资源，以逗号分隔
+        :param AppFiles: spark作业依赖文件资源（--files）（非jar、zip），以逗号分隔
         :type AppFiles: str
-        :param CmdArgs: spark作业命令行参数
+        :param CmdArgs: spark作业程序入参，空格分割
         :type CmdArgs: str
-        :param MaxRetries: 只对spark流任务生效
+        :param MaxRetries: 最大重试次数，只对spark流任务生效
         :type MaxRetries: int
-        :param DataSource: 数据源名
+        :param DataSource: 数据源名称
         :type DataSource: str
-        :param IsLocalPythonFiles: pyspark：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalPythonFiles: pyspark：依赖上传方式，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalPythonFiles: str
-        :param AppPythonFiles: pyspark：python依赖, 除py文件外，还支持zip/egg等归档格式，多文件以逗号分隔
+        :param AppPythonFiles: pyspark作业依赖python资源（--py-files），支持py/zip/egg等归档格式，多文件以逗号分隔
         :type AppPythonFiles: str
-        :param IsLocalArchives: archives：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalArchives: spark作业依赖archives资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalArchives: str
-        :param AppArchives: archives：依赖资源
+        :param AppArchives: spark作业依赖archives资源（--archives），支持tar.gz/tgz/tar等归档格式，以逗号分隔
         :type AppArchives: str
-        :param SparkImage: Spark Image 版本
+        :param SparkImage: Spark Image 版本号
         :type SparkImage: str
+        :param SparkImageVersion: Spark Image 版本名称
+        :type SparkImageVersion: str
+        :param AppExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于AppExecutorNums
+        :type AppExecutorMaxNumbers: int
+        :param SessionId: 关联dlc查询脚本id
+        :type SessionId: str
+        :param IsInherit: 任务资源配置是否继承集群模板，0（默认）不继承，1：继承
+        :type IsInherit: int
         """
         self.AppName = None
         self.AppType = None
         self.DataEngine = None
         self.AppFile = None
         self.RoleArn = None
         self.AppDriverSize = None
@@ -4819,14 +6154,18 @@
         self.MaxRetries = None
         self.DataSource = None
         self.IsLocalPythonFiles = None
         self.AppPythonFiles = None
         self.IsLocalArchives = None
         self.AppArchives = None
         self.SparkImage = None
+        self.SparkImageVersion = None
+        self.AppExecutorMaxNumbers = None
+        self.SessionId = None
+        self.IsInherit = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.AppType = params.get("AppType")
         self.DataEngine = params.get("DataEngine")
         self.AppFile = params.get("AppFile")
@@ -4846,14 +6185,18 @@
         self.MaxRetries = params.get("MaxRetries")
         self.DataSource = params.get("DataSource")
         self.IsLocalPythonFiles = params.get("IsLocalPythonFiles")
         self.AppPythonFiles = params.get("AppPythonFiles")
         self.IsLocalArchives = params.get("IsLocalArchives")
         self.AppArchives = params.get("AppArchives")
         self.SparkImage = params.get("SparkImage")
+        self.SparkImageVersion = params.get("SparkImageVersion")
+        self.AppExecutorMaxNumbers = params.get("AppExecutorMaxNumbers")
+        self.SessionId = params.get("SessionId")
+        self.IsInherit = params.get("IsInherit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4862,34 +6205,39 @@
 class CreateSparkAppResponse(AbstractModel):
     """CreateSparkApp返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param SparkAppId: App唯一标识
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SparkAppId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self.SparkAppId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
+        self.SparkAppId = params.get("SparkAppId")
         self.RequestId = params.get("RequestId")
 
 
 class CreateSparkAppTaskRequest(AbstractModel):
     """CreateSparkAppTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param JobName: spark作业名
         :type JobName: str
-        :param CmdArgs: spark作业的命令行参数，以空格分隔；一般用于周期性调用使用
+        :param CmdArgs: spark作业程序入参，以空格分隔；一般用于周期性调用使用
         :type CmdArgs: str
         """
         self.JobName = None
         self.CmdArgs = None
 
 
     def _deserialize(self, params):
@@ -4925,14 +6273,102 @@
 
     def _deserialize(self, params):
         self.BatchId = params.get("BatchId")
         self.TaskId = params.get("TaskId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateSparkSessionBatchSQLRequest(AbstractModel):
+    """CreateSparkSessionBatchSQL请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineName: DLC Spark作业引擎名称
+        :type DataEngineName: str
+        :param ExecuteSQL: 运行sql
+        :type ExecuteSQL: str
+        :param DriverSize: 指定的Driver规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
+        :type DriverSize: str
+        :param ExecutorSize: 指定的Executor规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
+        :type ExecutorSize: str
+        :param ExecutorNumbers: 指定的Executor数量，默认为1
+        :type ExecutorNumbers: int
+        :param ExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于ExecutorNumbers
+        :type ExecutorMaxNumbers: int
+        :param TimeoutInSecond: 指定的Session超时时间，单位秒，默认3600秒
+        :type TimeoutInSecond: int
+        :param SessionId: Session唯一标识，当指定sessionid，则使用该session运行任务。
+        :type SessionId: str
+        :param SessionName: 指定要创建的session名称
+        :type SessionName: str
+        :param Arguments: Session相关配置，当前支持：1.dlc.eni：用户配置的eni网关信息，可以用过该字段设置；
+2.dlc.role.arn：用户配置的roleArn鉴权策略配置信息，可以用过该字段设置；
+3.dlc.sql.set.config：用户配置的集群配置信息，可以用过该字段设置；
+        :type Arguments: list of KVPair
+        """
+        self.DataEngineName = None
+        self.ExecuteSQL = None
+        self.DriverSize = None
+        self.ExecutorSize = None
+        self.ExecutorNumbers = None
+        self.ExecutorMaxNumbers = None
+        self.TimeoutInSecond = None
+        self.SessionId = None
+        self.SessionName = None
+        self.Arguments = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineName = params.get("DataEngineName")
+        self.ExecuteSQL = params.get("ExecuteSQL")
+        self.DriverSize = params.get("DriverSize")
+        self.ExecutorSize = params.get("ExecutorSize")
+        self.ExecutorNumbers = params.get("ExecutorNumbers")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        self.TimeoutInSecond = params.get("TimeoutInSecond")
+        self.SessionId = params.get("SessionId")
+        self.SessionName = params.get("SessionName")
+        if params.get("Arguments") is not None:
+            self.Arguments = []
+            for item in params.get("Arguments"):
+                obj = KVPair()
+                obj._deserialize(item)
+                self.Arguments.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateSparkSessionBatchSQLResponse(AbstractModel):
+    """CreateSparkSessionBatchSQL返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务唯一标识
+        :type BatchId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BatchId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateStoreLocationRequest(AbstractModel):
     """CreateStoreLocation请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5402,34 +6838,38 @@
         :type TaskAction: str
         :param StartTime: 调度计划开始时间
         :type StartTime: str
         :param EndTime: 调度计划结束时间
         :type EndTime: str
         :param WorkflowDesc: 调度计划描述
         :type WorkflowDesc: str
+        :param OwnersUin: 调度计划责任人uin数组
+        :type OwnersUin: list of str
         """
         self.WorkflowName = None
         self.CycleType = None
         self.CycleStep = None
         self.DelayTime = None
         self.TaskAction = None
         self.StartTime = None
         self.EndTime = None
         self.WorkflowDesc = None
+        self.OwnersUin = None
 
 
     def _deserialize(self, params):
         self.WorkflowName = params.get("WorkflowName")
         self.CycleType = params.get("CycleType")
         self.CycleStep = params.get("CycleStep")
         self.DelayTime = params.get("DelayTime")
         self.TaskAction = params.get("TaskAction")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.WorkflowDesc = params.get("WorkflowDesc")
+        self.OwnersUin = params.get("OwnersUin")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5487,14 +6927,69 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DLCCHDFSBinding(AbstractModel):
+    """dlc引擎绑定桶列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EngineId: 引擎Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EngineId: str
+        :param EngineName: 引擎名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EngineName: str
+        :param SuperUser: 用户名称（该字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SuperUser: list of str
+        :param VpcInfo: vpc配置信息（该字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcInfo: list of CHDFSProductVpcInfo
+        :param Permissions: 引擎绑定权限
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Permissions: list of str
+        :param IsBind: 是否与该桶绑定
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsBind: bool
+        """
+        self.EngineId = None
+        self.EngineName = None
+        self.SuperUser = None
+        self.VpcInfo = None
+        self.Permissions = None
+        self.IsBind = None
+
+
+    def _deserialize(self, params):
+        self.EngineId = params.get("EngineId")
+        self.EngineName = params.get("EngineName")
+        self.SuperUser = params.get("SuperUser")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = CHDFSProductVpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        self.Permissions = params.get("Permissions")
+        self.IsBind = params.get("IsBind")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DMSColumn(AbstractModel):
     """迁移列对象
 
     """
 
     def __init__(self):
         r"""
@@ -6112,14 +7607,286 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DataEngineBasicInfo(AbstractModel):
+    """DataEngine基本信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineName: DataEngine名称
+        :type DataEngineName: str
+        :param State: 数据引擎状态  -2已删除 -1失败 0初始化中 1挂起 2运行中 3准备删除 4删除中
+        :type State: int
+        :param CreateTime: 创建时间
+        :type CreateTime: int
+        :param UpdateTime: 更新时间
+        :type UpdateTime: int
+        :param Message: 返回信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param DataEngineId: 引擎id
+        :type DataEngineId: str
+        :param DataEngineType: 引擎类型，有效值：PrestoSQL/SparkSQL/SparkBatch
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataEngineType: str
+        :param AppId: 用户ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param UserUin: 账号ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserUin: str
+        """
+        self.DataEngineName = None
+        self.State = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.Message = None
+        self.DataEngineId = None
+        self.DataEngineType = None
+        self.AppId = None
+        self.UserUin = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineName = params.get("DataEngineName")
+        self.State = params.get("State")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.Message = params.get("Message")
+        self.DataEngineId = params.get("DataEngineId")
+        self.DataEngineType = params.get("DataEngineType")
+        self.AppId = params.get("AppId")
+        self.UserUin = params.get("UserUin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DataEngineConfigInstanceInfo(AbstractModel):
+    """引擎配置信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataEngineId: str
+        :param DataEngineConfigPairs: 用户自定义配置项集合
+        :type DataEngineConfigPairs: list of DataEngineConfigPair
+        :param SessionResourceTemplate: 作业集群资源参数配置模版
+        :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
+        """
+        self.DataEngineId = None
+        self.DataEngineConfigPairs = None
+        self.SessionResourceTemplate = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        if params.get("DataEngineConfigPairs") is not None:
+            self.DataEngineConfigPairs = []
+            for item in params.get("DataEngineConfigPairs"):
+                obj = DataEngineConfigPair()
+                obj._deserialize(item)
+                self.DataEngineConfigPairs.append(obj)
+        if params.get("SessionResourceTemplate") is not None:
+            self.SessionResourceTemplate = SessionResourceTemplate()
+            self.SessionResourceTemplate._deserialize(params.get("SessionResourceTemplate"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DataEngineConfigPair(AbstractModel):
+    """引擎配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ConfigItem: 配置项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConfigItem: str
+        :param ConfigValue: 配置值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConfigValue: str
+        """
+        self.ConfigItem = None
+        self.ConfigValue = None
+
+
+    def _deserialize(self, params):
+        self.ConfigItem = params.get("ConfigItem")
+        self.ConfigValue = params.get("ConfigValue")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DataEngineImageSessionParameter(AbstractModel):
+    """集群Session配置信息.
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ParameterId: 配置id
+        :type ParameterId: str
+        :param ChildImageVersionId: 小版本镜像ID
+        :type ChildImageVersionId: str
+        :param EngineType: 集群类型：SparkSQL/PrestoSQL/SparkBatch
+        :type EngineType: str
+        :param KeyName: 参数key
+        :type KeyName: str
+        :param KeyDescription: Key描述信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type KeyDescription: str
+        :param ValueType: value类型
+        :type ValueType: str
+        :param ValueLengthLimit: value长度限制
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ValueLengthLimit: str
+        :param ValueRegexpLimit: value正则限制
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ValueRegexpLimit: str
+        :param ValueDefault: value默认值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ValueDefault: str
+        :param IsPublic: 是否为公共版本：1：公共；2：私有
+        :type IsPublic: int
+        :param ParameterType: 配置类型：1：session配置（默认）；2：common配置；3：cluster配置
+        :type ParameterType: int
+        :param SubmitMethod: 提交方式：User(用户)、BackGround（后台）
+        :type SubmitMethod: str
+        :param Operator: 操作者
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Operator: str
+        :param InsertTime: 插入时间
+        :type InsertTime: str
+        :param UpdateTime: 更新时间
+        :type UpdateTime: str
+        """
+        self.ParameterId = None
+        self.ChildImageVersionId = None
+        self.EngineType = None
+        self.KeyName = None
+        self.KeyDescription = None
+        self.ValueType = None
+        self.ValueLengthLimit = None
+        self.ValueRegexpLimit = None
+        self.ValueDefault = None
+        self.IsPublic = None
+        self.ParameterType = None
+        self.SubmitMethod = None
+        self.Operator = None
+        self.InsertTime = None
+        self.UpdateTime = None
+
+
+    def _deserialize(self, params):
+        self.ParameterId = params.get("ParameterId")
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        self.EngineType = params.get("EngineType")
+        self.KeyName = params.get("KeyName")
+        self.KeyDescription = params.get("KeyDescription")
+        self.ValueType = params.get("ValueType")
+        self.ValueLengthLimit = params.get("ValueLengthLimit")
+        self.ValueRegexpLimit = params.get("ValueRegexpLimit")
+        self.ValueDefault = params.get("ValueDefault")
+        self.IsPublic = params.get("IsPublic")
+        self.ParameterType = params.get("ParameterType")
+        self.SubmitMethod = params.get("SubmitMethod")
+        self.Operator = params.get("Operator")
+        self.InsertTime = params.get("InsertTime")
+        self.UpdateTime = params.get("UpdateTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DataEngineImageVersion(AbstractModel):
+    """集群大版本镜像信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ImageVersionId: 镜像大版本ID
+        :type ImageVersionId: str
+        :param ImageVersion: 镜像大版本名称
+        :type ImageVersion: str
+        :param Description: 镜像大版本描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param IsPublic: 是否为公共版本：1：公共；2：私有
+        :type IsPublic: int
+        :param EngineType: 集群类型：SparkSQL/PrestoSQL/SparkBatch
+        :type EngineType: str
+        :param IsSharedEngine: 版本状态：1：初始化；2：上线；3：下线
+        :type IsSharedEngine: int
+        :param State: 版本状态：1：初始化；2：上线；3：下线
+        :type State: int
+        :param InsertTime: 插入时间
+        :type InsertTime: str
+        :param UpdateTime: 更新时间
+        :type UpdateTime: str
+        """
+        self.ImageVersionId = None
+        self.ImageVersion = None
+        self.Description = None
+        self.IsPublic = None
+        self.EngineType = None
+        self.IsSharedEngine = None
+        self.State = None
+        self.InsertTime = None
+        self.UpdateTime = None
+
+
+    def _deserialize(self, params):
+        self.ImageVersionId = params.get("ImageVersionId")
+        self.ImageVersion = params.get("ImageVersion")
+        self.Description = params.get("Description")
+        self.IsPublic = params.get("IsPublic")
+        self.EngineType = params.get("EngineType")
+        self.IsSharedEngine = params.get("IsSharedEngine")
+        self.State = params.get("State")
+        self.InsertTime = params.get("InsertTime")
+        self.UpdateTime = params.get("UpdateTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DataEngineInfo(AbstractModel):
     """DataEngine详细信息
 
     """
 
     def __init__(self):
         r"""
@@ -6206,14 +7973,56 @@
         :type RenewFlag: int
         :param AutoSuspendTime: 集群自动挂起时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type AutoSuspendTime: int
         :param NetworkConnectionSet: 网络连接配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type NetworkConnectionSet: list of NetworkConnection
+        :param UiURL: ui的跳转地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UiURL: str
+        :param ResourceType: 引擎的资源类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceType: str
+        :param ImageVersionId: 集群镜像版本ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageVersionId: str
+        :param ChildImageVersionId: 集群镜像小版本ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChildImageVersionId: str
+        :param ImageVersionName: 集群镜像版本名字
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageVersionName: str
+        :param StartStandbyCluster: 是否开启备集群
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartStandbyCluster: bool
+        :param ElasticSwitch: spark jar 包年包月集群是否开启弹性
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ElasticSwitch: bool
+        :param ElasticLimit: spark jar 包年包月集群弹性上限
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ElasticLimit: int
+        :param DefaultHouse: 是否为默认引擎
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefaultHouse: bool
+        :param MaxConcurrency: 单个集群任务最大并发数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MaxConcurrency: int
+        :param TolerableQueueTime: 任务排队上限时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TolerableQueueTime: int
+        :param UserAppId: 用户appid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserAppId: int
+        :param UserUin: 用户uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserUin: str
+        :param SessionResourceTemplate: SessionResourceTemplate
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
         """
         self.DataEngineName = None
         self.EngineType = None
         self.ClusterType = None
         self.Id = None
         self.QuotaId = None
         self.State = None
@@ -6241,14 +8050,28 @@
         self.AutoSuspend = None
         self.CrontabResumeSuspend = None
         self.CrontabResumeSuspendStrategy = None
         self.EngineExecType = None
         self.RenewFlag = None
         self.AutoSuspendTime = None
         self.NetworkConnectionSet = None
+        self.UiURL = None
+        self.ResourceType = None
+        self.ImageVersionId = None
+        self.ChildImageVersionId = None
+        self.ImageVersionName = None
+        self.StartStandbyCluster = None
+        self.ElasticSwitch = None
+        self.ElasticLimit = None
+        self.DefaultHouse = None
+        self.MaxConcurrency = None
+        self.TolerableQueueTime = None
+        self.UserAppId = None
+        self.UserUin = None
+        self.SessionResourceTemplate = None
 
 
     def _deserialize(self, params):
         self.DataEngineName = params.get("DataEngineName")
         self.EngineType = params.get("EngineType")
         self.ClusterType = params.get("ClusterType")
         self.Id = params.get("Id")
@@ -6290,14 +8113,30 @@
         self.AutoSuspendTime = params.get("AutoSuspendTime")
         if params.get("NetworkConnectionSet") is not None:
             self.NetworkConnectionSet = []
             for item in params.get("NetworkConnectionSet"):
                 obj = NetworkConnection()
                 obj._deserialize(item)
                 self.NetworkConnectionSet.append(obj)
+        self.UiURL = params.get("UiURL")
+        self.ResourceType = params.get("ResourceType")
+        self.ImageVersionId = params.get("ImageVersionId")
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        self.ImageVersionName = params.get("ImageVersionName")
+        self.StartStandbyCluster = params.get("StartStandbyCluster")
+        self.ElasticSwitch = params.get("ElasticSwitch")
+        self.ElasticLimit = params.get("ElasticLimit")
+        self.DefaultHouse = params.get("DefaultHouse")
+        self.MaxConcurrency = params.get("MaxConcurrency")
+        self.TolerableQueueTime = params.get("TolerableQueueTime")
+        self.UserAppId = params.get("UserAppId")
+        self.UserUin = params.get("UserUin")
+        if params.get("SessionResourceTemplate") is not None:
+            self.SessionResourceTemplate = SessionResourceTemplate()
+            self.SessionResourceTemplate._deserialize(params.get("SessionResourceTemplate"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6391,14 +8230,77 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DataGovernPolicy(AbstractModel):
+    """数据治理规则
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RewriteDataPolicy: 数据排布治理项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RewriteDataPolicy: :class:`tencentcloud.dlc.v20210125.models.RewriteDataInfo`
+        :param ExpiredSnapshotsPolicy: 快照过期治理项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExpiredSnapshotsPolicy: :class:`tencentcloud.dlc.v20210125.models.ExpiredSnapshotsInfo`
+        :param RemoveOrphanFilesPolicy: 移除孤立文件治理项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RemoveOrphanFilesPolicy: :class:`tencentcloud.dlc.v20210125.models.RemoveOrphanFilesInfo`
+        :param MergeManifestsPolicy: 合并元数据Manifests治理项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MergeManifestsPolicy: :class:`tencentcloud.dlc.v20210125.models.MergeManifestsInfo`
+        :param InheritDataBase: 是否集成库规则：default（默认继承）、none（不继承）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InheritDataBase: str
+        :param RuleType: 治理规则类型，Customize: 自定义；Intelligence: 智能治理
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RuleType: str
+        :param GovernEngine: 治理引擎
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GovernEngine: str
+        """
+        self.RewriteDataPolicy = None
+        self.ExpiredSnapshotsPolicy = None
+        self.RemoveOrphanFilesPolicy = None
+        self.MergeManifestsPolicy = None
+        self.InheritDataBase = None
+        self.RuleType = None
+        self.GovernEngine = None
+
+
+    def _deserialize(self, params):
+        if params.get("RewriteDataPolicy") is not None:
+            self.RewriteDataPolicy = RewriteDataInfo()
+            self.RewriteDataPolicy._deserialize(params.get("RewriteDataPolicy"))
+        if params.get("ExpiredSnapshotsPolicy") is not None:
+            self.ExpiredSnapshotsPolicy = ExpiredSnapshotsInfo()
+            self.ExpiredSnapshotsPolicy._deserialize(params.get("ExpiredSnapshotsPolicy"))
+        if params.get("RemoveOrphanFilesPolicy") is not None:
+            self.RemoveOrphanFilesPolicy = RemoveOrphanFilesInfo()
+            self.RemoveOrphanFilesPolicy._deserialize(params.get("RemoveOrphanFilesPolicy"))
+        if params.get("MergeManifestsPolicy") is not None:
+            self.MergeManifestsPolicy = MergeManifestsInfo()
+            self.MergeManifestsPolicy._deserialize(params.get("MergeManifestsPolicy"))
+        self.InheritDataBase = params.get("InheritDataBase")
+        self.RuleType = params.get("RuleType")
+        self.GovernEngine = params.get("GovernEngine")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DataQuery(AbstractModel):
     """数据查询实例
 
     """
 
     def __init__(self):
         r"""
@@ -6594,23 +8496,31 @@
         :type Location: str
         :param UserAlias: 建库用户昵称
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserAlias: str
         :param UserSubUin: 建库用户ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserSubUin: str
+        :param GovernPolicy: 数据治理配置项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GovernPolicy: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
+        :param DatabaseId: 数据库ID（无效字段）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DatabaseId: str
         """
         self.DatabaseName = None
         self.Comment = None
         self.Properties = None
         self.CreateTime = None
         self.ModifiedTime = None
         self.Location = None
         self.UserAlias = None
         self.UserSubUin = None
+        self.GovernPolicy = None
+        self.DatabaseId = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.Comment = params.get("Comment")
         if params.get("Properties") is not None:
             self.Properties = []
@@ -6619,14 +8529,18 @@
                 obj._deserialize(item)
                 self.Properties.append(obj)
         self.CreateTime = params.get("CreateTime")
         self.ModifiedTime = params.get("ModifiedTime")
         self.Location = params.get("Location")
         self.UserAlias = params.get("UserAlias")
         self.UserSubUin = params.get("UserSubUin")
+        if params.get("GovernPolicy") is not None:
+            self.GovernPolicy = DataGovernPolicy()
+            self.GovernPolicy._deserialize(params.get("GovernPolicy"))
+        self.DatabaseId = params.get("DatabaseId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6659,23 +8573,27 @@
         :type SqlServer: :class:`tencentcloud.dlc.v20210125.models.DataSourceInfo`
         :param ClickHouse: ClickHouse数据源连接的属性
 注意：此字段可能返回 null，表示取不到有效值。
         :type ClickHouse: :class:`tencentcloud.dlc.v20210125.models.DataSourceInfo`
         :param Elasticsearch: Elasticsearch数据源连接的属性
 注意：此字段可能返回 null，表示取不到有效值。
         :type Elasticsearch: :class:`tencentcloud.dlc.v20210125.models.ElasticsearchInfo`
+        :param TDSQLPostgreSql: TDSQL-PostgreSQL数据源连接的属性
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TDSQLPostgreSql: :class:`tencentcloud.dlc.v20210125.models.DataSourceInfo`
         """
         self.Mysql = None
         self.Hive = None
         self.Kafka = None
         self.OtherDatasourceConnection = None
         self.PostgreSql = None
         self.SqlServer = None
         self.ClickHouse = None
         self.Elasticsearch = None
+        self.TDSQLPostgreSql = None
 
 
     def _deserialize(self, params):
         if params.get("Mysql") is not None:
             self.Mysql = MysqlInfo()
             self.Mysql._deserialize(params.get("Mysql"))
         if params.get("Hive") is not None:
@@ -6695,14 +8613,17 @@
             self.SqlServer._deserialize(params.get("SqlServer"))
         if params.get("ClickHouse") is not None:
             self.ClickHouse = DataSourceInfo()
             self.ClickHouse._deserialize(params.get("ClickHouse"))
         if params.get("Elasticsearch") is not None:
             self.Elasticsearch = ElasticsearchInfo()
             self.Elasticsearch._deserialize(params.get("Elasticsearch"))
+        if params.get("TDSQLPostgreSql") is not None:
+            self.TDSQLPostgreSql = DataSourceInfo()
+            self.TDSQLPostgreSql._deserialize(params.get("TDSQLPostgreSql"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6902,14 +8823,117 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DeleteCHDFSBindingProductRequest(AbstractModel):
+    """DeleteCHDFSBindingProduct请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MountPoint: 需要解绑的元数据加速桶名
+        :type MountPoint: str
+        :param BucketType: 桶的类型，分为cos和lakefs
+        :type BucketType: str
+        :param ProductName: 产品名称
+        :type ProductName: str
+        :param EngineName: 引擎名称，ProductName选择DLC产品时，必传此参数。其他产品可不传
+        :type EngineName: str
+        :param VpcInfo: vpc信息，ProductName选择other时，必传此参数
+        :type VpcInfo: list of VpcInfo
+        """
+        self.MountPoint = None
+        self.BucketType = None
+        self.ProductName = None
+        self.EngineName = None
+        self.VpcInfo = None
+
+
+    def _deserialize(self, params):
+        self.MountPoint = params.get("MountPoint")
+        self.BucketType = params.get("BucketType")
+        self.ProductName = params.get("ProductName")
+        self.EngineName = params.get("EngineName")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = VpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteCHDFSBindingProductResponse(AbstractModel):
+    """DeleteCHDFSBindingProduct返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class DeleteCHDFSProductRequest(AbstractModel):
+    """DeleteCHDFSProduct请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductName: 产品名称
+        :type ProductName: str
+        """
+        self.ProductName = None
+
+
+    def _deserialize(self, params):
+        self.ProductName = params.get("ProductName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteCHDFSProductResponse(AbstractModel):
+    """DeleteCHDFSProduct返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteColumnsRequest(AbstractModel):
     """DeleteColumns请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7193,24 +9217,28 @@
 
     """
 
     def __init__(self):
         r"""
         :param MountPoint: 挂载点
         :type MountPoint: str
-        :param DataEngine: 引擎名称
+        :param DataEngine: DLC引擎名称，删除指定DLC引擎和chdfs绑定关系
         :type DataEngine: str
+        :param AccessGroupId: 权限组ID，删除指定权限组和chdfs绑定关系
+        :type AccessGroupId: str
         """
         self.MountPoint = None
         self.DataEngine = None
+        self.AccessGroupId = None
 
 
     def _deserialize(self, params):
         self.MountPoint = params.get("MountPoint")
         self.DataEngine = params.get("DataEngine")
+        self.AccessGroupId = params.get("AccessGroupId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -7229,14 +9257,55 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteLakeFsRequest(AbstractModel):
+    """DeleteLakeFs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FsPath: 托管存储路径
+        :type FsPath: list of str
+        """
+        self.FsPath = None
+
+
+    def _deserialize(self, params):
+        self.FsPath = params.get("FsPath")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteLakeFsResponse(AbstractModel):
+    """DeleteLakeFs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteLinkRequest(AbstractModel):
     """DeleteLink请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7684,15 +9753,15 @@
 class DeleteSparkAppRequest(AbstractModel):
     """DeleteSparkApp请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AppName: spark应用名
+        :param AppName: spark作业名
         :type AppName: str
         :param ForceKillJob: 删掉spark应用时，是否强制杀掉当前正在运行的任务
         :type ForceKillJob: bool
         """
         self.AppName = None
         self.ForceKillJob = None
 
@@ -7774,22 +9843,26 @@
 
     def __init__(self):
         r"""
         :param ImageId: 镜像编码
         :type ImageId: str
         :param UserAppId: 用户APPID
         :type UserAppId: int
+        :param ImageType: 枚举值：1（父版本）、2（子版本）、3（pyspark）
+        :type ImageType: str
         """
         self.ImageId = None
         self.UserAppId = None
+        self.ImageType = None
 
 
     def _deserialize(self, params):
         self.ImageId = params.get("ImageId")
         self.UserAppId = params.get("UserAppId")
+        self.ImageType = params.get("ImageType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -7808,14 +9881,71 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteTableBatchRequest(AbstractModel):
+    """DeleteTableBatch请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DatasourceConnectionName: Catalog名称
+        :type DatasourceConnectionName: str
+        :param DatabaseName: 库名
+        :type DatabaseName: str
+        :param TableNames: 表名列表
+        :type TableNames: list of str
+        """
+        self.DatasourceConnectionName = None
+        self.DatabaseName = None
+        self.TableNames = None
+
+
+    def _deserialize(self, params):
+        self.DatasourceConnectionName = params.get("DatasourceConnectionName")
+        self.DatabaseName = params.get("DatabaseName")
+        self.TableNames = params.get("TableNames")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteTableBatchResponse(AbstractModel):
+    """DeleteTableBatch返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务Id
+        :type BatchId: str
+        :param TaskIdSet: TaskId列表
+        :type TaskIdSet: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BatchId = None
+        self.TaskIdSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        self.TaskIdSet = params.get("TaskIdSet")
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteTableRequest(AbstractModel):
     """DeleteTable请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8136,27 +10266,37 @@
         r"""
         :param Enable: 是否启用高级设置：0-否，1-是
         :type Enable: int
         :param StoreLocation: 查询结果保存cos路径
         :type StoreLocation: str
         :param HasLakeFs: 是否有托管存储权限
         :type HasLakeFs: bool
+        :param LakeFsStatus: 托管存储状态，HasLakeFs等于true时，该值才有意义
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LakeFsStatus: str
+        :param BucketType: 托管存储桶类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BucketType: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Enable = None
         self.StoreLocation = None
         self.HasLakeFs = None
+        self.LakeFsStatus = None
+        self.BucketType = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Enable = params.get("Enable")
         self.StoreLocation = params.get("StoreLocation")
         self.HasLakeFs = params.get("HasLakeFs")
+        self.LakeFsStatus = params.get("LakeFsStatus")
+        self.BucketType = params.get("BucketType")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeAllColumnsRequest(AbstractModel):
     """DescribeAllColumns请求参数结构体
 
     """
@@ -8316,14 +10456,146 @@
                 obj._deserialize(item)
                 self.AuditEvents.append(obj)
         self.NextToken = params.get("NextToken")
         self.ListOver = params.get("ListOver")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeAvailableVpcRequest(AbstractModel):
+    """DescribeAvailableVpc请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PayMode: 付费模式，0:后付费，1:预付费
+        :type PayMode: int
+        """
+        self.PayMode = None
+
+
+    def _deserialize(self, params):
+        self.PayMode = params.get("PayMode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAvailableVpcResponse(AbstractModel):
+    """DescribeAvailableVpc返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcConfigures: vpc配置信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcConfigures: list of VpcConfigure
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.VpcConfigures = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("VpcConfigures") is not None:
+            self.VpcConfigures = []
+            for item in params.get("VpcConfigures"):
+                obj = VpcConfigure()
+                obj._deserialize(item)
+                self.VpcConfigures.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeBucketTypeRequest(AbstractModel):
+    """DescribeBucketType请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Path: 路径：可以是lakefs://xxx，cos://xxx，cosn://xxx
+        :type Path: str
+        """
+        self.Path = None
+
+
+    def _deserialize(self, params):
+        self.Path = params.get("Path")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeBucketTypeResponse(AbstractModel):
+    """DescribeBucketType返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BucketType: 桶类型：cos/chdfs
+        :type BucketType: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BucketType = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BucketType = params.get("BucketType")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeCHDFSAccessInfosRequest(AbstractModel):
+    """DescribeCHDFSAccessInfos请求参数结构体
+
+    """
+
+
+class DescribeCHDFSAccessInfosResponse(AbstractModel):
+    """DescribeCHDFSAccessInfos返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CHDFSAccessInfos: chdfs产品列表
+        :type CHDFSAccessInfos: list of CHDFSAccessInfo
+        :param Total: 总条数
+        :type Total: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.CHDFSAccessInfos = None
+        self.Total = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("CHDFSAccessInfos") is not None:
+            self.CHDFSAccessInfos = []
+            for item in params.get("CHDFSAccessInfos"):
+                obj = CHDFSAccessInfo()
+                obj._deserialize(item)
+                self.CHDFSAccessInfos.append(obj)
+        self.Total = params.get("Total")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeCHDFSMountPointAssociateInfosRequest(AbstractModel):
     """DescribeCHDFSMountPointAssociateInfos请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8375,14 +10647,59 @@
                 obj = MountPointAssociateInfo()
                 obj._deserialize(item)
                 self.AssociateInfos.append(obj)
         self.TotalElements = params.get("TotalElements")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeCHDFSMountPointSuperuserRequest(AbstractModel):
+    """DescribeCHDFSMountPointSuperuser请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BucketId: 桶id
+        :type BucketId: str
+        """
+        self.BucketId = None
+
+
+    def _deserialize(self, params):
+        self.BucketId = params.get("BucketId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeCHDFSMountPointSuperuserResponse(AbstractModel):
+    """DescribeCHDFSMountPointSuperuser返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Superusers: Superuser列表
+        :type Superusers: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Superusers = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Superusers = params.get("Superusers")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeCHDFSMountPointsRequest(AbstractModel):
     """DescribeCHDFSMountPoints请求参数结构体
 
     """
 
 
 class DescribeCHDFSMountPointsResponse(AbstractModel):
@@ -8407,14 +10724,48 @@
             for item in params.get("MountPoints"):
                 obj = MountPoint()
                 obj._deserialize(item)
                 self.MountPoints.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeCHDFSProductsRequest(AbstractModel):
+    """DescribeCHDFSProducts请求参数结构体
+
+    """
+
+
+class DescribeCHDFSProductsResponse(AbstractModel):
+    """元数据加速桶产品列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CHDFSProductInfos: 产品列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CHDFSProductInfos: list of CHDFSProductInfo
+        :param Total: 列表数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        """
+        self.CHDFSProductInfos = None
+        self.Total = None
+
+
+    def _deserialize(self, params):
+        if params.get("CHDFSProductInfos") is not None:
+            self.CHDFSProductInfos = []
+            for item in params.get("CHDFSProductInfos"):
+                obj = CHDFSProductInfo()
+                obj._deserialize(item)
+                self.CHDFSProductInfos.append(obj)
+        self.Total = params.get("Total")
+
+
 class DescribeColumnsRequest(AbstractModel):
     """DescribeColumns请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8505,14 +10856,68 @@
                 obj._deserialize(item)
                 self.Columns.append(obj)
         self.TotalElements = params.get("TotalElements")
         self.TotalPages = params.get("TotalPages")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDLCCHDFSBindingListRequest(AbstractModel):
+    """DescribeDLCCHDFSBindingList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BucketId: 桶名
+        :type BucketId: str
+        """
+        self.BucketId = None
+
+
+    def _deserialize(self, params):
+        self.BucketId = params.get("BucketId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDLCCHDFSBindingListResponse(AbstractModel):
+    """DescribeDLCCHDFSBindingList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DLCCHDFSBindingList: dlc引擎绑定桶列表
+        :type DLCCHDFSBindingList: list of DLCCHDFSBinding
+        :param Total: 列表数
+        :type Total: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DLCCHDFSBindingList = None
+        self.Total = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("DLCCHDFSBindingList") is not None:
+            self.DLCCHDFSBindingList = []
+            for item in params.get("DLCCHDFSBindingList"):
+                obj = DLCCHDFSBinding()
+                obj._deserialize(item)
+                self.DLCCHDFSBindingList.append(obj)
+        self.Total = params.get("Total")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDMSDatabaseRequest(AbstractModel):
     """DescribeDMSDatabase请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9171,14 +11576,150 @@
         self.Page = params.get("Page")
         self.Size = params.get("Size")
         self.TotalPages = params.get("TotalPages")
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDataEngineImageOperateRecordsRequest(AbstractModel):
+    """DescribeDataEngineImageOperateRecords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RecordId: 日志记录唯一id
+        :type RecordId: str
+        :param DataEngineId: 引擎唯一id
+        :type DataEngineId: str
+        :param ImageVersionId: 集群镜像大版本唯一id
+        :type ImageVersionId: str
+        :param ChildImageVersionId: 集群镜像小版本唯一id
+        :type ChildImageVersionId: str
+        :param Operate: 操作类型：初始化：InitImage、变配ModifyResource、升级：UpgradeImage、切换：SwitchImage、回滚：RollbackImage
+        :type Operate: str
+        :param Sort: 排序字段：InsertTime(默认)
+        :type Sort: str
+        :param Asc: 排序字段：true(默认)、false
+        :type Asc: bool
+        :param Limit: 分页字段：10（默认），传-1查全部
+        :type Limit: int
+        :param Offset: 分页字段
+        :type Offset: int
+        """
+        self.RecordId = None
+        self.DataEngineId = None
+        self.ImageVersionId = None
+        self.ChildImageVersionId = None
+        self.Operate = None
+        self.Sort = None
+        self.Asc = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        self.RecordId = params.get("RecordId")
+        self.DataEngineId = params.get("DataEngineId")
+        self.ImageVersionId = params.get("ImageVersionId")
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        self.Operate = params.get("Operate")
+        self.Sort = params.get("Sort")
+        self.Asc = params.get("Asc")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDataEngineImageOperateRecordsResponse(AbstractModel):
+    """DescribeDataEngineImageOperateRecords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ImageOperateRecords: 镜像操作日志记录列表
+        :type ImageOperateRecords: list of ImageOperateRecord
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ImageOperateRecords = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("ImageOperateRecords") is not None:
+            self.ImageOperateRecords = []
+            for item in params.get("ImageOperateRecords"):
+                obj = ImageOperateRecord()
+                obj._deserialize(item)
+                self.ImageOperateRecords.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeDataEngineImageVersionsRequest(AbstractModel):
+    """DescribeDataEngineImageVersions请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EngineType: 引擎类型：SQL、SparkBatch
+        :type EngineType: str
+        """
+        self.EngineType = None
+
+
+    def _deserialize(self, params):
+        self.EngineType = params.get("EngineType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDataEngineImageVersionsResponse(AbstractModel):
+    """DescribeDataEngineImageVersions返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ImageParentVersions: 集群大版本镜像信息列表
+        :type ImageParentVersions: list of DataEngineImageVersion
+        :param Total: 总数
+        :type Total: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ImageParentVersions = None
+        self.Total = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("ImageParentVersions") is not None:
+            self.ImageParentVersions = []
+            for item in params.get("ImageParentVersions"):
+                obj = DataEngineImageVersion()
+                obj._deserialize(item)
+                self.ImageParentVersions.append(obj)
+        self.Total = params.get("Total")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDataEngineParametersRequest(AbstractModel):
     """DescribeDataEngineParameters请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9229,14 +11770,64 @@
             for item in params.get("EngineParameters"):
                 obj = EngineParameter()
                 obj._deserialize(item)
                 self.EngineParameters.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDataEnginePythonSparkImagesRequest(AbstractModel):
+    """DescribeDataEnginePythonSparkImages请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ChildImageVersionId: 集群镜像小版本ID
+        :type ChildImageVersionId: str
+        """
+        self.ChildImageVersionId = None
+
+
+    def _deserialize(self, params):
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDataEnginePythonSparkImagesResponse(AbstractModel):
+    """DescribeDataEnginePythonSparkImages返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PythonSparkImages: PYSPARK镜像信息列表
+        :type PythonSparkImages: list of PythonSparkImage
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.PythonSparkImages = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("PythonSparkImages") is not None:
+            self.PythonSparkImages = []
+            for item in params.get("PythonSparkImages"):
+                obj = PythonSparkImage()
+                obj._deserialize(item)
+                self.PythonSparkImages.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDataEngineRequest(AbstractModel):
     """DescribeDataEngine请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9276,44 +11867,92 @@
     def _deserialize(self, params):
         if params.get("DataEngine") is not None:
             self.DataEngine = DataEngineInfo()
             self.DataEngine._deserialize(params.get("DataEngine"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDataEngineSessionParametersRequest(AbstractModel):
+    """DescribeDataEngineSessionParameters请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎id
+        :type DataEngineId: str
+        :param DataEngineName: 引擎名称，当指定引擎名称后优先使用名称获取配置
+        :type DataEngineName: str
+        """
+        self.DataEngineId = None
+        self.DataEngineName = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        self.DataEngineName = params.get("DataEngineName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDataEngineSessionParametersResponse(AbstractModel):
+    """DescribeDataEngineSessionParameters返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineParameters: 集群Session配置列表
+        :type DataEngineParameters: list of DataEngineImageSessionParameter
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DataEngineParameters = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("DataEngineParameters") is not None:
+            self.DataEngineParameters = []
+            for item in params.get("DataEngineParameters"):
+                obj = DataEngineImageSessionParameter()
+                obj._deserialize(item)
+                self.DataEngineParameters.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDataEnginesRequest(AbstractModel):
     """DescribeDataEngines请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Offset: 偏移量，默认为0。
         :type Offset: int
-        :param Filters: 滤类型，传参Name应为以下其中一个,
-data-engine-name - String 
-engine-type - String
-state - String 
-mode - String 
-create-time - String 
-message - String
+        :param Filters: 过滤类型，支持如下的过滤类型，传参Name应为以下其中一个, data-engine-name - String（数据引擎名称）：engine-type - String（引擎类型：spark：spark 引擎，presto：presto引擎），state - String (数据引擎状态 -2已删除 -1失败 0初始化中 1挂起 2运行中 3准备删除 4删除中) ， mode - String（计费模式 0共享模式 1按量计费 2包年包月） ， create-time - String（创建时间，10位时间戳） message - String （描述信息），cluster-type - String (集群资源类型 spark_private/presto_private/presto_cu/spark_cu)，engine-id - String（数据引擎ID），key-word - String（数据引擎名称或集群资源类型或描述信息模糊搜索），engine-exec-type - String（引擎执行任务类型，SQL/BATCH）
         :type Filters: list of Filter
         :param SortBy: 排序字段，支持如下字段类型，create-time
         :type SortBy: str
         :param Sorting: 排序方式，desc表示正序，asc表示反序， 默认为asc。
         :type Sorting: str
         :param Limit: 返回数量，默认为10，最大值为100。
         :type Limit: int
         :param DatasourceConnectionName: 已废弃，请使用DatasourceConnectionNameSet
         :type DatasourceConnectionName: str
         :param ExcludePublicEngine: 是否不返回共享引擎，true不返回共享引擎，false可以返回共享引擎
         :type ExcludePublicEngine: bool
         :param AccessTypes: 参数应该为引擎权限类型，有效类型："USE", "MODIFY", "OPERATE", "MONITOR", "DELETE"
         :type AccessTypes: list of str
-        :param EngineExecType: 引擎执行任务类型，有效值：SQL/BATCH
+        :param EngineExecType: 引擎执行任务类型，有效值：SQL/BATCH，默认为SQL
         :type EngineExecType: str
         :param EngineType: 引擎类型，有效值：spark/presto
         :type EngineType: str
         :param DatasourceConnectionNameSet: 网络配置列表，若传入该参数，则返回网络配置关联的计算引擎
         :type DatasourceConnectionNameSet: list of str
         """
         self.Offset = None
@@ -9506,14 +12145,59 @@
             for item in params.get("Queries"):
                 obj = DataQuery()
                 obj._deserialize(item)
                 self.Queries.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDataTaskAlarmFiledRequest(AbstractModel):
+    """DescribeDataTaskAlarmFiled请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataTaskId: 数据任务ID
+        :type DataTaskId: str
+        """
+        self.DataTaskId = None
+
+
+    def _deserialize(self, params):
+        self.DataTaskId = params.get("DataTaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDataTaskAlarmFiledResponse(AbstractModel):
+    """DescribeDataTaskAlarmFiled返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskName: 任务名称
+        :type TaskName: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskName = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskName = params.get("TaskName")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDatabaseRequest(AbstractModel):
     """DescribeDatabase请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9656,15 +12340,15 @@
         :type Limit: int
         :param Offset: 数据偏移量，从0开始，默认为0。
         :type Offset: int
         :param KeyWord: 模糊匹配，库名关键字。
         :type KeyWord: str
         :param DatasourceConnectionName: 数据源唯名称，该名称可以通过DescribeDatasourceConnection接口查询到。默认为DataLakeCatalog
         :type DatasourceConnectionName: str
-        :param Sort: 排序字段，当前版本仅支持按库名排序
+        :param Sort: 排序字段，CreateTime：创建时间，Name：数据库名称
         :type Sort: str
         :param Asc: 排序类型：false：降序（默认）、true：升序
         :type Asc: bool
         """
         self.Limit = None
         self.Offset = None
         self.KeyWord = None
@@ -9861,14 +12545,67 @@
             for item in params.get("DefaultEngineConfigs"):
                 obj = DefaultEngineConfig()
                 obj._deserialize(item)
                 self.DefaultEngineConfigs.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeEngineUsageInfoRequest(AbstractModel):
+    """DescribeEngineUsageInfo请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 数据引擎ID
+        :type DataEngineId: str
+        """
+        self.DataEngineId = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeEngineUsageInfoResponse(AbstractModel):
+    """DescribeEngineUsageInfo返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 集群总规格
+        :type Total: int
+        :param Used: 已占用集群规格
+        :type Used: int
+        :param Available: 剩余集群规格
+        :type Available: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Used = None
+        self.Available = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        self.Used = params.get("Used")
+        self.Available = params.get("Available")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeExportResultTasksRequest(AbstractModel):
     """DescribeExportResultTasks请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10071,14 +12808,68 @@
                 obj = ScheduleTaskInfo()
                 obj._deserialize(item)
                 self.ScheduleTasks.append(obj)
         self.TotalElements = params.get("TotalElements")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeForbiddenTableProRequest(AbstractModel):
+    """DescribeForbiddenTablePro请求参数结构体
+
+    """
+
+
+class DescribeForbiddenTableProResponse(AbstractModel):
+    """DescribeForbiddenTablePro返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ForbiddenTableProperties: 被禁用的表属性列表，该列表的属性不可进行增删改操作
+        :type ForbiddenTableProperties: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ForbiddenTableProperties = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.ForbiddenTableProperties = params.get("ForbiddenTableProperties")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeForbiddenTablePropertiesRequest(AbstractModel):
+    """DescribeForbiddenTableProperties请求参数结构体
+
+    """
+
+
+class DescribeForbiddenTablePropertiesResponse(AbstractModel):
+    """DescribeForbiddenTableProperties返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ForbiddenTableProperties: 被禁用的表属性列表，该列表的属性不可进行增删改操作
+        :type ForbiddenTableProperties: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ForbiddenTableProperties = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.ForbiddenTableProperties = params.get("ForbiddenTableProperties")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeFunctionsRequest(AbstractModel):
     """DescribeFunctions请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10139,14 +12930,145 @@
             for item in params.get("Rows"):
                 obj = FunctionSimpleData()
                 obj._deserialize(item)
                 self.Rows.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeGovernDefaultPolicyRequest(AbstractModel):
+    """DescribeGovernDefaultPolicy请求参数结构体
+
+    """
+
+
+class DescribeGovernDefaultPolicyResponse(AbstractModel):
+    """DescribeGovernDefaultPolicy返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Threshold: 数据值里规则默认值
+        :type Threshold: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Threshold = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Threshold") is not None:
+            self.Threshold = DataGovernPolicy()
+            self.Threshold._deserialize(params.get("Threshold"))
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeGovernEventRuleRequest(AbstractModel):
+    """DescribeGovernEventRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 数据治理事件阈值名称
+        :type Name: str
+        """
+        self.Name = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeGovernEventRuleResponse(AbstractModel):
+    """DescribeGovernEventRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RuleThreshold: 用户的数据治理事件阈值
+        :type RuleThreshold: :class:`tencentcloud.dlc.v20210125.models.TenantGovernEventRules`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RuleThreshold = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("RuleThreshold") is not None:
+            self.RuleThreshold = TenantGovernEventRules()
+            self.RuleThreshold._deserialize(params.get("RuleThreshold"))
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeGovernMetaInfoRequest(AbstractModel):
+    """DescribeGovernMetaInfo请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Catalog: 数据目录名称
+        :type Catalog: str
+        :param Database: 数据库名称
+        :type Database: str
+        :param Table: 数据表名称
+        :type Table: str
+        """
+        self.Catalog = None
+        self.Database = None
+        self.Table = None
+
+
+    def _deserialize(self, params):
+        self.Catalog = params.get("Catalog")
+        self.Database = params.get("Database")
+        self.Table = params.get("Table")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeGovernMetaInfoResponse(AbstractModel):
+    """DescribeGovernMetaInfo返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GovernMeta: 数据治理元信息
+        :type GovernMeta: :class:`tencentcloud.dlc.v20210125.models.GovernMetaInfo`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.GovernMeta = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("GovernMeta") is not None:
+            self.GovernMeta = GovernMetaInfo()
+            self.GovernMeta._deserialize(params.get("GovernMeta"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeHouseEventsRequest(AbstractModel):
     """DescribeHouseEvents请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10386,14 +13308,98 @@
 
     def _deserialize(self, params):
         self.Names = params.get("Names")
         self.Total = params.get("Total")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLakeFsDirSummaryRequest(AbstractModel):
+    """DescribeLakeFsDirSummary请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 托管存储名称
+        :type Name: str
+        :param Path: 目录全路径
+        :type Path: str
+        """
+        self.Name = None
+        self.Path = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Path = params.get("Path")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLakeFsDirSummaryResponse(AbstractModel):
+    """DescribeLakeFsDirSummary返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Summary: Summary统计信息
+        :type Summary: :class:`tencentcloud.dlc.v20210125.models.LakeFsSummary`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Summary = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Summary") is not None:
+            self.Summary = LakeFsSummary()
+            self.Summary._deserialize(params.get("Summary"))
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeLakeFsInfoRequest(AbstractModel):
+    """DescribeLakeFsInfo请求参数结构体
+
+    """
+
+
+class DescribeLakeFsInfoResponse(AbstractModel):
+    """DescribeLakeFsInfo返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LakeFsInfos: 托管存储信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LakeFsInfos: list of LakeFsInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.LakeFsInfos = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("LakeFsInfos") is not None:
+            self.LakeFsInfos = []
+            for item in params.get("LakeFsInfos"):
+                obj = LakeFsInfo()
+                obj._deserialize(item)
+                self.LakeFsInfos.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeLakeFsPathRequest(AbstractModel):
     """DescribeLakeFsPath请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10433,14 +13439,66 @@
     def _deserialize(self, params):
         if params.get("AccessToken") is not None:
             self.AccessToken = LakeFileSystemToken()
             self.AccessToken._deserialize(params.get("AccessToken"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLakeFsWarehouseAccessRequest(AbstractModel):
+    """DescribeLakeFsWarehouseAccess请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 托管存储名称
+        :type Name: str
+        :param Mode: 访问模式
+        :type Mode: int
+        """
+        self.Name = None
+        self.Mode = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Mode = params.get("Mode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLakeFsWarehouseAccessResponse(AbstractModel):
+    """DescribeLakeFsWarehouseAccess返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AccessToken: 访问token
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AccessToken: :class:`tencentcloud.dlc.v20210125.models.LakeFileSystemToken`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.AccessToken = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("AccessToken") is not None:
+            self.AccessToken = LakeFileSystemToken()
+            self.AccessToken._deserialize(params.get("AccessToken"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeMainDataDataEngineRequest(AbstractModel):
     """DescribeMainDataDataEngine请求参数结构体
 
     """
 
 
 class DescribeMainDataDataEngineResponse(AbstractModel):
@@ -10947,20 +14005,20 @@
 class DescribeMetaTablesRequest(AbstractModel):
     """DescribeMetaTables请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DatabaseName: 列出该数据库下所属数据表。
-        :type DatabaseName: str
         :param Limit: 返回数量，默认为10，最大值为100。
         :type Limit: int
         :param Offset: 数据偏移量，从0开始，默认为0。
         :type Offset: int
+        :param DatabaseName: 列出该数据库下所属数据表。
+        :type DatabaseName: str
         :param Filters: 过滤条件，如下支持的过滤类型，传参Name应为其一
 table-name - String - （过滤条件）数据表名称,形如：table-001。
 table-id - String - （过滤条件）table id形如：12342。
         :type Filters: list of Filter
         :param DatasourceConnectionName: 指定查询的数据源名称，默认为DataLakeCatalog
         :type DatasourceConnectionName: str
         :param StartTime: 起始时间：用于对更新时间的筛选
@@ -10970,30 +14028,30 @@
         :param Sort: 排序字段，支持：ModifiedTime（默认）；CreateTime
         :type Sort: str
         :param Asc: 排序字段，false：降序（默认）；true
         :type Asc: bool
         :param TableType: table type，表类型查询,可用值:EXTERNAL_TABLE,INDEX_TABLE,MANAGED_TABLE,MATERIALIZED_VIEW,TABLE,VIEW,VIRTUAL_VIEW
         :type TableType: str
         """
-        self.DatabaseName = None
         self.Limit = None
         self.Offset = None
+        self.DatabaseName = None
         self.Filters = None
         self.DatasourceConnectionName = None
         self.StartTime = None
         self.EndTime = None
         self.Sort = None
         self.Asc = None
         self.TableType = None
 
 
     def _deserialize(self, params):
-        self.DatabaseName = params.get("DatabaseName")
         self.Limit = params.get("Limit")
         self.Offset = params.get("Offset")
+        self.DatabaseName = params.get("DatabaseName")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
         self.DatasourceConnectionName = params.get("DatasourceConnectionName")
@@ -11288,22 +14346,26 @@
 
     def __init__(self):
         r"""
         :param SessionId: Session唯一标识
         :type SessionId: str
         :param StatementId: Session Statement唯一标识
         :type StatementId: str
+        :param TaskId: 任务唯一标识
+        :type TaskId: str
         """
         self.SessionId = None
         self.StatementId = None
+        self.TaskId = None
 
 
     def _deserialize(self, params):
         self.SessionId = params.get("SessionId")
         self.StatementId = params.get("StatementId")
+        self.TaskId = params.get("TaskId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -11328,14 +14390,141 @@
     def _deserialize(self, params):
         if params.get("NotebookSessionStatement") is not None:
             self.NotebookSessionStatement = NotebookSessionStatementInfo()
             self.NotebookSessionStatement._deserialize(params.get("NotebookSessionStatement"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeNotebookSessionStatementSqlResultRequest(AbstractModel):
+    """DescribeNotebookSessionStatementSqlResult请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务唯一ID
+        :type TaskId: str
+        :param MaxResults: 返回结果的最大行数，范围0~1000，默认为1000.
+        :type MaxResults: int
+        :param NextToken: 上一次请求响应返回的分页信息。第一次可以不带，从头开始返回数据，每次返回MaxResults字段设置的数据量。
+        :type NextToken: str
+        """
+        self.TaskId = None
+        self.MaxResults = None
+        self.NextToken = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.MaxResults = params.get("MaxResults")
+        self.NextToken = params.get("NextToken")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeNotebookSessionStatementSqlResultResponse(AbstractModel):
+    """DescribeNotebookSessionStatementSqlResult返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务Id
+        :type TaskId: str
+        :param ResultSet: 结果数据
+        :type ResultSet: str
+        :param ResultSchema: schema
+        :type ResultSchema: list of Column
+        :param NextToken: 分页信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NextToken: str
+        :param OutputPath: 存储结果地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputPath: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.ResultSet = None
+        self.ResultSchema = None
+        self.NextToken = None
+        self.OutputPath = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.ResultSet = params.get("ResultSet")
+        if params.get("ResultSchema") is not None:
+            self.ResultSchema = []
+            for item in params.get("ResultSchema"):
+                obj = Column()
+                obj._deserialize(item)
+                self.ResultSchema.append(obj)
+        self.NextToken = params.get("NextToken")
+        self.OutputPath = params.get("OutputPath")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeNotebookSessionStatementsRequest(AbstractModel):
+    """DescribeNotebookSessionStatements请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SessionId: Session唯一标识
+        :type SessionId: str
+        :param BatchId: 批任务id
+        :type BatchId: str
+        """
+        self.SessionId = None
+        self.BatchId = None
+
+
+    def _deserialize(self, params):
+        self.SessionId = params.get("SessionId")
+        self.BatchId = params.get("BatchId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeNotebookSessionStatementsResponse(AbstractModel):
+    """DescribeNotebookSessionStatements返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NotebookSessionStatements: Session Statement详情
+        :type NotebookSessionStatements: :class:`tencentcloud.dlc.v20210125.models.NotebookSessionStatementBatchInformation`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.NotebookSessionStatements = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("NotebookSessionStatements") is not None:
+            self.NotebookSessionStatements = NotebookSessionStatementBatchInformation()
+            self.NotebookSessionStatements._deserialize(params.get("NotebookSessionStatements"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeNotebookSessionsRequest(AbstractModel):
     """DescribeNotebookSessions请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11343,17 +14532,17 @@
         :type DataEngineName: str
         :param State: Session状态，包含：not_started（未启动）、starting（已启动）、idle（等待输入）、busy(正在运行statement)、shutting_down（停止）、error（异常）、dead（已退出）、killed（被杀死）、success（正常停止）
         :type State: list of str
         :param SortFields: 排序字段（默认按创建时间）
         :type SortFields: list of str
         :param Asc: 排序字段：true：升序、false：降序（默认）
         :type Asc: bool
-        :param Limit: 分页字段
+        :param Limit: 分页参数，默认10
         :type Limit: int
-        :param Offset: 分页字段
+        :param Offset: 分页参数，默认0
         :type Offset: int
         """
         self.DataEngineName = None
         self.State = None
         self.SortFields = None
         self.Asc = None
         self.Limit = None
@@ -11469,14 +14658,68 @@
             for item in params.get("AssociateInfos"):
                 obj = MountPointAssociateInfo()
                 obj._deserialize(item)
                 self.AssociateInfos.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeOtherCHDFSBindingListRequest(AbstractModel):
+    """DescribeOtherCHDFSBindingList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BucketId: 桶名
+        :type BucketId: str
+        """
+        self.BucketId = None
+
+
+    def _deserialize(self, params):
+        self.BucketId = params.get("BucketId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOtherCHDFSBindingListResponse(AbstractModel):
+    """DescribeOtherCHDFSBindingList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param OtherCHDFSBindingList: 非DLC 产品绑定列表
+        :type OtherCHDFSBindingList: list of OtherCHDFSBinding
+        :param Total: 总记录数
+        :type Total: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.OtherCHDFSBindingList = None
+        self.Total = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("OtherCHDFSBindingList") is not None:
+            self.OtherCHDFSBindingList = []
+            for item in params.get("OtherCHDFSBindingList"):
+                obj = OtherCHDFSBinding()
+                obj._deserialize(item)
+                self.OtherCHDFSBindingList.append(obj)
+        self.Total = params.get("Total")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeQueryDirRequest(AbstractModel):
     """DescribeQueryDir请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11642,20 +14885,37 @@
 
     """
 
     def __init__(self):
         r"""
         :param DataPath: SQL查询结果存放的路径，目前只支持托管的查询结果导出，即Path是lakefs协议的路径
         :type DataPath: str
+        :param TaskId: SQL 任务id
+        :type TaskId: str
+        :param Format: 格式类型 csv/ excel
+        :type Format: str
+        :param Options: 格式化参数
+        :type Options: list of KVPair
         """
         self.DataPath = None
+        self.TaskId = None
+        self.Format = None
+        self.Options = None
 
 
     def _deserialize(self, params):
         self.DataPath = params.get("DataPath")
+        self.TaskId = params.get("TaskId")
+        self.Format = params.get("Format")
+        if params.get("Options") is not None:
+            self.Options = []
+            for item in params.get("Options"):
+                obj = KVPair()
+                obj._deserialize(item)
+                self.Options.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -11666,25 +14926,105 @@
 
     """
 
     def __init__(self):
         r"""
         :param Fs: 托管存储对象
         :type Fs: :class:`tencentcloud.dlc.v20210125.models.LakeFileSystem`
+        :param Status: 状态  init | queue | format |  compress | success | error |timeout
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param Reason: 原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Reason: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Fs = None
+        self.Status = None
+        self.Reason = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Fs") is not None:
             self.Fs = LakeFileSystem()
             self.Fs._deserialize(params.get("Fs"))
+        self.Status = params.get("Status")
+        self.Reason = params.get("Reason")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeResultDownloadRequest(AbstractModel):
+    """DescribeResultDownload请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DownloadId: 查询任务Id
+        :type DownloadId: str
+        """
+        self.DownloadId = None
+
+
+    def _deserialize(self, params):
+        self.DownloadId = params.get("DownloadId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeResultDownloadResponse(AbstractModel):
+    """DescribeResultDownload返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Path: 下载文件路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Path: str
+        :param Status: 任务状态 init | queue | format | compress | success|  timeout | error
+        :type Status: str
+        :param Reason: 任务异常原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Reason: str
+        :param SecretId: 临时SecretId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SecretId: str
+        :param SecretKey: 临时SecretKey
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SecretKey: str
+        :param Token: 临时Token
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Token: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Path = None
+        self.Status = None
+        self.Reason = None
+        self.SecretId = None
+        self.SecretKey = None
+        self.Token = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Path = params.get("Path")
+        self.Status = params.get("Status")
+        self.Reason = params.get("Reason")
+        self.SecretId = params.get("SecretId")
+        self.SecretKey = params.get("SecretKey")
+        self.Token = params.get("Token")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeResultSizeRequest(AbstractModel):
     """DescribeResultSize请求参数结构体
 
     """
@@ -12336,15 +15676,15 @@
 class DescribeSparkAppJobRequest(AbstractModel):
     """DescribeSparkAppJob请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param JobId: spark作业Id，与JobName同时存在时，JobName无效
+        :param JobId: spark作业Id，与JobName同时存在时，JobName无效，JobId与JobName至少存在一个
         :type JobId: str
         :param JobName: spark作业名
         :type JobName: str
         """
         self.JobId = None
         self.JobName = None
 
@@ -12449,23 +15789,23 @@
 
     def __init__(self):
         r"""
         :param SortBy: 返回结果按照该字段排序
         :type SortBy: str
         :param Sorting: 正序或者倒序，例如：desc
         :type Sorting: str
-        :param Filters: 按照该参数过滤,支持spark-job-name
+        :param Filters: 过滤条件，如下支持的过滤类型，传参Name应为其一:spark-job-name（作业名称），spark-job-id（作业id），spark-app-type（作业类型，1：批任务，2：流任务，4：SQL作业），user-name（创建人），key-word（作业名称或ID关键词模糊搜索）
         :type Filters: list of Filter
-        :param StartTime: 更新时间起始点
+        :param StartTime: 更新时间起始点，支持格式：yyyy-MM-dd HH:mm:ss
         :type StartTime: str
-        :param EndTime: 更新时间截止点
+        :param EndTime: 更新时间截止点，支持格式：yyyy-MM-dd HH:mm:ss
         :type EndTime: str
-        :param Offset: 查询列表偏移量
+        :param Offset: 查询列表偏移量, 默认值0
         :type Offset: int
-        :param Limit: 查询列表限制数量
+        :param Limit: 查询列表限制数量, 默认值100
         :type Limit: int
         """
         self.SortBy = None
         self.Sorting = None
         self.Filters = None
         self.StartTime = None
         self.EndTime = None
@@ -12536,17 +15876,17 @@
         :type JobId: str
         :param Offset: 分页查询偏移量
         :type Offset: int
         :param Limit: 分页查询Limit
         :type Limit: int
         :param TaskId: 执行实例id
         :type TaskId: str
-        :param StartTime: 更新时间起始点
+        :param StartTime: 更新时间起始点，支持格式：yyyy-MM-dd HH:mm:ss
         :type StartTime: str
-        :param EndTime: 更新时间截止点
+        :param EndTime: 更新时间截止点，支持格式：yyyy-MM-dd HH:mm:ss
         :type EndTime: str
         :param Filters: 按照该参数过滤,支持task-state
         :type Filters: list of Filter
         """
         self.JobId = None
         self.Offset = None
         self.Limit = None
@@ -12612,14 +15952,163 @@
             for item in params.get("SparkAppTasks"):
                 obj = TaskResponseInfo()
                 obj._deserialize(item)
                 self.SparkAppTasks.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeSparkSessionBatchSqlLogRequest(AbstractModel):
+    """DescribeSparkSessionBatchSqlLog请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: SparkSQL唯一标识
+        :type BatchId: str
+        """
+        self.BatchId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeSparkSessionBatchSqlLogResponse(AbstractModel):
+    """DescribeSparkSessionBatchSqlLog返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param State: 状态：0：初始化、1：成功、2：失败、3：取消、4：异常；
+        :type State: int
+        :param LogSet: 日志信息列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogSet: list of SparkSessionBatchLog
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.State = None
+        self.LogSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.State = params.get("State")
+        if params.get("LogSet") is not None:
+            self.LogSet = []
+            for item in params.get("LogSet"):
+                obj = SparkSessionBatchLog()
+                obj._deserialize(item)
+                self.LogSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeSparkSessionBatchSqlTasksRequest(AbstractModel):
+    """DescribeSparkSessionBatchSqlTasks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filters: 过滤条件，如下支持的过滤类型，传参Name应为以下其中一个,其中task-id支持最大50个过滤个数，其他过滤参数支持的总数不超过5个。
+batch-id - String - （批任务ID准确过滤）batch-id取值形如：e386471f-139a-4e59-877f-50ece8135b99;
+session-id - String - (livy Session ID过滤)，如：livy-session-12321;
+task-state - String - （任务状态过滤）取值范围 0(初始化)， 1(运行中)， 2(成功)， -1(失败)、-3（已终止）;
+task-sql-keyword - String - （SQL语句关键字模糊过滤）取值形如：DROP TABLE;
+task-operator- string （子uin过滤）;
+task-kind - string （任务类型过滤）;
+        :type Filters: list of Filter
+        :param SortBy: 排序字段，支持如下字段类型，create-time（创建时间，默认）、update-time（更新时间）
+        :type SortBy: str
+        :param Sorting: 排序方式，desc表示正序，asc表示反序， 默认为asc。
+        :type Sorting: str
+        :param StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。默认为45天前的当前时刻
+        :type StartTime: str
+        :param EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS时间跨度在(0,30天]，支持最近45天数据查询。默认为当前时刻
+        :type EndTime: str
+        :param DataEngineName: 支持计算资源名字筛选
+        :type DataEngineName: str
+        :param Limit: 返回数量，默认为10，最大值为100。
+        :type Limit: int
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
+        """
+        self.Filters = None
+        self.SortBy = None
+        self.Sorting = None
+        self.StartTime = None
+        self.EndTime = None
+        self.DataEngineName = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.SortBy = params.get("SortBy")
+        self.Sorting = params.get("Sorting")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.DataEngineName = params.get("DataEngineName")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeSparkSessionBatchSqlTasksResponse(AbstractModel):
+    """DescribeSparkSessionBatchSqlTasks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SparkBatchSQLInformation: 批任务详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SparkBatchSQLInformation: list of SparkSessionBatchSQL
+        :param Total: 数量
+        :type Total: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.SparkBatchSQLInformation = None
+        self.Total = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("SparkBatchSQLInformation") is not None:
+            self.SparkBatchSQLInformation = []
+            for item in params.get("SparkBatchSQLInformation"):
+                obj = SparkSessionBatchSQL()
+                obj._deserialize(item)
+                self.SparkBatchSQLInformation.append(obj)
+        self.Total = params.get("Total")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeSparkTaskLogDownloadInfoRequest(AbstractModel):
     """DescribeSparkTaskLogDownloadInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12729,14 +16218,64 @@
 
     def _deserialize(self, params):
         self.SparkUiUrl = params.get("SparkUiUrl")
         self.TaskId = params.get("TaskId")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeStandbyDataEngineRequest(AbstractModel):
+    """DescribeStandbyDataEngine请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineName: 主集群名称
+        :type DataEngineName: str
+        """
+        self.DataEngineName = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineName = params.get("DataEngineName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeStandbyDataEngineResponse(AbstractModel):
+    """DescribeStandbyDataEngine返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SpareDataEngineList: 备集群详细信息
+        :type SpareDataEngineList: list of DataEngineInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.SpareDataEngineList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("SpareDataEngineList") is not None:
+            self.SpareDataEngineList = []
+            for item in params.get("SpareDataEngineList"):
+                obj = DataEngineInfo()
+                obj._deserialize(item)
+                self.SpareDataEngineList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeStoreLocationRequest(AbstractModel):
     """DescribeStoreLocation请求参数结构体
 
     """
 
 
 class DescribeStoreLocationResponse(AbstractModel):
@@ -13036,19 +16575,19 @@
         :type Offset: int
         :param Filters: 过滤条件，如下支持的过滤类型，传参Name应为其一
 table-name - String - （过滤条件）数据表名称,形如：table-001。
 table-id - String - （过滤条件）table id形如：12342。
         :type Filters: list of Filter
         :param DatasourceConnectionName: 指定查询的数据源名称，默认为DataLakeCatalog
         :type DatasourceConnectionName: str
-        :param StartTime: 起始时间：用于对更新时间的筛选
+        :param StartTime: 起始时间：用于对更新时间的筛选，格式为yyyy-mm-dd HH:MM:SS
         :type StartTime: str
-        :param EndTime: 终止时间：用于对更新时间的筛选
+        :param EndTime: 终止时间：用于对更新时间的筛选，格式为yyyy-mm-dd HH:MM:SS
         :type EndTime: str
-        :param Sort: 排序字段，支持：CreateTime、UpdateTime、StorageSize、RecordCount、Name（不传则默认按name升序）
+        :param Sort: 排序字段，支持：CreateTime（创建时间）、UpdateTime（更新时间）、StorageSize（存储空间）、RecordCount（行数）、Name（表名称）（不传则默认按name升序）
         :type Sort: str
         :param Asc: 排序字段，false：降序（默认）；true：升序
         :type Asc: bool
         :param TableType: table type，表类型查询,可用值:EXTERNAL_TABLE,INDEX_TABLE,MANAGED_TABLE,MATERIALIZED_VIEW,TABLE,VIEW,VIRTUAL_VIEW
         :type TableType: str
         :param TableFormat: 筛选字段-表格式：不传（默认）为查全部；LAKEFS：托管表；ICEBERG：非托管iceberg表；HIVE：非托管hive表；OTHER：非托管其它；
         :type TableFormat: str
@@ -13118,14 +16657,62 @@
                 obj = TableResponseInfo()
                 obj._deserialize(item)
                 self.TableList.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeTaskMetricsRequest(AbstractModel):
+    """DescribeTaskMetrics请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务Id
+        :type TaskId: str
+        """
+        self.TaskId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeTaskMetricsResponse(AbstractModel):
+    """DescribeTaskMetrics返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Metrics: 指标
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Metrics: :class:`tencentcloud.dlc.v20210125.models.TaskStatisticMetrics`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Metrics = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Metrics") is not None:
+            self.Metrics = TaskStatisticMetrics()
+            self.Metrics._deserialize(params.get("Metrics"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeTaskResultRequest(AbstractModel):
     """DescribeTaskResult请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -13185,22 +16772,35 @@
 
     def __init__(self):
         r"""
         :param StartTime: 开始时间
         :type StartTime: str
         :param EndTime: 结束时间
         :type EndTime: str
+        :param Filters: 筛选条件
+        :type Filters: list of Filter
+        :param DataEngineName: 引擎名
+        :type DataEngineName: str
         """
         self.StartTime = None
         self.EndTime = None
+        self.Filters = None
+        self.DataEngineName = None
 
 
     def _deserialize(self, params):
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.DataEngineName = params.get("DataEngineName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13251,15 +16851,15 @@
         :type SortBy: str
         :param Sorting: 排序方式，desc表示正序，asc表示反序， 默认为asc。
         :type Sorting: str
         :param StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。默认为45天前的当前时刻
         :type StartTime: str
         :param EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS时间跨度在(0,30天]，支持最近45天数据查询。默认为当前时刻
         :type EndTime: str
-        :param DataEngineName: 支持计算资源名字筛选
+        :param DataEngineName: 数据引擎名称，用于筛选
         :type DataEngineName: str
         :param Config: 配置信息，key-value数组，对外不可见。key1：AuthorityRole（鉴权角色，默认传SubUin，base64加密，仅在jdbc提交任务时使用）
         :type Config: list of KVPair
         :param NoNeedDataset: 是否不需要返回数据集，false:需要返回数据集，true:不需要返回数据集
         :type NoNeedDataset: bool
         """
         self.Limit = None
@@ -13337,24 +16937,156 @@
         self.TotalCount = params.get("TotalCount")
         if params.get("TasksOverview") is not None:
             self.TasksOverview = TasksOverview()
             self.TasksOverview._deserialize(params.get("TasksOverview"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeUpdatableDataEnginesRequest(AbstractModel):
+    """DescribeUpdatableDataEngines请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineConfigCommand: 引擎配置操作命令，UpdateSparkSQLLakefsPath 更新托管表路径，UpdateSparkSQLResultPath 更新结果桶路径
+        :type DataEngineConfigCommand: str
+        """
+        self.DataEngineConfigCommand = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineConfigCommand = params.get("DataEngineConfigCommand")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeUpdatableDataEnginesResponse(AbstractModel):
+    """DescribeUpdatableDataEngines返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineBasicInfos: 集群基础信息
+        :type DataEngineBasicInfos: list of DataEngineBasicInfo
+        :param TotalCount: 集群个数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DataEngineBasicInfos = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("DataEngineBasicInfos") is not None:
+            self.DataEngineBasicInfos = []
+            for item in params.get("DataEngineBasicInfos"):
+                obj = DataEngineBasicInfo()
+                obj._deserialize(item)
+                self.DataEngineBasicInfos.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeUserDataEngineConfigRequest(AbstractModel):
+    """DescribeUserDataEngineConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Sorting: 排序方式，desc表示正序，asc表示反序
+        :type Sorting: str
+        :param Limit: 返回数量，默认为10，最大值为100。
+        :type Limit: int
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
+        :param SortBy: 排序字段，支持如下字段类型，create-time
+        :type SortBy: str
+        :param Filters: 过滤条件，如下支持的过滤类型，传参Name应为以下其中一个,每种过滤参数支持的过滤值不超过5个。
+app-id - String - （appid过滤）
+engine-id - String - （引擎ID过滤）
+        :type Filters: list of Filter
+        """
+        self.Sorting = None
+        self.Limit = None
+        self.Offset = None
+        self.SortBy = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.Sorting = params.get("Sorting")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.SortBy = params.get("SortBy")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeUserDataEngineConfigResponse(AbstractModel):
+    """DescribeUserDataEngineConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineConfigInstanceInfos: 用户引擎自定义配置项列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataEngineConfigInstanceInfos: list of DataEngineConfigInstanceInfo
+        :param TotalCount: 配置项总数。
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DataEngineConfigInstanceInfos = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("DataEngineConfigInstanceInfos") is not None:
+            self.DataEngineConfigInstanceInfos = []
+            for item in params.get("DataEngineConfigInstanceInfos"):
+                obj = DataEngineConfigInstanceInfo()
+                obj._deserialize(item)
+                self.DataEngineConfigInstanceInfos.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeUserInfoRequest(AbstractModel):
     """DescribeUserInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param UserId: 用户Id
         :type UserId: str
-        :param Type: 查询的信息类型，Group：工作组 DataAuth：数据权限 EngineAuth:引擎权限
+        :param Type: 查询的信息类型，Group：工作组 DataAuth：数据权限 EngineAuth:引擎权限 RowFilter：行级别权限
         :type Type: str
         :param Filters: 查询的过滤条件。
 
 当Type为Group时，支持Key为workgroup-name的模糊搜索；
 
 当Type为DataAuth时，支持key：
 
@@ -14105,14 +17837,41 @@
             for item in params.get("WorkloadStats"):
                 obj = WorkloadStat()
                 obj._deserialize(item)
                 self.WorkloadStats.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeYuntiUserRequest(AbstractModel):
+    """DescribeYuntiUser请求参数结构体
+
+    """
+
+
+class DescribeYuntiUserResponse(AbstractModel):
+    """DescribeYuntiUser返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param YuntiUser: 用户是否是云梯账号
+        :type YuntiUser: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.YuntiUser = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.YuntiUser = params.get("YuntiUser")
+        self.RequestId = params.get("RequestId")
+
+
 class DetachUserPolicyRequest(AbstractModel):
     """DetachUserPolicy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -14769,14 +18528,58 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ExpiredSnapshotsInfo(AbstractModel):
+    """快照过期数据治理项信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ExpiredSnapshotsEnable: 是否启用快照过期治理项：enable、none
+        :type ExpiredSnapshotsEnable: str
+        :param Engine: 用于运行快照过期治理项的引擎名称
+        :type Engine: str
+        :param RetainLast: 需要保留的最近快照个数
+        :type RetainLast: int
+        :param BeforeDays: 过期指定天前的快照
+        :type BeforeDays: int
+        :param MaxConcurrentDeletes: 清理过期快照的并行数
+        :type MaxConcurrentDeletes: int
+        :param IntervalMin: 快照过期治理运行周期，单位为分钟
+        :type IntervalMin: int
+        """
+        self.ExpiredSnapshotsEnable = None
+        self.Engine = None
+        self.RetainLast = None
+        self.BeforeDays = None
+        self.MaxConcurrentDeletes = None
+        self.IntervalMin = None
+
+
+    def _deserialize(self, params):
+        self.ExpiredSnapshotsEnable = params.get("ExpiredSnapshotsEnable")
+        self.Engine = params.get("Engine")
+        self.RetainLast = params.get("RetainLast")
+        self.BeforeDays = params.get("BeforeDays")
+        self.MaxConcurrentDeletes = params.get("MaxConcurrentDeletes")
+        self.IntervalMin = params.get("IntervalMin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ExportResultRequest(AbstractModel):
     """ExportResult请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -15022,31 +18825,116 @@
         r"""
         :param Id: udf对应id
 注意：此字段可能返回 null，表示取不到有效值。
         :type Id: int
         :param FuncName: 函数名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type FuncName: str
+        :param Desc: 描述信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Desc: str
         """
         self.Id = None
         self.FuncName = None
+        self.Desc = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.FuncName = params.get("FuncName")
+        self.Desc = params.get("Desc")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class GenerateCreateMangedTableSqlRequest(AbstractModel):
+    """GenerateCreateMangedTableSql请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TableBaseInfo: 表基本信息
+        :type TableBaseInfo: :class:`tencentcloud.dlc.v20210125.models.TableBaseInfo`
+        :param Columns: 表字段信息
+        :type Columns: list of TColumn
+        :param Partitions: 表分区信息
+        :type Partitions: list of TPartition
+        :param Properties: 表属性信息
+        :type Properties: list of Property
+        :param UpsertKeys: V2 upsert表 upsert键
+        :type UpsertKeys: list of str
+        """
+        self.TableBaseInfo = None
+        self.Columns = None
+        self.Partitions = None
+        self.Properties = None
+        self.UpsertKeys = None
+
+
+    def _deserialize(self, params):
+        if params.get("TableBaseInfo") is not None:
+            self.TableBaseInfo = TableBaseInfo()
+            self.TableBaseInfo._deserialize(params.get("TableBaseInfo"))
+        if params.get("Columns") is not None:
+            self.Columns = []
+            for item in params.get("Columns"):
+                obj = TColumn()
+                obj._deserialize(item)
+                self.Columns.append(obj)
+        if params.get("Partitions") is not None:
+            self.Partitions = []
+            for item in params.get("Partitions"):
+                obj = TPartition()
+                obj._deserialize(item)
+                self.Partitions.append(obj)
+        if params.get("Properties") is not None:
+            self.Properties = []
+            for item in params.get("Properties"):
+                obj = Property()
+                obj._deserialize(item)
+                self.Properties.append(obj)
+        self.UpsertKeys = params.get("UpsertKeys")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GenerateCreateMangedTableSqlResponse(AbstractModel):
+    """GenerateCreateMangedTableSql返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Execution: 创建托管存储内表sql语句描述
+        :type Execution: :class:`tencentcloud.dlc.v20210125.models.Execution`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Execution = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Execution") is not None:
+            self.Execution = Execution()
+            self.Execution._deserialize(params.get("Execution"))
+        self.RequestId = params.get("RequestId")
+
+
 class GetWorkflowCanvasRequest(AbstractModel):
     """GetWorkflowCanvas请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -15133,14 +19021,56 @@
     def _deserialize(self, params):
         if params.get("WorkflowInfo") is not None:
             self.WorkflowInfo = WorkflowInfo()
             self.WorkflowInfo._deserialize(params.get("WorkflowInfo"))
         self.RequestId = params.get("RequestId")
 
 
+class GovernMetaInfo(AbstractModel):
+    """数据实例元信息数据结构
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Version: 数据表版本信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Version: int
+        :param UpsertEnable: 表是否支持Upsert操过
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpsertEnable: bool
+        :param InheritEnable: 表是否是继承库策略
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InheritEnable: bool
+        :param GovernPolicy: 表有效治理规则
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GovernPolicy: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
+        """
+        self.Version = None
+        self.UpsertEnable = None
+        self.InheritEnable = None
+        self.GovernPolicy = None
+
+
+    def _deserialize(self, params):
+        self.Version = params.get("Version")
+        self.UpsertEnable = params.get("UpsertEnable")
+        self.InheritEnable = params.get("InheritEnable")
+        if params.get("GovernPolicy") is not None:
+            self.GovernPolicy = DataGovernPolicy()
+            self.GovernPolicy._deserialize(params.get("GovernPolicy"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class HiveInfo(AbstractModel):
     """hive类型数据源的信息
 
     """
 
     def __init__(self):
         r"""
@@ -15252,14 +19182,78 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ImageOperateRecord(AbstractModel):
+    """集群镜像操作日志。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RecordId: 日志记录唯一id
+        :type RecordId: str
+        :param DataEngineId: 引擎唯一id
+        :type DataEngineId: str
+        :param ImageVersionId: 集群镜像大版本id
+        :type ImageVersionId: str
+        :param ImageVersion: 集群镜像大版本名称
+        :type ImageVersion: str
+        :param ChildImageVersionId: 集群镜像小版本id
+        :type ChildImageVersionId: str
+        :param Operate: 操作类型：初始化：InitImage、变配ModifyResource、升级： UpgradeImage、切换：SwitchImage、回滚：RollbackImage
+        :type Operate: str
+        :param EngineSize: 引擎规格
+        :type EngineSize: str
+        :param UserAppId: 用户appid
+        :type UserAppId: int
+        :param UserAlias: 用户昵称
+        :type UserAlias: str
+        :param UserUin: 用户Uin
+        :type UserUin: str
+        :param InsertTime: 创建时间
+        :type InsertTime: str
+        """
+        self.RecordId = None
+        self.DataEngineId = None
+        self.ImageVersionId = None
+        self.ImageVersion = None
+        self.ChildImageVersionId = None
+        self.Operate = None
+        self.EngineSize = None
+        self.UserAppId = None
+        self.UserAlias = None
+        self.UserUin = None
+        self.InsertTime = None
+
+
+    def _deserialize(self, params):
+        self.RecordId = params.get("RecordId")
+        self.DataEngineId = params.get("DataEngineId")
+        self.ImageVersionId = params.get("ImageVersionId")
+        self.ImageVersion = params.get("ImageVersion")
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        self.Operate = params.get("Operate")
+        self.EngineSize = params.get("EngineSize")
+        self.UserAppId = params.get("UserAppId")
+        self.UserAlias = params.get("UserAlias")
+        self.UserUin = params.get("UserUin")
+        self.InsertTime = params.get("InsertTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class InferInternalTableSchemaRequest(AbstractModel):
     """InferInternalTableSchema请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -15374,30 +19368,34 @@
         :type MaxClusters: int
         :param PayMode: 计费模式。0：按量计费；1：包年包月计费
         :type PayMode: int
         :param TimeSpan: 计费时长。按量计费下固定为1；包年包月计费下表示购买的月份
         :type TimeSpan: int
         :param TimeUnit: 计费时长单位。按量计费下固定为h；包年包月计费下固定为m
         :type TimeUnit: str
+        :param ResourceType: 资源类型。Standard_CU：标准型，Memory_CU：内存型。
+        :type ResourceType: str
         """
         self.Size = None
         self.MinClusters = None
         self.MaxClusters = None
         self.PayMode = None
         self.TimeSpan = None
         self.TimeUnit = None
+        self.ResourceType = None
 
 
     def _deserialize(self, params):
         self.Size = params.get("Size")
         self.MinClusters = params.get("MinClusters")
         self.MaxClusters = params.get("MaxClusters")
         self.PayMode = params.get("PayMode")
         self.TimeSpan = params.get("TimeSpan")
         self.TimeUnit = params.get("TimeUnit")
+        self.ResourceType = params.get("ResourceType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -15449,30 +19447,34 @@
         :type MaxClusters: int
         :param PayMode: 计费模式。0：按量计费；1：包年包月计费
         :type PayMode: int
         :param TimeSpan: 计费时长。按量计费下固定为3600；包年包月计费下表示购买的月份
         :type TimeSpan: int
         :param TimeUnit: 计费时长单位。按量计费下固定为s；包年包月计费下固定为m
         :type TimeUnit: str
+        :param ResourceType: 资源类型，Standard_CU：标准型；Memory_CU：内存型。
+        :type ResourceType: str
         """
         self.Size = None
         self.MinClusters = None
         self.MaxClusters = None
         self.PayMode = None
         self.TimeSpan = None
         self.TimeUnit = None
+        self.ResourceType = None
 
 
     def _deserialize(self, params):
         self.Size = params.get("Size")
         self.MinClusters = params.get("MinClusters")
         self.MaxClusters = params.get("MaxClusters")
         self.PayMode = params.get("PayMode")
         self.TimeSpan = params.get("TimeSpan")
         self.TimeUnit = params.get("TimeUnit")
+        self.ResourceType = params.get("ResourceType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -15677,26 +19679,31 @@
         :type TopicId: str
         :param TopicName: 日志topic name
 注意：此字段可能返回 null，表示取不到有效值。
         :type TopicName: str
         :param LogJson: 日志内容，json字符串
 注意：此字段可能返回 null，表示取不到有效值。
         :type LogJson: str
+        :param PkgLogId: 日志ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PkgLogId: str
         """
         self.Time = None
         self.TopicId = None
         self.TopicName = None
         self.LogJson = None
+        self.PkgLogId = None
 
 
     def _deserialize(self, params):
         self.Time = params.get("Time")
         self.TopicId = params.get("TopicId")
         self.TopicName = params.get("TopicName")
         self.LogJson = params.get("LogJson")
+        self.PkgLogId = params.get("PkgLogId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -15959,14 +19966,86 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class LakeFsInfo(AbstractModel):
+    """描述DLC托管存储基本信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 托管存储名称
+        :type Name: str
+        :param Type: 托管存储类型
+        :type Type: str
+        :param SpaceUsedSize: 容量
+        :type SpaceUsedSize: float
+        :param CreateTimeStamp: 创建时候的时间戳
+        :type CreateTimeStamp: int
+        """
+        self.Name = None
+        self.Type = None
+        self.SpaceUsedSize = None
+        self.CreateTimeStamp = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Type = params.get("Type")
+        self.SpaceUsedSize = params.get("SpaceUsedSize")
+        self.CreateTimeStamp = params.get("CreateTimeStamp")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LakeFsSummary(AbstractModel):
+    """托管存储Summary统计信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Truncated: 是否是截断统计
+        :type Truncated: bool
+        :param TotalSubDirs: 子目录个数
+        :type TotalSubDirs: int
+        :param TotalFiles: 文件个数
+        :type TotalFiles: int
+        :param TotalBytes: 总文件大小字节数
+        :type TotalBytes: int
+        """
+        self.Truncated = None
+        self.TotalSubDirs = None
+        self.TotalFiles = None
+        self.TotalBytes = None
+
+
+    def _deserialize(self, params):
+        self.Truncated = params.get("Truncated")
+        self.TotalSubDirs = params.get("TotalSubDirs")
+        self.TotalFiles = params.get("TotalFiles")
+        self.TotalBytes = params.get("TotalBytes")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Link(AbstractModel):
     """任务依赖关系
 
     """
 
     def __init__(self):
         r"""
@@ -16206,22 +20285,25 @@
         :type Limit: int
         :param Context: 下一次分页参数，第一次传空
         :type Context: str
         :param Asc: 最近1000条日志是否升序排列，true:升序排序，false:倒序，默认false，倒序排列
         :type Asc: bool
         :param Filters: 预览日志的通用过滤条件
         :type Filters: list of Filter
+        :param BatchId: SparkSQL任务唯一ID
+        :type BatchId: str
         """
         self.TaskId = None
         self.StartTime = None
         self.EndTime = None
         self.Limit = None
         self.Context = None
         self.Asc = None
         self.Filters = None
+        self.BatchId = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.Limit = params.get("Limit")
@@ -16229,14 +20311,15 @@
         self.Asc = params.get("Asc")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
+        self.BatchId = params.get("BatchId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16254,50 +20337,59 @@
         :type Context: str
         :param ListOver: 是否获取完结
 注意：此字段可能返回 null，表示取不到有效值。
         :type ListOver: bool
         :param Results: 日志详情
 注意：此字段可能返回 null，表示取不到有效值。
         :type Results: list of JobLogResult
+        :param LogUrl: 日志url
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogUrl: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Context = None
         self.ListOver = None
         self.Results = None
+        self.LogUrl = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Context = params.get("Context")
         self.ListOver = params.get("ListOver")
         if params.get("Results") is not None:
             self.Results = []
             for item in params.get("Results"):
                 obj = JobLogResult()
                 obj._deserialize(item)
                 self.Results.append(obj)
+        self.LogUrl = params.get("LogUrl")
         self.RequestId = params.get("RequestId")
 
 
 class ListTaskJobLogNameRequest(AbstractModel):
     """ListTaskJobLogName请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param TaskId: 查询的taskId
         :type TaskId: str
+        :param BatchId: SparkSQL批任务唯一ID
+        :type BatchId: str
         """
         self.TaskId = None
+        self.BatchId = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
+        self.BatchId = params.get("BatchId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16308,23 +20400,27 @@
 
     """
 
     def __init__(self):
         r"""
         :param Names: 日志名称列表
         :type Names: list of str
+        :param TopicId: 日志topic
+        :type TopicId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Names = None
+        self.TopicId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Names = params.get("Names")
+        self.TopicId = params.get("TopicId")
         self.RequestId = params.get("RequestId")
 
 
 class ListWorkflowRequest(AbstractModel):
     """ListWorkflow请求参数结构体
 
     """
@@ -16708,24 +20804,29 @@
         :type StorageAmount: str
         :param PrivateEngineCount: 独享数据引擎个数
 注意：此字段可能返回 null，表示取不到有效值。
         :type PrivateEngineCount: int
         :param YesterdayCuCount: 昨日CU时用量
 注意：此字段可能返回 null，表示取不到有效值。
         :type YesterdayCuCount: float
+        :param LakeFsStorageAmount: 托管存储用量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LakeFsStorageAmount: str
         """
         self.StorageAmount = None
         self.PrivateEngineCount = None
         self.YesterdayCuCount = None
+        self.LakeFsStorageAmount = None
 
 
     def _deserialize(self, params):
         self.StorageAmount = params.get("StorageAmount")
         self.PrivateEngineCount = params.get("PrivateEngineCount")
         self.YesterdayCuCount = params.get("YesterdayCuCount")
+        self.LakeFsStorageAmount = params.get("LakeFsStorageAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16757,14 +20858,46 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class MergeManifestsInfo(AbstractModel):
+    """合并元数据Manifests文件数据治理项信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MergeManifestsEnable: 是否启用合并元数据Manifests文件治理项：enable、none
+        :type MergeManifestsEnable: str
+        :param Engine: 用于运行合并元数据Manifests文件治理项的引擎名称
+        :type Engine: str
+        :param IntervalMin: 合并元数据Manifests文件治理运行周期，单位为分钟
+        :type IntervalMin: int
+        """
+        self.MergeManifestsEnable = None
+        self.Engine = None
+        self.IntervalMin = None
+
+
+    def _deserialize(self, params):
+        self.MergeManifestsEnable = params.get("MergeManifestsEnable")
+        self.Engine = params.get("Engine")
+        self.IntervalMin = params.get("IntervalMin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class MetaDatabaseInfo(AbstractModel):
     """元数据库基本信息
 
     """
 
     def __init__(self):
         r"""
@@ -17031,14 +21164,113 @@
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
+class ModifyCHDFSMountPointSuperuserRequest(AbstractModel):
+    """ModifyCHDFSMountPointSuperuser请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BucketId: 桶id
+        :type BucketId: str
+        :param Superuser: superuser列表
+        :type Superuser: list of str
+        """
+        self.BucketId = None
+        self.Superuser = None
+
+
+    def _deserialize(self, params):
+        self.BucketId = params.get("BucketId")
+        self.Superuser = params.get("Superuser")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyCHDFSMountPointSuperuserResponse(AbstractModel):
+    """ModifyCHDFSMountPointSuperuser返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class ModifyCHDFSProductRequest(AbstractModel):
+    """ModifyCHDFSProduct请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductName: 产品名称
+        :type ProductName: str
+        :param SuperUser: 超级用户名称数组
+        :type SuperUser: list of str
+        :param VpcInfo: vpc配置信息数组
+        :type VpcInfo: list of CHDFSProductVpcInfo
+        """
+        self.ProductName = None
+        self.SuperUser = None
+        self.VpcInfo = None
+
+
+    def _deserialize(self, params):
+        self.ProductName = params.get("ProductName")
+        self.SuperUser = params.get("SuperUser")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = CHDFSProductVpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyCHDFSProductResponse(AbstractModel):
+    """ModifyCHDFSProduct返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyDataEngineDescriptionRequest(AbstractModel):
     """ModifyDataEngineDescription请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -17097,44 +21329,44 @@
         :type PackageSource: int
         :param PackagePath: cos路径
         :type PackagePath: str
         :param PackageName: jar包名称
         :type PackageName: str
         :param MainClass: 主类
         :type MainClass: str
-        :param DataEngineName: udf对应的spark计算资源
-        :type DataEngineName: str
         :param Id: 主键id
         :type Id: int
         :param Description: 描述
         :type Description: str
+        :param DataEngineName: udf对应的spark计算资源
+        :type DataEngineName: str
         """
         self.DatabaseName = None
         self.Name = None
         self.StoreType = None
         self.PackageSource = None
         self.PackagePath = None
         self.PackageName = None
         self.MainClass = None
-        self.DataEngineName = None
         self.Id = None
         self.Description = None
+        self.DataEngineName = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.Name = params.get("Name")
         self.StoreType = params.get("StoreType")
         self.PackageSource = params.get("PackageSource")
         self.PackagePath = params.get("PackagePath")
         self.PackageName = params.get("PackageName")
         self.MainClass = params.get("MainClass")
-        self.DataEngineName = params.get("DataEngineName")
         self.Id = params.get("Id")
         self.Description = params.get("Description")
+        self.DataEngineName = params.get("DataEngineName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -17218,35 +21450,88 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyGovernEventRuleRequest(AbstractModel):
+    """ModifyGovernEventRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 数据治理事件阈值名称
+        :type Name: str
+        :param Rule: 数据治理事件阈值
+        :type Rule: :class:`tencentcloud.dlc.v20210125.models.RuleThreshold`
+        """
+        self.Name = None
+        self.Rule = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        if params.get("Rule") is not None:
+            self.Rule = RuleThreshold()
+            self.Rule._deserialize(params.get("Rule"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyGovernEventRuleResponse(AbstractModel):
+    """ModifyGovernEventRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyMetaDatabaseRequest(AbstractModel):
     """ModifyMetaDatabase请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param MetaDatabaseInfo: 元数据库基本信息
         :type MetaDatabaseInfo: :class:`tencentcloud.dlc.v20210125.models.MetaDatabaseInfo`
         :param DatasourceConnectionName: 数据源名称，默认DataLakeCatalog
         :type DatasourceConnectionName: str
+        :param GovernPolicy: 数据治理配置项
+        :type GovernPolicy: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
         """
         self.MetaDatabaseInfo = None
         self.DatasourceConnectionName = None
+        self.GovernPolicy = None
 
 
     def _deserialize(self, params):
         if params.get("MetaDatabaseInfo") is not None:
             self.MetaDatabaseInfo = MetaDatabaseInfo()
             self.MetaDatabaseInfo._deserialize(params.get("MetaDatabaseInfo"))
         self.DatasourceConnectionName = params.get("DatasourceConnectionName")
+        if params.get("GovernPolicy") is not None:
+            self.GovernPolicy = DataGovernPolicy()
+            self.GovernPolicy._deserialize(params.get("GovernPolicy"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -17288,26 +21573,39 @@
         :type OldPath: str
         :param NewPath: 支持路径移动，存移动之后的路径
         :type NewPath: str
         :param Type: 节点类型：0：目录，1：会话
         :type Type: str
         :param Operator: 操作用户
         :type Operator: str
+        :param UserVisibility: 授权的子用户，空为自己和管理员可见
+        :type UserVisibility: str
+        :param PurviewInfoSet: 权限信息
+        :type PurviewInfoSet: list of PurviewInfo
         """
         self.OldPath = None
         self.NewPath = None
         self.Type = None
         self.Operator = None
+        self.UserVisibility = None
+        self.PurviewInfoSet = None
 
 
     def _deserialize(self, params):
         self.OldPath = params.get("OldPath")
         self.NewPath = params.get("NewPath")
         self.Type = params.get("Type")
         self.Operator = params.get("Operator")
+        self.UserVisibility = params.get("UserVisibility")
+        if params.get("PurviewInfoSet") is not None:
+            self.PurviewInfoSet = []
+            for item in params.get("PurviewInfoSet"):
+                obj = PurviewInfo()
+                obj._deserialize(item)
+                self.PurviewInfoSet.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -17492,71 +21790,144 @@
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
+class ModifySparkAppBatchRequest(AbstractModel):
+    """ModifySparkAppBatch请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SparkAppId: 需要批量修改的Spark作业任务ID列表
+        :type SparkAppId: list of str
+        :param DataEngine: 引擎ID
+        :type DataEngine: str
+        :param AppDriverSize: driver规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+        :type AppDriverSize: str
+        :param AppExecutorSize: executor规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+        :type AppExecutorSize: str
+        :param AppExecutorNums: 指定executor数量，最小值为1，最大值小于集群规格
+        :type AppExecutorNums: int
+        :param AppExecutorMaxNumbers: 指定executor max数量（动态配置场景下），最小值为1，最大值小于集群规格（当ExecutorMaxNumbers小于ExecutorNums时，改值设定为ExecutorNums）
+        :type AppExecutorMaxNumbers: int
+        :param IsInherit: 任务资源配置是否继承集群模板，0（默认）不继承，1：继承
+        :type IsInherit: int
+        """
+        self.SparkAppId = None
+        self.DataEngine = None
+        self.AppDriverSize = None
+        self.AppExecutorSize = None
+        self.AppExecutorNums = None
+        self.AppExecutorMaxNumbers = None
+        self.IsInherit = None
+
+
+    def _deserialize(self, params):
+        self.SparkAppId = params.get("SparkAppId")
+        self.DataEngine = params.get("DataEngine")
+        self.AppDriverSize = params.get("AppDriverSize")
+        self.AppExecutorSize = params.get("AppExecutorSize")
+        self.AppExecutorNums = params.get("AppExecutorNums")
+        self.AppExecutorMaxNumbers = params.get("AppExecutorMaxNumbers")
+        self.IsInherit = params.get("IsInherit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifySparkAppBatchResponse(AbstractModel):
+    """ModifySparkAppBatch返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifySparkAppRequest(AbstractModel):
     """ModifySparkApp请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AppName: spark应用名
+        :param AppName: spark作业名
         :type AppName: str
-        :param AppType: 1代表spark jar应用，2代表spark streaming应用
+        :param AppType: spark作业类型，1代表spark jar作业，2代表spark streaming作业
         :type AppType: int
-        :param DataEngine: 执行spark作业的数据引擎
+        :param DataEngine: 执行spark作业的数据引擎名称
         :type DataEngine: str
-        :param AppFile: spark应用的执行入口
+        :param AppFile: spark作业程序包文件路径
         :type AppFile: str
-        :param RoleArn: 执行spark作业的角色ID
+        :param RoleArn: 数据访问策略，CAM Role arn
         :type RoleArn: int
-        :param AppDriverSize: spark作业driver资源规格大小, 可取small,medium,large,xlarge
+        :param AppDriverSize: 指定的Driver规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppDriverSize: str
-        :param AppExecutorSize: spark作业executor资源规格大小, 可取small,medium,large,xlarge
+        :param AppExecutorSize: 指定的Executor规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppExecutorSize: str
         :param AppExecutorNums: spark作业executor个数
         :type AppExecutorNums: int
-        :param SparkAppId: spark应用Id
+        :param SparkAppId: spark作业Id
         :type SparkAppId: str
         :param Eni: 该字段已下线，请使用字段Datasource
         :type Eni: str
-        :param IsLocal: 是否本地上传，可取cos,lakefs
+        :param IsLocal: spark作业程序包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocal: str
-        :param MainClass: spark jar作业时的主类
+        :param MainClass: spark作业主类
         :type MainClass: str
         :param AppConf: spark配置，以换行符分隔
         :type AppConf: str
-        :param IsLocalJars: jar资源依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalJars: spark 作业依赖jar包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalJars: str
-        :param AppJars: spark jar作业依赖jars，以逗号分隔
+        :param AppJars: spark 作业依赖jar包（--jars），以逗号分隔
         :type AppJars: str
-        :param IsLocalFiles: file资源依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalFiles: spark作业依赖文件资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalFiles: str
-        :param AppFiles: spark作业依赖资源，以逗号分隔
+        :param AppFiles: spark作业依赖文件资源（--files）（非jar、zip），以逗号分隔
         :type AppFiles: str
-        :param IsLocalPythonFiles: pyspark：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalPythonFiles: pyspark：依赖上传方式，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalPythonFiles: str
-        :param AppPythonFiles: pyspark：python依赖, 除py文件外，还支持zip/egg等归档格式，多文件以逗号分隔
+        :param AppPythonFiles: pyspark作业依赖python资源（--py-files），支持py/zip/egg等归档格式，多文件以逗号分隔
         :type AppPythonFiles: str
-        :param CmdArgs: spark作业命令行参数
+        :param CmdArgs: spark作业程序入参
         :type CmdArgs: str
-        :param MaxRetries: 只对spark流任务生效
+        :param MaxRetries: 最大重试次数，只对spark流任务生效
         :type MaxRetries: int
         :param DataSource: 数据源名
         :type DataSource: str
-        :param IsLocalArchives: archives：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalArchives: spark作业依赖archives资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalArchives: str
-        :param AppArchives: archives：依赖资源
+        :param AppArchives: spark作业依赖archives资源（--archives），支持tar.gz/tgz/tar等归档格式，以逗号分隔
         :type AppArchives: str
-        :param SparkImage: Spark Image 版本
+        :param SparkImage: Spark Image 版本号
         :type SparkImage: str
+        :param SparkImageVersion: Spark Image 版本名称
+        :type SparkImageVersion: str
+        :param AppExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于AppExecutorNums
+        :type AppExecutorMaxNumbers: int
+        :param SessionId: 关联dlc查询脚本
+        :type SessionId: str
+        :param IsInherit: 任务资源配置是否继承集群配置模板：0（默认）不继承、1：继承
+        :type IsInherit: int
         """
         self.AppName = None
         self.AppType = None
         self.DataEngine = None
         self.AppFile = None
         self.RoleArn = None
         self.AppDriverSize = None
@@ -17575,14 +21946,18 @@
         self.AppPythonFiles = None
         self.CmdArgs = None
         self.MaxRetries = None
         self.DataSource = None
         self.IsLocalArchives = None
         self.AppArchives = None
         self.SparkImage = None
+        self.SparkImageVersion = None
+        self.AppExecutorMaxNumbers = None
+        self.SessionId = None
+        self.IsInherit = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.AppType = params.get("AppType")
         self.DataEngine = params.get("DataEngine")
         self.AppFile = params.get("AppFile")
@@ -17603,14 +21978,18 @@
         self.AppPythonFiles = params.get("AppPythonFiles")
         self.CmdArgs = params.get("CmdArgs")
         self.MaxRetries = params.get("MaxRetries")
         self.DataSource = params.get("DataSource")
         self.IsLocalArchives = params.get("IsLocalArchives")
         self.AppArchives = params.get("AppArchives")
         self.SparkImage = params.get("SparkImage")
+        self.SparkImageVersion = params.get("SparkImageVersion")
+        self.AppExecutorMaxNumbers = params.get("AppExecutorMaxNumbers")
+        self.SessionId = params.get("SessionId")
+        self.IsInherit = params.get("IsInherit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -17644,26 +22023,30 @@
         :type ImageId: str
         :param ImageTag: 镜像tag
         :type ImageTag: str
         :param Description: 镜像描述
         :type Description: str
         :param IsPublic: 是否为公共镜像：0：非公共；1：公共
         :type IsPublic: int
+        :param Operator: 操作者
+        :type Operator: str
         """
         self.ImageId = None
         self.ImageTag = None
         self.Description = None
         self.IsPublic = None
+        self.Operator = None
 
 
     def _deserialize(self, params):
         self.ImageId = params.get("ImageId")
         self.ImageTag = params.get("ImageTag")
         self.Description = params.get("Description")
         self.IsPublic = params.get("IsPublic")
+        self.Operator = params.get("Operator")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18236,14 +22619,17 @@
         :type CreateTime: str
         :param AppInfo: 其它信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppInfo: list of KVPair
         :param SparkUiUrl: Spark ui地址
 注意：此字段可能返回 null，表示取不到有效值。
         :type SparkUiUrl: str
+        :param ExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于ExecutorNumbers
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorMaxNumbers: int
         """
         self.Name = None
         self.Kind = None
         self.DataEngineName = None
         self.Arguments = None
         self.ProgramDependentFiles = None
         self.ProgramDependentJars = None
@@ -18256,14 +22642,15 @@
         self.TimeoutInSecond = None
         self.SparkAppId = None
         self.SessionId = None
         self.State = None
         self.CreateTime = None
         self.AppInfo = None
         self.SparkUiUrl = None
+        self.ExecutorMaxNumbers = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Kind = params.get("Kind")
         self.DataEngineName = params.get("DataEngineName")
         if params.get("Arguments") is not None:
@@ -18288,14 +22675,60 @@
         if params.get("AppInfo") is not None:
             self.AppInfo = []
             for item in params.get("AppInfo"):
                 obj = KVPair()
                 obj._deserialize(item)
                 self.AppInfo.append(obj)
         self.SparkUiUrl = params.get("SparkUiUrl")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class NotebookSessionStatementBatchInformation(AbstractModel):
+    """按批提交Statement运行SQL任务。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NotebookSessionStatementBatch: 任务详情列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NotebookSessionStatementBatch: list of NotebookSessionStatementInfo
+        :param IsAvailable: 当前批任务是否运行完成
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsAvailable: bool
+        :param SessionId: Session唯一标识
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionId: str
+        :param BatchId: Batch唯一标识
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BatchId: str
+        """
+        self.NotebookSessionStatementBatch = None
+        self.IsAvailable = None
+        self.SessionId = None
+        self.BatchId = None
+
+
+    def _deserialize(self, params):
+        if params.get("NotebookSessionStatementBatch") is not None:
+            self.NotebookSessionStatementBatch = []
+            for item in params.get("NotebookSessionStatementBatch"):
+                obj = NotebookSessionStatementInfo()
+                obj._deserialize(item)
+                self.NotebookSessionStatementBatch.append(obj)
+        self.IsAvailable = params.get("IsAvailable")
+        self.SessionId = params.get("SessionId")
+        self.BatchId = params.get("BatchId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18320,32 +22753,47 @@
         :param StatementId: Session Statement唯一标识
         :type StatementId: str
         :param State: Session Statement状态，包含：waiting（排队中）、running（运行中）、available（正常）、error（异常）、cancelling（取消中）、cancelled（已取消）
         :type State: str
         :param OutPut: Statement输出信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type OutPut: :class:`tencentcloud.dlc.v20210125.models.StatementOutput`
+        :param BatchId: 批任务id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BatchId: str
+        :param Code: 运行语句
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Code: str
+        :param TaskId: 任务ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskId: str
         """
         self.Completed = None
         self.Started = None
         self.Progress = None
         self.StatementId = None
         self.State = None
         self.OutPut = None
+        self.BatchId = None
+        self.Code = None
+        self.TaskId = None
 
 
     def _deserialize(self, params):
         self.Completed = params.get("Completed")
         self.Started = params.get("Started")
         self.Progress = params.get("Progress")
         self.StatementId = params.get("StatementId")
         self.State = params.get("State")
         if params.get("OutPut") is not None:
             self.OutPut = StatementOutput()
             self.OutPut._deserialize(params.get("OutPut"))
+        self.BatchId = params.get("BatchId")
+        self.Code = params.get("Code")
+        self.TaskId = params.get("TaskId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18467,14 +22915,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class OtherCHDFSBinding(AbstractModel):
+    """非DLC产品CHDFS绑定
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductName: 产品名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProductName: str
+        :param SuperUser: 用户名称（该字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SuperUser: list of str
+        :param VpcInfo: vpc配置信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcInfo: list of CHDFSProductVpcInfo
+        :param IsBind: 是否与该桶绑定（该字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsBind: bool
+        """
+        self.ProductName = None
+        self.SuperUser = None
+        self.VpcInfo = None
+        self.IsBind = None
+
+
+    def _deserialize(self, params):
+        self.ProductName = params.get("ProductName")
+        self.SuperUser = params.get("SuperUser")
+        if params.get("VpcInfo") is not None:
+            self.VpcInfo = []
+            for item in params.get("VpcInfo"):
+                obj = CHDFSProductVpcInfo()
+                obj._deserialize(item)
+                self.VpcInfo.append(obj)
+        self.IsBind = params.get("IsBind")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class OtherDatasourceConnection(AbstractModel):
     """其他数据源
 
     """
 
     def __init__(self):
         r"""
@@ -18618,14 +23111,17 @@
         :type CreateTime: str
         :param SourceId: 权限所属工作组的ID，只有当该权限的来源为工作组时才会有值。即仅当Source字段的值为WORKGROUP时该字段才有值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SourceId: int
         :param SourceName: 权限所属工作组的名称，只有当该权限的来源为工作组时才会有值。即仅当Source字段的值为WORKGROUP时该字段才有值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SourceName: str
+        :param Id: 策略ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: int
         """
         self.Database = None
         self.Catalog = None
         self.Table = None
         self.Operation = None
         self.PolicyType = None
         self.Function = None
@@ -18635,14 +23131,15 @@
         self.ReAuth = None
         self.Source = None
         self.Mode = None
         self.Operator = None
         self.CreateTime = None
         self.SourceId = None
         self.SourceName = None
+        self.Id = None
 
 
     def _deserialize(self, params):
         self.Database = params.get("Database")
         self.Catalog = params.get("Catalog")
         self.Table = params.get("Table")
         self.Operation = params.get("Operation")
@@ -18654,14 +23151,15 @@
         self.ReAuth = params.get("ReAuth")
         self.Source = params.get("Source")
         self.Mode = params.get("Mode")
         self.Operator = params.get("Operator")
         self.CreateTime = params.get("CreateTime")
         self.SourceId = params.get("SourceId")
         self.SourceName = params.get("SourceName")
+        self.Id = params.get("Id")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18698,14 +23196,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PrestoMonitorMetrics(AbstractModel):
+    """Presto监控指标
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LocalCacheHitRate: 	Alluxio本地缓存命中率
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalCacheHitRate: float
+        :param FragmentCacheHitRate: Fragment缓存命中率
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FragmentCacheHitRate: float
+        """
+        self.LocalCacheHitRate = None
+        self.FragmentCacheHitRate = None
+
+
+    def _deserialize(self, params):
+        self.LocalCacheHitRate = params.get("LocalCacheHitRate")
+        self.FragmentCacheHitRate = params.get("FragmentCacheHitRate")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Price(AbstractModel):
     """价格信息
 
     """
 
     def __init__(self):
         r"""
@@ -18775,14 +23303,143 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PurviewInfo(AbstractModel):
+    """查询脚本权限信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param WorkGroupSet: 用户组Id列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WorkGroupSet: list of int
+        :param UserSet: 用户id列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserSet: list of str
+        :param PurviewSet: 权限范围：1-读取 2-修改 3-删除
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PurviewSet: list of int
+        """
+        self.WorkGroupSet = None
+        self.UserSet = None
+        self.PurviewSet = None
+
+
+    def _deserialize(self, params):
+        self.WorkGroupSet = params.get("WorkGroupSet")
+        self.UserSet = params.get("UserSet")
+        self.PurviewSet = params.get("PurviewSet")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PythonSparkImage(AbstractModel):
+    """python-spark镜像信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SparkImageId: spark镜像唯一id
+        :type SparkImageId: str
+        :param ChildImageVersionId: 集群小版本镜像id
+        :type ChildImageVersionId: str
+        :param SparkImageVersion: spark镜像名称
+        :type SparkImageVersion: str
+        :param Description: spark镜像描述信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param CreateTime: 创建时间
+        :type CreateTime: str
+        :param UpdateTime: 更新时间
+        :type UpdateTime: str
+        """
+        self.SparkImageId = None
+        self.ChildImageVersionId = None
+        self.SparkImageVersion = None
+        self.Description = None
+        self.CreateTime = None
+        self.UpdateTime = None
+
+
+    def _deserialize(self, params):
+        self.SparkImageId = params.get("SparkImageId")
+        self.ChildImageVersionId = params.get("ChildImageVersionId")
+        self.SparkImageVersion = params.get("SparkImageVersion")
+        self.Description = params.get("Description")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class QueryInternalTableWarehouseRequest(AbstractModel):
+    """QueryInternalTableWarehouse请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DatabaseName: 库名
+        :type DatabaseName: str
+        :param TableName: 表名
+        :type TableName: str
+        """
+        self.DatabaseName = None
+        self.TableName = None
+
+
+    def _deserialize(self, params):
+        self.DatabaseName = params.get("DatabaseName")
+        self.TableName = params.get("TableName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class QueryInternalTableWarehouseResponse(AbstractModel):
+    """QueryInternalTableWarehouse返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param WarehousePath: warehouse路径
+        :type WarehousePath: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.WarehousePath = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.WarehousePath = params.get("WarehousePath")
+        self.RequestId = params.get("RequestId")
+
+
 class QueryResultRequest(AbstractModel):
     """QueryResult请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -19086,14 +23743,54 @@
     def _deserialize(self, params):
         if params.get("TaskInfo") is not None:
             self.TaskInfo = TaskResultInfo()
             self.TaskInfo._deserialize(params.get("TaskInfo"))
         self.RequestId = params.get("RequestId")
 
 
+class RemoveOrphanFilesInfo(AbstractModel):
+    """移除孤立文件数据治理项信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RemoveOrphanFilesEnable: 是否启用移除孤立文件治理项：enable、none
+        :type RemoveOrphanFilesEnable: str
+        :param Engine: 用于运行移除孤立文件治理项的引擎名称
+        :type Engine: str
+        :param BeforeDays: 移除指定天前的孤立文件
+        :type BeforeDays: int
+        :param MaxConcurrentDeletes: 移除孤立文件的并行数
+        :type MaxConcurrentDeletes: int
+        :param IntervalMin: 移除孤立文件治理运行周期，单位为分钟
+        :type IntervalMin: int
+        """
+        self.RemoveOrphanFilesEnable = None
+        self.Engine = None
+        self.BeforeDays = None
+        self.MaxConcurrentDeletes = None
+        self.IntervalMin = None
+
+
+    def _deserialize(self, params):
+        self.RemoveOrphanFilesEnable = params.get("RemoveOrphanFilesEnable")
+        self.Engine = params.get("Engine")
+        self.BeforeDays = params.get("BeforeDays")
+        self.MaxConcurrentDeletes = params.get("MaxConcurrentDeletes")
+        self.IntervalMin = params.get("IntervalMin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RemoveTaskRequest(AbstractModel):
     """RemoveTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -19346,14 +24043,59 @@
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
+class RestartDataEngineRequest(AbstractModel):
+    """RestartDataEngine请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎ID
+        :type DataEngineId: str
+        :param ForcedOperation: 是否强制重启，忽略任务
+        :type ForcedOperation: bool
+        """
+        self.DataEngineId = None
+        self.ForcedOperation = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        self.ForcedOperation = params.get("ForcedOperation")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RestartDataEngineResponse(AbstractModel):
+    """RestartDataEngine返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ResultExportResponseInfo(AbstractModel):
     """结果数据导出信息
 
     """
 
     def __init__(self):
         r"""
@@ -19397,14 +24139,139 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RewriteDataInfo(AbstractModel):
+    """数据重排布数据治理信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RewriteDataEnable: 是否启用数据重排布治理项：enable（启动）、disable（不启用，默认）
+        :type RewriteDataEnable: str
+        :param Engine: 用于运行数据重排布治理项的引擎名称
+        :type Engine: str
+        :param MinInputFiles: 重排布任务执行的文件个数
+        :type MinInputFiles: int
+        :param TargetFileSizeBytes: 数据重排布写后的数据文件大小，单位为字节
+        :type TargetFileSizeBytes: int
+        :param IntervalMin: 数据重排布治理运行周期，单位为分钟
+        :type IntervalMin: int
+        """
+        self.RewriteDataEnable = None
+        self.Engine = None
+        self.MinInputFiles = None
+        self.TargetFileSizeBytes = None
+        self.IntervalMin = None
+
+
+    def _deserialize(self, params):
+        self.RewriteDataEnable = params.get("RewriteDataEnable")
+        self.Engine = params.get("Engine")
+        self.MinInputFiles = params.get("MinInputFiles")
+        self.TargetFileSizeBytes = params.get("TargetFileSizeBytes")
+        self.IntervalMin = params.get("IntervalMin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RollbackDataEngineImageRequest(AbstractModel):
+    """RollbackDataEngineImage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎ID
+        :type DataEngineId: str
+        :param FromRecordId: 检查是否能回滚的接口返回的FromRecordId参数
+        :type FromRecordId: str
+        :param ToRecordId: 检查是否能回滚的接口返回的ToRecordId参数
+        :type ToRecordId: str
+        """
+        self.DataEngineId = None
+        self.FromRecordId = None
+        self.ToRecordId = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        self.FromRecordId = params.get("FromRecordId")
+        self.ToRecordId = params.get("ToRecordId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RollbackDataEngineImageResponse(AbstractModel):
+    """RollbackDataEngineImage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class RuleThreshold(AbstractModel):
+    """数据治理事件规则阈值定义
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AddDataFiles: 增加的文件数量阈值, 超过值将触发小文件合并
+        :type AddDataFiles: int
+        :param AddEqualityDeletes: 增加的Equality delete数量阈值, 超过值将触发小文件合并
+        :type AddEqualityDeletes: int
+        :param AddPositionDeletes: 增加的Position delete数量阈值, 超过值将触发小文件合并
+        :type AddPositionDeletes: int
+        :param AddDeleteFiles: 增加的delete file数量阈值，过期快照的AddDataFiles + AddDeleteFiles的总和大于阈值AddDataFiles + AddDeleteFiles将从该快照处删除快照
+        :type AddDeleteFiles: int
+        """
+        self.AddDataFiles = None
+        self.AddEqualityDeletes = None
+        self.AddPositionDeletes = None
+        self.AddDeleteFiles = None
+
+
+    def _deserialize(self, params):
+        self.AddDataFiles = params.get("AddDataFiles")
+        self.AddEqualityDeletes = params.get("AddEqualityDeletes")
+        self.AddPositionDeletes = params.get("AddPositionDeletes")
+        self.AddDeleteFiles = params.get("AddDeleteFiles")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RunScheduleTaskRequest(AbstractModel):
     """RunScheduleTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -19473,38 +24340,43 @@
         :type IsOpened: int
         :param Type: 节点类型：0：目录节点、1：会话节点
         :type Type: str
         :param Version: 版本号：更新时会迭代，用于做更新校验
         :type Version: int
         :param Path: 父节点目录信息
         :type Path: str
+        :param UserVisibility: 授权的子用户，空为自己和管理员可见
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserVisibility: str
         """
         self.Id = None
         self.Name = None
         self.Operator = None
         self.CreateTime = None
         self.UpdateTime = None
         self.LastUsed = None
         self.IsOpened = None
         self.Type = None
         self.Version = None
         self.Path = None
+        self.UserVisibility = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.Name = params.get("Name")
         self.Operator = params.get("Operator")
         self.CreateTime = params.get("CreateTime")
         self.UpdateTime = params.get("UpdateTime")
         self.LastUsed = params.get("LastUsed")
         self.IsOpened = params.get("IsOpened")
         self.Type = params.get("Type")
         self.Version = params.get("Version")
         self.Path = params.get("Path")
+        self.UserVisibility = params.get("UserVisibility")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -19604,14 +24476,20 @@
         :type Version: int
         :param Path: 会话路径
         :type Path: str
         :param IsMove: 是否移动目录：0（默认，不移动）、1（移动）
         :type IsMove: int
         :param ViewKey: 记录历史运行用户选择的可视化关键词，包含：BatchId、SessionSQL、ComputeEngine、ComputeResource、DataAmount、DataNumber、DeployStatus、SubmitTime
         :type ViewKey: list of str
+        :param UserVisibility: 授权的子用户，空为自己和管理员可见
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserVisibility: str
+        :param PurviewInfoSet: 权限组信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PurviewInfoSet: list of PurviewInfo
         """
         self.SessionName = None
         self.SessionResourceConfig = None
         self.Operator = None
         self.SessionId = None
         self.SessionSQL = None
         self.SessionSQLSelection = None
@@ -19621,14 +24499,16 @@
         self.LastUsed = None
         self.IsOpened = None
         self.Params = None
         self.Version = None
         self.Path = None
         self.IsMove = None
         self.ViewKey = None
+        self.UserVisibility = None
+        self.PurviewInfoSet = None
 
 
     def _deserialize(self, params):
         self.SessionName = params.get("SessionName")
         if params.get("SessionResourceConfig") is not None:
             self.SessionResourceConfig = SessionResourceConfig()
             self.SessionResourceConfig._deserialize(params.get("SessionResourceConfig"))
@@ -19647,14 +24527,21 @@
                 obj = Config()
                 obj._deserialize(item)
                 self.Params.append(obj)
         self.Version = params.get("Version")
         self.Path = params.get("Path")
         self.IsMove = params.get("IsMove")
         self.ViewKey = params.get("ViewKey")
+        self.UserVisibility = params.get("UserVisibility")
+        if params.get("PurviewInfoSet") is not None:
+            self.PurviewInfoSet = []
+            for item in params.get("PurviewInfoSet"):
+                obj = PurviewInfo()
+                obj._deserialize(item)
+                self.PurviewInfoSet.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -19704,14 +24591,16 @@
         :type DataNumber: int
         :param TotalTime: 任务总耗时：单位ms
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalTime: int
         :param UsedTime: 任务计算耗时：单位ms
 注意：此字段可能返回 null，表示取不到有效值。
         :type UsedTime: int
+        :param TotalNumber: 总的任务数
+        :type TotalNumber: int
         """
         self.SessionId = None
         self.BatchId = None
         self.TaskIdSet = None
         self.DeployStatus = None
         self.SuccessNumber = None
         self.FailNumber = None
@@ -19720,14 +24609,15 @@
         self.SessionSQL = None
         self.ComputeEngine = None
         self.ComputeResource = None
         self.DataAmount = None
         self.DataNumber = None
         self.TotalTime = None
         self.UsedTime = None
+        self.TotalNumber = None
 
 
     def _deserialize(self, params):
         self.SessionId = params.get("SessionId")
         self.BatchId = params.get("BatchId")
         self.TaskIdSet = params.get("TaskIdSet")
         self.DeployStatus = params.get("DeployStatus")
@@ -19738,14 +24628,15 @@
         self.SessionSQL = params.get("SessionSQL")
         self.ComputeEngine = params.get("ComputeEngine")
         self.ComputeResource = params.get("ComputeResource")
         self.DataAmount = params.get("DataAmount")
         self.DataNumber = params.get("DataNumber")
         self.TotalTime = params.get("TotalTime")
         self.UsedTime = params.get("UsedTime")
+        self.TotalNumber = params.get("TotalNumber")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -20080,14 +24971,29 @@
         :type ExecuteInfo: str
         :param KVPairs: 调度任务自定义参数，[{"Key":"abc","Value":"edf"}]
 注意：此字段可能返回 null，表示取不到有效值。
         :type KVPairs: list of KVPair
         :param WaitingTimeout: 任务等待调度超时时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type WaitingTimeout: int
+        :param RetryWait: 重试等待
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RetryWait: int
+        :param IsDelete: 是否被删除
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsDelete: int
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param UpdateTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param NonFinishedInstancesCount: 无
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NonFinishedInstancesCount: int
         """
         self.TaskId = None
         self.TaskName = None
         self.VirtualFlag = None
         self.LeftCoordinate = None
         self.TopCoordinate = None
         self.DataEngineName = None
@@ -20122,14 +25028,19 @@
         self.UserUin = None
         self.TaskType = None
         self.CreateUserUin = None
         self.CreateUserName = None
         self.ExecuteInfo = None
         self.KVPairs = None
         self.WaitingTimeout = None
+        self.RetryWait = None
+        self.IsDelete = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.NonFinishedInstancesCount = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.TaskName = params.get("TaskName")
         self.VirtualFlag = params.get("VirtualFlag")
         self.LeftCoordinate = params.get("LeftCoordinate")
@@ -20171,14 +25082,19 @@
         if params.get("KVPairs") is not None:
             self.KVPairs = []
             for item in params.get("KVPairs"):
                 obj = KVPair()
                 obj._deserialize(item)
                 self.KVPairs.append(obj)
         self.WaitingTimeout = params.get("WaitingTimeout")
+        self.RetryWait = params.get("RetryWait")
+        self.IsDelete = params.get("IsDelete")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.NonFinishedInstancesCount = params.get("NonFinishedInstancesCount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -20271,14 +25187,120 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SessionResourceTemplate(AbstractModel):
+    """Spark批作业集群Session资源配置模板；
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DriverSize: driver规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DriverSize: str
+        :param ExecutorSize: executor规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorSize: str
+        :param ExecutorNums: 指定executor数量，最小值为1，最大值小于集群规格
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorNums: int
+        :param ExecutorMaxNumbers: 指定executor max数量（动态配置场景下），最小值为1，最大值小于集群规格（当ExecutorMaxNumbers小于ExecutorNums时，改值设定为ExecutorNums）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorMaxNumbers: int
+        """
+        self.DriverSize = None
+        self.ExecutorSize = None
+        self.ExecutorNums = None
+        self.ExecutorMaxNumbers = None
+
+
+    def _deserialize(self, params):
+        self.DriverSize = params.get("DriverSize")
+        self.ExecutorSize = params.get("ExecutorSize")
+        self.ExecutorNums = params.get("ExecutorNums")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SetTablePropertiesRequest(AbstractModel):
+    """SetTableProperties请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DatasourceConnectionName: Catalog名称
+        :type DatasourceConnectionName: str
+        :param DatabaseName: 库名
+        :type DatabaseName: str
+        :param TableName: 表名
+        :type TableName: str
+        :param Properties: 属性列表
+        :type Properties: list of Property
+        """
+        self.DatasourceConnectionName = None
+        self.DatabaseName = None
+        self.TableName = None
+        self.Properties = None
+
+
+    def _deserialize(self, params):
+        self.DatasourceConnectionName = params.get("DatasourceConnectionName")
+        self.DatabaseName = params.get("DatabaseName")
+        self.TableName = params.get("TableName")
+        if params.get("Properties") is not None:
+            self.Properties = []
+            for item in params.get("Properties"):
+                obj = Property()
+                obj._deserialize(item)
+                self.Properties.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SetTablePropertiesResponse(AbstractModel):
+    """SetTableProperties返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务Id
+        :type BatchId: str
+        :param TaskIdSet: TaskId列表
+        :type TaskIdSet: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BatchId = None
+        self.TaskIdSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        self.TaskIdSet = params.get("TaskIdSet")
+        self.RequestId = params.get("RequestId")
+
+
 class SparkAppJobImage(AbstractModel):
     """Spark镜像返回值信息。
 
     """
 
     def __init__(self):
         r"""
@@ -20391,15 +25413,15 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class SparkJobInfo(AbstractModel):
-    """spark作业详情
+    """spark作业详情。
 
     """
 
     def __init__(self):
         r"""
         :param JobId: spark作业ID
         :type JobId: str
@@ -20475,14 +25497,32 @@
         :type JobPythonFiles: str
         :param TaskNum: 当前job正在运行或准备运行的任务个数
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskNum: int
         :param DataEngineStatus: 引擎状态：-100（默认：未知状态），-2~11：引擎正常状态；
 注意：此字段可能返回 null，表示取不到有效值。
         :type DataEngineStatus: int
+        :param JobExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于JobExecutorNums
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobExecutorMaxNumbers: int
+        :param SparkImageVersion: 镜像版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SparkImageVersion: str
+        :param SessionId: 查询脚本关联id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionId: str
+        :param DataEngineClusterType: spark_emr_livy
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataEngineClusterType: str
+        :param DataEngineImageVersion: Spark 3.2-EMR
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataEngineImageVersion: str
+        :param IsInherit: 任务资源配置是否继承集群模板，0（默认）不继承，1：继承
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsInherit: int
         """
         self.JobId = None
         self.JobName = None
         self.JobType = None
         self.DataEngine = None
         self.Eni = None
         self.IsLocal = None
@@ -20510,14 +25550,20 @@
         self.AppPythonFiles = None
         self.IsLocalArchives = None
         self.JobArchives = None
         self.SparkImage = None
         self.JobPythonFiles = None
         self.TaskNum = None
         self.DataEngineStatus = None
+        self.JobExecutorMaxNumbers = None
+        self.SparkImageVersion = None
+        self.SessionId = None
+        self.DataEngineClusterType = None
+        self.DataEngineImageVersion = None
+        self.IsInherit = None
 
 
     def _deserialize(self, params):
         self.JobId = params.get("JobId")
         self.JobName = params.get("JobName")
         self.JobType = params.get("JobType")
         self.DataEngine = params.get("DataEngine")
@@ -20549,14 +25595,20 @@
         self.AppPythonFiles = params.get("AppPythonFiles")
         self.IsLocalArchives = params.get("IsLocalArchives")
         self.JobArchives = params.get("JobArchives")
         self.SparkImage = params.get("SparkImage")
         self.JobPythonFiles = params.get("JobPythonFiles")
         self.TaskNum = params.get("TaskNum")
         self.DataEngineStatus = params.get("DataEngineStatus")
+        self.JobExecutorMaxNumbers = params.get("JobExecutorMaxNumbers")
+        self.SparkImageVersion = params.get("SparkImageVersion")
+        self.SessionId = params.get("SessionId")
+        self.DataEngineClusterType = params.get("DataEngineClusterType")
+        self.DataEngineImageVersion = params.get("DataEngineImageVersion")
+        self.IsInherit = params.get("IsInherit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -20617,14 +25669,228 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SparkMonitorMetrics(AbstractModel):
+    """Spark监控数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ShuffleWriteBytesCos: shuffle写溢出到COS数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ShuffleWriteBytesCos: int
+        :param ShuffleWriteBytesTotal: shuffle写数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ShuffleWriteBytesTotal: int
+        """
+        self.ShuffleWriteBytesCos = None
+        self.ShuffleWriteBytesTotal = None
+
+
+    def _deserialize(self, params):
+        self.ShuffleWriteBytesCos = params.get("ShuffleWriteBytesCos")
+        self.ShuffleWriteBytesTotal = params.get("ShuffleWriteBytesTotal")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SparkSessionBatchLog(AbstractModel):
+    """SparkSQL批任务运行日志
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Step: 日志步骤：BEG/CS/DS/DSS/DSF/FINF/RTO/CANCEL/CT/DT/DTS/DTF/FINT/EXCE
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Step: str
+        :param Time: 时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Time: str
+        :param Message: 日志提示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param Operate: 日志操作
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Operate: list of SparkSessionBatchLogOperate
+        """
+        self.Step = None
+        self.Time = None
+        self.Message = None
+        self.Operate = None
+
+
+    def _deserialize(self, params):
+        self.Step = params.get("Step")
+        self.Time = params.get("Time")
+        self.Message = params.get("Message")
+        if params.get("Operate") is not None:
+            self.Operate = []
+            for item in params.get("Operate"):
+                obj = SparkSessionBatchLogOperate()
+                obj._deserialize(item)
+                self.Operate.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SparkSessionBatchLogOperate(AbstractModel):
+    """SparkSQL批任务日志操作信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 操作提示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Text: str
+        :param Operate: 操作类型：COPY、LOG、UI、RESULT、List、TAB
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Operate: str
+        :param Supplement: 补充信息：如：taskid、sessionid、sparkui等
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Supplement: list of KVPair
+        """
+        self.Text = None
+        self.Operate = None
+        self.Supplement = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.Operate = params.get("Operate")
+        if params.get("Supplement") is not None:
+            self.Supplement = []
+            for item in params.get("Supplement"):
+                obj = KVPair()
+                obj._deserialize(item)
+                self.Supplement.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SparkSessionBatchSQL(AbstractModel):
+    """SparkSQL批任务详情。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务唯一标识
+        :type BatchId: str
+        :param SessionId: session唯一标识
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionId: str
+        :param Type: 任务类型：默认：SparkBatchSQL
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param ExecuteSQL: 运行sql
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecuteSQL: str
+        :param State: 任务运行状态：1：初始化、5：运行中、0：成功、-1：失败、-3：取消；-4：过期；
+注意：此字段可能返回 null，表示取不到有效值。
+        :type State: int
+        :param Creator: 创建人
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Creator: str
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param UpdateTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param UseTime: 任务运行时间：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UseTime: int
+        :param DataEngineId: 引擎ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataEngineId: str
+        :param DataEngineName: 引擎名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataEngineName: str
+        :param SparkUI: spark ui地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SparkUI: str
+        :param BatchLog: 任务日志列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BatchLog: list of SparkSessionBatchLog
+        :param ResourceUsage: 任务使用资源：如：10CU
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceUsage: int
+        :param ImageVersionName: 镜像版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageVersionName: str
+        """
+        self.BatchId = None
+        self.SessionId = None
+        self.Type = None
+        self.ExecuteSQL = None
+        self.State = None
+        self.Creator = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.UseTime = None
+        self.DataEngineId = None
+        self.DataEngineName = None
+        self.SparkUI = None
+        self.BatchLog = None
+        self.ResourceUsage = None
+        self.ImageVersionName = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        self.SessionId = params.get("SessionId")
+        self.Type = params.get("Type")
+        self.ExecuteSQL = params.get("ExecuteSQL")
+        self.State = params.get("State")
+        self.Creator = params.get("Creator")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.UseTime = params.get("UseTime")
+        self.DataEngineId = params.get("DataEngineId")
+        self.DataEngineName = params.get("DataEngineName")
+        self.SparkUI = params.get("SparkUI")
+        if params.get("BatchLog") is not None:
+            self.BatchLog = []
+            for item in params.get("BatchLog"):
+                obj = SparkSessionBatchLog()
+                obj._deserialize(item)
+                self.BatchLog.append(obj)
+        self.ResourceUsage = params.get("ResourceUsage")
+        self.ImageVersionName = params.get("ImageVersionName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class StatementOutput(AbstractModel):
     """notebook session statement输出信息。
 
     """
 
     def __init__(self):
         r"""
@@ -20642,35 +25908,40 @@
         :type ErrorName: str
         :param ErrorValue: 错误类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type ErrorValue: str
         :param ErrorMessage: 错误堆栈信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ErrorMessage: list of str
+        :param SQLResult: SQL类型任务结果返回
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SQLResult: str
         """
         self.ExecutionCount = None
         self.Data = None
         self.Status = None
         self.ErrorName = None
         self.ErrorValue = None
         self.ErrorMessage = None
+        self.SQLResult = None
 
 
     def _deserialize(self, params):
         self.ExecutionCount = params.get("ExecutionCount")
         if params.get("Data") is not None:
             self.Data = []
             for item in params.get("Data"):
                 obj = KVPair()
                 obj._deserialize(item)
                 self.Data.append(obj)
         self.Status = params.get("Status")
         self.ErrorName = params.get("ErrorName")
         self.ErrorValue = params.get("ErrorValue")
         self.ErrorMessage = params.get("ErrorMessage")
+        self.SQLResult = params.get("SQLResult")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -20942,14 +26213,104 @@
     def _deserialize(self, params):
         if params.get("House") is not None:
             self.House = DataEngineInfo()
             self.House._deserialize(params.get("House"))
         self.RequestId = params.get("RequestId")
 
 
+class SwitchDataEngineImageRequest(AbstractModel):
+    """SwitchDataEngineImage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎ID
+        :type DataEngineId: str
+        :param NewImageVersionId: 新镜像版本ID
+        :type NewImageVersionId: str
+        """
+        self.DataEngineId = None
+        self.NewImageVersionId = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        self.NewImageVersionId = params.get("NewImageVersionId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SwitchDataEngineImageResponse(AbstractModel):
+    """SwitchDataEngineImage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class SwitchDataEngineRequest(AbstractModel):
+    """SwitchDataEngine请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineName: 主集群名称
+        :type DataEngineName: str
+        :param StartStandbyCluster: 是否开启备集群
+        :type StartStandbyCluster: bool
+        """
+        self.DataEngineName = None
+        self.StartStandbyCluster = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineName = params.get("DataEngineName")
+        self.StartStandbyCluster = params.get("StartStandbyCluster")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SwitchDataEngineResponse(AbstractModel):
+    """SwitchDataEngine返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class TColumn(AbstractModel):
     """表字段描述信息
 
     """
 
     def __init__(self):
         r"""
@@ -20959,28 +26320,37 @@
         :type Type: str
         :param Comment: 字段描述
         :type Comment: str
         :param Default: 字段默认值
         :type Default: str
         :param NotNull: 字段是否是非空
         :type NotNull: bool
+        :param Precision: 表示整个 numeric 的长度,取值1-38
+        :type Precision: int
+        :param Scale: 表示小数部分的长度
+Scale小于Precision
+        :type Scale: int
         """
         self.Name = None
         self.Type = None
         self.Comment = None
         self.Default = None
         self.NotNull = None
+        self.Precision = None
+        self.Scale = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Type = params.get("Type")
         self.Comment = params.get("Comment")
         self.Default = params.get("Default")
         self.NotNull = params.get("NotNull")
+        self.Precision = params.get("Precision")
+        self.Scale = params.get("Scale")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -21063,34 +26433,46 @@
         :type TableFormat: str
         :param UserAlias: 建表用户昵称
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserAlias: str
         :param UserSubUin: 建表用户ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserSubUin: str
+        :param GovernPolicy: 数据治理配置项
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GovernPolicy: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
+        :param DbGovernPolicyIsDisable: 库数据治理是否关闭，关闭：true，开启：false
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DbGovernPolicyIsDisable: str
         """
         self.DatabaseName = None
         self.TableName = None
         self.DatasourceConnectionName = None
         self.TableComment = None
         self.Type = None
         self.TableFormat = None
         self.UserAlias = None
         self.UserSubUin = None
+        self.GovernPolicy = None
+        self.DbGovernPolicyIsDisable = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.TableName = params.get("TableName")
         self.DatasourceConnectionName = params.get("DatasourceConnectionName")
         self.TableComment = params.get("TableComment")
         self.Type = params.get("Type")
         self.TableFormat = params.get("TableFormat")
         self.UserAlias = params.get("UserAlias")
         self.UserSubUin = params.get("UserSubUin")
+        if params.get("GovernPolicy") is not None:
+            self.GovernPolicy = DataGovernPolicy()
+            self.GovernPolicy._deserialize(params.get("GovernPolicy"))
+        self.DbGovernPolicyIsDisable = params.get("DbGovernPolicyIsDisable")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -21182,25 +26564,45 @@
         :type InputFormat: str
         :param StorageSize: 数据表存储大小（单位：Byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type StorageSize: int
         :param RecordCount: 数据表行数
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecordCount: int
+        :param MapMaterializedViewName: xxxx
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MapMaterializedViewName: str
+        :param Comment: test
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Comment: str
+        :param ViewOriginalText: 创建视图原始文本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ViewOriginalText: str
+        :param ViewExpandedText: 创建视图展开文本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ViewExpandedText: str
+        :param Guid: 唯一标识
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Guid: str
         """
         self.TableBaseInfo = None
         self.Columns = None
         self.Partitions = None
         self.Location = None
         self.Properties = None
         self.ModifiedTime = None
         self.CreateTime = None
         self.InputFormat = None
         self.StorageSize = None
         self.RecordCount = None
+        self.MapMaterializedViewName = None
+        self.Comment = None
+        self.ViewOriginalText = None
+        self.ViewExpandedText = None
+        self.Guid = None
 
 
     def _deserialize(self, params):
         if params.get("TableBaseInfo") is not None:
             self.TableBaseInfo = TableBaseInfo()
             self.TableBaseInfo._deserialize(params.get("TableBaseInfo"))
         if params.get("Columns") is not None:
@@ -21223,14 +26625,19 @@
                 obj._deserialize(item)
                 self.Properties.append(obj)
         self.ModifiedTime = params.get("ModifiedTime")
         self.CreateTime = params.get("CreateTime")
         self.InputFormat = params.get("InputFormat")
         self.StorageSize = params.get("StorageSize")
         self.RecordCount = params.get("RecordCount")
+        self.MapMaterializedViewName = params.get("MapMaterializedViewName")
+        self.Comment = params.get("Comment")
+        self.ViewOriginalText = params.get("ViewOriginalText")
+        self.ViewExpandedText = params.get("ViewExpandedText")
+        self.Guid = params.get("Guid")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -21424,14 +26831,50 @@
         :type UiUrl: str
         :param TotalTime: 任务耗时，单位： ms
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalTime: int
         :param CmdArgs: spark app job执行task的程序入口参数
 注意：此字段可能返回 null，表示取不到有效值。
         :type CmdArgs: str
+        :param ImageVersion: 集群镜像大版本名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageVersion: str
+        :param StreamingStat: streaming任务统计信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StreamingStat: :class:`tencentcloud.dlc.v20210125.models.StreamingStatistics`
+        :param ResourceUsage: 任务预设资源大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceUsage: int
+        :param OutputConf: 输出配置信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputConf: str
+        :param TaskKind: 任务类别
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskKind: str
+        :param DriverSize: driver规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DriverSize: str
+        :param ExecutorSize: executor规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorSize: str
+        :param ExecutorNums: 指定executor数量，最小值为1，最大值小于集群规格
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorNums: int
+        :param ExecutorMaxNumbers: 指定executor max数量（动态配置场景下），最小值为1，最大值小于集群规格（当ExecutorMaxNumbers小于ExecutorNums时，改值设定为ExecutorNums）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorMaxNumbers: int
+        :param CommonMetrics: 任务公共指标数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CommonMetrics: :class:`tencentcloud.dlc.v20210125.models.CommonMetrics`
+        :param SparkMonitorMetrics: spark任务指标数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SparkMonitorMetrics: :class:`tencentcloud.dlc.v20210125.models.SparkMonitorMetrics`
+        :param PrestoMonitorMetrics: presto任务指标数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PrestoMonitorMetrics: :class:`tencentcloud.dlc.v20210125.models.PrestoMonitorMetrics`
         """
         self.DatabaseName = None
         self.DataAmount = None
         self.Id = None
         self.UsedTime = None
         self.OutputPath = None
         self.CreateTime = None
@@ -21460,14 +26903,26 @@
         self.UserAlias = None
         self.SparkJobName = None
         self.SparkJobId = None
         self.SparkJobFile = None
         self.UiUrl = None
         self.TotalTime = None
         self.CmdArgs = None
+        self.ImageVersion = None
+        self.StreamingStat = None
+        self.ResourceUsage = None
+        self.OutputConf = None
+        self.TaskKind = None
+        self.DriverSize = None
+        self.ExecutorSize = None
+        self.ExecutorNums = None
+        self.ExecutorMaxNumbers = None
+        self.CommonMetrics = None
+        self.SparkMonitorMetrics = None
+        self.PrestoMonitorMetrics = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.DataAmount = params.get("DataAmount")
         self.Id = params.get("Id")
         self.UsedTime = params.get("UsedTime")
@@ -21498,14 +26953,34 @@
         self.UserAlias = params.get("UserAlias")
         self.SparkJobName = params.get("SparkJobName")
         self.SparkJobId = params.get("SparkJobId")
         self.SparkJobFile = params.get("SparkJobFile")
         self.UiUrl = params.get("UiUrl")
         self.TotalTime = params.get("TotalTime")
         self.CmdArgs = params.get("CmdArgs")
+        self.ImageVersion = params.get("ImageVersion")
+        if params.get("StreamingStat") is not None:
+            self.StreamingStat = StreamingStatistics()
+            self.StreamingStat._deserialize(params.get("StreamingStat"))
+        self.ResourceUsage = params.get("ResourceUsage")
+        self.OutputConf = params.get("OutputConf")
+        self.TaskKind = params.get("TaskKind")
+        self.DriverSize = params.get("DriverSize")
+        self.ExecutorSize = params.get("ExecutorSize")
+        self.ExecutorNums = params.get("ExecutorNums")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        if params.get("CommonMetrics") is not None:
+            self.CommonMetrics = CommonMetrics()
+            self.CommonMetrics._deserialize(params.get("CommonMetrics"))
+        if params.get("SparkMonitorMetrics") is not None:
+            self.SparkMonitorMetrics = SparkMonitorMetrics()
+            self.SparkMonitorMetrics._deserialize(params.get("SparkMonitorMetrics"))
+        if params.get("PrestoMonitorMetrics") is not None:
+            self.PrestoMonitorMetrics = PrestoMonitorMetrics()
+            self.PrestoMonitorMetrics._deserialize(params.get("PrestoMonitorMetrics"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -21526,15 +27001,15 @@
         :param DatabaseName: 数据库名称，当前任务执行时候选中的默认数据库
 注意：此字段可能返回 null，表示取不到有效值。
         :type DatabaseName: str
         :param SQL: 当前执行的SQL，一个任务包含一个SQL
         :type SQL: str
         :param SQLType: 执行任务的类型，现在分为DDL、DML、DQL
         :type SQLType: str
-        :param State: 任务当前的状态，0：初始化 1：任务运行中 2：任务执行成功 -1：任务执行失败 -3：用户手动终止。只有任务执行成功的情况下，才会返回任务执行的结果
+        :param State: 任务当前的状态，0：初始化 1：任务运行中 2：任务执行成功  3：数据写入中 4：排队中 -1：任务执行失败 -3：用户手动终止 。只有任务执行成功的情况下，才会返回任务执行的结果
         :type State: int
         :param DataAmount: 扫描的数据量，单位byte
         :type DataAmount: int
         :param UsedTime: 计算耗时，单位： ms
         :type UsedTime: int
         :param OutputPath: 任务结果输出的COS桶地址
         :type OutputPath: str
@@ -21620,14 +27095,39 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class TaskStatisticMetrics(AbstractModel):
+    """任务指标信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param QueryResultTime: 获取结果时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QueryResultTime: float
+        """
+        self.QueryResultTime = None
+
+
+    def _deserialize(self, params):
+        self.QueryResultTime = params.get("QueryResultTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class TasksInfo(AbstractModel):
     """批量顺序执行任务集合
 
     """
 
     def __init__(self):
         r"""
@@ -21706,14 +27206,56 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class TenantGovernEventRules(AbstractModel):
+    """用户数据治理事件阈值
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 事件阈值ID
+        :type Id: int
+        :param Type: 事件阈值类型
+        :type Type: str
+        :param AppId: 用户AppId
+        :type AppId: str
+        :param Name: 治理事件阈值名称
+        :type Name: str
+        :param Rule: 数据治理时间阈值
+        :type Rule: :class:`tencentcloud.dlc.v20210125.models.RuleThreshold`
+        """
+        self.Id = None
+        self.Type = None
+        self.AppId = None
+        self.Name = None
+        self.Rule = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.Type = params.get("Type")
+        self.AppId = params.get("AppId")
+        self.Name = params.get("Name")
+        if params.get("Rule") is not None:
+            self.Rule = RuleThreshold()
+            self.Rule._deserialize(params.get("Rule"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class TextFile(AbstractModel):
     """文本格式
 
     """
 
     def __init__(self):
         r"""
@@ -22051,14 +27593,59 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class UpdateDataEngineConfigRequest(AbstractModel):
+    """UpdateDataEngineConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineIds: 引擎ID
+        :type DataEngineIds: list of str
+        :param DataEngineConfigCommand: 引擎配置命令，支持UpdateSparkSQLLakefsPath（更新原生表配置）、UpdateSparkSQLResultPath（更新结果路径配置）
+        :type DataEngineConfigCommand: str
+        """
+        self.DataEngineIds = None
+        self.DataEngineConfigCommand = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineIds = params.get("DataEngineIds")
+        self.DataEngineConfigCommand = params.get("DataEngineConfigCommand")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateDataEngineConfigResponse(AbstractModel):
+    """UpdateDataEngineConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class UpdateDataEngineRequest(AbstractModel):
     """UpdateDataEngine请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -22082,27 +27669,36 @@
         :type CrontabResumeSuspendStrategy: :class:`tencentcloud.dlc.v20210125.models.CrontabResumeSuspendStrategy`
         :param MaxConcurrency: 单个集群最大并发任务数，默认5
         :type MaxConcurrency: int
         :param TolerableQueueTime: 可容忍的排队时间，默认0。当任务排队的时间超过可容忍的时间时可能会触发扩容。如果该参数为0，则表示一旦有任务排队就可能立即触发扩容。
         :type TolerableQueueTime: int
         :param AutoSuspendTime: 集群自动挂起时间
         :type AutoSuspendTime: int
+        :param ElasticSwitch: spark jar 包年包月集群是否开启弹性
+        :type ElasticSwitch: bool
+        :param ElasticLimit: spark jar 包年包月集群弹性上限
+        :type ElasticLimit: int
+        :param SessionResourceTemplate: Spark批作业集群Session资源配置模板
+        :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
         """
         self.Size = None
         self.MinClusters = None
         self.MaxClusters = None
         self.AutoResume = None
         self.DataEngineName = None
         self.Message = None
         self.AutoSuspend = None
         self.CrontabResumeSuspend = None
         self.CrontabResumeSuspendStrategy = None
         self.MaxConcurrency = None
         self.TolerableQueueTime = None
         self.AutoSuspendTime = None
+        self.ElasticSwitch = None
+        self.ElasticLimit = None
+        self.SessionResourceTemplate = None
 
 
     def _deserialize(self, params):
         self.Size = params.get("Size")
         self.MinClusters = params.get("MinClusters")
         self.MaxClusters = params.get("MaxClusters")
         self.AutoResume = params.get("AutoResume")
@@ -22112,14 +27708,19 @@
         self.CrontabResumeSuspend = params.get("CrontabResumeSuspend")
         if params.get("CrontabResumeSuspendStrategy") is not None:
             self.CrontabResumeSuspendStrategy = CrontabResumeSuspendStrategy()
             self.CrontabResumeSuspendStrategy._deserialize(params.get("CrontabResumeSuspendStrategy"))
         self.MaxConcurrency = params.get("MaxConcurrency")
         self.TolerableQueueTime = params.get("TolerableQueueTime")
         self.AutoSuspendTime = params.get("AutoSuspendTime")
+        self.ElasticSwitch = params.get("ElasticSwitch")
+        self.ElasticLimit = params.get("ElasticLimit")
+        if params.get("SessionResourceTemplate") is not None:
+            self.SessionResourceTemplate = SessionResourceTemplate()
+            self.SessionResourceTemplate._deserialize(params.get("SessionResourceTemplate"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -22338,14 +27939,162 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class UpdateRowFilterRequest(AbstractModel):
+    """UpdateRowFilter请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PolicyId: 行过滤策略的id，此值可以通过DescribeUserInfo或者DescribeWorkGroupInfo接口获取
+        :type PolicyId: int
+        :param Policy: 新的过滤策略。
+        :type Policy: :class:`tencentcloud.dlc.v20210125.models.Policy`
+        """
+        self.PolicyId = None
+        self.Policy = None
+
+
+    def _deserialize(self, params):
+        self.PolicyId = params.get("PolicyId")
+        if params.get("Policy") is not None:
+            self.Policy = Policy()
+            self.Policy._deserialize(params.get("Policy"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateRowFilterResponse(AbstractModel):
+    """UpdateRowFilter返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class UpdateTaskStatusRequest(AbstractModel):
+    """UpdateTaskStatus请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务id
+        :type TaskId: str
+        :param TaskStatus: 任务状态 0-执行完成 1-初始化 5-执行中
+        :type TaskStatus: int
+        """
+        self.TaskId = None
+        self.TaskStatus = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.TaskStatus = params.get("TaskStatus")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateTaskStatusResponse(AbstractModel):
+    """UpdateTaskStatus返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class UpdateUserDataEngineConfigRequest(AbstractModel):
+    """UpdateUserDataEngineConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎ID
+        :type DataEngineId: str
+        :param DataEngineConfigPairs: 引擎配置项
+        :type DataEngineConfigPairs: list of DataEngineConfigPair
+        :param SessionResourceTemplate: 作业引擎资源配置模版
+        :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
+        """
+        self.DataEngineId = None
+        self.DataEngineConfigPairs = None
+        self.SessionResourceTemplate = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        if params.get("DataEngineConfigPairs") is not None:
+            self.DataEngineConfigPairs = []
+            for item in params.get("DataEngineConfigPairs"):
+                obj = DataEngineConfigPair()
+                obj._deserialize(item)
+                self.DataEngineConfigPairs.append(obj)
+        if params.get("SessionResourceTemplate") is not None:
+            self.SessionResourceTemplate = SessionResourceTemplate()
+            self.SessionResourceTemplate._deserialize(params.get("SessionResourceTemplate"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateUserDataEngineConfigResponse(AbstractModel):
+    """UpdateUserDataEngineConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class UpdateUserRoleRequest(AbstractModel):
     """UpdateUserRole请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -22408,36 +28157,40 @@
         :type TaskAction: str
         :param StartTime: 调度计划开始时间
         :type StartTime: str
         :param EndTime: 调度计划结束时间
         :type EndTime: str
         :param WorkflowDesc: 调度计划描述
         :type WorkflowDesc: str
+        :param OwnersUin: 责任人uin
+        :type OwnersUin: list of str
         """
         self.WorkflowId = None
         self.WorkflowName = None
         self.CycleType = None
         self.CycleStep = None
         self.DelayTime = None
         self.TaskAction = None
         self.StartTime = None
         self.EndTime = None
         self.WorkflowDesc = None
+        self.OwnersUin = None
 
 
     def _deserialize(self, params):
         self.WorkflowId = params.get("WorkflowId")
         self.WorkflowName = params.get("WorkflowName")
         self.CycleType = params.get("CycleType")
         self.CycleStep = params.get("CycleStep")
         self.DelayTime = params.get("DelayTime")
         self.TaskAction = params.get("TaskAction")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.WorkflowDesc = params.get("WorkflowDesc")
+        self.OwnersUin = params.get("OwnersUin")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -22456,14 +28209,55 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class UpgradeDataEngineImageRequest(AbstractModel):
+    """UpgradeDataEngineImage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineId: 引擎ID
+        :type DataEngineId: str
+        """
+        self.DataEngineId = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineId = params.get("DataEngineId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpgradeDataEngineImageResponse(AbstractModel):
+    """UpgradeDataEngineImage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class UserAliasInfo(AbstractModel):
     """用户id和名字信息
 
     """
 
     def __init__(self):
         r"""
@@ -22515,23 +28309,27 @@
         :type EnginePolicyInfo: :class:`tencentcloud.dlc.v20210125.models.Policys`
         :param WorkGroupInfo: 绑定到该用户的工作组集合信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type WorkGroupInfo: :class:`tencentcloud.dlc.v20210125.models.WorkGroups`
         :param UserAlias: 用户别名
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserAlias: str
+        :param RowFilterInfo: 行过滤集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RowFilterInfo: :class:`tencentcloud.dlc.v20210125.models.Policys`
         """
         self.UserId = None
         self.Type = None
         self.UserType = None
         self.UserDescription = None
         self.DataPolicyInfo = None
         self.EnginePolicyInfo = None
         self.WorkGroupInfo = None
         self.UserAlias = None
+        self.RowFilterInfo = None
 
 
     def _deserialize(self, params):
         self.UserId = params.get("UserId")
         self.Type = params.get("Type")
         self.UserType = params.get("UserType")
         self.UserDescription = params.get("UserDescription")
@@ -22541,14 +28339,17 @@
         if params.get("EnginePolicyInfo") is not None:
             self.EnginePolicyInfo = Policys()
             self.EnginePolicyInfo._deserialize(params.get("EnginePolicyInfo"))
         if params.get("WorkGroupInfo") is not None:
             self.WorkGroupInfo = WorkGroups()
             self.WorkGroupInfo._deserialize(params.get("WorkGroupInfo"))
         self.UserAlias = params.get("UserAlias")
+        if params.get("RowFilterInfo") is not None:
+            self.RowFilterInfo = Policys()
+            self.RowFilterInfo._deserialize(params.get("RowFilterInfo"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -22839,26 +28640,41 @@
         :type DatabaseName: str
         :param ViewName: 视图名称
         :type ViewName: str
         :param UserAlias: 视图创建人昵称
         :type UserAlias: str
         :param UserSubUin: 视图创建人ID
         :type UserSubUin: str
+        :param ViewId: 视图ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ViewId: str
+        :param ViewOriginalText: 创建视图原始文本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ViewOriginalText: str
+        :param ViewExpandedText: 创建视图展开文本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ViewExpandedText: str
         """
         self.DatabaseName = None
         self.ViewName = None
         self.UserAlias = None
         self.UserSubUin = None
+        self.ViewId = None
+        self.ViewOriginalText = None
+        self.ViewExpandedText = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.ViewName = params.get("ViewName")
         self.UserAlias = params.get("UserAlias")
         self.UserSubUin = params.get("UserSubUin")
+        self.ViewId = params.get("ViewId")
+        self.ViewOriginalText = params.get("ViewOriginalText")
+        self.ViewExpandedText = params.get("ViewExpandedText")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -22879,20 +28695,24 @@
         :param Properties: 视图属性信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Properties: list of Property
         :param CreateTime: 视图创建时间。
         :type CreateTime: str
         :param ModifiedTime: 视图更新时间。
         :type ModifiedTime: str
+        :param Comment: 视图的描述信息，已废弃
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Comment: str
         """
         self.ViewBaseInfo = None
         self.Columns = None
         self.Properties = None
         self.CreateTime = None
         self.ModifiedTime = None
+        self.Comment = None
 
 
     def _deserialize(self, params):
         if params.get("ViewBaseInfo") is not None:
             self.ViewBaseInfo = ViewBaseInfo()
             self.ViewBaseInfo._deserialize(params.get("ViewBaseInfo"))
         if params.get("Columns") is not None:
@@ -22905,14 +28725,115 @@
             self.Properties = []
             for item in params.get("Properties"):
                 obj = Property()
                 obj._deserialize(item)
                 self.Properties.append(obj)
         self.CreateTime = params.get("CreateTime")
         self.ModifiedTime = params.get("ModifiedTime")
+        self.Comment = params.get("Comment")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class VpcCidrBlock(AbstractModel):
+    """VPC子网信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CidrId: 子网Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CidrId: str
+        :param CidrAddr: 子网网段
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CidrAddr: str
+        """
+        self.CidrId = None
+        self.CidrAddr = None
+
+
+    def _deserialize(self, params):
+        self.CidrId = params.get("CidrId")
+        self.CidrAddr = params.get("CidrAddr")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class VpcConfigure(AbstractModel):
+    """vpc配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcId: vpc的唯一ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param VpcName: vpc的名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcName: str
+        :param VpcCidrBlock: vpc网段
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcCidrBlock: str
+        :param AvailableIpAddressCount: 可用的ip个数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AvailableIpAddressCount: int
+        """
+        self.VpcId = None
+        self.VpcName = None
+        self.VpcCidrBlock = None
+        self.AvailableIpAddressCount = None
+
+
+    def _deserialize(self, params):
+        self.VpcId = params.get("VpcId")
+        self.VpcName = params.get("VpcName")
+        self.VpcCidrBlock = params.get("VpcCidrBlock")
+        self.AvailableIpAddressCount = params.get("AvailableIpAddressCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class VpcInfo(AbstractModel):
+    """vpc信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcId: vpc Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param VpcCidrBlock: vpc子网
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcCidrBlock: str
+        """
+        self.VpcId = None
+        self.VpcCidrBlock = None
+
+
+    def _deserialize(self, params):
+        self.VpcId = params.get("VpcId")
+        self.VpcCidrBlock = params.get("VpcCidrBlock")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -22975,22 +28896,26 @@
         :type DataPolicyInfo: :class:`tencentcloud.dlc.v20210125.models.Policys`
         :param EnginePolicyInfo: 引擎权限集合
 注意：此字段可能返回 null，表示取不到有效值。
         :type EnginePolicyInfo: :class:`tencentcloud.dlc.v20210125.models.Policys`
         :param WorkGroupDescription: 工作组描述信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type WorkGroupDescription: str
+        :param RowFilterInfo: 行过滤信息集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RowFilterInfo: :class:`tencentcloud.dlc.v20210125.models.Policys`
         """
         self.WorkGroupId = None
         self.WorkGroupName = None
         self.Type = None
         self.UserInfo = None
         self.DataPolicyInfo = None
         self.EnginePolicyInfo = None
         self.WorkGroupDescription = None
+        self.RowFilterInfo = None
 
 
     def _deserialize(self, params):
         self.WorkGroupId = params.get("WorkGroupId")
         self.WorkGroupName = params.get("WorkGroupName")
         self.Type = params.get("Type")
         if params.get("UserInfo") is not None:
@@ -22999,14 +28924,17 @@
         if params.get("DataPolicyInfo") is not None:
             self.DataPolicyInfo = Policys()
             self.DataPolicyInfo._deserialize(params.get("DataPolicyInfo"))
         if params.get("EnginePolicyInfo") is not None:
             self.EnginePolicyInfo = Policys()
             self.EnginePolicyInfo._deserialize(params.get("EnginePolicyInfo"))
         self.WorkGroupDescription = params.get("WorkGroupDescription")
+        if params.get("RowFilterInfo") is not None:
+            self.RowFilterInfo = Policys()
+            self.RowFilterInfo._deserialize(params.get("RowFilterInfo"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -23205,38 +29133,43 @@
         :type DelayTime: int
         :param TaskAction: 在指定周期的第n个单位时间运行（周和月任务使用），比如周任务周日运行：TaskAction=1；周一运行：TaskAction=2，月任务当月第1天运行：TaskAction=1，等
         :type TaskAction: str
         :param StartTime: 调度计划开始时间
         :type StartTime: str
         :param EndTime: 调度计划结束时间
         :type EndTime: str
+        :param OwnersUin: 责任人uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OwnersUin: list of str
         """
         self.WorkflowId = None
         self.WorkflowName = None
         self.WorkflowDesc = None
         self.CreateTime = None
         self.CycleType = None
         self.CycleStep = None
         self.DelayTime = None
         self.TaskAction = None
         self.StartTime = None
         self.EndTime = None
+        self.OwnersUin = None
 
 
     def _deserialize(self, params):
         self.WorkflowId = params.get("WorkflowId")
         self.WorkflowName = params.get("WorkflowName")
         self.WorkflowDesc = params.get("WorkflowDesc")
         self.CreateTime = params.get("CreateTime")
         self.CycleType = params.get("CycleType")
         self.CycleStep = params.get("CycleStep")
         self.DelayTime = params.get("DelayTime")
         self.TaskAction = params.get("TaskAction")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
+        self.OwnersUin = params.get("OwnersUin")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/common.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/common.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/configurations.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/configurations.py`

 * *Files 18% similar despite different names*

```diff
@@ -109,73 +109,79 @@
 
         if value is None:
             return
 
         self._value = value
         if save:
             _save(self._key, self._value)
+    
+    def __str__(self):
+        return '{}: {}'.format(self._key, self._value)
 
     
 CONF = Configuration
 
 
-DEBUG = CONF('debug', True)
-
 LOG_FILE = CONF("log.file", os.path.join(constants.HOME_PATH,f"tdlc.log"))
-LOG_LEVEL = CONF("log.level", "INFO")
+LOG_LEVEL = CONF("log.level", "DEBUG")
 
 REGION = CONF('qcloud.region')
 SECRET_ID = CONF('qcloud.secret_id')
 SECRET_KEY = CONF('qcloud.secret_key')
 TOKEN = CONF('qcloud.token')
 ENDPOINT = CONF('qcloud.endpoint')
 ROLE_ARN = CONF('qcloud.role_arn')
 ENGINE = CONF('qcloud.dlc.engine')
 
-LANGUAGE = CONF('session.option.notebook.language', constants.LANGUAGE_PYTHON)
+LANGUAGE = CONF('session.notebook.language', constants.LANGUAGE_PYTHON)
+
+JARS = CONF('session.jars')
+PYFILES = CONF('session.pyfiles')
+ARCHIVES = CONF('session.archives')
+IMAGE = CONF('session.image')
 
-PYFILES = CONF('session.option.pyfiles')
-ARCHIVES = CONF('session.option.archives')
-PROXY_USER = CONF('session.option.proxy_user', 'root')
-EXTRACONF = CONF('session.option.conf')
+PROXY_USER = CONF('session.proxy_user', 'root')
+EXTRACONF = CONF('session.conf')
 
-SESSION_TIMEOUT = CONF("session.option.timeout", 3600, int)
-WAIT_IDLE_TIMEOUT = CONF("session.option.wait.idle.timeout", 180, int)
+SESSION_TIMEOUT = CONF("session.timeout", 3600, int)
+WAIT_IDLE_TIMEOUT = CONF("session.wait.idle.timeout", 600, int)
 
 SESSION_NUM_MAX = CONF('session.limit.max_num', 5, int)
 
-DRIVER_SIZE = CONF('session.option.spark.driver.size', constants.CU_SIZE_SMALL)
-EXECUTOR_SIZE = CONF('session.option.spark.executor.size', constants.CU_SIZE_SMALL)
-EXECUTOR_NUM = CONF('session.option.spark.executor.num', 1, int)
+DRIVER_SIZE = CONF('session.spark.driver.size', constants.CU_SIZE_SMALL)
+EXECUTOR_SIZE = CONF('session.spark.executor.size', constants.CU_SIZE_SMALL)
+EXECUTOR_NUM = CONF('session.spark.executor.num', 1, int)
+
 
 RESULT_MAX_ROWS = CONF("result.max.rows", 2500, int)
 RESULT_SAMPLE_METHOD = CONF("result.sample.method", "take")
 RESULT_SAMPLE_FRACTION = CONF("result.sample.fraction", 0.1, float)
 
 SPARK_CONF = CONF("spark.conf", {}, _toJSON)
 
-
-def setAll(JSON, save):
+def setAll(JSON: dict, save):
 
     REGION.set(JSON.get("region", ""), save)
-    SECRET_ID.set(JSON.get("secret-id", ""), save)
-    SECRET_KEY.set(JSON.get("secret-key", ""), save)
+    SECRET_ID.set(JSON.get("secret-id") or JSON.get("secretId", ""), save)
+    SECRET_KEY.set(JSON.get("secret-key") or JSON.get("secretKey", ""), save)
     ENDPOINT.set(JSON.get("endpoint", ""), save)
-    ROLE_ARN.set(JSON.get("role-arn", ""), save)
+    ROLE_ARN.set(JSON.get("role-arn") or JSON.get("roleArn", ""), save)
     ENGINE.set(JSON.get("engine", ""), save)
 
     LANGUAGE.set(JSON.get("language"), save)
-    PYFILES.set(JSON.get("py-files"), save)
+    PYFILES.set(JSON.get("pyfiles"), save)
     ARCHIVES.set(JSON.get("archives"), save)
     # PROXY_USER.set(JSON.get("proxy_user"), save)
 
     SESSION_TIMEOUT.set(JSON.get("timeout"), save)
-    DRIVER_SIZE.set(JSON.get("driver-size"), save)
-    EXECUTOR_SIZE.set(JSON.get("executor-size"), save)
-    EXECUTOR_NUM.set(JSON.get("executor-num"), save)
+    DRIVER_SIZE.set(JSON.get("driver-size") or JSON.get("driverSize"), save)
+    EXECUTOR_SIZE.set(JSON.get("executor-size") or JSON.get("executorSize"), save)
+    EXECUTOR_NUM.set(JSON.get("executor-num") or JSON.get("executorNum"), save)
+
+    IMAGE.set(JSON.get('image'), save)
 
     SPARK_CONF.set(JSON.get("conf"), save)
 
 
     #  TODO
     #  EXTRACONF
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/constants.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,38 +43,41 @@
 SESSION_STATUS_IDLE = 'idle'
 SESSION_STATUS_BUSY = 'busy'
 SESSION_STATUS_SHUTTING_DOWN = 'shutting_down'
 SESSION_STATUS_ERROR = 'error'
 SESSION_STATUS_DEAD = 'dead'
 SESSION_STATUS_KILLED = 'killed'
 SESSION_STATUS_SUCCESS = 'success'
+SESSION_STATUS_LOST = 'lost'
 
 SESSION_STATUS_SUPPORTED = [
     SESSION_STATUS_NOT_STARTED,
     SESSION_STATUS_STARTING,
     SESSION_STATUS_IDLE,
     SESSION_STATUS_BUSY,
     SESSION_STATUS_SHUTTING_DOWN,
     SESSION_STATUS_ERROR,
     SESSION_STATUS_DEAD,
     SESSION_STATUS_KILLED,
-    SESSION_STATUS_SUCCESS
+    SESSION_STATUS_SUCCESS,
+    SESSION_STATUS_LOST,
 ]
 
 SESSION_ACTIVE_STATUS = (
     SESSION_STATUS_STARTING,
     SESSION_STATUS_IDLE,
     SESSION_STATUS_BUSY,
 )
 
 SESSION_FINAL_STATUS = (
     SESSION_STATUS_DEAD,
     SESSION_STATUS_ERROR,
     SESSION_STATUS_KILLED,
     SESSION_STATUS_SUCCESS,
+    SESSION_STATUS_LOST,
 )
 
 STATEMENT_STATUS_WAITING = 'waiting'
 STATEMENT_STATUS_RUNNING = 'running'
 STATEMENT_STATUS_AVAILABLE = 'available'
 STATEMENT_STATUS_ERROR = 'error'
 STATEMENT_STATUS_CANCELLING = 'cancelling'
```

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/log.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/log.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/render.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/render.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/utils/validators.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/utils/validators.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/widgets/configuiwidget.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/widgets/configuiwidget.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tdlc/widgets/createsessionwidget.py` & `tencentcloud-dlc-jupyter-1.1.0/tdlc/widgets/createsessionwidget.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-jupyter-1.0.0b0/tencentcloud_dlc_jupyter.egg-info/SOURCES.txt` & `tencentcloud-dlc-jupyter-1.1.0/tencentcloud_dlc_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

