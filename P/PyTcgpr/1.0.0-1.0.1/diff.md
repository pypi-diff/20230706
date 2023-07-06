# Comparing `tmp/PyTcgpr-1.0.0.tar.gz` & `tmp/PyTcgpr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTcgpr-1.0.0.tar", last modified: Sun May 14 11:54:56 2023, max compression
+gzip compressed data, was "PyTcgpr-1.0.1.tar", last modified: Thu Jul  6 02:45:03 2023, max compression
```

## Comparing `PyTcgpr-1.0.0.tar` & `PyTcgpr-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-14 11:54:56.492969 PyTcgpr-1.0.0/
--rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-05-14 11:54:56.492840 PyTcgpr-1.0.0/PKG-INFO
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-14 11:54:56.491370 PyTcgpr-1.0.0/PyTcgpr/
--rw-rw-rw-   0 jacob      (501) staff       (20)    12768 2023-05-14 09:04:37.000000 PyTcgpr-1.0.0/PyTcgpr/TCGPR.py
--rw-r--r--   0 jacob      (501) staff       (20)      480 2023-05-14 09:06:54.000000 PyTcgpr-1.0.0/PyTcgpr/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-14 11:54:56.492360 PyTcgpr-1.0.0/PyTcgpr/data/
--rw-rw-rw-   0 jacob      (501) staff       (20)    21513 2023-05-14 10:45:53.000000 PyTcgpr-1.0.0/PyTcgpr/data/DatasetPartition.py
--rw-rw-rw-   0 jacob      (501) staff       (20)    17365 2023-05-14 10:45:49.000000 PyTcgpr-1.0.0/PyTcgpr/data/OutliersIdentification.py
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.0.0/PyTcgpr/data/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-14 11:54:56.492653 PyTcgpr-1.0.0/PyTcgpr/feature/
--rw-rw-rw-   0 jacob      (501) staff       (20)    23959 2023-05-14 10:45:49.000000 PyTcgpr-1.0.0/PyTcgpr/feature/FeaturesSelection.py
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.0.0/PyTcgpr/feature/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-14 11:54:56.491965 PyTcgpr-1.0.0/PyTcgpr.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-05-14 11:54:56.000000 PyTcgpr-1.0.0/PyTcgpr.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      371 2023-05-14 11:54:56.000000 PyTcgpr-1.0.0/PyTcgpr.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 11:54:56.000000 PyTcgpr-1.0.0/PyTcgpr.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       21 2023-05-14 11:54:56.000000 PyTcgpr-1.0.0/PyTcgpr.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        8 2023-05-14 11:54:56.000000 PyTcgpr-1.0.0/PyTcgpr.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1142 2023-05-14 09:09:04.000000 PyTcgpr-1.0.0/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-14 11:54:56.493010 PyTcgpr-1.0.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1404 2023-05-14 09:08:29.000000 PyTcgpr-1.0.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 02:45:03.992197 PyTcgpr-1.0.1/
+-rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-07-06 02:45:03.992064 PyTcgpr-1.0.1/PKG-INFO
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 02:45:03.990628 PyTcgpr-1.0.1/PyTcgpr/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    12770 2023-07-06 02:43:31.000000 PyTcgpr-1.0.1/PyTcgpr/TCGPR.py
+-rw-r--r--   0 jacob      (501) staff       (20)      482 2023-07-06 02:44:04.000000 PyTcgpr-1.0.1/PyTcgpr/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 02:45:03.991646 PyTcgpr-1.0.1/PyTcgpr/data/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    21513 2023-05-14 10:45:53.000000 PyTcgpr-1.0.1/PyTcgpr/data/DatasetPartition.py
+-rw-rw-rw-   0 jacob      (501) staff       (20)    17365 2023-05-14 10:45:49.000000 PyTcgpr-1.0.1/PyTcgpr/data/OutliersIdentification.py
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.0.1/PyTcgpr/data/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 02:45:03.991903 PyTcgpr-1.0.1/PyTcgpr/feature/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    23959 2023-05-14 10:45:49.000000 PyTcgpr-1.0.1/PyTcgpr/feature/FeaturesSelection.py
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.0.1/PyTcgpr/feature/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 02:45:03.991233 PyTcgpr-1.0.1/PyTcgpr.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-07-06 02:45:03.000000 PyTcgpr-1.0.1/PyTcgpr.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      371 2023-07-06 02:45:03.000000 PyTcgpr-1.0.1/PyTcgpr.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-06 02:45:03.000000 PyTcgpr-1.0.1/PyTcgpr.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       21 2023-07-06 02:45:03.000000 PyTcgpr-1.0.1/PyTcgpr.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        8 2023-07-06 02:45:03.000000 PyTcgpr-1.0.1/PyTcgpr.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1142 2023-05-14 09:09:04.000000 PyTcgpr-1.0.1/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-06 02:45:03.992237 PyTcgpr-1.0.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1404 2023-07-06 02:44:22.000000 PyTcgpr-1.0.1/setup.py
```

### Comparing `PyTcgpr-1.0.0/PKG-INFO` & `PyTcgpr-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTcgpr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.
 Home-page: https://github.com/Bin-Cao/TCGPR
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: 17734910905@163.com
 License: MIT License
```

### Comparing `PyTcgpr-1.0.0/PyTcgpr/TCGPR.py` & `PyTcgpr-1.0.1/PyTcgpr/TCGPR.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # =============================================================================
 # Public estimators
 # =============================================================================
 
 
 def fit(filePath, Mission = 'DATA', Task = 'Partition', initial_set_cap=3, sampling_cap=1, 
-    ratio=None, target=1, weight = 2, up_search = None, exploit_coef=2, exploit_model = False, CV =5,
+    ratio=None, target=1, weight = .2, up_search = None, exploit_coef=2, exploit_model = False, CV =5,
     alpha=1e-10, n_restarts_optimizer=10, normalize_y=True,):
 
     """
     Algorithm name: Tree classifier for gaussian process regression
     Tasks : Dataset Partition & Outliers Identification & Features Selection
     Author: Bin CAO <binjacobcao@gmail.com> 
     Zhejiang LAB, HangZhou, CHINA.
@@ -84,15 +84,15 @@
     :param target:
     used in feature selection when Mission = 'FEATURE'
         int, default 1, the number of target in regression mission
         target = 1 for single_task regression and =k for k_task regression (Multiobjective regression)
     otherwise : param target is masked 
     
     :param weight
-    a weight imposed on R value in calculating GGMF, default = 2 , recommend =  1-10
+    a weight imposed on R value in calculating GGMF, default = .2 , recommend =  1-10
     i.e.,
         weight * (1-R) +  mean / std (mean, std is the mean and standard deviation of length scales) 
 
     :param up_search: 
     for Mission = 'DATA':
         up boundary of candidates for brute force search, default = 5e2 , recommend =  2e2-2e3
     for Mission = 'FEATURE':
```

### Comparing `PyTcgpr-1.0.0/PyTcgpr/data/DatasetPartition.py` & `PyTcgpr-1.0.1/PyTcgpr/data/DatasetPartition.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.0.0/PyTcgpr/data/OutliersIdentification.py` & `PyTcgpr-1.0.1/PyTcgpr/data/OutliersIdentification.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.0.0/PyTcgpr/feature/FeaturesSelection.py` & `PyTcgpr-1.0.1/PyTcgpr/feature/FeaturesSelection.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.0.0/PyTcgpr.egg-info/PKG-INFO` & `PyTcgpr-1.0.1/PyTcgpr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTcgpr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.
 Home-page: https://github.com/Bin-Cao/TCGPR
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: 17734910905@163.com
 License: MIT License
```

### Comparing `PyTcgpr-1.0.0/README.md` & `PyTcgpr-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.0.0/setup.py` & `PyTcgpr-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='PyTcgpr',  # 包名
-    version='1.0.0',  # 版本
+    version='1.0.1',  # 版本
     description="Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='17734910905@163.com',  # 维护者邮件
```

