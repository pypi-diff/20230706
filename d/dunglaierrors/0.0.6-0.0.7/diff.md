# Comparing `tmp/dunglaierrors-0.0.6.tar.gz` & `tmp/dunglaierrors-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dunglaierrors-0.0.6.tar", last modified: Tue Jul 12 14:49:47 2022, max compression
+gzip compressed data, was "C:\Users\HIEU\Documents\dunglaierror\dist\.tmp-jh61sjdi\dunglaierrors-0.0.7.tar", last modified: Thu Jul  6 17:30:03 2023, max compression
```

## Comparing `dunglaierrors-0.0.6.tar` & `dunglaierrors-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-07-12 14:49:47.212899 dunglaierrors-0.0.6/
--rw-rw-rw-   0        0        0     1092 2022-07-12 06:59:19.000000 dunglaierrors-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1833 2022-07-12 14:49:47.211897 dunglaierrors-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1337 2022-07-12 06:43:25.000000 dunglaierrors-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-07-12 14:49:47.187898 dunglaierrors-0.0.6/dunglaierrors/
--rw-rw-rw-   0        0        0   139243 2022-07-12 14:49:27.000000 dunglaierrors-0.0.6/dunglaierrors/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-12 14:49:47.209899 dunglaierrors-0.0.6/dunglaierrors.egg-info/
--rw-rw-rw-   0        0        0     1833 2022-07-12 14:49:46.000000 dunglaierrors-0.0.6/dunglaierrors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2022-07-12 14:49:47.000000 dunglaierrors-0.0.6/dunglaierrors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-12 14:49:46.000000 dunglaierrors-0.0.6/dunglaierrors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-07-12 14:49:46.000000 dunglaierrors-0.0.6/dunglaierrors.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-07-12 14:49:46.000000 dunglaierrors-0.0.6/dunglaierrors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-12 14:49:47.213899 dunglaierrors-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1257 2022-07-12 14:49:42.000000 dunglaierrors-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:30:03.011948 dunglaierrors-0.0.7/
+-rw-rw-rw-   0        0        0     1092 2023-07-06 17:27:14.000000 dunglaierrors-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1833 2023-07-06 17:30:03.010947 dunglaierrors-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1337 2023-07-06 17:27:14.000000 dunglaierrors-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 17:30:02.986809 dunglaierrors-0.0.7/dunglaierrors/
+-rw-rw-rw-   0        0        0   139245 2023-07-06 17:27:14.000000 dunglaierrors-0.0.7/dunglaierrors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:30:03.008946 dunglaierrors-0.0.7/dunglaierrors.egg-info/
+-rw-rw-rw-   0        0        0     1833 2023-07-06 17:30:02.000000 dunglaierrors-0.0.7/dunglaierrors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-06 17:30:02.000000 dunglaierrors-0.0.7/dunglaierrors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 17:30:02.000000 dunglaierrors-0.0.7/dunglaierrors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 17:30:02.000000 dunglaierrors-0.0.7/dunglaierrors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 17:30:02.000000 dunglaierrors-0.0.7/dunglaierrors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 17:30:03.011948 dunglaierrors-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1257 2023-07-06 17:27:52.000000 dunglaierrors-0.0.7/setup.py
```

### Comparing `dunglaierrors-0.0.6/LICENSE` & `dunglaierrors-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dunglaierrors-0.0.6/PKG-INFO` & `dunglaierrors-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunglaierrors
-Version: 0.0.6
+Version: 0.0.7
 Summary: Detect Dung Lai's common errors
 Home-page: https://github.com/MHP0920/dunglaierror
 Author: MHP
 Author-email: admin@hieudeeptry.ml
 License: MIT
 Keywords: dunglai,error,python,python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dunglaierrors-0.0.6/README.md` & `dunglaierrors-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dunglaierrors-0.0.6/dunglaierrors/__init__.py` & `dunglaierrors-0.0.7/dunglaierrors/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 
 class Docs:
     def doitiente(self) -> str:
         '''
         Thông tin về cách chuyển đổi tiền tệ (Vd: USD -> VND)
         '''
         _1 = colorama.Fore.LIGHTGREEN_EX + '-'*20 + ' ' + 'Cách chuyển đổi tiền tệ (Vd: USD -> VND)' + ' ' + '-'*20 + colorama.Fore.RESET
-        _2 = colorama.Fore.LIGHTCYAN_EX + '1. Xác định tỉ giá USD/VND, 1 USD = 23.000 VND' + colorama.Fore.RESET
+        _2 = colorama.Fore.LIGHTCYAN_EX + '1. Xác định tỉ giá USD/VND, 1 USD = 22.000 VND' + colorama.Fore.RESET
         _3 = colorama.Fore.LIGHTCYAN_EX + '2. Tính tổng tiền cần chuyển đổi' + colorama.Fore.RESET
         _4 = colorama.Fore.LIGHTCYAN_EX + '3. Tính tổng tiền sau khi chuyển đổi' + colorama.Fore.RESET
         _5 = colorama.Fore.LIGHTCYAN_EX + '4. Hiển thị kết quả' + colorama.Fore.RESET
         _7 = colorama.Fore.LIGHTGREEN_EX + '-'*20 + ' ' + 'Example code' + ' ' + '-'*20 + colorama.Fore.RESET
         _8 = colorama.Fore.LIGHTCYAN_EX + '''
 USD = int(input('Nhập số tiền USD: '))
-VND = USD * 23000
+VND = USD * 22000
 print('Số tiền sau khi chuyển đổi là: ', VND)
         ''' + colorama.Fore.RESET
         _9 = colorama.Fore.LIGHTGREEN_EX + '-'*20 + ' ' + 'Example Input' + ' ' + '-'*20 + colorama.Fore.RESET
         _10 = colorama.Fore.LIGHTCYAN_EX + '''
 Nhập số tiền USD: 100
         ''' + colorama.Fore.RESET
         _11 = colorama.Fore.LIGHTGREEN_EX + '-'*20 + ' ' + 'Example Output' + ' ' + '-'*20 + colorama.Fore.RESET
         _12 = colorama.Fore.LIGHTCYAN_EX + '''
-Số tiền sau khi chuyển đổi là: 2300000
+Số tiền sau khi chuyển đổi là: 2200000
         ''' + colorama.Fore.RESET
         _13 = colorama.Fore.LIGHTGREEN_EX + '-'*20 + ' ' + 'End of text' + ' ' + '-'*20 + colorama.Fore.RESET
         return '\n'.join([_1,_2,_3,_4,_5,_7,_8,_9,_10,_11,_12,_13])
     
     def ifelse(self) -> str:
         '''
         Thông tin về cách sử dụng if else
@@ -11666,8 +11666,8 @@
 yểu
 yểu điệu
 yếu
 yếu điểm
 yếu đuối
 yếu lược
 yếu nhân
-yếu tố'''
+yếu tố'''
```

### Comparing `dunglaierrors-0.0.6/dunglaierrors.egg-info/PKG-INFO` & `dunglaierrors-0.0.7/dunglaierrors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunglaierrors
-Version: 0.0.6
+Version: 0.0.7
 Summary: Detect Dung Lai's common errors
 Home-page: https://github.com/MHP0920/dunglaierror
 Author: MHP
 Author-email: admin@hieudeeptry.ml
 License: MIT
 Keywords: dunglai,error,python,python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dunglaierrors-0.0.6/setup.py` & `dunglaierrors-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dunglaierrors",                     # This is the name of the package
-    version="0.0.6",                        # The initial release version
+    version="0.0.7",                        # The initial release version
     author="MHP",                     # Full name of the author
     author_email='admin@hieudeeptry.ml',
     keywords=['dunglai', 'error', 'python', 'python3'],
     url='https://github.com/MHP0920/dunglaierror',
     license="MIT",
     description="Detect Dung Lai's common errors",
     long_description=long_description,      # Long description read from the the readme file
```

