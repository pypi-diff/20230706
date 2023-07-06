# Comparing `tmp/stigg_api_client_v2-0.474.0.tar.gz` & `tmp/stigg_api_client_v2-0.475.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.474.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.475.5.tar", max compression
```

## Comparing `stigg_api_client_v2-0.474.0.tar` & `stigg_api_client_v2-0.475.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-07-05 03:16:34.813516 stigg_api_client_v2-0.474.0/README.md
--rw-r--r--   0        0        0      432 2023-07-05 03:17:22.426191 stigg_api_client_v2-0.474.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-05 03:16:34.813516 stigg_api_client_v2-0.474.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-05 03:16:34.813516 stigg_api_client_v2-0.474.0/stigg/client.py
--rw-r--r--   0        0        0    39793 2023-07-05 03:17:20.486167 stigg_api_client_v2-0.474.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-07-05 03:17:20.114163 stigg_api_client_v2-0.474.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    66833 2023-07-05 03:17:20.330165 stigg_api_client_v2-0.474.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-05 03:17:14.586088 stigg_api_client_v2-0.474.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-05 03:17:20.114163 stigg_api_client_v2-0.474.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-05 03:17:19.034149 stigg_api_client_v2-0.474.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-05 03:17:19.050150 stigg_api_client_v2-0.474.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    66418 2023-07-05 03:17:14.798091 stigg_api_client_v2-0.474.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-05 03:17:19.078150 stigg_api_client_v2-0.474.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    23994 2023-07-05 03:17:16.494115 stigg_api_client_v2-0.474.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-05 03:17:19.038149 stigg_api_client_v2-0.474.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-05 03:17:19.046149 stigg_api_client_v2-0.474.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-05 03:17:20.114163 stigg_api_client_v2-0.474.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    54916 2023-07-05 03:17:20.110162 stigg_api_client_v2-0.474.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-05 03:17:19.102150 stigg_api_client_v2-0.474.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-05 03:17:19.110150 stigg_api_client_v2-0.474.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-05 03:17:19.094150 stigg_api_client_v2-0.474.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-05 03:17:19.154151 stigg_api_client_v2-0.474.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-05 03:17:19.126150 stigg_api_client_v2-0.474.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-05 03:17:19.122150 stigg_api_client_v2-0.474.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-05 03:17:19.162151 stigg_api_client_v2-0.474.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-05 03:17:19.114150 stigg_api_client_v2-0.474.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-05 03:17:19.138151 stigg_api_client_v2-0.474.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-05 03:17:19.146151 stigg_api_client_v2-0.474.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-05 03:17:18.998149 stigg_api_client_v2-0.474.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-05 03:17:18.990149 stigg_api_client_v2-0.474.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-05 03:17:19.018149 stigg_api_client_v2-0.474.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126193 2023-07-05 03:17:18.970148 stigg_api_client_v2-0.474.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-05 03:17:19.086150 stigg_api_client_v2-0.474.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-05 03:17:18.982149 stigg_api_client_v2-0.474.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-05 03:17:19.014149 stigg_api_client_v2-0.474.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-05 03:17:19.070150 stigg_api_client_v2-0.474.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-05 03:17:19.066150 stigg_api_client_v2-0.474.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-05 03:17:19.062150 stigg_api_client_v2-0.474.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-05 03:17:20.118162 stigg_api_client_v2-0.474.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-05 03:17:19.002149 stigg_api_client_v2-0.474.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-05 03:17:19.026149 stigg_api_client_v2-0.474.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-05 03:17:19.170151 stigg_api_client_v2-0.474.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.474.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-06 13:22:57.896727 stigg_api_client_v2-0.475.5/README.md
+-rw-r--r--   0        0        0      432 2023-07-06 13:24:04.741698 stigg_api_client_v2-0.475.5/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-06 13:22:57.900727 stigg_api_client_v2-0.475.5/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-06 13:22:57.900727 stigg_api_client_v2-0.475.5/stigg/client.py
+-rw-r--r--   0        0        0    39793 2023-07-06 13:24:02.453669 stigg_api_client_v2-0.475.5/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-07-06 13:24:01.957663 stigg_api_client_v2-0.475.5/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    66833 2023-07-06 13:24:02.241666 stigg_api_client_v2-0.475.5/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-06 13:23:55.133563 stigg_api_client_v2-0.475.5/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-06 13:24:01.957663 stigg_api_client_v2-0.475.5/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-06 13:24:00.693646 stigg_api_client_v2-0.475.5/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-06 13:24:00.713647 stigg_api_client_v2-0.475.5/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    66418 2023-07-06 13:23:55.421567 stigg_api_client_v2-0.475.5/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-06 13:24:00.749647 stigg_api_client_v2-0.475.5/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    23994 2023-07-06 13:23:57.441597 stigg_api_client_v2-0.475.5/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-06 13:24:00.697646 stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-06 13:24:00.709647 stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-06 13:24:01.957663 stigg_api_client_v2-0.475.5/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    54916 2023-07-06 13:24:01.953662 stigg_api_client_v2-0.475.5/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-06 13:24:00.777648 stigg_api_client_v2-0.475.5/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-06 13:24:00.785648 stigg_api_client_v2-0.475.5/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-06 13:24:00.765647 stigg_api_client_v2-0.475.5/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-06 13:24:00.837648 stigg_api_client_v2-0.475.5/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-06 13:24:00.805648 stigg_api_client_v2-0.475.5/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-06 13:24:00.801648 stigg_api_client_v2-0.475.5/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-06 13:24:00.849649 stigg_api_client_v2-0.475.5/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-06 13:24:00.793648 stigg_api_client_v2-0.475.5/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-06 13:24:00.821648 stigg_api_client_v2-0.475.5/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-06 13:24:00.833648 stigg_api_client_v2-0.475.5/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-06 13:24:00.649646 stigg_api_client_v2-0.475.5/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-06 13:24:00.641646 stigg_api_client_v2-0.475.5/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-06 13:24:00.673646 stigg_api_client_v2-0.475.5/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126250 2023-07-06 13:24:00.617645 stigg_api_client_v2-0.475.5/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-06 13:24:00.757647 stigg_api_client_v2-0.475.5/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-06 13:24:00.633645 stigg_api_client_v2-0.475.5/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-06 13:24:00.669646 stigg_api_client_v2-0.475.5/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-06 13:24:00.741647 stigg_api_client_v2-0.475.5/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-06 13:24:00.733647 stigg_api_client_v2-0.475.5/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-06 13:24:00.725647 stigg_api_client_v2-0.475.5/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-06 13:24:01.961663 stigg_api_client_v2-0.475.5/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-06 13:24:00.653646 stigg_api_client_v2-0.475.5/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-06 13:24:00.685646 stigg_api_client_v2-0.475.5/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-06 13:24:00.861649 stigg_api_client_v2-0.475.5/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.475.5/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.474.0/README.md` & `stigg_api_client_v2-0.475.5/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.474.0/stigg/client.py` & `stigg_api_client_v2-0.475.5/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.475.5/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.475.5/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.475.5/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.475.5/stigg/generated/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:23
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.475.5/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.475.5/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/client.py` & `stigg_api_client_v2-0.475.5/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:23
 # Source: operations.graphql
 
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.475.5/stigg/generated/create_subscription.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.475.5/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:23
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.475.5/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.475.5/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -124,14 +124,25 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -146,25 +157,14 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,18 +328,14 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalSubscriptionPriceFragment(BaseModel):
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     billing_model: Optional[BillingModel] = Field(alias="billingModel")
     price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
     feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
@@ -352,21 +348,14 @@
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -410,14 +399,21 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -504,14 +500,18 @@
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -546,14 +546,65 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -633,65 +684,14 @@
 
 
 class TotalPriceFragmentTotal(BaseModel):
     amount: float
     currency: Currency
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -842,34 +842,14 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -884,14 +864,34 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1322,17 +1322,17 @@
 PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1346,63 +1346,63 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
@@ -1418,19 +1418,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.475.5/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.475.5/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.475.5/stigg/generated/get_customer_by_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.475.5/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.475.5/stigg/generated/get_mock_paywall.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.475.5/stigg/generated/get_products.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.475.5/stigg/generated/get_sdk_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.475.5/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -539,14 +539,15 @@
     custom_css: Optional[str] = Field(alias="customCss")
     palette: Optional["CustomerPortalColorsPaletteInput"]
     typography: Optional["TypographyConfigurationInput"]
 
 
 class CustomerPortalInput(BaseModel):
     customer_id: str = Field(alias="customerId")
+    product_id: Optional[str] = Field(alias="productId")
     resource_id: Optional[str] = Field(alias="resourceId")
 
 
 class CustomerResourceFilter(BaseModel):
     and_: Optional[List["CustomerResourceFilter"]] = Field(alias="and")
     created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
     customer: Optional["CustomerResourceFilterCustomerFilter"]
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.475.5/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.475.5/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.475.5/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.474.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.475.5/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-05 03:17
+# Generated by ariadne-codegen on 2023-07-06 13:24
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.474.0/PKG-INFO` & `stigg_api_client_v2-0.475.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.474.0
+Version: 0.475.5
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

