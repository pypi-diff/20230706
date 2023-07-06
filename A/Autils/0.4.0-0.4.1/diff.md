# Comparing `tmp/Autils-0.4.0.tar.gz` & `tmp/Autils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Autils-0.4.0.tar", last modified: Wed Dec  7 07:48:53 2022, max compression
+gzip compressed data, was "Autils-0.4.1.tar", last modified: Thu Jul  6 02:39:59 2023, max compression
```

## Comparing `Autils-0.4.0.tar` & `Autils-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 07:48:53.832007 Autils-0.4.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 07:48:53.788007 Autils-0.4.0/Autils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1514 2022-12-07 07:48:53.000000 Autils-0.4.0/Autils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      627 2022-12-07 07:48:53.000000 Autils-0.4.0/Autils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-07 07:48:53.000000 Autils-0.4.0/Autils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-12-07 07:48:53.000000 Autils-0.4.0/Autils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-12-07 07:48:53.000000 Autils-0.4.0/Autils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-23 01:37:36.000000 Autils-0.4.0/Autils.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)    35821 2022-06-23 01:19:48.000000 Autils-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1514 2022-12-07 07:48:53.832007 Autils-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      776 2022-06-23 01:19:48.000000 Autils-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 07:48:53.796007 Autils-0.4.0/autils/
--rw-r--r--   0 root         (0) root         (0)      207 2022-12-07 07:46:54.000000 Autils-0.4.0/autils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      541 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/authentication.py
--rw-r--r--   0 root         (0) root         (0)      886 2022-12-07 07:45:48.000000 Autils-0.4.0/autils/date.py
--rw-r--r--   0 root         (0) root         (0)     1429 2022-12-07 07:45:41.000000 Autils-0.4.0/autils/datetime.py
--rwxr-xr-x   0 root         (0) root         (0)      476 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/dict.py
--rwxr-xr-x   0 root         (0) root         (0)      619 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/digits.py
--rwxr-xr-x   0 root         (0) root         (0)      199 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/excepts.py
--rwxr-xr-x   0 root         (0) root         (0)      907 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1351 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/ost.py
--rw-r--r--   0 root         (0) root         (0)     5448 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/sign.py
--rwxr-xr-x   0 root         (0) root         (0)      482 2022-06-23 01:19:48.000000 Autils-0.4.0/autils/singleton.py
--rwxr-xr-x   0 root         (0) root         (0)     1025 2022-12-07 07:46:15.000000 Autils-0.4.0/autils/string.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-07 07:48:53.832007 Autils-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1565 2022-06-23 01:19:48.000000 Autils-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 07:48:53.832007 Autils-0.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      471 2022-12-07 07:47:23.000000 Autils-0.4.0/tests/test_date.py
--rw-r--r--   0 root         (0) root         (0)      983 2022-12-07 07:48:01.000000 Autils-0.4.0/tests/test_datetime.py
--rw-r--r--   0 root         (0) root         (0)      299 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/test_dict.py
--rw-r--r--   0 root         (0) root         (0)      266 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/test_digits.py
--rw-r--r--   0 root         (0) root         (0)      488 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/test_dt.py
--rw-r--r--   0 root         (0) root         (0)      204 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)      313 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/test_ost.py
--rw-r--r--   0 root         (0) root         (0)     1244 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/test_sign.py
--rw-r--r--   0 root         (0) root         (0)      482 2022-12-07 07:48:25.000000 Autils-0.4.0/tests/test_str.py
--rw-r--r--   0 root         (0) root         (0)      164 2022-06-23 01:19:48.000000 Autils-0.4.0/tests/test_two_step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:39:59.746431 Autils-0.4.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:39:59.662430 Autils-0.4.1/Autils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-07-06 02:39:59.000000 Autils-0.4.1/Autils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-06 02:39:59.000000 Autils-0.4.1/Autils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 02:39:59.000000 Autils-0.4.1/Autils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-06 02:39:59.000000 Autils-0.4.1/Autils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 02:39:59.000000 Autils-0.4.1/Autils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-23 01:37:36.000000 Autils-0.4.1/Autils.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)    35821 2022-06-23 01:19:48.000000 Autils-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-07-06 02:39:59.746431 Autils-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      776 2022-06-23 01:19:48.000000 Autils-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:39:59.714431 Autils-0.4.1/autils/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-06 02:39:17.000000 Autils-0.4.1/autils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      541 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-07-06 02:37:05.000000 Autils-0.4.1/autils/date.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2022-12-07 07:45:41.000000 Autils-0.4.1/autils/datetime.py
+-rwxr-xr-x   0 root         (0) root         (0)      476 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/dict.py
+-rwxr-xr-x   0 root         (0) root         (0)      619 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/digits.py
+-rwxr-xr-x   0 root         (0) root         (0)      199 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/excepts.py
+-rwxr-xr-x   0 root         (0) root         (0)      907 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/ost.py
+-rw-r--r--   0 root         (0) root         (0)     5448 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/sign.py
+-rwxr-xr-x   0 root         (0) root         (0)      482 2022-06-23 01:19:48.000000 Autils-0.4.1/autils/singleton.py
+-rwxr-xr-x   0 root         (0) root         (0)     1025 2022-12-07 07:46:15.000000 Autils-0.4.1/autils/string.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 02:39:59.746431 Autils-0.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1565 2022-06-23 01:19:48.000000 Autils-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:39:59.746431 Autils-0.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      601 2023-07-06 02:38:02.000000 Autils-0.4.1/tests/test_date.py
+-rw-r--r--   0 root         (0) root         (0)      983 2022-12-07 07:50:19.000000 Autils-0.4.1/tests/test_datetime.py
+-rw-r--r--   0 root         (0) root         (0)      299 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/test_dict.py
+-rw-r--r--   0 root         (0) root         (0)      266 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/test_digits.py
+-rw-r--r--   0 root         (0) root         (0)      488 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/test_dt.py
+-rw-r--r--   0 root         (0) root         (0)      204 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)      313 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/test_ost.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/test_sign.py
+-rw-r--r--   0 root         (0) root         (0)      482 2022-12-07 07:48:25.000000 Autils-0.4.1/tests/test_str.py
+-rw-r--r--   0 root         (0) root         (0)      164 2022-06-23 01:19:48.000000 Autils-0.4.1/tests/test_two_step.py
```

### Comparing `Autils-0.4.0/Autils.egg-info/PKG-INFO` & `Autils-0.4.1/Autils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Autils
-Version: 0.4.0
+Version: 0.4.1
 Summary: A hepler tools for kevin kong
 Home-page: https://github.com/block-cat/autils
 Author: blackcat
 Author-email: kfx2007@163.com
 License: GNU
 Keywords: Autils
 Platform: UNKNOWN
```

### Comparing `Autils-0.4.0/Autils.egg-info/SOURCES.txt` & `Autils-0.4.1/Autils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/LICENSE` & `Autils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/PKG-INFO` & `Autils-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Autils
-Version: 0.4.0
+Version: 0.4.1
 Summary: A hepler tools for kevin kong
 Home-page: https://github.com/block-cat/autils
 Author: blackcat
 Author-email: kfx2007@163.com
 License: GNU
 Keywords: Autils
 Platform: UNKNOWN
```

### Comparing `Autils-0.4.0/README.md` & `Autils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/autils/authentication.py` & `Autils-0.4.1/autils/authentication.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/autils/datetime.py` & `Autils-0.4.1/autils/datetime.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/autils/digits.py` & `Autils-0.4.1/autils/digits.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/autils/logger.py` & `Autils-0.4.1/autils/logger.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/autils/ost.py` & `Autils-0.4.1/autils/ost.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/autils/sign.py` & `Autils-0.4.1/autils/sign.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/autils/string.py` & `Autils-0.4.1/autils/string.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/setup.py` & `Autils-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `Autils-0.4.0/tests/test_datetime.py` & `Autils-0.4.1/tests/test_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         """测试转换本地时间"""
         local = self.date.to_local_time()
         self.assertEqual(datetime.strftime(
             local, '%Y-%m-%d %H:%M:%S'), "2019-12-31 08:00:00")
 
     def test_current_week(self):
         """获取当前第几周"""
-        print(DateTime.get_current_week())
+        print(timeutil.get_current_week())
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `Autils-0.4.0/tests/test_sign.py` & `Autils-0.4.1/tests/test_sign.py`

 * *Files identical despite different names*

