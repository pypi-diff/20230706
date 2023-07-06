# Comparing `tmp/mypy-boto3-ec2-1.27.0.tar.gz` & `tmp/mypy-boto3-ec2-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ec2-1.27.0.tar", last modified: Mon Jul  3 19:50:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ec2-1.28.0.tar", last modified: Thu Jul  6 20:59:29 2023, max compression
```

## Comparing `mypy-boto3-ec2-1.27.0.tar` & `mypy-boto3-ec2-1.28.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.431178 mypy-boto3-ec2-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:36:17.000000 mypy-boto3-ec2-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)   170442 2023-07-03 19:50:42.427178 mypy-boto3-ec2-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   168973 2023-07-03 19:36:17.000000 mypy-boto3-ec2-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.419177 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/
--rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-07-03 19:36:17.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46233 2023-07-03 19:36:17.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:36:17.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   519979 2023-07-03 19:36:23.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   519205 2023-07-03 19:36:20.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    89583 2023-07-03 19:36:30.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    89581 2023-07-03 19:36:29.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   182527 2023-07-03 19:36:27.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)   182386 2023-07-03 19:36:27.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:36:17.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   269571 2023-07-03 19:36:26.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   269106 2023-07-03 19:36:24.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   954628 2023-07-03 19:36:53.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   953621 2023-07-03 19:36:41.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:36:17.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-07-03 19:36:28.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38492 2023-07-03 19:36:27.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.427178 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   170442 2023-07-03 19:50:42.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 19:50:42.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:42.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:42.000000 mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:42.431178 mypy-boto3-ec2-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:36:16.000000 mypy-boto3-ec2-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.514290 mypy-boto3-ec2-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)   170472 2023-07-06 20:59:29.502290 mypy-boto3-ec2-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   169003 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.490290 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46233 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   519979 2023-07-06 20:39:01.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   519205 2023-07-06 20:38:56.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    89678 2023-07-06 20:39:11.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89676 2023-07-06 20:39:10.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   182527 2023-07-06 20:39:07.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182386 2023-07-06 20:39:06.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   269571 2023-07-06 20:39:05.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   269106 2023-07-06 20:39:04.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   954716 2023-07-06 20:39:45.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   953709 2023-07-06 20:39:28.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-07-06 20:39:09.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38492 2023-07-06 20:39:09.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.502290 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   170472 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:29.514290 mypy-boto3-ec2-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:38:51.000000 mypy-boto3-ec2-1.28.0/setup.py
```

### Comparing `mypy-boto3-ec2-1.27.0/LICENSE` & `mypy-boto3-ec2-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/PKG-INFO` & `mypy-boto3-ec2-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.27.0
-Summary: Type annotations for boto3.EC2 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.EC2 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -1464,14 +1464,15 @@
     NatGatewayStateType,
     NetworkInterfaceAttributeType,
     NetworkInterfaceAvailableWaiterName,
     NetworkInterfaceCreationTypeType,
     NetworkInterfacePermissionStateCodeType,
     NetworkInterfaceStatusType,
     NetworkInterfaceTypeType,
+    NitroEnclavesSupportType,
     OfferingClassTypeType,
     OfferingTypeValuesType,
     OnDemandAllocationStrategyType,
     OperationTypeType,
     PartitionLoadFrequencyType,
     PasswordDataAvailableWaiterName,
     PayerResponsibilityType,
```

### Comparing `mypy-boto3-ec2-1.27.0/README.md` & `mypy-boto3-ec2-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -1432,14 +1432,15 @@
     NatGatewayStateType,
     NetworkInterfaceAttributeType,
     NetworkInterfaceAvailableWaiterName,
     NetworkInterfaceCreationTypeType,
     NetworkInterfacePermissionStateCodeType,
     NetworkInterfaceStatusType,
     NetworkInterfaceTypeType,
+    NitroEnclavesSupportType,
     OfferingClassTypeType,
     OfferingTypeValuesType,
     OnDemandAllocationStrategyType,
     OperationTypeType,
     PartitionLoadFrequencyType,
     PasswordDataAvailableWaiterName,
     PayerResponsibilityType,
```

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/__init__.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/__init__.pyi` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/__main__.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.EC2 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.27.0")
+    print("1.28.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/client.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/client.pyi` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/literals.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,15 @@
     "NatGatewayStateType",
     "NetworkInterfaceAttributeType",
     "NetworkInterfaceAvailableWaiterName",
     "NetworkInterfaceCreationTypeType",
     "NetworkInterfacePermissionStateCodeType",
     "NetworkInterfaceStatusType",
     "NetworkInterfaceTypeType",
+    "NitroEnclavesSupportType",
     "OfferingClassTypeType",
     "OfferingTypeValuesType",
     "OnDemandAllocationStrategyType",
     "OperationTypeType",
     "PartitionLoadFrequencyType",
     "PasswordDataAvailableWaiterName",
     "PayerResponsibilityType",
@@ -1808,14 +1809,15 @@
     "natGateway",
     "network_load_balancer",
     "quicksight",
     "transit_gateway",
     "trunk",
     "vpc_endpoint",
 ]
+NitroEnclavesSupportType = Literal["supported", "unsupported"]
 OfferingClassTypeType = Literal["convertible", "standard"]
 OfferingTypeValuesType = Literal[
     "All Upfront",
     "Heavy Utilization",
     "Light Utilization",
     "Medium Utilization",
     "No Upfront",
```

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/literals.pyi` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -360,14 +360,15 @@
     "NatGatewayStateType",
     "NetworkInterfaceAttributeType",
     "NetworkInterfaceAvailableWaiterName",
     "NetworkInterfaceCreationTypeType",
     "NetworkInterfacePermissionStateCodeType",
     "NetworkInterfaceStatusType",
     "NetworkInterfaceTypeType",
+    "NitroEnclavesSupportType",
     "OfferingClassTypeType",
     "OfferingTypeValuesType",
     "OnDemandAllocationStrategyType",
     "OperationTypeType",
     "PartitionLoadFrequencyType",
     "PasswordDataAvailableWaiterName",
     "PayerResponsibilityType",
@@ -1806,14 +1807,15 @@
     "natGateway",
     "network_load_balancer",
     "quicksight",
     "transit_gateway",
     "trunk",
     "vpc_endpoint",
 ]
+NitroEnclavesSupportType = Literal["supported", "unsupported"]
 OfferingClassTypeType = Literal["convertible", "standard"]
 OfferingTypeValuesType = Literal[
     "All Upfront",
     "Heavy Utilization",
     "Light Utilization",
     "Medium Utilization",
     "No Upfront",
```

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/paginator.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/paginator.pyi` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/service_resource.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/service_resource.pyi` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/type_defs.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     NatGatewayAddressStatusType,
     NatGatewayStateType,
     NetworkInterfaceAttributeType,
     NetworkInterfaceCreationTypeType,
     NetworkInterfacePermissionStateCodeType,
     NetworkInterfaceStatusType,
     NetworkInterfaceTypeType,
+    NitroEnclavesSupportType,
     OfferingClassTypeType,
     OfferingTypeValuesType,
     OnDemandAllocationStrategyType,
     OperationTypeType,
     PartitionLoadFrequencyType,
     PaymentOptionType,
     PeriodTypeType,
@@ -31401,14 +31402,15 @@
         "PlacementGroupInfo": PlacementGroupInfoTypeDef,
         "InferenceAcceleratorInfo": InferenceAcceleratorInfoTypeDef,
         "HibernationSupported": bool,
         "BurstablePerformanceSupported": bool,
         "DedicatedHostsSupported": bool,
         "AutoRecoverySupported": bool,
         "SupportedBootModes": List[BootModeTypeType],
+        "NitroEnclavesSupport": NitroEnclavesSupportType,
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
```

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/type_defs.pyi` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     NatGatewayAddressStatusType,
     NatGatewayStateType,
     NetworkInterfaceAttributeType,
     NetworkInterfaceCreationTypeType,
     NetworkInterfacePermissionStateCodeType,
     NetworkInterfaceStatusType,
     NetworkInterfaceTypeType,
+    NitroEnclavesSupportType,
     OfferingClassTypeType,
     OfferingTypeValuesType,
     OnDemandAllocationStrategyType,
     OperationTypeType,
     PartitionLoadFrequencyType,
     PaymentOptionType,
     PeriodTypeType,
@@ -30418,14 +30419,15 @@
         "PlacementGroupInfo": PlacementGroupInfoTypeDef,
         "InferenceAcceleratorInfo": InferenceAcceleratorInfoTypeDef,
         "HibernationSupported": bool,
         "BurstablePerformanceSupported": bool,
         "DedicatedHostsSupported": bool,
         "AutoRecoverySupported": bool,
         "SupportedBootModes": List[BootModeTypeType],
+        "NitroEnclavesSupport": NitroEnclavesSupportType,
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
```

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/waiter.py` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2/waiter.pyi` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.27.0
-Summary: Type annotations for boto3.EC2 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.EC2 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -1464,14 +1464,15 @@
     NatGatewayStateType,
     NetworkInterfaceAttributeType,
     NetworkInterfaceAvailableWaiterName,
     NetworkInterfaceCreationTypeType,
     NetworkInterfacePermissionStateCodeType,
     NetworkInterfaceStatusType,
     NetworkInterfaceTypeType,
+    NitroEnclavesSupportType,
     OfferingClassTypeType,
     OfferingTypeValuesType,
     OnDemandAllocationStrategyType,
     OperationTypeType,
     PartitionLoadFrequencyType,
     PasswordDataAvailableWaiterName,
     PayerResponsibilityType,
```

### Comparing `mypy-boto3-ec2-1.27.0/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.27.0/setup.py` & `mypy-boto3-ec2-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EC2 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EC2 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

