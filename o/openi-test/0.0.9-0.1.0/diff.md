# Comparing `tmp/openi-test-0.0.9.tar.gz` & `tmp/openi-test-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi-test-0.0.9.tar", last modified: Fri Jun  9 02:04:42 2023, max compression
+gzip compressed data, was "dist\openi-test-0.1.0.tar", last modified: Thu Jul  6 07:50:11 2023, max compression
```

## Comparing `openi-test-0.0.9.tar` & `openi-test-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 02:04:42.551477 openi-test-0.0.9/
--rw-rw-rw-   0        0        0     1994 2023-06-09 02:04:42.548668 openi-test-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-06-08 09:05:33.000000 openi-test-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 02:04:42.552474 openi-test-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-06-09 02:04:38.000000 openi-test-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:04:42.491321 openi-test-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 02:04:42.499319 openi-test-0.0.9/src/openi/
--rw-rw-rw-   0        0        0       44 2023-06-08 10:08:34.000000 openi-test-0.0.9/src/openi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:04:42.507319 openi-test-0.0.9/src/openi/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.0.9/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0    10925 2023-06-08 07:26:17.000000 openi-test-0.0.9/src/openi/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:04:42.529678 openi-test-0.0.9/src/openi/utils/
--rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.0.9/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi-test-0.0.9/src/openi/utils/helper.py
--rw-rw-rw-   0        0        0     1440 2023-06-09 01:59:04.000000 openi-test-0.0.9/src/openi/utils/minio.py
--rw-rw-rw-   0        0        0     1718 2023-06-08 07:56:06.000000 openi-test-0.0.9/src/openi/utils/modelarts.py
--rw-rw-rw-   0        0        0     2370 2023-06-09 01:59:04.000000 openi-test-0.0.9/src/openi/utils/obs.py
--rw-rw-rw-   0        0        0     2146 2023-06-09 02:02:42.000000 openi-test-0.0.9/src/openi/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 02:04:42.546670 openi-test-0.0.9/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     1994 2023-06-09 02:04:42.000000 openi-test-0.0.9/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-06-09 02:04:42.000000 openi-test-0.0.9/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 02:04:42.000000 openi-test-0.0.9/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-09 02:04:42.000000 openi-test-0.0.9/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 02:04:42.000000 openi-test-0.0.9/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 07:50:11.063827 openi-test-0.1.0/
+-rw-rw-rw-   0        0        0     4160 2023-07-06 07:50:11.057823 openi-test-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2858 2023-07-05 10:13:44.000000 openi-test-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 07:50:11.064822 openi-test-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-06 07:43:13.000000 openi-test-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:50:10.970823 openi-test-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 07:50:10.984826 openi-test-0.1.0/src/openi/
+-rw-rw-rw-   0        0        0      120 2023-07-05 10:23:41.000000 openi-test-0.1.0/src/openi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:50:10.992824 openi-test-0.1.0/src/openi/dataset/
+-rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.1.0/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0    12954 2023-07-05 09:26:46.000000 openi-test-0.1.0/src/openi/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:50:11.006825 openi-test-0.1.0/src/openi/utils/
+-rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.1.0/src/openi/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:50:11.041826 openi-test-0.1.0/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     4160 2023-07-06 07:50:10.000000 openi-test-0.1.0/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-06 07:50:10.000000 openi-test-0.1.0/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:50:10.000000 openi-test-0.1.0/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-06 07:50:10.000000 openi-test-0.1.0/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:50:10.000000 openi-test-0.1.0/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 07:50:11.051827 openi-test-0.1.0/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi-test-0.1.0/test/test_upload_multi.py
```

### Comparing `openi-test-0.0.9/setup.py` & `openi-test-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# python setup.py sdist bdist_wheel  
-# twine upload dist/*    
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
+# twine upload --repository testpypi dist/*
+# pip install -i https://test.pypi.org/pypi/ --extra-index-url https://pypi.org/simple <your_package_in_testpypi>
 
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-test',
-    version='0.0.9',
+    version='0.1.0',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
-    packages=find_packages('src'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
     author_email='chenzh.ds@outlook.com',
     license='MIT',
     classifiers=[
```

