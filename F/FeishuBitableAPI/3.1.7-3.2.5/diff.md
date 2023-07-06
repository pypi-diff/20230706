# Comparing `tmp/FeishuBitableAPI-3.1.7.tar.gz` & `tmp/FeishuBitableAPI-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeishuBitableAPI-3.1.7.tar", last modified: Mon Jul  3 09:07:25 2023, max compression
+gzip compressed data, was "FeishuBitableAPI-3.2.5.tar", last modified: Thu Jul  6 09:13:31 2023, max compression
```

## Comparing `FeishuBitableAPI-3.1.7.tar` & `FeishuBitableAPI-3.2.5.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:07:25.045332 FeishuBitableAPI-3.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:07:25.045332 FeishuBitableAPI-3.1.7/FeishuBitableAPI/
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/BUILD_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/CHECK_FIELD_EXIST.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/CREATE_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/CREATE_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/CREATE_TABLE_QUICK.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/DELETE_FIELDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/DELETE_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/FeishuBitableAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_FIELD_INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_INFO_FROM_URL.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_LOGIN_CODE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_RECORD_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_TABLE_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_VIEW_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_FIELDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_RECORDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_TABLES.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_VIEWS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/UPDATE_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/UPDATE_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_FIELD_INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_INFO_FROM_URL.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_LOGIN_CODE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_RECORD_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_TABLE_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_VIEW_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 09:07:17.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:07:25.045332 FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 09:07:25.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-03 09:07:25.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:07:25.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 09:07:25.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 09:07:25.000000 FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 09:07:09.000000 FeishuBitableAPI-3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-03 09:07:25.045332 FeishuBitableAPI-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 09:07:09.000000 FeishuBitableAPI-3.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:07:25.045332 FeishuBitableAPI-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 09:07:09.000000 FeishuBitableAPI-3.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:07:25.045332 FeishuBitableAPI-3.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-03 09:07:09.000000 FeishuBitableAPI-3.1.7/test/test#GET_INFO_FROM_URL-2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 09:07:09.000000 FeishuBitableAPI-3.1.7/test/test#GET_INFO_FROM_URL.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:31.351940 FeishuBitableAPI-3.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:31.347940 FeishuBitableAPI-3.2.5/FeishuBitableAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/BUILD_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/CHECK_FIELD_EXIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/CONVERSION_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/CREATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/CREATE_TABLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/CREATE_TABLE_QUICK.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/DELETE_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/DELETE_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/FeishuBitableAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_RECORDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_TABLES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_VIEWS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/UPDATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/UPDATE_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-06 09:13:23.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:31.351940 FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-06 09:13:31.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-06 09:13:31.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:13:31.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 09:13:31.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 09:13:31.000000 FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 09:13:12.000000 FeishuBitableAPI-3.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-06 09:13:31.351940 FeishuBitableAPI-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 09:13:12.000000 FeishuBitableAPI-3.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:13:31.351940 FeishuBitableAPI-3.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-06 09:13:12.000000 FeishuBitableAPI-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:31.351940 FeishuBitableAPI-3.2.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-06 09:13:12.000000 FeishuBitableAPI-3.2.5/test/test#GET_INFO_FROM_URL-2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-06 09:13:12.000000 FeishuBitableAPI-3.2.5/test/test#GET_INFO_FROM_URL.py
```

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/BUILD_FIELD.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/BUILD_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/CHECK_FIELD_EXIST.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/CHECK_FIELD_EXIST.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/CREATE_FIELD.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/CREATE_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/CREATE_TABLE.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/CREATE_TABLE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/CREATE_TABLE_QUICK.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/CREATE_TABLE_QUICK.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/DELETE_FIELDS.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/DELETE_FIELDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/DELETE_RECORD.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/DELETE_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/FeishuBitableAPI.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/FeishuBitableAPI.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .GET_APP_ACCESS_TOKEN import GET_APP_ACCESS_TOKEN
 from .GET_FIELD_INFO import GET_FIELD_INFO, GET_FIELD_ID, GET_FIELD_NAME
-from .GET_INFO_FROM_URL import GET_INFO_FROM_URL,GET_INFO_FROM_URL_JSON,GET_APPTOKEN_FROM_URL,GET_TABLEID_FROM_URL,GET_VIEWID_FROM_URL
+from .GET_INFO_FROM_URL import GET_INFO_FROM_URL, GET_INFO_FROM_URL_JSON, GET_APPTOKEN_FROM_URL, GET_TABLEID_FROM_URL, GET_VIEWID_FROM_URL
 from .GET_LOGIN_CODE import GET_LOGIN_CODE
 from .GET_RECORD_ID import GET_RECORD_ID
 from .GET_RECORD import GET_RECORD
 from .GET_TABLE_ID import GET_TABLE_ID
 from .GET_USER_ACCESS_TOKEN import GET_USER_ACCESS_TOKEN
 from .GET_VIEW_ID import GET_VIEW_ID
 
@@ -35,14 +35,16 @@
 from .BUILD_FIELD import BUILD_FIELD
 
 from .UPDATE_FIELD import UPDATE_FIELD
 from .UPDATE_RECORD import UPDATE_RECORD
 
 from .ADD_RECORDS_FROM_CSV import ADD_RECORDS_FROM_CSV
 
+from CONVERSION_FIELDS import CONVERSION_FIELDS_HUMAN_TO_MACHINE, CONVERSION_FIELDS_MACHINE_TO_HUMAN
+
 
 class FeishuBitableAPI:
     def __init__(self):
         pass
 
     # 调用 ping 函数进行验证
     def ping(self):
@@ -181,8 +183,14 @@
     
     #UPDATE_RECORD
     def UPDATE_RECORD(self, app_token=None, table_id=None, record_id=None, fields=None, config_file=None):
         return UPDATE_RECORD(app_token, table_id, record_id, fields, config_file)
     
     #ADD_RECORDS_FROM_CSV
     def ADD_RECORDS_FROM_CSV(self, app_token=None, table_id=None, view_id=None, page_token=None, page_size=None, csv_file=None, config_file=None, field_file=None):
-        return ADD_RECORDS_FROM_CSV(app_token, table_id, view_id, page_token, page_size, csv_file, config_file, field_file)
+        return ADD_RECORDS_FROM_CSV(app_token, table_id, view_id, page_token, page_size, csv_file, config_file, field_file)
+    
+    #CONVERSION_FIELDS
+    def CONVERSION_FIELDS_HUMAN_TO_MACHINE(self, app_token=None, table_id=None, view_id=None, page_token=None, page_size=None, config_file=None):
+        return CONVERSION_FIELDS_HUMAN_TO_MACHINE(app_token, table_id, view_id, page_token, page_size, config_file)
+    def CONVERSION_FIELDS_MACHINE_TO_HUMAN(app_token=None, table_id=None, view_id=None, page_token=None, page_size=None, config_file=None):
+        return CONVERSION_FIELDS_MACHINE_TO_HUMAN(app_token, table_id, view_id, page_token, page_size, config_file)
```

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_FIELD_INFO.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_FIELD_INFO.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_INFO_FROM_URL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_LOGIN_CODE.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_LOGIN_CODE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_RECORD.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_RECORD_ID.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_RECORD_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_TABLE_ID.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_TABLE_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/GET_VIEW_ID.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/GET_VIEW_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_FIELDS.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_FIELDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_RECORDS.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_RECORDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_TABLES.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_TABLES.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/LIST_VIEWS.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/LIST_VIEWS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/UPDATE_FIELD.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/UPDATE_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/UPDATE_RECORD.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/UPDATE_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_FIELD_INFO.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_FIELD_INFO.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_INFO_FROM_URL.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_INFO_FROM_URL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_LOGIN_CODE.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_LOGIN_CODE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_RECORD_ID.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_RECORD_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_TABLE_ID.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_TABLE_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/WRITE_VIEW_ID.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/WRITE_VIEW_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI/setup.py` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FeishuBitableAPI',
-    version='3.1.7',
+    version='3.2.5',
     packages=find_packages(),
     #py_modules=[],
     url='https://github.com/BlueSkyXN/Feishu-Bitable-Python-API',
     author='BlueSkyXN',
     author_email='bluesky@000714.xyz',
     description='A Python API for Feishu Bitable',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
```

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/PKG-INFO` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.1.7
+Version: 3.2.5
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.1.7/FeishuBitableAPI.egg-info/SOURCES.txt` & `FeishuBitableAPI-3.2.5/FeishuBitableAPI.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py
 FeishuBitableAPI/BUILD_FIELD.py
 FeishuBitableAPI/CHECK_FIELD_EXIST.py
 FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py
+FeishuBitableAPI/CONVERSION_FIELDS.py
 FeishuBitableAPI/CREATE_FIELD.py
 FeishuBitableAPI/CREATE_TABLE.py
 FeishuBitableAPI/CREATE_TABLE_QUICK.py
 FeishuBitableAPI/DELETE_FIELDS.py
 FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py
 FeishuBitableAPI/DELETE_RECORD.py
 FeishuBitableAPI/FeishuBitableAPI.py
```

### Comparing `FeishuBitableAPI-3.1.7/LICENSE` & `FeishuBitableAPI-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/PKG-INFO` & `FeishuBitableAPI-3.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.1.7
+Version: 3.2.5
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.1.7/README.md` & `FeishuBitableAPI-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.1.7/setup.py` & `FeishuBitableAPI-3.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FeishuBitableAPI',
-    version='3.1.7',
+    version='3.2.5',
     packages=find_packages(),
     #py_modules=[],
     url='https://github.com/BlueSkyXN/Feishu-Bitable-Python-API',
     author='BlueSkyXN',
     author_email='bluesky@000714.xyz',
     description='A Python API for Feishu Bitable',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
```

### Comparing `FeishuBitableAPI-3.1.7/test/test#GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.2.5/test/test#GET_INFO_FROM_URL.py`

 * *Files identical despite different names*

