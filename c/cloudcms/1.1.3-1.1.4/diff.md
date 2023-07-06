# Comparing `tmp/cloudcms-1.1.3.tar.gz` & `tmp/cloudcms-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudcms-1.1.3.tar", last modified: Tue Jan  4 21:22:00 2022, max compression
+gzip compressed data, was "cloudcms-1.1.4.tar", last modified: Thu Jul  6 19:54:22 2023, max compression
```

## Comparing `cloudcms-1.1.3.tar` & `cloudcms-1.1.4.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.352571 cloudcms-1.1.3/
--rw-r--r--   0 mwhitman   (501) staff       (20)     3042 2022-01-04 21:22:00.352111 cloudcms-1.1.3/PKG-INFO
--rw-r--r--   0 mwhitman   (501) staff       (20)     1900 2020-07-15 19:26:41.000000 cloudcms-1.1.3/README.md
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.317655 cloudcms-1.1.3/cloudcms/
--rw-r--r--   0 mwhitman   (501) staff       (20)       30 2020-07-15 19:26:41.000000 cloudcms-1.1.3/cloudcms/__init__.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.321173 cloudcms-1.1.3/cloudcms/association/
--rw-r--r--   0 mwhitman   (501) staff       (20)      112 2020-07-20 14:32:32.000000 cloudcms-1.1.3/cloudcms/association/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     1664 2020-07-20 20:12:03.000000 cloudcms-1.1.3/cloudcms/association/association.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      184 2020-07-20 15:19:50.000000 cloudcms-1.1.3/cloudcms/association/direction.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      157 2020-07-20 15:19:31.000000 cloudcms-1.1.3/cloudcms/association/directionality.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.322505 cloudcms-1.1.3/cloudcms/attachment/
--rw-r--r--   0 mwhitman   (501) staff       (20)       34 2020-07-20 14:36:08.000000 cloudcms-1.1.3/cloudcms/attachment/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      652 2020-07-20 20:48:50.000000 cloudcms-1.1.3/cloudcms/attachment/attachment.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.323865 cloudcms-1.1.3/cloudcms/branch/
--rw-r--r--   0 mwhitman   (501) staff       (20)       26 2020-07-20 14:32:46.000000 cloudcms-1.1.3/cloudcms/branch/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     3417 2021-11-29 19:09:54.000000 cloudcms-1.1.3/cloudcms/branch/branch.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     3233 2021-11-29 21:46:39.000000 cloudcms-1.1.3/cloudcms/cloudcms.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.326336 cloudcms-1.1.3/cloudcms/error/
--rw-r--r--   0 mwhitman   (501) staff       (20)      122 2021-11-29 18:28:07.000000 cloudcms-1.1.3/cloudcms/error/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      176 2020-07-20 14:37:26.000000 cloudcms-1.1.3/cloudcms/error/invalid_qname_error.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      155 2021-11-29 18:27:38.000000 cloudcms-1.1.3/cloudcms/error/job_error.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      127 2020-07-20 14:24:09.000000 cloudcms-1.1.3/cloudcms/error/request_error.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.327651 cloudcms-1.1.3/cloudcms/job/
--rw-r--r--   0 mwhitman   (501) staff       (20)       21 2021-11-29 21:23:57.000000 cloudcms-1.1.3/cloudcms/job/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      322 2021-11-30 16:08:16.000000 cloudcms-1.1.3/cloudcms/job/job.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.330083 cloudcms-1.1.3/cloudcms/node/
--rw-r--r--   0 mwhitman   (501) staff       (20)      102 2020-07-20 20:05:34.000000 cloudcms-1.1.3/cloudcms/node/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     3666 2021-11-30 17:07:59.000000 cloudcms-1.1.3/cloudcms/node/base_node.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     5500 2022-01-04 21:16:27.000000 cloudcms-1.1.3/cloudcms/node/node.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      720 2020-07-20 21:09:52.000000 cloudcms-1.1.3/cloudcms/node/traversal_results.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.332086 cloudcms-1.1.3/cloudcms/platform/
--rw-r--r--   0 mwhitman   (501) staff       (20)       74 2020-07-20 14:33:59.000000 cloudcms-1.1.3/cloudcms/platform/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      836 2020-07-20 16:21:53.000000 cloudcms-1.1.3/cloudcms/platform/cloudcms_object.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     2169 2021-11-30 16:30:42.000000 cloudcms-1.1.3/cloudcms/platform/platform.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.333712 cloudcms-1.1.3/cloudcms/project/
--rw-r--r--   0 mwhitman   (501) staff       (20)       29 2021-11-29 21:09:20.000000 cloudcms-1.1.3/cloudcms/project/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      362 2021-11-30 15:55:40.000000 cloudcms-1.1.3/cloudcms/project/project.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.335496 cloudcms-1.1.3/cloudcms/release/
--rw-r--r--   0 mwhitman   (501) staff       (20)       28 2021-11-29 18:52:45.000000 cloudcms-1.1.3/cloudcms/release/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      386 2021-11-29 18:53:43.000000 cloudcms-1.1.3/cloudcms/release/release.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.337791 cloudcms-1.1.3/cloudcms/repository/
--rw-r--r--   0 mwhitman   (501) staff       (20)       82 2020-07-20 17:33:31.000000 cloudcms-1.1.3/cloudcms/repository/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     2477 2021-11-30 16:39:49.000000 cloudcms-1.1.3/cloudcms/repository/repository.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      326 2020-07-20 14:45:03.000000 cloudcms-1.1.3/cloudcms/repository/repository_object.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.340216 cloudcms-1.1.3/cloudcms/support/
--rw-r--r--   0 mwhitman   (501) staff       (20)       72 2020-07-20 14:32:23.000000 cloudcms-1.1.3/cloudcms/support/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      703 2020-07-20 14:24:47.000000 cloudcms-1.1.3/cloudcms/support/connection_config.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      666 2020-07-20 14:45:11.000000 cloudcms-1.1.3/cloudcms/support/qname.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.319189 cloudcms-1.1.3/cloudcms.egg-info/
--rw-r--r--   0 mwhitman   (501) staff       (20)     3042 2022-01-04 21:22:00.000000 cloudcms-1.1.3/cloudcms.egg-info/PKG-INFO
--rw-r--r--   0 mwhitman   (501) staff       (20)     1506 2022-01-04 21:22:00.000000 cloudcms-1.1.3/cloudcms.egg-info/SOURCES.txt
--rw-r--r--   0 mwhitman   (501) staff       (20)        1 2022-01-04 21:22:00.000000 cloudcms-1.1.3/cloudcms.egg-info/dependency_links.txt
--rw-r--r--   0 mwhitman   (501) staff       (20)       57 2022-01-04 21:22:00.000000 cloudcms-1.1.3/cloudcms.egg-info/requires.txt
--rw-r--r--   0 mwhitman   (501) staff       (20)       15 2022-01-04 21:22:00.000000 cloudcms-1.1.3/cloudcms.egg-info/top_level.txt
--rw-r--r--   0 mwhitman   (501) staff       (20)       38 2022-01-04 21:22:00.352719 cloudcms-1.1.3/setup.cfg
--rw-r--r--   0 mwhitman   (501) staff       (20)      754 2022-01-04 21:21:36.000000 cloudcms-1.1.3/setup.py
-drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2022-01-04 21:22:00.351328 cloudcms-1.1.3/tests/
--rw-r--r--   0 mwhitman   (501) staff       (20)      856 2021-11-29 20:57:51.000000 cloudcms-1.1.3/tests/__init__.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      515 2020-07-15 19:26:41.000000 cloudcms-1.1.3/tests/abstract_test.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      411 2020-07-20 14:59:09.000000 cloudcms-1.1.3/tests/abstract_with_repository_test.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     2994 2020-07-20 21:03:37.000000 cloudcms-1.1.3/tests/test_association.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     1932 2020-07-20 20:54:35.000000 cloudcms-1.1.3/tests/test_attachment.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      814 2021-11-29 20:27:08.000000 cloudcms-1.1.3/tests/test_branch.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     2316 2020-07-24 18:09:56.000000 cloudcms-1.1.3/tests/test_file_folder.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      586 2021-05-24 14:14:55.000000 cloudcms-1.1.3/tests/test_graphql.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     5618 2021-11-30 17:08:10.000000 cloudcms-1.1.3/tests/test_node.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      242 2020-07-15 19:26:41.000000 cloudcms-1.1.3/tests/test_platform.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      572 2021-11-30 16:32:12.000000 cloudcms-1.1.3/tests/test_project.py
--rw-r--r--   0 mwhitman   (501) staff       (20)      710 2021-11-30 16:39:57.000000 cloudcms-1.1.3/tests/test_release.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     1029 2021-11-29 22:02:04.000000 cloudcms-1.1.3/tests/test_repository.py
--rw-r--r--   0 mwhitman   (501) staff       (20)     2048 2022-01-04 21:16:45.000000 cloudcms-1.1.3/tests/test_traverse.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.494096 cloudcms-1.1.4/
+-rw-r--r--   0 mwhitman   (501) staff       (20)    11357 2020-07-15 19:26:41.000000 cloudcms-1.1.4/LICENSE
+-rw-r--r--   0 mwhitman   (501) staff       (20)     2329 2023-07-06 19:54:22.493812 cloudcms-1.1.4/PKG-INFO
+-rw-r--r--   0 mwhitman   (501) staff       (20)     1900 2023-07-06 19:21:40.000000 cloudcms-1.1.4/README.md
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.472185 cloudcms-1.1.4/cloudcms/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       30 2020-07-15 19:26:41.000000 cloudcms-1.1.4/cloudcms/__init__.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.476084 cloudcms-1.1.4/cloudcms/association/
+-rw-r--r--   0 mwhitman   (501) staff       (20)      112 2020-07-20 14:32:32.000000 cloudcms-1.1.4/cloudcms/association/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     1664 2020-07-20 20:12:03.000000 cloudcms-1.1.4/cloudcms/association/association.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      184 2020-07-20 15:19:50.000000 cloudcms-1.1.4/cloudcms/association/direction.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      157 2020-07-20 15:19:31.000000 cloudcms-1.1.4/cloudcms/association/directionality.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.476809 cloudcms-1.1.4/cloudcms/attachment/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       34 2020-07-20 14:36:08.000000 cloudcms-1.1.4/cloudcms/attachment/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      652 2020-07-20 20:48:50.000000 cloudcms-1.1.4/cloudcms/attachment/attachment.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.477709 cloudcms-1.1.4/cloudcms/branch/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       26 2020-07-20 14:32:46.000000 cloudcms-1.1.4/cloudcms/branch/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     3417 2021-11-29 19:09:54.000000 cloudcms-1.1.4/cloudcms/branch/branch.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     3233 2023-07-06 19:36:13.000000 cloudcms-1.1.4/cloudcms/cloudcms.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.479443 cloudcms-1.1.4/cloudcms/error/
+-rw-r--r--   0 mwhitman   (501) staff       (20)      122 2021-11-29 18:28:07.000000 cloudcms-1.1.4/cloudcms/error/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      176 2020-07-20 14:37:26.000000 cloudcms-1.1.4/cloudcms/error/invalid_qname_error.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      155 2021-11-29 18:27:38.000000 cloudcms-1.1.4/cloudcms/error/job_error.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      127 2020-07-20 14:24:09.000000 cloudcms-1.1.4/cloudcms/error/request_error.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.480316 cloudcms-1.1.4/cloudcms/job/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       21 2021-11-29 21:23:57.000000 cloudcms-1.1.4/cloudcms/job/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      322 2021-11-30 16:08:16.000000 cloudcms-1.1.4/cloudcms/job/job.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.482125 cloudcms-1.1.4/cloudcms/node/
+-rw-r--r--   0 mwhitman   (501) staff       (20)      102 2020-07-20 20:05:34.000000 cloudcms-1.1.4/cloudcms/node/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     3666 2021-11-30 17:07:59.000000 cloudcms-1.1.4/cloudcms/node/base_node.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     5500 2022-01-04 21:16:27.000000 cloudcms-1.1.4/cloudcms/node/node.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      720 2020-07-20 21:09:52.000000 cloudcms-1.1.4/cloudcms/node/traversal_results.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.483876 cloudcms-1.1.4/cloudcms/platform/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       74 2020-07-20 14:33:59.000000 cloudcms-1.1.4/cloudcms/platform/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      836 2020-07-20 16:21:53.000000 cloudcms-1.1.4/cloudcms/platform/cloudcms_object.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     3262 2023-07-06 19:45:17.000000 cloudcms-1.1.4/cloudcms/platform/platform.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.484942 cloudcms-1.1.4/cloudcms/project/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       29 2021-11-29 21:09:20.000000 cloudcms-1.1.4/cloudcms/project/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      362 2021-11-30 15:55:40.000000 cloudcms-1.1.4/cloudcms/project/project.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.485854 cloudcms-1.1.4/cloudcms/release/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       28 2021-11-29 18:52:45.000000 cloudcms-1.1.4/cloudcms/release/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      386 2021-11-29 18:53:43.000000 cloudcms-1.1.4/cloudcms/release/release.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.487313 cloudcms-1.1.4/cloudcms/repository/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       82 2020-07-20 17:33:31.000000 cloudcms-1.1.4/cloudcms/repository/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     2477 2021-11-30 16:39:49.000000 cloudcms-1.1.4/cloudcms/repository/repository.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      326 2020-07-20 14:45:03.000000 cloudcms-1.1.4/cloudcms/repository/repository_object.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.488869 cloudcms-1.1.4/cloudcms/support/
+-rw-r--r--   0 mwhitman   (501) staff       (20)       72 2020-07-20 14:32:23.000000 cloudcms-1.1.4/cloudcms/support/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      703 2020-07-20 14:24:47.000000 cloudcms-1.1.4/cloudcms/support/connection_config.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      666 2020-07-20 14:45:11.000000 cloudcms-1.1.4/cloudcms/support/qname.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.474465 cloudcms-1.1.4/cloudcms.egg-info/
+-rw-r--r--   0 mwhitman   (501) staff       (20)     2329 2023-07-06 19:54:22.000000 cloudcms-1.1.4/cloudcms.egg-info/PKG-INFO
+-rw-r--r--   0 mwhitman   (501) staff       (20)     1546 2023-07-06 19:54:22.000000 cloudcms-1.1.4/cloudcms.egg-info/SOURCES.txt
+-rw-r--r--   0 mwhitman   (501) staff       (20)        1 2023-07-06 19:54:22.000000 cloudcms-1.1.4/cloudcms.egg-info/dependency_links.txt
+-rw-r--r--   0 mwhitman   (501) staff       (20)       57 2023-07-06 19:54:22.000000 cloudcms-1.1.4/cloudcms.egg-info/requires.txt
+-rw-r--r--   0 mwhitman   (501) staff       (20)       15 2023-07-06 19:54:22.000000 cloudcms-1.1.4/cloudcms.egg-info/top_level.txt
+-rw-r--r--   0 mwhitman   (501) staff       (20)       38 2023-07-06 19:54:22.494190 cloudcms-1.1.4/setup.cfg
+-rw-r--r--   0 mwhitman   (501) staff       (20)      754 2023-07-06 19:46:35.000000 cloudcms-1.1.4/setup.py
+drwxr-xr-x   0 mwhitman   (501) staff       (20)        0 2023-07-06 19:54:22.493438 cloudcms-1.1.4/tests/
+-rw-r--r--   0 mwhitman   (501) staff       (20)      953 2023-07-06 19:25:06.000000 cloudcms-1.1.4/tests/__init__.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      515 2020-07-15 19:26:41.000000 cloudcms-1.1.4/tests/abstract_test.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      411 2020-07-20 14:59:09.000000 cloudcms-1.1.4/tests/abstract_with_repository_test.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     2994 2020-07-20 21:03:37.000000 cloudcms-1.1.4/tests/test_association.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     1932 2020-07-20 20:54:35.000000 cloudcms-1.1.4/tests/test_attachment.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      814 2021-11-29 20:27:08.000000 cloudcms-1.1.4/tests/test_branch.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     1494 2023-07-06 19:46:06.000000 cloudcms-1.1.4/tests/test_deployment_target.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     2316 2020-07-24 18:09:56.000000 cloudcms-1.1.4/tests/test_file_folder.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      586 2021-05-24 14:14:55.000000 cloudcms-1.1.4/tests/test_graphql.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     5618 2022-05-06 15:49:35.000000 cloudcms-1.1.4/tests/test_node.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      242 2020-07-15 19:26:41.000000 cloudcms-1.1.4/tests/test_platform.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      572 2021-11-30 16:32:12.000000 cloudcms-1.1.4/tests/test_project.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)      710 2021-11-30 16:39:57.000000 cloudcms-1.1.4/tests/test_release.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     1029 2021-11-29 22:02:04.000000 cloudcms-1.1.4/tests/test_repository.py
+-rw-r--r--   0 mwhitman   (501) staff       (20)     2048 2022-01-04 21:16:45.000000 cloudcms-1.1.4/tests/test_traverse.py
```

### Comparing `cloudcms-1.1.3/PKG-INFO` & `cloudcms-1.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 Metadata-Version: 2.1
 Name: cloudcms
-Version: 1.1.3
+Version: 1.1.4
 Summary: Cloud CMS Python Driver
 Home-page: https://github.com/gitana/cloudcms-python-driver
 Author: Michael Whitman
 Author-email: michael.whitman@cloudcms.com
-License: UNKNOWN
-Description: # Cloud CMS Python Driver
-        
-        Basic driver for the [Cloud CMS](https://www.cloudcms.com) API
-        
-        Runs with Python 3
-        
-        Currently supports the following functionality:
-        - Connect to and refresh access tokens with the API
-        - Read platform, branch, and repositories
-        - Read, query, search, create, update, and delete nodes
-        
-        ## Installation
-        
-        `pip install cloudcms`
-        
-        ## Examples
-        
-        Below are some examples of how you might use this driver:
-        
-        ```python
-        from cloudcms import CloudCMS
-        
-        # Connect to Cloud CMS
-        client = CloudCMS()
-        platform = client.connect(filename='gitana.json')
-        
-        # List repositories
-        repositories = platform.list_repositories()
-        
-        # Read repository
-        repository = platform.read_repository('<repository_id>')
-        
-        # List branches
-        branches = repository.list_branches()
-        
-        # Read branch
-        branch = repository.read_branch('<branch_id>')
-        
-        # Read Node
-        node = branch.read_node('<node_id>')
-        
-        # Create node
-        obj = {
-            'title': 'Twelfth Night',
-            'description': 'An old play'
-        }
-        newNode = branch.create_node(obj)
-        
-        # Query nodes
-        query = {
-            '_type': 'store:book'
-        }
-        pagination = {
-            'limit': 2
-        }
-        queried_nodes = branch.query_nodes(query, pagination)
-        
-        # Search/Find nodes
-        find = {
-            'search': 'Shakespeare',
-            'query': {
-                '_type': 'store:book'
-            }
-        }
-        searched_nodes = branch.find_nodes(find)
-        ```
-        
-        ## Tests
-        
-        To perform the unit tests for this driver, ensure that you have a `gitana.json` file in the driver directory, then run:
-        
-        ```
-        python -m unittest tests
-        ```
-        
-        ## Resources
-        
-        * Cloud CMS: https://www.cloudcms.com
-        * Github: https://github.com/gitana/cloudcms-python-driver
-        * Python Driver Download: https://pypi.org/project/cloudcms/
-        * Cloud CMS Documentation: https://www.cloudcms.com/documentation.html
-        * Developers Guide: https://www.cloudcms.com/developers.html
-        
-        ## Support
-        
-        For information or questions about the Python Driver, please contact Cloud CMS
-        at [support@cloudcms.com](mailto:support@cloudcms.com).
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Cloud CMS Python Driver
+
+Basic driver for the [Cloud CMS](https://www.cloudcms.com) API
+
+Runs with Python 3
+
+Currently supports the following functionality:
+- Connect to and refresh access tokens with the API
+- Read platform, branch, and repositories
+- Read, query, search, create, update, and delete nodes
+
+## Installation
+
+`pip install cloudcms`
+
+## Examples
+
+Below are some examples of how you might use this driver:
+
+```python
+from cloudcms import CloudCMS
+
+# Connect to Cloud CMS
+client = CloudCMS()
+platform = client.connect(filename='gitana.json')
+
+# List repositories
+repositories = platform.list_repositories()
+
+# Read repository
+repository = platform.read_repository('<repository_id>')
+
+# List branches
+branches = repository.list_branches()
+
+# Read branch
+branch = repository.read_branch('<branch_id>')
+
+# Read Node
+node = branch.read_node('<node_id>')
+
+# Create node
+obj = {
+    'title': 'Twelfth Night',
+    'description': 'An old play'
+}
+newNode = branch.create_node(obj)
+
+# Query nodes
+query = {
+    '_type': 'store:book'
+}
+pagination = {
+    'limit': 2
+}
+queried_nodes = branch.query_nodes(query, pagination)
+
+# Search/Find nodes
+find = {
+    'search': 'Shakespeare',
+    'query': {
+        '_type': 'store:book'
+    }
+}
+searched_nodes = branch.find_nodes(find)
+```
+
+## Tests
+
+To perform the unit tests for this driver, ensure that you have a `gitana.json` file in the driver directory, then run:
+
+```
+python -m unittest tests
+```
+
+## Resources
+
+* Cloud CMS: https://www.cloudcms.com
+* Github: https://github.com/gitana/cloudcms-python-driver
+* Python Driver Download: https://pypi.org/project/cloudcms/
+* Cloud CMS Documentation: https://www.cloudcms.com/documentation.html
+* Developers Guide: https://www.cloudcms.com/developers.html
+
+## Support
+
+For information or questions about the Python Driver, please contact Cloud CMS
+at [support@cloudcms.com](mailto:support@cloudcms.com).
```

### Comparing `cloudcms-1.1.3/README.md` & `cloudcms-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/association/association.py` & `cloudcms-1.1.4/cloudcms/association/association.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/attachment/attachment.py` & `cloudcms-1.1.4/cloudcms/attachment/attachment.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/branch/branch.py` & `cloudcms-1.1.4/cloudcms/branch/branch.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/cloudcms.py` & `cloudcms-1.1.4/cloudcms/cloudcms.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/node/base_node.py` & `cloudcms-1.1.4/cloudcms/node/base_node.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/node/node.py` & `cloudcms-1.1.4/cloudcms/node/node.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/node/traversal_results.py` & `cloudcms-1.1.4/cloudcms/node/traversal_results.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/platform/cloudcms_object.py` & `cloudcms-1.1.4/cloudcms/platform/cloudcms_object.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/platform/platform.py` & `cloudcms-1.1.4/cloudcms/platform/platform.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from cloudcms.deployment.deployment_target import DeploymentTarget
 from . import CloudCMSObject
 from ..repository import Repository
 from ..project import Project
 from ..job import Job
-from ..error import JobError
+from ..error import JobError, RequestError
 
 import time
 
 class Platform(CloudCMSObject):
 
     def __init__(self, client, data):
         super(Platform, self).__init__(client, data)
@@ -56,14 +57,44 @@
         res = self.client.post(uri, pagination, query)
         return Job.job_map(self.client, res['rows'])
 
     def kill_job(self, jobId):
         uri = self.uri() + '/jobs/' + jobId + '/kill'
         res = self.client.post(uri, {}, {})
         return Job(self.client, res)
+    
+    # Deployment 
+
+    # Targets
+    def list_deployment_targets(self, pagination={}):
+        uri = self.uri() + '/deployment/targets'
+        res = self.client.get(uri, pagination)
+        return DeploymentTarget.deployment_target_map(self.client, res['rows'])
+
+    def query_deployment_targets(self, query, pagination={}):
+        uri = self.uri() + '/deployment/targets/query'
+        res = self.client.post(uri, pagination, query)
+        return DeploymentTarget.deployment_target_map(self.client, res['rows'])
+    
+    def read_deployment_target(self, id):
+        uri = self.uri() + '/deployment/targets/' + id
+        try:
+            res = self.client.get(uri)
+            target = DeploymentTarget(self.client, res)
+        except RequestError:
+            target = None
+
+        return target 
+    
+    def create_deployment_target(self, obj):
+        uri = self.uri() + '/deployment/targets/'
+        res = self.client.post(uri, data=obj)
+        targetId = res['_doc']
+
+        return targetId
 
     def wait_for_job_completion(self, jobId):
         
         # Use with caution
         while True:
             job = self.read_job(jobId)
```

### Comparing `cloudcms-1.1.3/cloudcms/repository/repository.py` & `cloudcms-1.1.4/cloudcms/repository/repository.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/support/connection_config.py` & `cloudcms-1.1.4/cloudcms/support/connection_config.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms/support/qname.py` & `cloudcms-1.1.4/cloudcms/support/qname.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/cloudcms.egg-info/PKG-INFO` & `cloudcms-1.1.4/cloudcms.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 Metadata-Version: 2.1
 Name: cloudcms
-Version: 1.1.3
+Version: 1.1.4
 Summary: Cloud CMS Python Driver
 Home-page: https://github.com/gitana/cloudcms-python-driver
 Author: Michael Whitman
 Author-email: michael.whitman@cloudcms.com
-License: UNKNOWN
-Description: # Cloud CMS Python Driver
-        
-        Basic driver for the [Cloud CMS](https://www.cloudcms.com) API
-        
-        Runs with Python 3
-        
-        Currently supports the following functionality:
-        - Connect to and refresh access tokens with the API
-        - Read platform, branch, and repositories
-        - Read, query, search, create, update, and delete nodes
-        
-        ## Installation
-        
-        `pip install cloudcms`
-        
-        ## Examples
-        
-        Below are some examples of how you might use this driver:
-        
-        ```python
-        from cloudcms import CloudCMS
-        
-        # Connect to Cloud CMS
-        client = CloudCMS()
-        platform = client.connect(filename='gitana.json')
-        
-        # List repositories
-        repositories = platform.list_repositories()
-        
-        # Read repository
-        repository = platform.read_repository('<repository_id>')
-        
-        # List branches
-        branches = repository.list_branches()
-        
-        # Read branch
-        branch = repository.read_branch('<branch_id>')
-        
-        # Read Node
-        node = branch.read_node('<node_id>')
-        
-        # Create node
-        obj = {
-            'title': 'Twelfth Night',
-            'description': 'An old play'
-        }
-        newNode = branch.create_node(obj)
-        
-        # Query nodes
-        query = {
-            '_type': 'store:book'
-        }
-        pagination = {
-            'limit': 2
-        }
-        queried_nodes = branch.query_nodes(query, pagination)
-        
-        # Search/Find nodes
-        find = {
-            'search': 'Shakespeare',
-            'query': {
-                '_type': 'store:book'
-            }
-        }
-        searched_nodes = branch.find_nodes(find)
-        ```
-        
-        ## Tests
-        
-        To perform the unit tests for this driver, ensure that you have a `gitana.json` file in the driver directory, then run:
-        
-        ```
-        python -m unittest tests
-        ```
-        
-        ## Resources
-        
-        * Cloud CMS: https://www.cloudcms.com
-        * Github: https://github.com/gitana/cloudcms-python-driver
-        * Python Driver Download: https://pypi.org/project/cloudcms/
-        * Cloud CMS Documentation: https://www.cloudcms.com/documentation.html
-        * Developers Guide: https://www.cloudcms.com/developers.html
-        
-        ## Support
-        
-        For information or questions about the Python Driver, please contact Cloud CMS
-        at [support@cloudcms.com](mailto:support@cloudcms.com).
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Cloud CMS Python Driver
+
+Basic driver for the [Cloud CMS](https://www.cloudcms.com) API
+
+Runs with Python 3
+
+Currently supports the following functionality:
+- Connect to and refresh access tokens with the API
+- Read platform, branch, and repositories
+- Read, query, search, create, update, and delete nodes
+
+## Installation
+
+`pip install cloudcms`
+
+## Examples
+
+Below are some examples of how you might use this driver:
+
+```python
+from cloudcms import CloudCMS
+
+# Connect to Cloud CMS
+client = CloudCMS()
+platform = client.connect(filename='gitana.json')
+
+# List repositories
+repositories = platform.list_repositories()
+
+# Read repository
+repository = platform.read_repository('<repository_id>')
+
+# List branches
+branches = repository.list_branches()
+
+# Read branch
+branch = repository.read_branch('<branch_id>')
+
+# Read Node
+node = branch.read_node('<node_id>')
+
+# Create node
+obj = {
+    'title': 'Twelfth Night',
+    'description': 'An old play'
+}
+newNode = branch.create_node(obj)
+
+# Query nodes
+query = {
+    '_type': 'store:book'
+}
+pagination = {
+    'limit': 2
+}
+queried_nodes = branch.query_nodes(query, pagination)
+
+# Search/Find nodes
+find = {
+    'search': 'Shakespeare',
+    'query': {
+        '_type': 'store:book'
+    }
+}
+searched_nodes = branch.find_nodes(find)
+```
+
+## Tests
+
+To perform the unit tests for this driver, ensure that you have a `gitana.json` file in the driver directory, then run:
+
+```
+python -m unittest tests
+```
+
+## Resources
+
+* Cloud CMS: https://www.cloudcms.com
+* Github: https://github.com/gitana/cloudcms-python-driver
+* Python Driver Download: https://pypi.org/project/cloudcms/
+* Cloud CMS Documentation: https://www.cloudcms.com/documentation.html
+* Developers Guide: https://www.cloudcms.com/developers.html
+
+## Support
+
+For information or questions about the Python Driver, please contact Cloud CMS
+at [support@cloudcms.com](mailto:support@cloudcms.com).
```

### Comparing `cloudcms-1.1.3/cloudcms.egg-info/SOURCES.txt` & `cloudcms-1.1.4/cloudcms.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 cloudcms/__init__.py
 cloudcms/cloudcms.py
 cloudcms.egg-info/PKG-INFO
 cloudcms.egg-info/SOURCES.txt
 cloudcms.egg-info/dependency_links.txt
@@ -40,14 +41,15 @@
 cloudcms/support/qname.py
 tests/__init__.py
 tests/abstract_test.py
 tests/abstract_with_repository_test.py
 tests/test_association.py
 tests/test_attachment.py
 tests/test_branch.py
+tests/test_deployment_target.py
 tests/test_file_folder.py
 tests/test_graphql.py
 tests/test_node.py
 tests/test_platform.py
 tests/test_project.py
 tests/test_release.py
 tests/test_repository.py
```

### Comparing `cloudcms-1.1.3/setup.py` & `cloudcms-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cloudcms',
-    version='1.1.3',
+    version='1.1.4',
     author='Michael Whitman',
     author_email='michael.whitman@cloudcms.com',
     description='Cloud CMS Python Driver',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/gitana/cloudcms-python-driver',
     packages=setuptools.find_packages(),
```

### Comparing `cloudcms-1.1.3/tests/abstract_test.py` & `cloudcms-1.1.4/tests/abstract_test.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_association.py` & `cloudcms-1.1.4/tests/test_association.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_attachment.py` & `cloudcms-1.1.4/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_branch.py` & `cloudcms-1.1.4/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_file_folder.py` & `cloudcms-1.1.4/tests/test_file_folder.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_graphql.py` & `cloudcms-1.1.4/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_node.py` & `cloudcms-1.1.4/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_project.py` & `cloudcms-1.1.4/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_release.py` & `cloudcms-1.1.4/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_repository.py` & `cloudcms-1.1.4/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `cloudcms-1.1.3/tests/test_traverse.py` & `cloudcms-1.1.4/tests/test_traverse.py`

 * *Files identical despite different names*

