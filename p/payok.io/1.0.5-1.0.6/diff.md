# Comparing `tmp/payok.io-1.0.5.tar.gz` & `tmp/payok.io-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payok.io-1.0.5.tar", last modified: Sun Jun 11 23:07:37 2023, max compression
+gzip compressed data, was "payok.io-1.0.6.tar", last modified: Thu Jul  6 10:29:02 2023, max compression
```

## Comparing `payok.io-1.0.5.tar` & `payok.io-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.5/LICENSE
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-06-11 23:07:37.327316 payok.io-1.0.5/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1518 2023-05-17 15:09:15.000000 payok.io-1.0.5/README.md
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.323316 payok.io-1.0.5/payok/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      494 2023-05-17 14:50:33.000000 payok.io-1.0.5/payok/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     7284 2023-06-11 23:05:53.000000 payok.io-1.0.5/payok/api.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/payok/enums/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      362 2023-05-17 13:37:52.000000 payok.io-1.0.5/payok/enums/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.5/payok/enums/base.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.5/payok/enums/comission_type.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.5/payok/enums/currency.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.5/payok/enums/pay_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.5/payok/enums/payment_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.5/payok/enums/payout_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.5/payok/enums/webhook_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      272 2023-05-17 14:06:53.000000 payok.io-1.0.5/payok/exceptions.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/payok/models/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.5/payok/models/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.5/payok/models/balance.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      196 2023-05-17 14:49:19.000000 payok.io-1.0.5/payok/models/new_payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      898 2023-06-11 23:05:12.000000 payok.io-1.0.5/payok/models/payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1021 2023-06-11 23:05:07.000000 payok.io-1.0.5/payok/models/transaction.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/payok.io.egg-info/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      576 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/SOURCES.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/dependency_links.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       17 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/requires.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        6 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/top_level.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-06-11 23:07:37.327316 payok.io-1.0.5/setup.cfg
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1269 2023-06-11 23:06:14.000000 payok.io-1.0.5/setup.py
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-07-06 10:29:02.512584 payok.io-1.0.6/
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.6/LICENSE
+-rw-r--r--   0 bifle     (1000) bifle     (1000)     2309 2023-07-06 10:29:02.512584 payok.io-1.0.6/PKG-INFO
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)     1518 2023-05-17 15:09:15.000000 payok.io-1.0.6/README.md
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-07-06 10:29:02.509250 payok.io-1.0.6/payok/
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      494 2023-07-06 10:28:33.000000 payok.io-1.0.6/payok/__init__.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)     7267 2023-07-06 10:28:10.000000 payok.io-1.0.6/payok/api.py
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-07-06 10:29:02.512584 payok.io-1.0.6/payok/enums/
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      362 2023-07-06 10:27:32.000000 payok.io-1.0.6/payok/enums/__init__.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.6/payok/enums/base.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.6/payok/enums/comission_type.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.6/payok/enums/currency.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.6/payok/enums/pay_status.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.6/payok/enums/payment_method.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.6/payok/enums/payout_method.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.6/payok/enums/webhook_status.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      268 2023-07-06 10:25:58.000000 payok.io-1.0.6/payok/exceptions.py
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-07-06 10:29:02.512584 payok.io-1.0.6/payok/models/
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.6/payok/models/__init__.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.6/payok/models/balance.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      196 2023-07-06 10:27:20.000000 payok.io-1.0.6/payok/models/new_payout.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      898 2023-07-06 10:27:15.000000 payok.io-1.0.6/payok/models/payout.py
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)     1087 2023-07-06 10:27:11.000000 payok.io-1.0.6/payok/models/transaction.py
+drwxr-xr-x   0 bifle     (1000) bifle     (1000)        0 2023-07-06 10:29:02.509250 payok.io-1.0.6/payok.io.egg-info/
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)     2309 2023-07-06 10:29:02.000000 payok.io-1.0.6/payok.io.egg-info/PKG-INFO
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)      576 2023-07-06 10:29:02.000000 payok.io-1.0.6/payok.io.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)        1 2023-07-06 10:29:02.000000 payok.io-1.0.6/payok.io.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)       17 2023-07-06 10:29:02.000000 payok.io-1.0.6/payok.io.egg-info/requires.txt
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)        6 2023-07-06 10:29:02.000000 payok.io-1.0.6/payok.io.egg-info/top_level.txt
+-rw-r--r--   0 bifle     (1000) bifle     (1000)       38 2023-07-06 10:29:02.512584 payok.io-1.0.6/setup.cfg
+-rwxr-xr-x   0 bifle     (1000) bifle     (1000)     1269 2023-07-06 10:28:50.000000 payok.io-1.0.6/setup.py
```

### Comparing `payok.io-1.0.5/LICENSE` & `payok.io-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.5/PKG-INFO` & `payok.io-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.5
+Version: 1.0.6
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
```

### Comparing `payok.io-1.0.5/README.md` & `payok.io-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.5/payok/api.py` & `payok.io-1.0.6/payok/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import hashlib
 
-from .models import (
-    Transaction, 
-    NewPayout,
-    Payout, 
-    Balance,
-)
+from typing import Union, Optional, List
+from urllib.parse import urlencode
+
+from aiohttp import ClientSession
+
 from .enums import (
     Currency,
     ComissionType,
     PaymentMethod,
     PayoutMethod,
 )
 from .exceptions import PayOKError
-
-from typing import Union, Optional, List
-from urllib.parse import urlencode
-
-from aiohttp import ClientSession
+from .models import (
+    Transaction,
+    NewPayout,
+    Payout,
+    Balance,
+)
 
 
 class PayOK(object):
     """
     PayOK API Wrapper
     """
 
     API_URL = 'https://payok.io/api/%s'
 
     def __init__(
-        self, 
-        api_id: int, 
-        api_key: str, 
-        project_id: Optional[int]=None, 
+        self,
+        api_id: int,
+        api_key: str,
+        project_id: Optional[int]=None,
         project_secret: Optional[str]=None,
         session: Optional[ClientSession]=None,
     ) -> None:
         """
         Initialize the wrapper
 
         :param int api_id: API ID
@@ -62,15 +62,15 @@
         :param dict response: API response
         :raises PayOKError: Base API error
         """
 
         if response.get('status') == 'error':
 
             raise PayOKError(
-                response['error_code'], 
+                response['error_code'],
                 response.get('error_text') or response.get('text'),
             )
 
 
     async def _make_request(self, endpoint: str, **kwargs) -> dict:
         """
         Make a request to the API
@@ -82,15 +82,15 @@
         async with self.session.post(
             self.API_URL % endpoint,
             data={
                 **{
                     key: value
                     for key, value in kwargs.items()
                     if value is not None
-                }, 
+                },
                 'API_ID': self.api_id,
                 'API_KEY': self.api_key,
             },
         ) as response:
 
             data = await response.json(content_type=None)
             self._check_response(data)
@@ -121,15 +121,15 @@
 
         result = await self._make_request(
             'transaction',
             payment=payment_id,
             offset=offset,
             shop=project_id or self.project_id,
         )
-        
+
         result.pop('status')
         return [
             Transaction(**transaction)
             for transaction in result.values()
         ]
 
 
@@ -182,15 +182,15 @@
             comission_type=comission_type,
             webhook_url=webhook_url,
         )
         return NewPayout(**result)
 
 
     async def create_bill(
-        self, 
+        self,
         pay_id: int,
         amount: Union[int, float],
         currency: Union[Currency, str]=Currency.RUB,
         description: str='Payment',
         method: Optional[Union[PaymentMethod, str]]=None,
         email: Optional[str]=None,
         success_url: Optional[str]=None,
```

### Comparing `payok.io-1.0.5/payok/models/payout.py` & `payok.io-1.0.6/payok/models/payout.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from ..enums import PayoutMethod, PayStatus
-
 from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel, validator
 from pydantic.fields import Field
 
+from ..enums import PayoutMethod, PayStatus
+
 
 class Payout(BaseModel):
     """
     Class for Payout model
     """
 
     payout_id: int = Field(..., alias='payout')
```

### Comparing `payok.io-1.0.5/payok/models/transaction.py` & `payok.io-1.0.6/payok/models/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import json
 
-from ..enums import (
-    Currency,
-    PayStatus, 
-    WebhookStatus, 
-)
-
 from datetime import datetime
-from typing import Dict, Any
+from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, validator
 from pydantic.fields import Field
 
+from ..enums import Currency, PayStatus, WebhookStatus
+
 
 class Transaction(BaseModel):
     """
     Class for Transaction model
     """
 
     id: int = Field(..., alias='payment_id')
     description: str
     email: str
     amount: float
-    amount_profit: float 
+    amount_profit: float
     currency: Currency
     comission_percent: float
     comission_fixed: float
     method: str
     transaction: int
     date: datetime
     pay_date: datetime = None
     status: PayStatus = Field(PayStatus.waiting, alias='transaction_status')
-    custom_fields: Dict[str, Any]
+    custom_fields: Optional[Dict[str, Any]]
     webhook_status: WebhookStatus
     webhook_amount: int
 
     @property
     def is_paid(self) -> bool:
 
         return bool(self.status)
 
     @validator('custom_fields', pre=True)
-    def validate_fields(raw_field: str) -> dict:
+    def validate_fields(raw_field: str) -> Optional[Dict]:
+
+        if raw_field is None:
+
+            return None
 
         string = raw_field.replace('&quot;', '"')
         return json.loads(string)
```

### Comparing `payok.io-1.0.5/payok.io.egg-info/PKG-INFO` & `payok.io-1.0.6/payok.io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.5
+Version: 1.0.6
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
```

### Comparing `payok.io-1.0.5/payok.io.egg-info/SOURCES.txt` & `payok.io-1.0.6/payok.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.5/setup.py` & `payok.io-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as file:
 
     long_description = "\n" + file.read()
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = 'Asynchronous PayOK API wrapper'
 
 setup(
     name="payok.io",
     version=VERSION,
     author="Nikita Minaev",
     author_email="<nikita@minaev.su>",
```

