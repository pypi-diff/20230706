# Comparing `tmp/alibabacloud_bpstudio20210931-2.0.0.tar.gz` & `tmp/alibabacloud_bpstudio20210931-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931-2.0.0.tar", last modified: Tue Jun 20 06:00:45 2023, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931-3.0.0.tar", last modified: Thu Jul  6 09:08:39 2023, max compression
```

## Comparing `alibabacloud_bpstudio20210931-2.0.0.tar` & `alibabacloud_bpstudio20210931-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56618 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)   118755 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 06:00:45.000000 alibabacloud_bpstudio20210931-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-06-20 06:00:44.000000 alibabacloud_bpstudio20210931-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58750 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)   121253 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-07-06 09:08:39.000000 alibabacloud_bpstudio20210931-3.0.0/setup.py
```

### Comparing `alibabacloud_bpstudio20210931-2.0.0/LICENSE` & `alibabacloud_bpstudio20210931-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-2.0.0/PKG-INFO` & `alibabacloud_bpstudio20210931-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bpstudio20210931
-Version: 2.0.0
+Version: 3.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-2.0.0/README-CN.md` & `alibabacloud_bpstudio20210931-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-2.0.0/README.md` & `alibabacloud_bpstudio20210931-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,14 +234,21 @@
         return await self.create_application_with_options_async(request, runtime)
 
     def delete_application_with_options(
         self,
         request: bpstudio_20210931_models.DeleteApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> bpstudio_20210931_models.DeleteApplicationResponse:
+        """
+        Before you call this operation to delete an application, make sure that the application is in the `Destroyed_Success` state. Otherwise, the application fails to be deleted.`` You can call the [GetApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-getapplication) operation to query the status of an application.
+        
+        @param request: DeleteApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
         if not UtilClient.is_unset(request.resource_group_id):
             body['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -264,14 +271,21 @@
         )
 
     async def delete_application_with_options_async(
         self,
         request: bpstudio_20210931_models.DeleteApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> bpstudio_20210931_models.DeleteApplicationResponse:
+        """
+        Before you call this operation to delete an application, make sure that the application is in the `Destroyed_Success` state. Otherwise, the application fails to be deleted.`` You can call the [GetApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-getapplication) operation to query the status of an application.
+        
+        @param request: DeleteApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
         if not UtilClient.is_unset(request.resource_group_id):
             body['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -293,21 +307,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_application(
         self,
         request: bpstudio_20210931_models.DeleteApplicationRequest,
     ) -> bpstudio_20210931_models.DeleteApplicationResponse:
+        """
+        Before you call this operation to delete an application, make sure that the application is in the `Destroyed_Success` state. Otherwise, the application fails to be deleted.`` You can call the [GetApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-getapplication) operation to query the status of an application.
+        
+        @param request: DeleteApplicationRequest
+        @return: DeleteApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_application_with_options(request, runtime)
 
     async def delete_application_async(
         self,
         request: bpstudio_20210931_models.DeleteApplicationRequest,
     ) -> bpstudio_20210931_models.DeleteApplicationResponse:
+        """
+        Before you call this operation to delete an application, make sure that the application is in the `Destroyed_Success` state. Otherwise, the application fails to be deleted.`` You can call the [GetApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-getapplication) operation to query the status of an application.
+        
+        @param request: DeleteApplicationRequest
+        @return: DeleteApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_application_with_options_async(request, runtime)
 
     def deploy_application_with_options(
         self,
         request: bpstudio_20210931_models.DeployApplicationRequest,
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931/models.py` & `alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 class ChangeResourceGroupRequest(TeaModel):
     def __init__(
         self,
         new_resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
     ):
-        # rg-aek2ajbjoloa23q
+        # The ID of the new resource group.
         self.new_resource_group_id = new_resource_group_id
-        # P7RMVSVM9LOVYQOM
+        # The ID of the resource.
         self.resource_id = resource_id
-        # APPLICATION
+        # The resource type.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -50,18 +50,21 @@
     def __init__(
         self,
         code: int = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
+        # The HTTP status code. A value of 200 indicates that the request is successful. Other values indicate that the request failed.
         self.code = code
+        # No business data is returned for this parameter.
         self.data = data
+        # The error message returned if the request failed.
         self.message = message
-        # Id of the request
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -194,15 +197,18 @@
         self.area_id = area_id
         # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # The parameters that are used to configure the application you want to create. For example, enableMonitor specifies whether to automatically create a CloudMonitor task for the application, and enableReport specifies whether to generate reports.
         self.configuration = configuration
         # The instances in which you want to create the application. You can create applications in an existing virtual private cloud (VPC).
         self.instances = instances
-        # The name of the application that you want to create.
+        # The name of the application.
+        # 
+        # *   The application name must be unique. You can call the [ListApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-listapplication) operation to query the existing applications.
+        # *   The application name must be 2 to 128 characters in length. The name must start with a letter and cannot start with [http:// or https://. The name can contain letters, digits, underscores (\_), and hyphens (-).](http://https://。、（\_）、（-）。)
         self.name = name
         # The ID of the resource group to which the application you want to create belongs.
         self.resource_group_id = resource_group_id
         # The ID of the template.
         self.template_id = template_id
         # The parameter values that are contained in the template. If the template contains no parameter values, the default values are used.
         self.variables = variables
@@ -279,15 +285,18 @@
         self.area_id = area_id
         # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # The parameters that are used to configure the application you want to create. For example, enableMonitor specifies whether to automatically create a CloudMonitor task for the application, and enableReport specifies whether to generate reports.
         self.configuration_shrink = configuration_shrink
         # The instances in which you want to create the application. You can create applications in an existing virtual private cloud (VPC).
         self.instances_shrink = instances_shrink
-        # The name of the application that you want to create.
+        # The name of the application.
+        # 
+        # *   The application name must be unique. You can call the [ListApplication](https://www.alibabacloud.com/help/zh/bp-studio/latest/api-doc-bpstudio-2021-09-31-api-doc-listapplication) operation to query the existing applications.
+        # *   The application name must be 2 to 128 characters in length. The name must start with a letter and cannot start with [http:// or https://. The name can contain letters, digits, underscores (\_), and hyphens (-).](http://https://。、（\_）、（-）。)
         self.name = name
         # The ID of the resource group to which the application you want to create belongs.
         self.resource_group_id = resource_group_id
         # The ID of the template.
         self.template_id = template_id
         # The parameter values that are contained in the template. If the template contains no parameter values, the default values are used.
         self.variables_shrink = variables_shrink
@@ -689,15 +698,15 @@
         operation: str = None,
         resource_group_id: str = None,
         service_type: str = None,
     ):
         self.attributes = attributes
         self.operation = operation
         self.resource_group_id = resource_group_id
-        # The HTTP status code. A value of 200 indicates that the request is successful, and other values indicate that the request fails.
+        # The type of the service. If you want to perform operations on an Elastic Compute Service (ECS) instance, set ServiceType to ecs.
         self.service_type = service_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -735,15 +744,15 @@
         operation: str = None,
         resource_group_id: str = None,
         service_type: str = None,
     ):
         self.attributes_shrink = attributes_shrink
         self.operation = operation
         self.resource_group_id = resource_group_id
-        # The HTTP status code. A value of 200 indicates that the request is successful, and other values indicate that the request fails.
+        # The type of the service. If you want to perform operations on an Elastic Compute Service (ECS) instance, set ServiceType to ecs.
         self.service_type = service_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -779,14 +788,15 @@
         self,
         code: int = None,
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
         self.code = code
+        # The ID of the operation.
         self.data = data
         self.message = message
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -980,14 +990,15 @@
         period: float = None,
         price: float = None,
         price_unit: str = None,
         region: str = None,
         remark: str = None,
         resource_code: str = None,
         specification: str = None,
+        type: str = None,
     ):
         # The price unit.
         self.charge_type = charge_type
         # The original price.
         self.count = count
         # The ID of the resource group to which the application belongs.
         self.instance_name = instance_name
@@ -1005,16 +1016,20 @@
         self.price_unit = price_unit
         # USD/Hour
         self.region = region
         # The instance type.
         self.remark = remark
         # The time when the application was created.
         self.resource_code = resource_code
-        # The total price.
+        # The instance type. This parameter indicates the information about the instance type. For example, 192.168.0.0/16 may be returned for a virtual private cloud (VPC), ecs.g5.large may be returned for an Elastic Compute Service (ECS) instance, and slb.s1.small may be returned for a Server Load Balancer (SLB) instance. If the resource does not have a specific type, an empty value is returned.
         self.specification = specification
+        # 创建类型：
+        # </br>新建-1
+        # </br>导入-2
+        self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1043,14 +1058,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ChargeType') is not None:
             self.charge_type = m.get('ChargeType')
         if m.get('Count') is not None:
@@ -1073,14 +1090,16 @@
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
     def __init__(
         self,
         charge_type: str = None,
@@ -1179,19 +1198,19 @@
         self.checklist = checklist
         # The URL of the application topology image.
         self.create_time = create_time
         # The message returned for the request.
         self.description = description
         # The resource type.
         self.error = error
-        # The ID of the request.
+        # The URL of the image in the database.
         self.image_url = image_url
         # The URL of the image in the database.
         self.name = name
-        # The ID of the template associated with the application.
+        # The billing results.
         self.price_list = price_list
         # 1411182597819805/topo-MCEXDI5EL2OM10NY.json
         self.resource_group_id = resource_group_id
         # The resource specification.
         self.resource_list = resource_list
         # Verification passed
         self.status = status
@@ -1287,22 +1306,22 @@
             self.template_id = m.get('TemplateId')
         return self
 
 
 class GetApplicationResponseBody(TeaModel):
     def __init__(
         self,
-        code: int = None,
+        code: str = None,
         data: GetApplicationResponseBodyData = None,
         message: str = None,
         request_id: str = None,
     ):
         # The deployment result.
         self.code = code
-        # The ID of the resource group.
+        # The details of the application.
         self.data = data
         # Possible application states:
         # 
         # *   Creating: The application is being created.
         # *   Modified: The application has been modified.
         # *   Verifying: The application is being verified.
         # *   Verified_Failure: The application failed to pass the verification.
@@ -1498,15 +1517,15 @@
         code: int = None,
         data: GetExecuteOperationResultResponseBodyData = None,
         message: str = None,
         request_id: str = None,
     ):
         # The HTTP status code. A value of 200 indicates that the request is successful.
         self.code = code
-        # The details of the operation.
+        # The detailed result of the queried operation.
         self.data = data
         # The error message.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
@@ -1630,21 +1649,17 @@
     def __init__(
         self,
         attribute: str = None,
         data_type: str = None,
         default_value: str = None,
         variable: str = None,
     ):
-        # 变量名
         self.attribute = attribute
-        # 变量类型
         self.data_type = data_type
-        # 默认值
         self.default_value = default_value
-        # 变量值
         self.variable = variable
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1751,14 +1766,15 @@
         self,
         code: int = None,
         data: GetTemplateResponseBodyData = None,
         message: str = None,
         request_id: str = None,
     ):
         self.code = code
+        # The details of the template.
         self.data = data
         self.message = message
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -1873,15 +1889,15 @@
         bucket: str = None,
         endpoint: str = None,
         security_token: str = None,
         snapshot_bucket: str = None,
     ):
         # The AccessKey ID that is used to access OSS.
         self.access_key_id = access_key_id
-        # The AccessKey secret that is used to access OSS.
+        # The AccessKey secret used to access OSS.
         self.access_key_secret = access_key_secret
         # The OSS bucket that is used to store the architecture image.
         self.bucket = bucket
         # The OSS endpoint.
         self.endpoint = endpoint
         # The token that is used to access the Object Storage Service (OSS) bucket that stores the architecture image.
         self.security_token = security_token
@@ -2036,14 +2052,15 @@
         self.keyword = keyword
         # The HTTP status code.
         self.max_results = max_results
         # The ID of the resource group to which the application belongs.
         self.next_token = next_token
         self.order_type = order_type
         self.resource_group_id = resource_group_id
+        # The status of the applications to be returned.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2093,14 +2110,15 @@
         status: str = None,
     ):
         self.application_id = application_id
         self.create_time = create_time
         self.image_url = image_url
         self.name = name
         self.resource_group_id = resource_group_id
+        # The status of the application.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2146,14 +2164,15 @@
         data: List[ListApplicationResponseBodyData] = None,
         message: str = None,
         next_token: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
         self.code = code
+        # The information about the applications.
         self.data = data
         self.message = message
         self.next_token = next_token
         self.request_id = request_id
         self.total_count = total_count
 
     def validate(self):
@@ -2524,24 +2543,27 @@
     ):
         # The keyword that is used to search for templates.
         self.keyword = keyword
         # The number of entries to return on each page.
         self.max_results = max_results
         # The number of the page to return.
         self.next_token = next_token
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
         self.order_type = order_type
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
-        # The tag of the template.
+        # The tag that you want to use to query templates.
         self.tag_list = tag_list
-        # The type of the template.
+        # The type of the templates to be returned. Valid values: public and private
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_bpstudio20210931-2.0.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931-3.0.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bpstudio20210931
-Version: 2.0.0
+Version: 3.0.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-2.0.0/setup.py` & `alibabacloud_bpstudio20210931-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931.
 
-Created on 20/06/2023
+Created on 06/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

