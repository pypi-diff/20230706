# Comparing `tmp/rosecape_airflow-0.0.6.tar.gz` & `tmp/rosecape_airflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosecape_airflow-0.0.6.tar", last modified: Thu Jun  1 17:28:45 2023, max compression
+gzip compressed data, was "rosecape_airflow-0.0.7.tar", last modified: Thu Jul  6 11:58:22 2023, max compression
```

## Comparing `rosecape_airflow-0.0.6.tar` & `rosecape_airflow-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.809230 rosecape_airflow-0.0.6/
--rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-06-01 17:28:45.809057 rosecape_airflow-0.0.6/PKG-INFO
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.794604 rosecape_airflow-0.0.6/rosecape_airflow/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:02:59.000000 rosecape_airflow-0.0.6/rosecape_airflow/__init__.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.808362 rosecape_airflow-0.0.6/rosecape_airflow/aws/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:57.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/__init__.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     1801 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/ec2.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     3941 2023-05-29 14:43:16.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/ecs.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)    10137 2023-06-01 17:23:56.000000 rosecape_airflow-0.0.6/rosecape_airflow/aws/efs.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.808807 rosecape_airflow-0.0.6/rosecape_airflow/slack/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:52.000000 rosecape_airflow-0.0.6/rosecape_airflow/slack/__init__.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     1507 2023-05-29 12:48:08.000000 rosecape_airflow-0.0.6/rosecape_airflow/slack/task_failed_slack_alert.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-06-01 17:28:45.795449 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/
--rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/PKG-INFO
--rw-r--r--   0 nickjoanis   (501) staff       (20)      438 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)        1 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       16 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/requires.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       17 2023-06-01 17:28:45.000000 rosecape_airflow-0.0.6/rosecape_airflow.egg-info/top_level.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       38 2023-06-01 17:28:45.809300 rosecape_airflow-0.0.6/setup.cfg
--rw-r--r--   0 nickjoanis   (501) staff       (20)      743 2023-06-01 17:24:06.000000 rosecape_airflow-0.0.6/setup.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-07-06 11:58:22.992874 rosecape_airflow-0.0.7/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-07-06 11:58:22.992717 rosecape_airflow-0.0.7/PKG-INFO
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-07-06 11:58:22.990926 rosecape_airflow-0.0.7/rosecape_airflow/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:02:59.000000 rosecape_airflow-0.0.7/rosecape_airflow/__init__.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-07-06 11:58:22.992211 rosecape_airflow-0.0.7/rosecape_airflow/aws/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:57.000000 rosecape_airflow-0.0.7/rosecape_airflow/aws/__init__.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     1801 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.7/rosecape_airflow/aws/ec2.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     3941 2023-05-29 14:43:16.000000 rosecape_airflow-0.0.7/rosecape_airflow/aws/ecs.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)    10137 2023-07-06 11:56:45.000000 rosecape_airflow-0.0.7/rosecape_airflow/aws/efs.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-07-06 11:58:22.992499 rosecape_airflow-0.0.7/rosecape_airflow/slack/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:52.000000 rosecape_airflow-0.0.7/rosecape_airflow/slack/__init__.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     1507 2023-05-29 12:48:08.000000 rosecape_airflow-0.0.7/rosecape_airflow/slack/task_failed_slack_alert.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-07-06 11:58:22.991632 rosecape_airflow-0.0.7/rosecape_airflow.egg-info/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-07-06 11:58:22.000000 rosecape_airflow-0.0.7/rosecape_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      438 2023-07-06 11:58:22.000000 rosecape_airflow-0.0.7/rosecape_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        1 2023-07-06 11:58:22.000000 rosecape_airflow-0.0.7/rosecape_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       16 2023-07-06 11:58:22.000000 rosecape_airflow-0.0.7/rosecape_airflow.egg-info/requires.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       17 2023-07-06 11:58:22.000000 rosecape_airflow-0.0.7/rosecape_airflow.egg-info/top_level.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       38 2023-07-06 11:58:22.992926 rosecape_airflow-0.0.7/setup.cfg
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      743 2023-07-06 11:58:16.000000 rosecape_airflow-0.0.7/setup.py
```

### Comparing `rosecape_airflow-0.0.6/rosecape_airflow/aws/ec2.py` & `rosecape_airflow-0.0.7/rosecape_airflow/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.6/rosecape_airflow/aws/ecs.py` & `rosecape_airflow-0.0.7/rosecape_airflow/aws/ecs.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.6/rosecape_airflow/aws/efs.py` & `rosecape_airflow-0.0.7/rosecape_airflow/aws/efs.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             logging.info('Mount target created: %s', mount_target)
 
             waiter_config = {
                 "version": 2,
                 "waiters": {
                     "EFSMountTargetLifeCycleStateWaiter": {
                         "operation": "DescribeMountTargets",
-                        "delay": 10,
+                        "delay": 30,
                         "maxAttempts": 10,
                         "acceptors": [
                             {
                                 "state": "success",
                                 "matcher": "path",
                                 "argument": f"length(MountTargets[?MountTargetId == '{mount_target['MountTargetId']}'] | [?"
                                                 f"LifeCycleState == 'available'"
```

### Comparing `rosecape_airflow-0.0.6/rosecape_airflow/slack/task_failed_slack_alert.py` & `rosecape_airflow-0.0.7/rosecape_airflow/slack/task_failed_slack_alert.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.6/setup.py` & `rosecape_airflow-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Airflow utilities'
 LONG_DESCRIPTION = 'A package that makes it easy to interact with AWS services from Airflow using PythonOperator'
 
 setup(
     name="rosecape_airflow",
     version=VERSION,
     description=DESCRIPTION,
```

