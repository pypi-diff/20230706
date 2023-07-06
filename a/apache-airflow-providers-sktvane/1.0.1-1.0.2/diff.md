# Comparing `tmp/apache-airflow-providers-sktvane-1.0.1.tar.gz` & `tmp/apache-airflow-providers-sktvane-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-1.0.1.tar", last modified: Tue Jul  4 09:53:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-1.0.2.tar", last modified: Thu Jul  6 07:59:08 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-1.0.1.tar` & `apache-airflow-providers-sktvane-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.824251 apache-airflow-providers-sktvane-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-04 09:53:46.824251 apache-airflow-providers-sktvane-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.820251 apache-airflow-providers-sktvane-1.0.1/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.820251 apache-airflow-providers-sktvane-1.0.1/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.820251 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.820251 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.820251 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.824251 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.824251 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/tests/operator_nes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:53:46.824251 apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-04 09:53:46.000000 apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-04 09:53:46.000000 apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:53:46.000000 apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 09:53:46.000000 apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 09:53:46.000000 apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 09:53:46.824251 apache-airflow-providers-sktvane-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 09:53:40.000000 apache-airflow-providers-sktvane-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.946046 apache-airflow-providers-sktvane-1.0.2/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.946046 apache-airflow-providers-sktvane-1.0.2/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.946046 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/tests/operator_nes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-06 07:59:08.000000 apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-06 07:59:08.000000 apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:59:08.000000 apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-06 07:59:08.000000 apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 07:59:08.000000 apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 07:59:08.950047 apache-airflow-providers-sktvane-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-06 07:59:03.000000 apache-airflow-providers-sktvane-1.0.2/setup.py
```

### Comparing `apache-airflow-providers-sktvane-1.0.1/PKG-INFO` & `apache-airflow-providers-sktvane-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-1.0.1/README.md` & `apache-airflow-providers-sktvane-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/macros/slack_notifier.py` & `apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/macros/slack_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import cached_property
+
 import pendulum
 from airflow.notifications.basenotifier import BaseNotifier
 from airflow.providers.slack.hooks.slack import SlackHook
 from airflow.utils.context import Context
 from slack_sdk.errors import SlackApiError
 
 from ..macros.vault import get_secrets
@@ -15,22 +17,27 @@
     )
 
     def __init__(self, slack_channel, slack_username, slack_email):
         super().__init__()
         self.slack_channel = slack_channel
         self.slack_username = slack_username
         self.slack_email = slack_email
-        self.slack_hook = SlackHook(
+
+    @cached_property
+    def slack_hook(self) -> SlackHook:
+        return SlackHook(
             token=get_secrets(path="airflow_k8s/slack/slack_alarmbot_token")["token"],
             proxy=get_secrets(path="proxy")["proxy"],
         )
 
     def _get_user_id_by_email(self) -> str:
         try:
-            response = self.slack_hook.client.users_lookupByEmail(email=self.slack_email)
+            response = self.slack_hook.client.users_lookupByEmail(
+                email=self.slack_email
+            )
             user_id = response.get("user")["id"]
             return f"<@{user_id}>"
         except SlackApiError:
             return "UNREGISTERED"
 
     @staticmethod
     def _generate_fail_alert_blocks(context: Context, user_id: str) -> list:
```

### Comparing `apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/operators/nes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import uuid
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
+from functools import cached_property
 from time import sleep
 
 import requests
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.utils.context import Context
@@ -91,15 +92,18 @@
     ) -> None:
         super().__init__(*args, **kwargs)
         self.input_nb = input_nb
         self.parameters = parameters
         self.runtime = runtime
         self.profile = profile
         self.host_network = host_network
-        self.processor = BaseProcessor.generate_processor(input_nb=self.input_nb)
+
+    @cached_property
+    def processor(self):
+        return BaseProcessor.generate_processor(input_nb=self.input_nb)
 
     def pre_execute(self, context):
         self.processor.pre_process()
 
     def execute(self, context):
         def submit_job() -> tuple[str, str]:
             request_body = dict(
```

### Comparing `apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-1.0.1/airflow/providers/sktvane/tests/operator_nes_test.py` & `apache-airflow-providers-sktvane-1.0.2/airflow/providers/sktvane/tests/operator_nes_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-1.0.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-1.0.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-1.0.1/setup.py` & `apache-airflow-providers-sktvane-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="1.0.1",
+    version="1.0.2",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

