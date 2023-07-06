# Comparing `tmp/lifeguard-k8s-1.2.1.tar.gz` & `tmp/lifeguard-k8s-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-k8s-1.2.1.tar", last modified: Fri Jun 16 12:07:34 2023, max compression
+gzip compressed data, was "lifeguard-k8s-1.3.0.tar", last modified: Thu Jul  6 18:36:40 2023, max compression
```

## Comparing `lifeguard-k8s-1.2.1.tar` & `lifeguard-k8s-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.274646 lifeguard-k8s-1.2.1/lifeguard_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.278646 lifeguard-k8s-1.2.1/lifeguard_k8s/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/actions/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.278646 lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/lifeguard_k8s/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/lifeguard_k8s/validations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.278646 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 12:07:34.000000 lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:07:34.286646 lifeguard-k8s-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/actions/test_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/infrastructure/test_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:34.282646 lifeguard-k8s-1.2.1/tests/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-16 12:07:05.000000 lifeguard-k8s-1.2.1/tests/validations/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/lifeguard_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/lifeguard_k8s/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/actions/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/lifeguard_k8s/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/infrastructure/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/infrastructure/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/infrastructure/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/lifeguard_k8s/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/lifeguard_k8s/validations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-06 18:36:40.000000 lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-06 18:36:40.000000 lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:36:40.000000 lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 18:36:40.000000 lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 18:36:40.000000 lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/actions/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/tests/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/infrastructure/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/infrastructure/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/infrastructure/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:40.416917 lifeguard-k8s-1.3.0/tests/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-06 18:36:13.000000 lifeguard-k8s-1.3.0/tests/validations/test_pods.py
```

### Comparing `lifeguard-k8s-1.2.1/PKG-INFO` & `lifeguard-k8s-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-k8s
-Version: 1.2.1
+Version: 1.3.0
 Summary: Lifeguard integration with Kubernetes
 Home-page: https://github.com/LifeguardSystem/lifeguard-k8s
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-k8s-1.2.1/README.md` & `lifeguard-k8s-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.1/lifeguard_k8s/actions/pods.py` & `lifeguard-k8s-1.3.0/lifeguard_k8s/actions/pods.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.1/lifeguard_k8s/infrastructure/pods.py` & `lifeguard-k8s-1.3.0/lifeguard_k8s/infrastructure/pods.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from kubernetes import client, config
+from lifeguard_k8s.infrastructure import get_client
 from lifeguard_k8s.settings import (
-    LIFEGUARD_KUBERNETES_CONFIG,
     LIFEGUARD_KUBERNETES_READ_LOG_MAX_SIZE,
 )
 
 RUNNING_STATUS = "Running"
 COMPLETED_STATUS = "Succeeded"
 
 NORMAL_STATUSES = [RUNNING_STATUS, COMPLETED_STATUS]
@@ -20,54 +19,18 @@
             job_pod.metadata.owner_references[0].name in pod.metadata.name
             and pod.status.phase == COMPLETED_STATUS
         ):
             return True
     return False
 
 
-def _get_clients():
-    if LIFEGUARD_KUBERNETES_CONFIG:
-        config.load_kube_config(LIFEGUARD_KUBERNETES_CONFIG)
-    else:
-        config.load_incluster_config()
-
-    return client.CoreV1Api()
-
-
-def get_namespace_infos(namespace):
-    """
-    Return current main infos of a namespace
-    """
-    infos = {"pods": []}
-
-    v1 = _get_clients()
-    pods = v1.list_namespaced_pod(namespace)
-
-    for pod in pods.items:
-        infos["pods"].append(
-            {
-                "name": pod.metadata.name,
-                "status": pod.status.phase,
-                "containers": [
-                    {
-                        "name": container.name,
-                        "ready": container.ready,
-                        "restart_count": container.restart_count,
-                    }
-                    for container in pod.status.container_statuses
-                ],
-            }
-        )
-    return infos
-
-
 def get_not_running_pods(namespace):
     not_running_pods = []
 
-    v1 = _get_clients()
+    v1 = get_client()
     pods = v1.list_namespaced_pod(namespace)
 
     for pod in pods.items:
         if pod.status.phase not in NORMAL_STATUSES or (
             not all(container.ready for container in pod.status.container_statuses)
         ):
             if _check_if_job_pod(pod):
@@ -76,20 +39,20 @@
             else:
                 not_running_pods.append(pod.metadata.name)
 
     return not_running_pods
 
 
 def delete_a_pod(namespace, pod_name):
-    v1 = _get_clients()
+    v1 = get_client()
     v1.delete_namespaced_pod(pod_name, namespace)
 
 
 def get_events_from_pod(namespace, pod_name):
-    v1 = _get_clients()
+    v1 = get_client()
     events = v1.list_namespaced_event(
         namespace, field_selector=f"involvedObject.name={pod_name}"
     )
     return [
         {"event_type": item.type, "message": item.message, "reason": item.reason}
         for item in events.items
     ]
@@ -105,10 +68,10 @@
             return failed[-1]
         return events[-1]
 
     return None
 
 
 def get_logs_from_pod(namespace, pod_name):
-    v1 = _get_clients()
+    v1 = get_client()
     log = v1.read_namespaced_pod_log(pod_name, namespace)
     return log[-LIFEGUARD_KUBERNETES_READ_LOG_MAX_SIZE:]
```

### Comparing `lifeguard-k8s-1.2.1/lifeguard_k8s/settings.py` & `lifeguard-k8s-1.3.0/lifeguard_k8s/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.1/lifeguard_k8s/validations/pods.py` & `lifeguard-k8s-1.3.0/lifeguard_k8s/validations/pods.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/PKG-INFO` & `lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-k8s
-Version: 1.2.1
+Version: 1.3.0
 Summary: Lifeguard integration with Kubernetes
 Home-page: https://github.com/LifeguardSystem/lifeguard-k8s
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-k8s-1.2.1/lifeguard_k8s.egg-info/SOURCES.txt` & `lifeguard-k8s-1.3.0/lifeguard_k8s.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 lifeguard_k8s.egg-info/SOURCES.txt
 lifeguard_k8s.egg-info/dependency_links.txt
 lifeguard_k8s.egg-info/requires.txt
 lifeguard_k8s.egg-info/top_level.txt
 lifeguard_k8s/actions/__init__.py
 lifeguard_k8s/actions/pods.py
 lifeguard_k8s/infrastructure/__init__.py
+lifeguard_k8s/infrastructure/deployments.py
+lifeguard_k8s/infrastructure/namespaces.py
 lifeguard_k8s/infrastructure/pods.py
 lifeguard_k8s/validations/__init__.py
 lifeguard_k8s/validations/pods.py
 tests/__init__.py
 tests/actions/__init__.py
 tests/actions/test_pods.py
 tests/infrastructure/__init__.py
+tests/infrastructure/test_deployments.py
+tests/infrastructure/test_namespaces.py
 tests/infrastructure/test_pods.py
 tests/validations/__init__.py
 tests/validations/test_pods.py
```

### Comparing `lifeguard-k8s-1.2.1/setup.py` & `lifeguard-k8s-1.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-k8s",
-    version="1.2.1",
+    version="1.3.0",
     url="https://github.com/LifeguardSystem/lifeguard-k8s",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with Kubernetes",
```

### Comparing `lifeguard-k8s-1.2.1/tests/actions/test_pods.py` & `lifeguard-k8s-1.3.0/tests/actions/test_pods.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.2.1/tests/infrastructure/test_pods.py` & `lifeguard-k8s-1.3.0/tests/infrastructure/test_pods.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,104 @@
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
 
+from tests.infrastructure import build_pod
+
 from lifeguard_k8s.infrastructure.pods import (
     get_not_running_pods,
     get_events_from_pod,
     get_last_error_event_from_pod,
     get_logs_from_pod,
     delete_a_pod,
-    get_namespace_infos,
 )
 
 
-def build_pod(status, container_status, pod_name, kind="ReplicaSet"):
-    container_statuses = MagicMock(name="container_statuses")
-    container_statuses.ready = container_status
-    container_statuses.restart_count = 0
-    container_statuses.name = "container_name"
-
-    owner_reference = MagicMock(name="owner_reference")
-    owner_reference.kind = kind
-    owner_reference.name = pod_name
-
-    pod = MagicMock(name="pod")
-    pod.status = MagicMock(name="status")
-    pod.status.phase = status
-    pod.status.container_statuses = [container_statuses]
-    pod.metadata.name = pod_name
-    pod.metadata.owner_references = [owner_reference]
-
-    return pod
-
-
 class InfrastructurePodsTests(TestCase):
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_not_return_pod_if_has_normal_statuses(self, mock_client, mock_config):
         pod = build_pod("Running", True, "pod_name")
 
         mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = [
             pod
         ]
 
         self.assertEqual(get_not_running_pods("namespace"), [])
         mock_config.load_incluster_config.assert_called()
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_return_pod_if_not_has_normal_statuses(self, mock_client, _mock_config):
         pod = build_pod("Failed", True, "pod_name")
 
         mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = [
             pod
         ]
 
         self.assertEqual(get_not_running_pods("namespace"), ["pod_name"])
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_return_pod_if_not_has_all_containers_ready(
         self, mock_client, _mock_config
     ):
         pod = build_pod("Running", False, "pod_name")
 
         mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = [
             pod
         ]
 
         self.assertEqual(get_not_running_pods("namespace"), ["pod_name"])
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_return_pod_if_is_job_and_not_has_success_pod_after_job(
         self, mock_client, _mock_config
     ):
         pod = build_pod("Failed", True, "pod_name", kind="Job")
 
         mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = [
             pod
         ]
 
         self.assertEqual(get_not_running_pods("namespace"), ["pod_name"])
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_not_return_pod_if_is_job_and_has_success_pod_after_job(
         self, mock_client, _mock_config
     ):
         pod = build_pod("Failed", True, "pod_name", kind="Job")
         success_pod = build_pod("Succeeded", True, "pod_name", kind="Job")
 
         mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = [
             pod,
             success_pod,
         ]
 
         self.assertEqual(get_not_running_pods("namespace"), [])
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_get_events_from_pod(self, mock_client, _mock_config):
         event = MagicMock(name="event")
         event.type = "Normal"
         event.message = "message"
         event.reason = "reason"
         mock_client.CoreV1Api.return_value.list_namespaced_event.return_value.items = [
             event
         ]
 
         self.assertEqual(
             get_events_from_pod("namespace", "pod_name"),
             [{"event_type": "Normal", "message": "message", "reason": "reason"}],
         )
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_get_last_error_event_from_pod_without_errors(
         self, mock_client, _mock_config
     ):
         event = MagicMock(name="event")
         event.type = "Normal"
         event.message = "message"
         mock_client.CoreV1Api.return_value.list_namespaced_event.return_value.items = [
@@ -125,16 +106,16 @@
         ]
 
         self.assertEqual(
             get_last_error_event_from_pod("namespace", "pod_name"),
             None,
         )
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_get_last_error_event_from_pod_with_errors(self, mock_client, _mock_config):
         event_normal = MagicMock(name="event")
         event_normal.type = "Normal"
         event_normal.message = "message"
         event_normal.reason = "reason"
 
         event_error = MagicMock(name="event")
@@ -148,16 +129,16 @@
         ]
 
         self.assertEqual(
             get_last_error_event_from_pod("namespace", "pod_name"),
             {"event_type": "Warning", "message": "message", "reason": "reason"},
         )
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_get_last_error_event_from_pod_with_failed(self, mock_client, _mock_config):
         event_normal = MagicMock(name="event")
         event_normal.type = "Normal"
         event_normal.message = "message"
         event_normal.reason = "reason"
 
         event_error = MagicMock(name="event")
@@ -172,73 +153,46 @@
 
         self.assertEqual(
             get_last_error_event_from_pod("namespace", "pod_name"),
             {"event_type": "Warning", "message": "failed", "reason": "Failed"},
         )
 
     @patch(
-        "lifeguard_k8s.infrastructure.pods.LIFEGUARD_KUBERNETES_CONFIG",
+        "lifeguard_k8s.infrastructure.LIFEGUARD_KUBERNETES_CONFIG",
         "path_to_file",
     )
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_call_load_kube_config_if_config_is_not_empty(
         self, mock_client, mock_config
     ):
         mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = []
 
         self.assertEqual(get_not_running_pods("namespace"), [])
         mock_config.load_kube_config.assert_called_with("path_to_file")
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_get_logs_from_pod(self, mock_client, _mock_config):
         mock_client.CoreV1Api.return_value.read_namespaced_pod_log.return_value = "log"
         self.assertEqual(get_logs_from_pod("namespace", "pod_name"), "log")
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     @patch(
         "lifeguard_k8s.infrastructure.pods.LIFEGUARD_KUBERNETES_READ_LOG_MAX_SIZE", 10
     )
     def test_get_logs_from_pod_with_limited_size(self, mock_client, _mock_config):
         mock_client.CoreV1Api.return_value.read_namespaced_pod_log.return_value = """
 a big log that will be limited
 send only last 10 characters"""
         self.assertEqual(get_logs_from_pod("namespace", "pod_name"), "characters")
 
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
+    @patch("lifeguard_k8s.infrastructure.config")
+    @patch("lifeguard_k8s.infrastructure.client")
     def test_delete_a_pod(self, mock_client, _mock_config):
         mock_client.CoreV1Api.return_value.delete_namespaced_pod.return_value = None
         delete_a_pod("namespace", "pod_name")
 
         mock_client.CoreV1Api.return_value.delete_namespaced_pod.assert_called_with(
             "pod_name", "namespace"
         )
-
-    @patch("lifeguard_k8s.infrastructure.pods.config")
-    @patch("lifeguard_k8s.infrastructure.pods.client")
-    def test_get_namespace_infos(self, mock_client, _mock_config):
-        pod = build_pod("Running", True, "pod_name")
-
-        mock_client.CoreV1Api.return_value.list_namespaced_pod.return_value.items = [
-            pod
-        ]
-        self.assertEqual(
-            get_namespace_infos("namespace"),
-            {
-                "pods": [
-                    {
-                        "containers": [
-                            {
-                                "name": "container_name",
-                                "ready": True,
-                                "restart_count": 0,
-                            }
-                        ],
-                        "name": "pod_name",
-                        "status": "Running",
-                    }
-                ]
-            },
-        )
```

### Comparing `lifeguard-k8s-1.2.1/tests/validations/test_pods.py` & `lifeguard-k8s-1.3.0/tests/validations/test_pods.py`

 * *Files identical despite different names*

