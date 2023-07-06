# Comparing `tmp/nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704.tar.gz` & `tmp/nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704.tar", last modified: Wed Jul  5 11:23:30 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705.tar", last modified: Wed Jul  5 17:03:35 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704.tar` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 11:23:30.372549 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-07-05 11:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-07-05 11:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-05 11:23:30.372549 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-07-05 11:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 11:23:30.372549 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-05 11:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-07-05 11:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-05 11:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-05 11:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-05 11:23:30.372549 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 17:03:35.863896 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-07-05 17:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-07-05 17:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-05 17:03:35.863896 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-07-05 17:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 17:03:35.863896 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-05 17:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-07-05 17:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-05 17:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-05 17:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-05 17:03:35.863896 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/setup.py
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/LICENSE.md` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda120
-Version: 1.28.0.dev20230704
+Version: 1.28.0.dev20230705
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda120
-Version: 1.28.0.dev20230704
+Version: 1.28.0.dev20230705
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230704/setup.py` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230705/setup.py`

 * *Files identical despite different names*

