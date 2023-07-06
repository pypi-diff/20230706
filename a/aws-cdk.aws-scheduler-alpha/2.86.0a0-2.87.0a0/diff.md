# Comparing `tmp/aws-cdk.aws-scheduler-alpha-2.86.0a0.tar.gz` & `tmp/aws-cdk.aws-scheduler-alpha-2.87.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src3755887465/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.86.0a0.tar", last modified: Thu Jun 29 08:23:31 2023, max compression
+gzip compressed data, was "/codebuild/output/src94387485/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.87.0a0.tar", last modified: Thu Jul  6 16:50:30 2023, max compression
```

## Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0.tar` & `aws-cdk.aws-scheduler-alpha-2.87.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8262 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7255 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/
--rw-r--r--   0 root         (0) root         (0)    22132 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25662 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8262 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9490 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8483 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/aws_scheduler_alpha/
+-rw-r--r--   0 root         (0) root         (0)    31152 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36742 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.87.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:50:23.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/aws_scheduler_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9490 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 16:50:30.000000 aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0/LICENSE` & `aws-cdk.aws-scheduler-alpha-2.87.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.87.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-scheduler-alpha
-Version: 2.86.0a0
+Version: 2.87.0a0
 Summary: The CDK Construct Library for Amazon Scheduler
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -59,15 +59,21 @@
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project. It allows you to define Event Bridge Schedules.
 
 > This module is in active development. Some features may not be implemented yet.
 
 ## Defining a schedule
 
-TODO: Schedule is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+TODO: Schedule is not yet fully implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+
+Only an L2 class is created that wraps the L1 class and handles the following properties:
+
+* schedule
+* target (only LambdaInvoke is supported for now)
+* flexibleTimeWindow will be set to `{ mode: 'OFF' }`
 
 ### Schedule Expressions
 
 You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
 
 Both rate-based and cron-based schedules are recurring schedules. You can configure each recurring schedule type using a schedule expression. For
 cron-based schedule you can specify a time zone in which EventBridge Scheduler evaluates the expression.
@@ -112,17 +118,39 @@
 
 TODO: Group is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ## Scheduler Targets
 
 TODO: Scheduler Targets Module is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
+Only LambdaInvoke target is added for now.
+
 ### Input
 
-TODO: Target Input is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+Target can be invoked with a custom input. Class `ScheduleTargetInput` supports free form text input and JSON-formatted object input:
+
+```python
+input = ScheduleTargetInput.from_object({
+    "QueueName": "MyQueue"
+})
+```
+
+You can include context attributes in your target payload. EventBridge Scheduler will replace each keyword with
+its respective value and deliver it to the target. See
+[full list of supported context attributes](https://docs.aws.amazon.com/scheduler/latest/UserGuide/managing-schedule-context-attributes.html):
+
+1. `ContextAttribute.scheduleArn()` – The ARN of the schedule.
+2. `ContextAttribute.scheduledTime()` – The time you specified for the schedule to invoke its target, for example, 2022-03-22T18:59:43Z.
+3. `ContextAttribute.executionId()` – The unique ID that EventBridge Scheduler assigns for each attempted invocation of a target, for example, d32c5kddcf5bb8c3.
+4. `ContextAttribute.attemptNumber()` – A counter that identifies the attempt number for the current invocation, for example, 1.
+
+```python
+text = f"Attempt number: {ContextAttribute.attemptNumber}"
+input = ScheduleTargetInput.from_text(text)
+```
 
 ### Specifying Execution Role
 
 TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ### Cross-account and cross-region targets
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0/README.md` & `aws-cdk.aws-scheduler-alpha-2.87.0a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -32,15 +32,21 @@
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project. It allows you to define Event Bridge Schedules.
 
 > This module is in active development. Some features may not be implemented yet.
 
 ## Defining a schedule
 
-TODO: Schedule is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+TODO: Schedule is not yet fully implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+
+Only an L2 class is created that wraps the L1 class and handles the following properties:
+
+* schedule
+* target (only LambdaInvoke is supported for now)
+* flexibleTimeWindow will be set to `{ mode: 'OFF' }`
 
 ### Schedule Expressions
 
 You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
 
 Both rate-based and cron-based schedules are recurring schedules. You can configure each recurring schedule type using a schedule expression. For
 cron-based schedule you can specify a time zone in which EventBridge Scheduler evaluates the expression.
@@ -85,17 +91,39 @@
 
 TODO: Group is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ## Scheduler Targets
 
 TODO: Scheduler Targets Module is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
+Only LambdaInvoke target is added for now.
+
 ### Input
 
-TODO: Target Input is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+Target can be invoked with a custom input. Class `ScheduleTargetInput` supports free form text input and JSON-formatted object input:
+
+```python
+input = ScheduleTargetInput.from_object({
+    "QueueName": "MyQueue"
+})
+```
+
+You can include context attributes in your target payload. EventBridge Scheduler will replace each keyword with
+its respective value and deliver it to the target. See
+[full list of supported context attributes](https://docs.aws.amazon.com/scheduler/latest/UserGuide/managing-schedule-context-attributes.html):
+
+1. `ContextAttribute.scheduleArn()` – The ARN of the schedule.
+2. `ContextAttribute.scheduledTime()` – The time you specified for the schedule to invoke its target, for example, 2022-03-22T18:59:43Z.
+3. `ContextAttribute.executionId()` – The unique ID that EventBridge Scheduler assigns for each attempted invocation of a target, for example, d32c5kddcf5bb8c3.
+4. `ContextAttribute.attemptNumber()` – A counter that identifies the attempt number for the current invocation, for example, 1.
+
+```python
+text = f"Attempt number: {ContextAttribute.attemptNumber}"
+input = ScheduleTargetInput.from_text(text)
+```
 
 ### Specifying Execution Role
 
 TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ### Cross-account and cross-region targets
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0/setup.py` & `aws-cdk.aws-scheduler-alpha-2.87.0a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-scheduler-alpha",
-    "version": "2.86.0.a0",
+    "version": "2.87.0.a0",
     "description": "The CDK Construct Library for Amazon Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_scheduler_alpha",
         "aws_cdk.aws_scheduler_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_scheduler_alpha._jsii": [
-            "aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz"
+            "aws-scheduler-alpha@2.87.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_scheduler_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.86.0",
+        "aws-cdk-lib==2.87.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py` & `aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,15 +33,21 @@
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project. It allows you to define Event Bridge Schedules.
 
 > This module is in active development. Some features may not be implemented yet.
 
 ## Defining a schedule
 
-TODO: Schedule is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+TODO: Schedule is not yet fully implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+
+Only an L2 class is created that wraps the L1 class and handles the following properties:
+
+* schedule
+* target (only LambdaInvoke is supported for now)
+* flexibleTimeWindow will be set to `{ mode: 'OFF' }`
 
 ### Schedule Expressions
 
 You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
 
 Both rate-based and cron-based schedules are recurring schedules. You can configure each recurring schedule type using a schedule expression. For
 cron-based schedule you can specify a time zone in which EventBridge Scheduler evaluates the expression.
@@ -86,17 +92,39 @@
 
 TODO: Group is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ## Scheduler Targets
 
 TODO: Scheduler Targets Module is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
+Only LambdaInvoke target is added for now.
+
 ### Input
 
-TODO: Target Input is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+Target can be invoked with a custom input. Class `ScheduleTargetInput` supports free form text input and JSON-formatted object input:
+
+```python
+input = ScheduleTargetInput.from_object({
+    "QueueName": "MyQueue"
+})
+```
+
+You can include context attributes in your target payload. EventBridge Scheduler will replace each keyword with
+its respective value and deliver it to the target. See
+[full list of supported context attributes](https://docs.aws.amazon.com/scheduler/latest/UserGuide/managing-schedule-context-attributes.html):
+
+1. `ContextAttribute.scheduleArn()` – The ARN of the schedule.
+2. `ContextAttribute.scheduledTime()` – The time you specified for the schedule to invoke its target, for example, 2022-03-22T18:59:43Z.
+3. `ContextAttribute.executionId()` – The unique ID that EventBridge Scheduler assigns for each attempted invocation of a target, for example, d32c5kddcf5bb8c3.
+4. `ContextAttribute.attemptNumber()` – A counter that identifies the attempt number for the current invocation, for example, 1.
+
+```python
+text = f"Attempt number: {ContextAttribute.attemptNumber}"
+input = ScheduleTargetInput.from_text(text)
+```
 
 ### Specifying Execution Role
 
 TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ### Cross-account and cross-region targets
 
@@ -144,14 +172,91 @@
 
 from ._jsii import *
 
 import aws_cdk as _aws_cdk_ceddda9d
 import aws_cdk.aws_events as _aws_cdk_aws_events_ceddda9d
 
 
+class ContextAttribute(
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@aws-cdk/aws-scheduler-alpha.ContextAttribute",
+):
+    '''(experimental) Represents a field in the event pattern.
+
+    :see: https://docs.aws.amazon.com/scheduler/latest/UserGuide/managing-schedule-context-attributes.html
+    :stability: experimental
+    '''
+
+    @jsii.member(jsii_name="fromName")
+    @builtins.classmethod
+    def from_name(cls, name: builtins.str) -> builtins.str:
+        '''(experimental) Escape hatch for other ContextAttribute that might be resolved in future.
+
+        :param name: - name will replace xxx in <aws.scheduler.xxx>.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fa3298180583c0ddbdf4d5fc4310e8726157d1b4b991a42e01360362e1c7d731)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "fromName", [name]))
+
+    @jsii.member(jsii_name="toString")
+    def to_string(self) -> builtins.str:
+        '''(experimental) Convert the path to the field in the event pattern to JSON.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.invoke(self, "toString", []))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="attemptNumber")
+    def attempt_number(cls) -> builtins.str:
+        '''(experimental) A counter that identifies the attempt number for the current invocation, for example, 1.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.sget(cls, "attemptNumber"))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="executionId")
+    def execution_id(cls) -> builtins.str:
+        '''(experimental) The unique ID that EventBridge Scheduler assigns for each attempted invocation of a target, for example, d32c5kddcf5bb8c3.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.sget(cls, "executionId"))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="scheduleArn")
+    def schedule_arn(cls) -> builtins.str:
+        '''(experimental) The ARN of the schedule.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.sget(cls, "scheduleArn"))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="scheduledTime")
+    def scheduled_time(cls) -> builtins.str:
+        '''(experimental) The time you specified for the schedule to invoke its target, for example, 2022-03-22T18:59:43Z.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.sget(cls, "scheduledTime"))
+
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "name"))
+
+
 @jsii.data_type(
     jsii_type="@aws-cdk/aws-scheduler-alpha.CronOptionsWithTimezone",
     jsii_struct_bases=[_aws_cdk_aws_events_ceddda9d.CronOptions],
     name_mapping={
         "day": "day",
         "hour": "hour",
         "minute": "minute",
@@ -307,14 +412,39 @@
 
     def __repr__(self) -> str:
         return "CronOptionsWithTimezone(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.interface(jsii_type="@aws-cdk/aws-scheduler-alpha.ISchedule")
+class ISchedule(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
+    '''(experimental) Interface representing a created or an imported ``Schedule``.
+
+    :stability: experimental
+    '''
+
+    pass
+
+
+class _IScheduleProxy(
+    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
+):
+    '''(experimental) Interface representing a created or an imported ``Schedule``.
+
+    :stability: experimental
+    '''
+
+    __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-scheduler-alpha.ISchedule"
+    pass
+
+# Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
+typing.cast(typing.Any, ISchedule).__jsii_proxy_class__ = lambda : _IScheduleProxy
+
+
 class ScheduleExpression(
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="@aws-cdk/aws-scheduler-alpha.ScheduleExpression",
 ):
     '''(experimental) ScheduleExpression for EventBridge Schedule.
 
     You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
@@ -475,21 +605,114 @@
         '''
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.TimeZone], jsii.get(self, "timeZone"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, ScheduleExpression).__jsii_proxy_class__ = lambda : _ScheduleExpressionProxy
 
 
+class ScheduleTargetInput(
+    metaclass=jsii.JSIIAbstractClass,
+    jsii_type="@aws-cdk/aws-scheduler-alpha.ScheduleTargetInput",
+):
+    '''(experimental) The text, or well-formed JSON, passed to the target of the schedule.
+
+    :stability: experimental
+    :exampleMetadata: infused
+
+    Example::
+
+        input = ScheduleTargetInput.from_object({
+            "QueueName": "MyQueue"
+        })
+    '''
+
+    def __init__(self) -> None:
+        '''
+        :stability: experimental
+        '''
+        jsii.create(self.__class__, self, [])
+
+    @jsii.member(jsii_name="fromObject")
+    @builtins.classmethod
+    def from_object(cls, obj: typing.Any) -> "ScheduleTargetInput":
+        '''(experimental) Pass a JSON object to the target, it is possible to embed ``ContextAttributes`` and other cdk references.
+
+        :param obj: object to use to convert to JSON to use as input for the target.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8c8ad466ed6529e9804ae78b120437ef13be3ec57499e1adc15762a5e00bccce)
+            check_type(argname="argument obj", value=obj, expected_type=type_hints["obj"])
+        return typing.cast("ScheduleTargetInput", jsii.sinvoke(cls, "fromObject", [obj]))
+
+    @jsii.member(jsii_name="fromText")
+    @builtins.classmethod
+    def from_text(cls, text: builtins.str) -> "ScheduleTargetInput":
+        '''(experimental) Pass text to the target, it is possible to embed ``ContextAttributes`` that will be resolved to actual values while the CloudFormation is deployed or cdk Tokens that will be resolved when the CloudFormation templates are generated by CDK.
+
+        The target input value will be a single string that you pass.
+        For passing complex values like JSON object to a target use method
+        ``ScheduleTargetInput.fromObject()`` instead.
+
+        :param text: Text to use as the input for the target.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__574fe803ab70d3031262c0aa59859d86504152f998a9cb5954d8eda9a4714e7d)
+            check_type(argname="argument text", value=text, expected_type=type_hints["text"])
+        return typing.cast("ScheduleTargetInput", jsii.sinvoke(cls, "fromText", [text]))
+
+    @jsii.member(jsii_name="bind")
+    @abc.abstractmethod
+    def bind(self, schedule: ISchedule) -> builtins.str:
+        '''(experimental) Return the input properties for this input object.
+
+        :param schedule: -
+
+        :stability: experimental
+        '''
+        ...
+
+
+class _ScheduleTargetInputProxy(ScheduleTargetInput):
+    @jsii.member(jsii_name="bind")
+    def bind(self, schedule: ISchedule) -> builtins.str:
+        '''(experimental) Return the input properties for this input object.
+
+        :param schedule: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e82eb20b61ddff46bbd14d8fd0a9b321cedc42dd29e60faa8e2d03dc8d7e9c9d)
+            check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
+        return typing.cast(builtins.str, jsii.invoke(self, "bind", [schedule]))
+
+# Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
+typing.cast(typing.Any, ScheduleTargetInput).__jsii_proxy_class__ = lambda : _ScheduleTargetInputProxy
+
+
 __all__ = [
+    "ContextAttribute",
     "CronOptionsWithTimezone",
+    "ISchedule",
     "ScheduleExpression",
+    "ScheduleTargetInput",
 ]
 
 publication.publish()
 
+def _typecheckingstub__fa3298180583c0ddbdf4d5fc4310e8726157d1b4b991a42e01360362e1c7d731(
+    name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__2b93c2b718a23f23063cb14b1618a13104c926d0bdf7230ce719160d882d285a(
     *,
     day: typing.Optional[builtins.str] = None,
     hour: typing.Optional[builtins.str] = None,
     minute: typing.Optional[builtins.str] = None,
     month: typing.Optional[builtins.str] = None,
     week_day: typing.Optional[builtins.str] = None,
@@ -514,7 +737,25 @@
     pass
 
 def _typecheckingstub__f2f7ba7d57267bb20d2ff8fd156c360c31850c2fb0387099338165ebc5ba04a4(
     duration: _aws_cdk_ceddda9d.Duration,
 ) -> None:
     """Type checking stubs"""
     pass
+
+def _typecheckingstub__8c8ad466ed6529e9804ae78b120437ef13be3ec57499e1adc15762a5e00bccce(
+    obj: typing.Any,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__574fe803ab70d3031262c0aa59859d86504152f998a9cb5954d8eda9a4714e7d(
+    text: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e82eb20b61ddff46bbd14d8fd0a9b321cedc42dd29e60faa8e2d03dc8d7e9c9d(
+    schedule: ISchedule,
+) -> None:
+    """Type checking stubs"""
+    pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-scheduler-alpha
-Version: 2.86.0a0
+Version: 2.87.0a0
 Summary: The CDK Construct Library for Amazon Scheduler
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -59,15 +59,21 @@
 
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project. It allows you to define Event Bridge Schedules.
 
 > This module is in active development. Some features may not be implemented yet.
 
 ## Defining a schedule
 
-TODO: Schedule is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+TODO: Schedule is not yet fully implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+
+Only an L2 class is created that wraps the L1 class and handles the following properties:
+
+* schedule
+* target (only LambdaInvoke is supported for now)
+* flexibleTimeWindow will be set to `{ mode: 'OFF' }`
 
 ### Schedule Expressions
 
 You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
 
 Both rate-based and cron-based schedules are recurring schedules. You can configure each recurring schedule type using a schedule expression. For
 cron-based schedule you can specify a time zone in which EventBridge Scheduler evaluates the expression.
@@ -112,17 +118,39 @@
 
 TODO: Group is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ## Scheduler Targets
 
 TODO: Scheduler Targets Module is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
+Only LambdaInvoke target is added for now.
+
 ### Input
 
-TODO: Target Input is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+Target can be invoked with a custom input. Class `ScheduleTargetInput` supports free form text input and JSON-formatted object input:
+
+```python
+input = ScheduleTargetInput.from_object({
+    "QueueName": "MyQueue"
+})
+```
+
+You can include context attributes in your target payload. EventBridge Scheduler will replace each keyword with
+its respective value and deliver it to the target. See
+[full list of supported context attributes](https://docs.aws.amazon.com/scheduler/latest/UserGuide/managing-schedule-context-attributes.html):
+
+1. `ContextAttribute.scheduleArn()` – The ARN of the schedule.
+2. `ContextAttribute.scheduledTime()` – The time you specified for the schedule to invoke its target, for example, 2022-03-22T18:59:43Z.
+3. `ContextAttribute.executionId()` – The unique ID that EventBridge Scheduler assigns for each attempted invocation of a target, for example, d32c5kddcf5bb8c3.
+4. `ContextAttribute.attemptNumber()` – A counter that identifies the attempt number for the current invocation, for example, 1.
+
+```python
+text = f"Attempt number: {ContextAttribute.attemptNumber}"
+input = ScheduleTargetInput.from_text(text)
+```
 
 ### Specifying Execution Role
 
 TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ### Cross-account and cross-region targets
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-scheduler-alpha-2.87.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_scheduler_alpha/__init__.py
 src/aws_cdk/aws_scheduler_alpha/py.typed
 src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
-src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.87.0-alpha.0.jsii.tgz
```

