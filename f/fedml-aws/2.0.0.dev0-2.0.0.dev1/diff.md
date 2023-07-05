# Comparing `tmp/fedml_aws-2.0.0.dev0.tar.gz` & `tmp/fedml_aws-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_aws-2.0.0.dev0.tar", last modified: Wed May 11 18:18:25 2022, max compression
+gzip compressed data, was "fedml_aws-2.0.0.dev1.tar", last modified: Wed Jun 28 21:06:04 2023, max compression
```

## Comparing `fedml_aws-2.0.0.dev0.tar` & `fedml_aws-2.0.0.dev1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2022-05-11 18:18:25.875291 fedml_aws-2.0.0.dev0/
--rw-r--r--   0 I542957    (501) staff       (20)    11307 2022-03-30 17:40:46.000000 fedml_aws-2.0.0.dev0/LICENSE.txt
--rw-r--r--   0 I542957    (501) staff       (20)      353 2022-05-11 18:18:25.874759 fedml_aws-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)    10381 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/README.md
--rw-r--r--   0 I542957    (501) staff       (20)      103 2022-03-30 17:40:46.000000 fedml_aws-2.0.0.dev0/pyproject.toml
--rw-r--r--   0 I542957    (501) staff       (20)       38 2022-05-11 18:18:25.875449 fedml_aws-2.0.0.dev0/setup.cfg
--rw-r--r--   0 I542957    (501) staff       (20)      726 2022-05-09 17:47:54.000000 fedml_aws-2.0.0.dev0/setup.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2022-05-11 18:18:25.853792 fedml_aws-2.0.0.dev0/src/
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2022-05-11 18:18:25.867489 fedml_aws-2.0.0.dev0/src/fedml_aws/
--rw-r--r--   0 I542957    (501) staff       (20)      175 2022-05-09 16:52:04.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/__init__.py
--rw-r--r--   0 I542957    (501) staff       (20)     2352 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/build_and_push.sh
--rw-r--r--   0 I542957    (501) staff       (20)     9031 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/dbconnection.py
--rw-r--r--   0 I542957    (501) staff       (20)    22560 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/dwcsagemaker.py
--rw-r--r--   0 I542957    (501) staff       (20)      199 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/install_kubectl.sh
--rw-r--r--   0 I542957    (501) staff       (20)      656 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/logger.py
--rw-r--r--   0 I542957    (501) staff       (20)     4647 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/predictor.py
--rw-r--r--   0 I542957    (501) staff       (20)    16482 2022-05-11 18:16:35.000000 fedml_aws-2.0.0.dev0/src/fedml_aws/script_generator.py
-drwxr-xr-x   0 I542957    (501) staff       (20)        0 2022-05-11 18:18:25.873822 fedml_aws-2.0.0.dev0/src/fedml_aws.egg-info/
--rw-r--r--   0 I542957    (501) staff       (20)      353 2022-05-11 18:18:25.000000 fedml_aws-2.0.0.dev0/src/fedml_aws.egg-info/PKG-INFO
--rw-r--r--   0 I542957    (501) staff       (20)      479 2022-05-11 18:18:25.000000 fedml_aws-2.0.0.dev0/src/fedml_aws.egg-info/SOURCES.txt
--rw-r--r--   0 I542957    (501) staff       (20)        1 2022-05-11 18:18:25.000000 fedml_aws-2.0.0.dev0/src/fedml_aws.egg-info/dependency_links.txt
--rw-r--r--   0 I542957    (501) staff       (20)       36 2022-05-11 18:18:25.000000 fedml_aws-2.0.0.dev0/src/fedml_aws.egg-info/requires.txt
--rw-r--r--   0 I542957    (501) staff       (20)       10 2022-05-11 18:18:25.000000 fedml_aws-2.0.0.dev0/src/fedml_aws.egg-info/top_level.txt
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-28 21:06:04.058340 fedml_aws-2.0.0.dev1/
+-rw-r--r--   0 I542957    (501) staff       (20)      327 2023-06-28 21:06:04.057628 fedml_aws-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)    10515 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/README.md
+-rw-r--r--   0 I542957    (501) staff       (20)      103 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0 I542957    (501) staff       (20)       38 2023-06-28 21:06:04.058524 fedml_aws-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 I542957    (501) staff       (20)      727 2023-06-28 21:05:23.000000 fedml_aws-2.0.0.dev1/setup.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-28 21:06:04.018844 fedml_aws-2.0.0.dev1/src/
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-28 21:06:04.040155 fedml_aws-2.0.0.dev1/src/fedml_aws/
+-rw-r--r--   0 I542957    (501) staff       (20)      175 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/__init__.py
+-rw-r--r--   0 I542957    (501) staff       (20)     2352 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/build_and_push.sh
+-rw-r--r--   0 I542957    (501) staff       (20)    15864 2023-06-28 21:02:54.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/dbconnection.py
+-rw-r--r--   0 I542957    (501) staff       (20)    22560 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/dwcsagemaker.py
+-rw-r--r--   0 I542957    (501) staff       (20)      199 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/install_kubectl.sh
+-rw-r--r--   0 I542957    (501) staff       (20)      656 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/logger.py
+-rw-r--r--   0 I542957    (501) staff       (20)     4647 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/predictor.py
+-rw-r--r--   0 I542957    (501) staff       (20)    16482 2023-06-28 21:02:27.000000 fedml_aws-2.0.0.dev1/src/fedml_aws/script_generator.py
+drwxr-xr-x   0 I542957    (501) staff       (20)        0 2023-06-28 21:06:04.056559 fedml_aws-2.0.0.dev1/src/fedml_aws.egg-info/
+-rw-r--r--   0 I542957    (501) staff       (20)      327 2023-06-28 21:06:03.000000 fedml_aws-2.0.0.dev1/src/fedml_aws.egg-info/PKG-INFO
+-rw-r--r--   0 I542957    (501) staff       (20)      467 2023-06-28 21:06:04.000000 fedml_aws-2.0.0.dev1/src/fedml_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 I542957    (501) staff       (20)        1 2023-06-28 21:06:03.000000 fedml_aws-2.0.0.dev1/src/fedml_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       36 2023-06-28 21:06:03.000000 fedml_aws-2.0.0.dev1/src/fedml_aws.egg-info/requires.txt
+-rw-r--r--   0 I542957    (501) staff       (20)       10 2023-06-28 21:06:03.000000 fedml_aws-2.0.0.dev1/src/fedml_aws.egg-info/top_level.txt
```

### Comparing `fedml_aws-2.0.0.dev0/README.md` & `fedml_aws-2.0.0.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **DwcSagemaker class**
 
-DwcSagemaker class initializes the resources required for the model training, and provides methods that enable the training data to be read from SAP DWC and trains a Machine Learning model on Amazon Sagemaker.
+DwcSagemaker class initializes the resources required for the model training, and provides methods that enable the training data to be read from SAP SAP Datasphere and trains a Machine Learning model on Amazon Sagemaker.
 
 ## **Prerequisites**
 - `sagemaker>=2`
 
 To update `sagemaker` module, run the following code:
 
 `!pip install --upgrade "sagemaker>=2"`
@@ -149,14 +149,16 @@
 You must have an IAM user that does not have MFA enabled and has EC2 container registry access permissions for pushing and pulling to ecr.
 https://docs.aws.amazon.com/AmazonECR/latest/userguide/registry_auth.html
 
 You must also create a profile using aws cli in jupyterlab that connects to the IAM user with EC2 container registry access permissions. 
 The name of this profile is then passed to the function as `profile_name`. Please ensure the region of this profile is the same region as the jupyter instance.
 https://docs.aws.amazon.com/cli/latest/reference/configure/index.html
 
+Finally, you also need a Kyma service account and a kubeconfig.yml that specifies the credentials for your Kyma account. 
+
 ### **Parameters**:
 
 **`clf` [(str)](https://docs.python.org/3/library/stdtypes.html#str) or [(Sagemaker SKLearn Estimator)](https://sagemaker.readthedocs.io/en/stable/frameworks/sklearn/sagemaker.sklearn.html)**
 
 The model to deploy. This can either be a string of the name of the training job in AWS Sagemaker Training Jobs, or the estimator object itself.
 
 **`initial_instance_count` [(int)](https://docs.python.org/3/library/functions.html#int):**
```

### Comparing `fedml_aws-2.0.0.dev0/setup.py` & `fedml_aws-2.0.0.dev1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="fedml_aws",
-    version="2.0.0.dev",
+    version="2.0.0.dev1",
     author="SAP SE",
     description="A python library for building machine learning models on AWS Sagemaker using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

### Comparing `fedml_aws-2.0.0.dev0/src/fedml_aws/build_and_push.sh` & `fedml_aws-2.0.0.dev1/src/fedml_aws/build_and_push.sh`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.0.dev0/src/fedml_aws/dwcsagemaker.py` & `fedml_aws-2.0.0.dev1/src/fedml_aws/dwcsagemaker.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.0.dev0/src/fedml_aws/logger.py` & `fedml_aws-2.0.0.dev1/src/fedml_aws/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.0.dev0/src/fedml_aws/predictor.py` & `fedml_aws-2.0.0.dev1/src/fedml_aws/predictor.py`

 * *Files identical despite different names*

### Comparing `fedml_aws-2.0.0.dev0/src/fedml_aws/script_generator.py` & `fedml_aws-2.0.0.dev1/src/fedml_aws/script_generator.py`

 * *Files identical despite different names*

