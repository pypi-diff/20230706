# Comparing `tmp/alibabacloud_bpstudio20210931_py2-2.0.0.tar.gz` & `tmp/alibabacloud_bpstudio20210931_py2-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-2.0.0.tar", last modified: Tue Jun 20 05:59:37 2023, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-3.0.0.tar", last modified: Thu Jul  6 09:08:08 2023, max compression
```

## Comparing `alibabacloud_bpstudio20210931_py2-2.0.0.tar` & `alibabacloud_bpstudio20210931_py2-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23930 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)   119210 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 05:59:37.000000 alibabacloud_bpstudio20210931_py2-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-06-20 05:59:36.000000 alibabacloud_bpstudio20210931_py2-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25001 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)   121706 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 09:08:08.000000 alibabacloud_bpstudio20210931_py2-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-07-06 09:08:07.000000 alibabacloud_bpstudio20210931_py2-3.0.0/setup.py
```

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/LICENSE` & `alibabacloud_bpstudio20210931_py2-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_bpstudio20210931_py2
-Version: 2.0.0
+Name: alibabacloud-bpstudio20210931-py2
+Version: 3.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/README-CN.md` & `alibabacloud_bpstudio20210931_py2-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/README.md` & `alibabacloud_bpstudio20210931_py2-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,24 @@
         )
 
     def create_application(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_application_with_options(request, runtime)
 
     def delete_application_with_options(self, request, runtime):
+        """
+        Before you call this operation to delete an application, make sure that the application is in the `Destroyed_Success` state. Otherwise, the application fails to be deleted.`` You can call the [GetApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-getapplication) operation to query the status of an application.
+        
+
+        @param request: DeleteApplicationRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
         if not UtilClient.is_unset(request.resource_group_id):
             body['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -135,14 +145,22 @@
         )
         return TeaCore.from_map(
             bpstudio_20210931_models.DeleteApplicationResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_application(self, request):
+        """
+        Before you call this operation to delete an application, make sure that the application is in the `Destroyed_Success` state. Otherwise, the application fails to be deleted.`` You can call the [GetApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-getapplication) operation to query the status of an application.
+        
+
+        @param request: DeleteApplicationRequest
+
+        @return: DeleteApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_application_with_options(request, runtime)
 
     def deploy_application_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.application_id):
```

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931/models.py` & `alibabacloud_bpstudio20210931_py2-3.0.0/alibabacloud_bpstudio20210931/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class ChangeResourceGroupRequest(TeaModel):
     def __init__(self, new_resource_group_id=None, resource_id=None, resource_type=None):
-        # rg-aek2ajbjoloa23q
+        # The ID of the new resource group.
         self.new_resource_group_id = new_resource_group_id  # type: str
-        # P7RMVSVM9LOVYQOM
+        # The ID of the resource.
         self.resource_id = resource_id  # type: str
-        # APPLICATION
+        # The resource type.
         self.resource_type = resource_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ChangeResourceGroupRequest, self).to_map()
@@ -38,18 +38,21 @@
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
 class ChangeResourceGroupResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
+        # The HTTP status code. A value of 200 indicates that the request is successful. Other values indicate that the request failed.
         self.code = code  # type: long
+        # No business data is returned for this parameter.
         self.data = data  # type: str
+        # The error message returned if the request failed.
         self.message = message  # type: str
-        # Id of the request
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ChangeResourceGroupResponseBody, self).to_map()
@@ -163,15 +166,18 @@
         self.area_id = area_id  # type: str
         # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
         # The parameters that are used to configure the application you want to create. For example, enableMonitor specifies whether to automatically create a CloudMonitor task for the application, and enableReport specifies whether to generate reports.
         self.configuration = configuration  # type: dict[str, str]
         # The instances in which you want to create the application. You can create applications in an existing virtual private cloud (VPC).
         self.instances = instances  # type: list[CreateApplicationRequestInstances]
-        # The name of the application that you want to create.
+        # The name of the application.
+        # 
+        # *   The application name must be unique. You can call the [ListApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-listapplication) operation to query the existing applications.
+        # *   The application name must be 2 to 128 characters in length. The name must start with a letter and cannot start with [http:// or https://. The name can contain letters, digits, underscores (\_), and hyphens (-).](http://https://。、（\_）、（-）。)
         self.name = name  # type: str
         # The ID of the resource group to which the application you want to create belongs.
         self.resource_group_id = resource_group_id  # type: str
         # The ID of the template.
         self.template_id = template_id  # type: str
         # The parameter values that are contained in the template. If the template contains no parameter values, the default values are used.
         self.variables = variables  # type: dict[str, str]
@@ -239,15 +245,18 @@
         self.area_id = area_id  # type: str
         # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
         # The parameters that are used to configure the application you want to create. For example, enableMonitor specifies whether to automatically create a CloudMonitor task for the application, and enableReport specifies whether to generate reports.
         self.configuration_shrink = configuration_shrink  # type: str
         # The instances in which you want to create the application. You can create applications in an existing virtual private cloud (VPC).
         self.instances_shrink = instances_shrink  # type: str
-        # The name of the application that you want to create.
+        # The name of the application.
+        # 
+        # *   The application name must be unique. You can call the [ListApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-listapplication) operation to query the existing applications.
+        # *   The application name must be 2 to 128 characters in length. The name must start with a letter and cannot start with [http:// or https://. The name can contain letters, digits, underscores (\_), and hyphens (-).](http://https://。、（\_）、（-）。)
         self.name = name  # type: str
         # The ID of the resource group to which the application you want to create belongs.
         self.resource_group_id = resource_group_id  # type: str
         # The ID of the template.
         self.template_id = template_id  # type: str
         # The parameter values that are contained in the template. If the template contains no parameter values, the default values are used.
         self.variables_shrink = variables_shrink  # type: str
@@ -603,15 +612,15 @@
 
 
 class ExecuteOperationASyncRequest(TeaModel):
     def __init__(self, attributes=None, operation=None, resource_group_id=None, service_type=None):
         self.attributes = attributes  # type: dict[str, str]
         self.operation = operation  # type: str
         self.resource_group_id = resource_group_id  # type: str
-        # The HTTP status code. A value of 200 indicates that the request is successful, and other values indicate that the request fails.
+        # The type of the service. If you want to perform operations on an Elastic Compute Service (ECS) instance, set ServiceType to ecs.
         self.service_type = service_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ExecuteOperationASyncRequest, self).to_map()
@@ -643,15 +652,15 @@
 
 
 class ExecuteOperationASyncShrinkRequest(TeaModel):
     def __init__(self, attributes_shrink=None, operation=None, resource_group_id=None, service_type=None):
         self.attributes_shrink = attributes_shrink  # type: str
         self.operation = operation  # type: str
         self.resource_group_id = resource_group_id  # type: str
-        # The HTTP status code. A value of 200 indicates that the request is successful, and other values indicate that the request fails.
+        # The type of the service. If you want to perform operations on an Elastic Compute Service (ECS) instance, set ServiceType to ecs.
         self.service_type = service_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ExecuteOperationASyncShrinkRequest, self).to_map()
@@ -681,14 +690,15 @@
             self.service_type = m.get('ServiceType')
         return self
 
 
 class ExecuteOperationASyncResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: int
+        # The ID of the operation.
         self.data = data  # type: str
         self.message = message  # type: str
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -852,15 +862,15 @@
             self.specification = m.get('Specification')
         return self
 
 
 class GetApplicationResponseBodyDataPriceList(TeaModel):
     def __init__(self, charge_type=None, count=None, instance_name=None, lifecycle=None, one_price=None,
                  original_price=None, period=None, price=None, price_unit=None, region=None, remark=None, resource_code=None,
-                 specification=None):
+                 specification=None, type=None):
         # The price unit.
         self.charge_type = charge_type  # type: str
         # The original price.
         self.count = count  # type: long
         # The ID of the resource group to which the application belongs.
         self.instance_name = instance_name  # type: str
         # The ID of the region.
@@ -877,16 +887,20 @@
         self.price_unit = price_unit  # type: str
         # USD/Hour
         self.region = region  # type: str
         # The instance type.
         self.remark = remark  # type: str
         # The time when the application was created.
         self.resource_code = resource_code  # type: str
-        # The total price.
+        # The instance type. This parameter indicates the information about the instance type. For example, 192.168.0.0/16 may be returned for a virtual private cloud (VPC), ecs.g5.large may be returned for an Elastic Compute Service (ECS) instance, and slb.s1.small may be returned for a Server Load Balancer (SLB) instance. If the resource does not have a specific type, an empty value is returned.
         self.specification = specification  # type: str
+        # 创建类型：
+        # </br>新建-1
+        # </br>导入-2
+        self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetApplicationResponseBodyDataPriceList, self).to_map()
         if _map is not None:
@@ -915,14 +929,16 @@
             result['Region'] = self.region
         if self.remark is not None:
             result['Remark'] = self.remark
         if self.resource_code is not None:
             result['ResourceCode'] = self.resource_code
         if self.specification is not None:
             result['Specification'] = self.specification
+        if self.type is not None:
+            result['type'] = self.type
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ChargeType') is not None:
             self.charge_type = m.get('ChargeType')
         if m.get('Count') is not None:
@@ -945,14 +961,16 @@
             self.region = m.get('Region')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
         if m.get('ResourceCode') is not None:
             self.resource_code = m.get('ResourceCode')
         if m.get('Specification') is not None:
             self.specification = m.get('Specification')
+        if m.get('type') is not None:
+            self.type = m.get('type')
         return self
 
 
 class GetApplicationResponseBodyDataResourceList(TeaModel):
     def __init__(self, charge_type=None, lifecycle=None, remark=None, resource_code=None, resource_id=None,
                  resource_name=None, resource_type=None, status=None):
         # The service code.
@@ -1030,19 +1048,19 @@
         self.checklist = checklist  # type: list[GetApplicationResponseBodyDataChecklist]
         # The URL of the application topology image.
         self.create_time = create_time  # type: str
         # The message returned for the request.
         self.description = description  # type: str
         # The resource type.
         self.error = error  # type: str
-        # The ID of the request.
+        # The URL of the image in the database.
         self.image_url = image_url  # type: str
         # The URL of the image in the database.
         self.name = name  # type: str
-        # The ID of the template associated with the application.
+        # The billing results.
         self.price_list = price_list  # type: list[GetApplicationResponseBodyDataPriceList]
         # 1411182597819805/topo-MCEXDI5EL2OM10NY.json
         self.resource_group_id = resource_group_id  # type: str
         # The resource specification.
         self.resource_list = resource_list  # type: list[GetApplicationResponseBodyDataResourceList]
         # Verification passed
         self.status = status  # type: str
@@ -1138,16 +1156,16 @@
             self.template_id = m.get('TemplateId')
         return self
 
 
 class GetApplicationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
         # The deployment result.
-        self.code = code  # type: int
-        # The ID of the resource group.
+        self.code = code  # type: str
+        # The details of the application.
         self.data = data  # type: GetApplicationResponseBodyData
         # Possible application states:
         # 
         # *   Creating: The application is being created.
         # *   Modified: The application has been modified.
         # *   Verifying: The application is being verified.
         # *   Verified_Failure: The application failed to pass the verification.
@@ -1322,15 +1340,15 @@
         return self
 
 
 class GetExecuteOperationResultResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
         # The HTTP status code. A value of 200 indicates that the request is successful.
         self.code = code  # type: int
-        # The details of the operation.
+        # The detailed result of the queried operation.
         self.data = data  # type: GetExecuteOperationResultResponseBodyData
         # The error message.
         self.message = message  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
@@ -1438,21 +1456,17 @@
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
 class GetTemplateResponseBodyDataVariables(TeaModel):
     def __init__(self, attribute=None, data_type=None, default_value=None, variable=None):
-        # 变量名
         self.attribute = attribute  # type: str
-        # 变量类型
         self.data_type = data_type  # type: str
-        # 默认值
         self.default_value = default_value  # type: str
-        # 变量值
         self.variable = variable  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetTemplateResponseBodyDataVariables, self).to_map()
@@ -1545,14 +1559,15 @@
                 self.variables.append(temp_model.from_map(k))
         return self
 
 
 class GetTemplateResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: int
+        # The details of the template.
         self.data = data  # type: GetTemplateResponseBodyData
         self.message = message  # type: str
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -1652,15 +1667,15 @@
 
 
 class GetTokenResponseBodyData(TeaModel):
     def __init__(self, access_key_id=None, access_key_secret=None, bucket=None, endpoint=None, security_token=None,
                  snapshot_bucket=None):
         # The AccessKey ID that is used to access OSS.
         self.access_key_id = access_key_id  # type: str
-        # The AccessKey secret that is used to access OSS.
+        # The AccessKey secret used to access OSS.
         self.access_key_secret = access_key_secret  # type: str
         # The OSS bucket that is used to store the architecture image.
         self.bucket = bucket  # type: str
         # The OSS endpoint.
         self.endpoint = endpoint  # type: str
         # The token that is used to access the Object Storage Service (OSS) bucket that stores the architecture image.
         self.security_token = security_token  # type: str
@@ -1797,14 +1812,15 @@
         self.keyword = keyword  # type: str
         # The HTTP status code.
         self.max_results = max_results  # type: int
         # The ID of the resource group to which the application belongs.
         self.next_token = next_token  # type: int
         self.order_type = order_type  # type: long
         self.resource_group_id = resource_group_id  # type: str
+        # The status of the applications to be returned.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListApplicationRequest, self).to_map()
@@ -1847,14 +1863,15 @@
     def __init__(self, application_id=None, create_time=None, image_url=None, name=None, resource_group_id=None,
                  status=None):
         self.application_id = application_id  # type: str
         self.create_time = create_time  # type: str
         self.image_url = image_url  # type: str
         self.name = name  # type: str
         self.resource_group_id = resource_group_id  # type: str
+        # The status of the application.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListApplicationResponseBodyData, self).to_map()
@@ -1892,14 +1909,15 @@
             self.status = m.get('Status')
         return self
 
 
 class ListApplicationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, next_token=None, request_id=None, total_count=None):
         self.code = code  # type: int
+        # The information about the applications.
         self.data = data  # type: list[ListApplicationResponseBodyData]
         self.message = message  # type: str
         self.next_token = next_token  # type: int
         self.request_id = request_id  # type: str
         self.total_count = total_count  # type: int
 
     def validate(self):
@@ -2228,24 +2246,27 @@
                  tag_list=None, type=None):
         # The keyword that is used to search for templates.
         self.keyword = keyword  # type: str
         # The number of entries to return on each page.
         self.max_results = max_results  # type: int
         # The number of the page to return.
         self.next_token = next_token  # type: int
-        # The criterion by which the templates are sorted. Valid values:
+        # The criterion by which the returned templates are sorted. Valid values:
         # 
-        # *   1: modification time
-        # *   2: creation time
+        # *   1: The templates are sorted by the time when they are updated.
+        # *   2: The templates are sorted by the time when they are created.
+        # *   3: The templates are sorted by the system.
+        # *   4: The templates are sorted by the number of times that they are used.
+        # *   If you specify an integer other than 1, 2, 3, and 4 or do not specify any value, the templates are sorted by the system.
         self.order_type = order_type  # type: long
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The tag of the template.
+        # The tag that you want to use to query templates.
         self.tag_list = tag_list  # type: int
-        # The type of the template.
+        # The type of the templates to be returned. Valid values: public and private
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTemplateRequest, self).to_map()
```

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-bpstudio20210931-py2
-Version: 2.0.0
+Name: alibabacloud_bpstudio20210931_py2
+Version: 3.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-2.0.0/setup.py` & `alibabacloud_bpstudio20210931_py2-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931_py2.
 
-Created on 20/06/2023
+Created on 06/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

