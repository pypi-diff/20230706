# Comparing `tmp/mypy-boto3-outposts-1.27.0.tar.gz` & `tmp/mypy-boto3-outposts-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-outposts-1.27.0.tar", last modified: Mon Jul  3 19:51:13 2023, max compression
+gzip compressed data, was "mypy-boto3-outposts-1.28.0.tar", last modified: Thu Jul  6 21:00:15 2023, max compression
```

## Comparing `mypy-boto3-outposts-1.27.0.tar` & `mypy-boto3-outposts-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-03 19:43:15.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-03 19:43:15.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-03 19:43:15.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.958387 mypy-boto3-outposts-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-07-06 21:00:15.946387 mypy-boto3-outposts-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.938387 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21380 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24615 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.946387 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:15.958387 mypy-boto3-outposts-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/setup.py
```

### Comparing `mypy-boto3-outposts-1.27.0/LICENSE` & `mypy-boto3-outposts-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.27.0/PKG-INFO` & `mypy-boto3-outposts-1.28.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.27.0
-Summary: Type annotations for boto3.Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -72,14 +72,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -266,14 +267,48 @@
 from mypy_boto3_outposts import OutpostsClient
 
 client: OutpostsClient = Session().client("outposts")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_outposts.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_outposts import OutpostsClient
+from mypy_boto3_outposts.paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
+
+client: OutpostsClient = Session().client("outposts")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
+    "get_outpost_instance_types"
+)
+list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
+list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
+list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
+list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_outposts.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
@@ -282,15 +317,21 @@
     AddressTypeType,
     AssetStateType,
     AssetTypeType,
     CatalogItemClassType,
     CatalogItemStatusType,
     ComputeAssetStateType,
     FiberOpticCableTypeType,
+    GetOutpostInstanceTypesPaginatorName,
     LineItemStatusType,
+    ListAssetsPaginatorName,
+    ListCatalogItemsPaginatorName,
+    ListOrdersPaginatorName,
+    ListOutpostsPaginatorName,
+    ListSitesPaginatorName,
     MaximumSupportedWeightLbsType,
     OpticalStandardType,
     OrderStatusType,
     OrderTypeType,
     PaymentOptionType,
     PaymentTermType,
     PowerConnectorType,
@@ -301,14 +342,15 @@
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
     OutpostsServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
@@ -334,28 +376,35 @@
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetOrderInputRequestTypeDef,
     GetOutpostInputRequestTypeDef,
+    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     GetOutpostInstanceTypesInputRequestTypeDef,
     InstanceTypeItemTypeDef,
     GetSiteAddressInputRequestTypeDef,
     GetSiteInputRequestTypeDef,
     LineItemAssetInformationTypeDef,
     ShipmentInformationTypeDef,
+    ListAssetsInputListAssetsPaginateTypeDef,
     ListAssetsInputRequestTypeDef,
+    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListCatalogItemsInputRequestTypeDef,
+    ListOrdersInputListOrdersPaginateTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
+    ListOutpostsInputListOutpostsPaginateTypeDef,
     ListOutpostsInputRequestTypeDef,
+    ListSitesInputListSitesPaginateTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
     StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
```

### Comparing `mypy-boto3-outposts-1.27.0/README.md` & `mypy-boto3-outposts-1.28.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -40,14 +40,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -234,14 +235,48 @@
 from mypy_boto3_outposts import OutpostsClient
 
 client: OutpostsClient = Session().client("outposts")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_outposts.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_outposts import OutpostsClient
+from mypy_boto3_outposts.paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
+
+client: OutpostsClient = Session().client("outposts")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
+    "get_outpost_instance_types"
+)
+list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
+list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
+list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
+list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_outposts.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
@@ -250,15 +285,21 @@
     AddressTypeType,
     AssetStateType,
     AssetTypeType,
     CatalogItemClassType,
     CatalogItemStatusType,
     ComputeAssetStateType,
     FiberOpticCableTypeType,
+    GetOutpostInstanceTypesPaginatorName,
     LineItemStatusType,
+    ListAssetsPaginatorName,
+    ListCatalogItemsPaginatorName,
+    ListOrdersPaginatorName,
+    ListOutpostsPaginatorName,
+    ListSitesPaginatorName,
     MaximumSupportedWeightLbsType,
     OpticalStandardType,
     OrderStatusType,
     OrderTypeType,
     PaymentOptionType,
     PaymentTermType,
     PowerConnectorType,
@@ -269,14 +310,15 @@
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
     OutpostsServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
@@ -302,28 +344,35 @@
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetOrderInputRequestTypeDef,
     GetOutpostInputRequestTypeDef,
+    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     GetOutpostInstanceTypesInputRequestTypeDef,
     InstanceTypeItemTypeDef,
     GetSiteAddressInputRequestTypeDef,
     GetSiteInputRequestTypeDef,
     LineItemAssetInformationTypeDef,
     ShipmentInformationTypeDef,
+    ListAssetsInputListAssetsPaginateTypeDef,
     ListAssetsInputRequestTypeDef,
+    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListCatalogItemsInputRequestTypeDef,
+    ListOrdersInputListOrdersPaginateTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
+    ListOutpostsInputListOutpostsPaginateTypeDef,
     ListOutpostsInputRequestTypeDef,
+    ListSitesInputListSitesPaginateTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
     StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__main__.py` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Outposts 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.Outposts 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
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

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.py` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     from boto3.session import Session
     from mypy_boto3_outposts.client import OutpostsClient
 
     session = Session()
     client: OutpostsClient = session.client("outposts")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+import sys
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
     CatalogItemClassType,
@@ -31,14 +32,22 @@
     PowerFeedDropType,
     PowerPhaseType,
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
 )
+from .paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
 from .type_defs import (
     AddressTypeDef,
     CreateOrderOutputTypeDef,
     CreateOutpostOutputTypeDef,
     CreateSiteOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     GetConnectionResponseTypeDef,
@@ -58,14 +67,20 @@
     StartConnectionResponseTypeDef,
     UpdateOutpostOutputTypeDef,
     UpdateSiteAddressOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 __all__ = ("OutpostsClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -429,7 +444,53 @@
     ) -> UpdateSiteRackPhysicalPropertiesOutputTypeDef:
         """
         Update the physical and logistical details for a rack at a site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_rack_physical_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#update_site_rack_physical_properties)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["get_outpost_instance_types"]
+    ) -> GetOutpostInstanceTypesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_assets"]) -> ListAssetsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_catalog_items"]
+    ) -> ListCatalogItemsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_outposts"]) -> ListOutpostsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_sites"]) -> ListSitesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.pyi` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     from boto3.session import Session
     from mypy_boto3_outposts.client import OutpostsClient
 
     session = Session()
     client: OutpostsClient = session.client("outposts")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+import sys
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
     CatalogItemClassType,
@@ -31,14 +32,22 @@
     PowerFeedDropType,
     PowerPhaseType,
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
 )
+from .paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
 from .type_defs import (
     AddressTypeDef,
     CreateOrderOutputTypeDef,
     CreateOutpostOutputTypeDef,
     CreateSiteOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     GetConnectionResponseTypeDef,
@@ -58,14 +67,19 @@
     StartConnectionResponseTypeDef,
     UpdateOutpostOutputTypeDef,
     UpdateSiteAddressOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("OutpostsClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -397,7 +411,47 @@
     ) -> UpdateSiteRackPhysicalPropertiesOutputTypeDef:
         """
         Update the physical and logistical details for a rack at a site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_rack_physical_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#update_site_rack_physical_properties)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["get_outpost_instance_types"]
+    ) -> GetOutpostInstanceTypesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_assets"]) -> ListAssetsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_catalog_items"]
+    ) -> ListCatalogItemsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_outposts"]) -> ListOutpostsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_sites"]) -> ListSitesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.py` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AddressTypeType",
     "AssetStateType",
     "AssetTypeType",
     "CatalogItemClassType",
     "CatalogItemStatusType",
     "ComputeAssetStateType",
     "FiberOpticCableTypeType",
+    "GetOutpostInstanceTypesPaginatorName",
     "LineItemStatusType",
+    "ListAssetsPaginatorName",
+    "ListCatalogItemsPaginatorName",
+    "ListOrdersPaginatorName",
+    "ListOutpostsPaginatorName",
+    "ListSitesPaginatorName",
     "MaximumSupportedWeightLbsType",
     "OpticalStandardType",
     "OrderStatusType",
     "OrderTypeType",
     "PaymentOptionType",
     "PaymentTermType",
     "PowerConnectorType",
@@ -42,36 +47,42 @@
     "SupportedHardwareTypeType",
     "SupportedStorageEnumType",
     "UplinkCountType",
     "UplinkGbpsType",
     "OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
-
 AddressTypeType = Literal["OPERATING_ADDRESS", "SHIPPING_ADDRESS"]
-AssetStateType = Literal["ACTIVE", "RETIRING"]
+AssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 AssetTypeType = Literal["COMPUTE"]
 CatalogItemClassType = Literal["RACK", "SERVER"]
 CatalogItemStatusType = Literal["AVAILABLE", "DISCONTINUED"]
 ComputeAssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 FiberOpticCableTypeType = Literal["MULTI_MODE", "SINGLE_MODE"]
+GetOutpostInstanceTypesPaginatorName = Literal["get_outpost_instance_types"]
 LineItemStatusType = Literal[
     "BUILDING",
     "CANCELLED",
     "DELIVERED",
     "ERROR",
     "INSTALLED",
     "INSTALLING",
     "PREPARING",
     "REPLACED",
     "SHIPPED",
 ]
+ListAssetsPaginatorName = Literal["list_assets"]
+ListCatalogItemsPaginatorName = Literal["list_catalog_items"]
+ListOrdersPaginatorName = Literal["list_orders"]
+ListOutpostsPaginatorName = Literal["list_outposts"]
+ListSitesPaginatorName = Literal["list_sites"]
 MaximumSupportedWeightLbsType = Literal[
     "MAX_1400_LBS", "MAX_1600_LBS", "MAX_1800_LBS", "MAX_2000_LBS", "NO_LIMIT"
 ]
 OpticalStandardType = Literal[
     "OPTIC_1000BASE_LX",
     "OPTIC_1000BASE_SX",
     "OPTIC_100GBASE_CWDM4",
@@ -482,14 +493,22 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal[
+    "get_outpost_instance_types",
+    "list_assets",
+    "list_catalog_items",
+    "list_orders",
+    "list_outposts",
+    "list_sites",
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.pyi` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,30 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AddressTypeType",
     "AssetStateType",
     "AssetTypeType",
     "CatalogItemClassType",
     "CatalogItemStatusType",
     "ComputeAssetStateType",
     "FiberOpticCableTypeType",
+    "GetOutpostInstanceTypesPaginatorName",
     "LineItemStatusType",
+    "ListAssetsPaginatorName",
+    "ListCatalogItemsPaginatorName",
+    "ListOrdersPaginatorName",
+    "ListOutpostsPaginatorName",
+    "ListSitesPaginatorName",
     "MaximumSupportedWeightLbsType",
     "OpticalStandardType",
     "OrderStatusType",
     "OrderTypeType",
     "PaymentOptionType",
     "PaymentTermType",
     "PowerConnectorType",
@@ -41,35 +48,43 @@
     "SupportedHardwareTypeType",
     "SupportedStorageEnumType",
     "UplinkCountType",
     "UplinkGbpsType",
     "OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
+
 AddressTypeType = Literal["OPERATING_ADDRESS", "SHIPPING_ADDRESS"]
-AssetStateType = Literal["ACTIVE", "RETIRING"]
+AssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 AssetTypeType = Literal["COMPUTE"]
 CatalogItemClassType = Literal["RACK", "SERVER"]
 CatalogItemStatusType = Literal["AVAILABLE", "DISCONTINUED"]
 ComputeAssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 FiberOpticCableTypeType = Literal["MULTI_MODE", "SINGLE_MODE"]
+GetOutpostInstanceTypesPaginatorName = Literal["get_outpost_instance_types"]
 LineItemStatusType = Literal[
     "BUILDING",
     "CANCELLED",
     "DELIVERED",
     "ERROR",
     "INSTALLED",
     "INSTALLING",
     "PREPARING",
     "REPLACED",
     "SHIPPED",
 ]
+ListAssetsPaginatorName = Literal["list_assets"]
+ListCatalogItemsPaginatorName = Literal["list_catalog_items"]
+ListOrdersPaginatorName = Literal["list_orders"]
+ListOutpostsPaginatorName = Literal["list_outposts"]
+ListSitesPaginatorName = Literal["list_sites"]
 MaximumSupportedWeightLbsType = Literal[
     "MAX_1400_LBS", "MAX_1600_LBS", "MAX_1800_LBS", "MAX_2000_LBS", "NO_LIMIT"
 ]
 OpticalStandardType = Literal[
     "OPTIC_1000BASE_LX",
     "OPTIC_1000BASE_SX",
     "OPTIC_100GBASE_CWDM4",
@@ -480,14 +495,22 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal[
+    "get_outpost_instance_types",
+    "list_assets",
+    "list_catalog_items",
+    "list_orders",
+    "list_outposts",
+    "list_sites",
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.py` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
@@ -63,28 +62,35 @@
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
+    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
+    "ListAssetsInputListAssetsPaginateTypeDef",
     "ListAssetsInputRequestTypeDef",
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
+    "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListOutpostsInputRequestTypeDef",
+    "ListSitesInputListSitesPaginateTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StartConnectionRequestRequestTypeDef",
     "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
@@ -137,19 +143,17 @@
         "AddressLine3": str,
         "DistrictOrCounty": str,
         "Municipality": str,
     },
     total=False,
 )
 
-
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
-
 AssetLocationTypeDef = TypedDict(
     "AssetLocationTypeDef",
     {
         "RackElevation": float,
     },
     total=False,
 )
@@ -217,21 +221,19 @@
         "AvailabilityZoneId": str,
         "Tags": Mapping[str, str],
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
-
 class CreateOutpostInputRequestTypeDef(
     _RequiredCreateOutpostInputRequestTypeDef, _OptionalCreateOutpostInputRequestTypeDef
 ):
     pass
 
-
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "OutpostId": str,
         "OwnerId": str,
         "OutpostArn": str,
         "SiteId": str,
@@ -301,14 +303,34 @@
 GetOutpostInputRequestTypeDef = TypedDict(
     "GetOutpostInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 
+_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
+    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
@@ -316,22 +338,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetOutpostInstanceTypesInputRequestTypeDef(
     _RequiredGetOutpostInstanceTypesInputRequestTypeDef,
     _OptionalGetOutpostInstanceTypesInputRequestTypeDef,
 ):
     pass
 
-
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": str,
     },
     total=False,
 )
@@ -365,14 +385,36 @@
     {
         "ShipmentTrackingNumber": str,
         "ShipmentCarrier": ShipmentCarrierType,
     },
     total=False,
 )
 
+_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+    },
+)
+_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "HostIdFilter": Sequence[str],
+        "StatusFilter": Sequence[AssetStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAssetsInputListAssetsPaginateTypeDef(
+    _RequiredListAssetsInputListAssetsPaginateTypeDef,
+    _OptionalListAssetsInputListAssetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssetsInputRequestTypeDef = TypedDict(
     "_RequiredListAssetsInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
     },
 )
 _OptionalListAssetsInputRequestTypeDef = TypedDict(
@@ -382,33 +424,51 @@
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": Sequence[AssetStateType],
     },
     total=False,
 )
 
-
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
+ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    {
+        "ItemClassFilter": Sequence[CatalogItemClassType],
+        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
+        "EC2FamilyFilter": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
         "EC2FamilyFilter": Sequence[str],
     },
     total=False,
 )
 
+ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOrdersInputRequestTypeDef = TypedDict(
     "ListOrdersInputRequestTypeDef",
     {
         "OutpostIdentifierFilter": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -425,26 +485,48 @@
         "LineItemCountsByStatus": Dict[LineItemStatusType, int],
         "OrderSubmissionDate": datetime,
         "OrderFulfilledDate": datetime,
     },
     total=False,
 )
 
+ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    {
+        "LifeCycleStatusFilter": Sequence[str],
+        "AvailabilityZoneFilter": Sequence[str],
+        "AvailabilityZoneIdFilter": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOutpostsInputRequestTypeDef = TypedDict(
     "ListOutpostsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "LifeCycleStatusFilter": Sequence[str],
         "AvailabilityZoneFilter": Sequence[str],
         "AvailabilityZoneIdFilter": Sequence[str],
     },
     total=False,
 )
 
+ListSitesInputListSitesPaginateTypeDef = TypedDict(
+    "ListSitesInputListSitesPaginateTypeDef",
+    {
+        "OperatingAddressCountryCodeFilter": Sequence[str],
+        "OperatingAddressStateOrRegionFilter": Sequence[str],
+        "OperatingAddressCityFilter": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSitesInputRequestTypeDef = TypedDict(
     "ListSitesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "OperatingAddressCountryCodeFilter": Sequence[str],
         "OperatingAddressStateOrRegionFilter": Sequence[str],
@@ -464,14 +546,24 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -526,21 +618,19 @@
         "Name": str,
         "Description": str,
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
-
 class UpdateOutpostInputRequestTypeDef(
     _RequiredUpdateOutpostInputRequestTypeDef, _OptionalUpdateOutpostInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSiteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteInputRequestTypeDef = TypedDict(
@@ -549,21 +639,19 @@
         "Name": str,
         "Description": str,
         "Notes": str,
     },
     total=False,
 )
 
-
 class UpdateSiteInputRequestTypeDef(
     _RequiredUpdateSiteInputRequestTypeDef, _OptionalUpdateSiteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
@@ -578,22 +666,20 @@
         "FiberOpticCableType": FiberOpticCableTypeType,
         "OpticalStandard": OpticalStandardType,
         "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
     },
     total=False,
 )
 
-
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
-
 GetSiteAddressOutputTypeDef = TypedDict(
     "GetSiteAddressOutputTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -665,21 +751,19 @@
     "_OptionalCreateOrderInputRequestTypeDef",
     {
         "PaymentTerm": PaymentTermType,
     },
     total=False,
 )
 
-
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
-
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -724,21 +808,19 @@
         "OperatingAddress": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
-
 SiteTypeDef = TypedDict(
     "SiteTypeDef",
     {
         "SiteId": str,
         "AccountId": str,
         "Name": str,
         "Description": str,
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.pyi` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
@@ -62,28 +63,35 @@
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
+    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
+    "ListAssetsInputListAssetsPaginateTypeDef",
     "ListAssetsInputRequestTypeDef",
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
+    "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListOutpostsInputRequestTypeDef",
+    "ListSitesInputListSitesPaginateTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StartConnectionRequestRequestTypeDef",
     "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
@@ -136,17 +144,19 @@
         "AddressLine3": str,
         "DistrictOrCounty": str,
         "Municipality": str,
     },
     total=False,
 )
 
+
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
+
 AssetLocationTypeDef = TypedDict(
     "AssetLocationTypeDef",
     {
         "RackElevation": float,
     },
     total=False,
 )
@@ -214,19 +224,21 @@
         "AvailabilityZoneId": str,
         "Tags": Mapping[str, str],
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
+
 class CreateOutpostInputRequestTypeDef(
     _RequiredCreateOutpostInputRequestTypeDef, _OptionalCreateOutpostInputRequestTypeDef
 ):
     pass
 
+
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "OutpostId": str,
         "OwnerId": str,
         "OutpostArn": str,
         "SiteId": str,
@@ -296,14 +308,36 @@
 GetOutpostInputRequestTypeDef = TypedDict(
     "GetOutpostInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 
+_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
+    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
@@ -311,20 +345,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetOutpostInstanceTypesInputRequestTypeDef(
     _RequiredGetOutpostInstanceTypesInputRequestTypeDef,
     _OptionalGetOutpostInstanceTypesInputRequestTypeDef,
 ):
     pass
 
+
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": str,
     },
     total=False,
 )
@@ -358,14 +394,38 @@
     {
         "ShipmentTrackingNumber": str,
         "ShipmentCarrier": ShipmentCarrierType,
     },
     total=False,
 )
 
+_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+    },
+)
+_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "HostIdFilter": Sequence[str],
+        "StatusFilter": Sequence[AssetStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAssetsInputListAssetsPaginateTypeDef(
+    _RequiredListAssetsInputListAssetsPaginateTypeDef,
+    _OptionalListAssetsInputListAssetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssetsInputRequestTypeDef = TypedDict(
     "_RequiredListAssetsInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
     },
 )
 _OptionalListAssetsInputRequestTypeDef = TypedDict(
@@ -375,31 +435,53 @@
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": Sequence[AssetStateType],
     },
     total=False,
 )
 
+
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
+
+ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    {
+        "ItemClassFilter": Sequence[CatalogItemClassType],
+        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
+        "EC2FamilyFilter": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
         "EC2FamilyFilter": Sequence[str],
     },
     total=False,
 )
 
+ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOrdersInputRequestTypeDef = TypedDict(
     "ListOrdersInputRequestTypeDef",
     {
         "OutpostIdentifierFilter": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -416,26 +498,48 @@
         "LineItemCountsByStatus": Dict[LineItemStatusType, int],
         "OrderSubmissionDate": datetime,
         "OrderFulfilledDate": datetime,
     },
     total=False,
 )
 
+ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    {
+        "LifeCycleStatusFilter": Sequence[str],
+        "AvailabilityZoneFilter": Sequence[str],
+        "AvailabilityZoneIdFilter": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOutpostsInputRequestTypeDef = TypedDict(
     "ListOutpostsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "LifeCycleStatusFilter": Sequence[str],
         "AvailabilityZoneFilter": Sequence[str],
         "AvailabilityZoneIdFilter": Sequence[str],
     },
     total=False,
 )
 
+ListSitesInputListSitesPaginateTypeDef = TypedDict(
+    "ListSitesInputListSitesPaginateTypeDef",
+    {
+        "OperatingAddressCountryCodeFilter": Sequence[str],
+        "OperatingAddressStateOrRegionFilter": Sequence[str],
+        "OperatingAddressCityFilter": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSitesInputRequestTypeDef = TypedDict(
     "ListSitesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "OperatingAddressCountryCodeFilter": Sequence[str],
         "OperatingAddressStateOrRegionFilter": Sequence[str],
@@ -455,14 +559,24 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -517,19 +631,21 @@
         "Name": str,
         "Description": str,
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
+
 class UpdateOutpostInputRequestTypeDef(
     _RequiredUpdateOutpostInputRequestTypeDef, _OptionalUpdateOutpostInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSiteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteInputRequestTypeDef = TypedDict(
@@ -538,19 +654,21 @@
         "Name": str,
         "Description": str,
         "Notes": str,
     },
     total=False,
 )
 
+
 class UpdateSiteInputRequestTypeDef(
     _RequiredUpdateSiteInputRequestTypeDef, _OptionalUpdateSiteInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
@@ -565,20 +683,22 @@
         "FiberOpticCableType": FiberOpticCableTypeType,
         "OpticalStandard": OpticalStandardType,
         "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
     },
     total=False,
 )
 
+
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
+
 GetSiteAddressOutputTypeDef = TypedDict(
     "GetSiteAddressOutputTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -650,19 +770,21 @@
     "_OptionalCreateOrderInputRequestTypeDef",
     {
         "PaymentTerm": PaymentTermType,
     },
     total=False,
 )
 
+
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
+
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -707,19 +829,21 @@
         "OperatingAddress": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
+
 SiteTypeDef = TypedDict(
     "SiteTypeDef",
     {
         "SiteId": str,
         "AccountId": str,
         "Name": str,
         "Description": str,
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/PKG-INFO` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.27.0
-Summary: Type annotations for boto3.Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -72,14 +72,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -266,14 +267,48 @@
 from mypy_boto3_outposts import OutpostsClient
 
 client: OutpostsClient = Session().client("outposts")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_outposts.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_outposts import OutpostsClient
+from mypy_boto3_outposts.paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
+
+client: OutpostsClient = Session().client("outposts")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
+    "get_outpost_instance_types"
+)
+list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")
+list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
+list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
+list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_outposts.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
@@ -282,15 +317,21 @@
     AddressTypeType,
     AssetStateType,
     AssetTypeType,
     CatalogItemClassType,
     CatalogItemStatusType,
     ComputeAssetStateType,
     FiberOpticCableTypeType,
+    GetOutpostInstanceTypesPaginatorName,
     LineItemStatusType,
+    ListAssetsPaginatorName,
+    ListCatalogItemsPaginatorName,
+    ListOrdersPaginatorName,
+    ListOutpostsPaginatorName,
+    ListSitesPaginatorName,
     MaximumSupportedWeightLbsType,
     OpticalStandardType,
     OrderStatusType,
     OrderTypeType,
     PaymentOptionType,
     PaymentTermType,
     PowerConnectorType,
@@ -301,14 +342,15 @@
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
     OutpostsServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
@@ -334,28 +376,35 @@
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetOrderInputRequestTypeDef,
     GetOutpostInputRequestTypeDef,
+    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     GetOutpostInstanceTypesInputRequestTypeDef,
     InstanceTypeItemTypeDef,
     GetSiteAddressInputRequestTypeDef,
     GetSiteInputRequestTypeDef,
     LineItemAssetInformationTypeDef,
     ShipmentInformationTypeDef,
+    ListAssetsInputListAssetsPaginateTypeDef,
     ListAssetsInputRequestTypeDef,
+    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListCatalogItemsInputRequestTypeDef,
+    ListOrdersInputListOrdersPaginateTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
+    ListOutpostsInputListOutpostsPaginateTypeDef,
     ListOutpostsInputRequestTypeDef,
+    ListSitesInputListSitesPaginateTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
     StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
```

### Comparing `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/SOURCES.txt` & `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mypy_boto3_outposts/__init__.py
 mypy_boto3_outposts/__init__.pyi
 mypy_boto3_outposts/__main__.py
 mypy_boto3_outposts/client.py
 mypy_boto3_outposts/client.pyi
 mypy_boto3_outposts/literals.py
 mypy_boto3_outposts/literals.pyi
+mypy_boto3_outposts/paginator.py
+mypy_boto3_outposts/paginator.pyi
 mypy_boto3_outposts/py.typed
 mypy_boto3_outposts/type_defs.py
 mypy_boto3_outposts/type_defs.pyi
 mypy_boto3_outposts/version.py
 mypy_boto3_outposts.egg-info/PKG-INFO
 mypy_boto3_outposts.egg-info/SOURCES.txt
 mypy_boto3_outposts.egg-info/dependency_links.txt
```

### Comparing `mypy-boto3-outposts-1.27.0/setup.py` & `mypy-boto3-outposts-1.28.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-outposts",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Outposts 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Outposts 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

