# Comparing `tmp/mbnk-0.1.3a0.tar.gz` & `tmp/mbnk-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.1.3a0.tar", max compression
+gzip compressed data, was "mbnk-0.2.0a1.tar", max compression
```

## Comparing `mbnk-0.1.3a0.tar` & `mbnk-0.2.0a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1799 2023-07-02 23:48:44.152523 mbnk-0.1.3a0/README.md
--rw-r--r--   0        0        0      275 2023-07-03 02:00:50.620267 mbnk-0.1.3a0/mbnk/__init__.py
--rw-r--r--   0        0        0    18631 2023-07-03 20:39:34.795786 mbnk-0.1.3a0/mbnk/api.py
--rw-r--r--   0        0        0      140 2023-07-03 20:40:21.439433 mbnk-0.1.3a0/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0     1031 2023-07-03 20:39:56.655610 mbnk-0.1.3a0/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     1347 2023-07-02 22:17:52.460089 mbnk-0.1.3a0/mbnk/enums.py
--rw-r--r--   0        0        0      576 2023-07-03 00:10:27.269164 mbnk-0.1.3a0/mbnk/exceptions.py
--rw-r--r--   0        0        0     2231 2023-07-03 20:43:41.014672 mbnk-0.1.3a0/mbnk/instances.py
--rw-r--r--   0        0        0     1001 2023-07-03 20:42:01.586927 mbnk-0.1.3a0/mbnk/mbnk.py
--rw-r--r--   0        0        0     2286 2023-07-03 20:44:17.082624 mbnk-0.1.3a0/mbnk/responses.py
--rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.1.3a0/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.1.3a0/mbnk/utils/webhook.py
--rw-r--r--   0        0        0      315 2023-07-03 20:49:16.142760 mbnk-0.1.3a0/pyproject.toml
--rw-r--r--   0        0        0     2332 1970-01-01 00:00:00.000000 mbnk-0.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-02 23:48:44.152523 mbnk-0.2.0a1/README.md
+-rw-r--r--   0        0        0      132 2023-07-04 19:21:42.905297 mbnk-0.2.0a1/mbnk/__init__.py
+-rw-r--r--   0        0        0    21427 2023-07-04 23:57:55.350130 mbnk-0.2.0a1/mbnk/api.py
+-rw-r--r--   0        0        0      140 2023-07-03 20:40:21.439433 mbnk-0.2.0a1/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0     1040 2023-07-04 19:35:03.317343 mbnk-0.2.0a1/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0      576 2023-07-03 00:10:27.269164 mbnk-0.2.0a1/mbnk/exceptions.py
+-rw-r--r--   0        0        0     1010 2023-07-04 23:55:38.778794 mbnk-0.2.0a1/mbnk/mbnk.py
+-rw-r--r--   0        0        0      112 2023-07-04 23:50:51.520123 mbnk-0.2.0a1/mbnk/responses.py
+-rw-r--r--   0        0        0     5286 2023-07-04 23:54:14.419195 mbnk-0.2.0a1/mbnk/types.py
+-rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.2.0a1/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      603 2023-07-04 23:49:14.420543 mbnk-0.2.0a1/mbnk/utils/signature.py
+-rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.2.0a1/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      315 2023-07-05 00:01:57.640919 mbnk-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2332 1970-01-01 00:00:00.000000 mbnk-0.2.0a1/PKG-INFO
```

### Comparing `mbnk-0.1.3a0/README.md` & `mbnk-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.3a0/mbnk/api.py` & `mbnk-0.2.0a1/mbnk/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 __all__ = [
     'MonobankOpenAPIModel',
     'MonobankCorporateOpenAPIModel',
     'MonoAcquiringAPIModel'
 ]
 
+import base64
+import codecs
+
+import ecdsa
+import hashlib
+
 import re
 import json
 import requests
 
+from enum import Enum
+from datetime import datetime
+
 from requests import Response
 from aiohttp import (
     ClientSession,
     ClientResponse
 )
 from typing import Union, Optional
 
-from mbnk.enums import APIPaths
-
 from mbnk.exceptions import *
 
-from mbnk.instances import *
+from mbnk.types import *
 
 from mbnk.responses import *
 
+import dataclasses
+
 
 class APIMethod:
 
     __api_token = None
     __headers = {}
 
     def __init__(
             self,
             base_url: str,
-            api_token: str,
             _async: bool,
+            api_token: Optional[str] = None,
     ):
         self.__is_async: bool = _async
-        self.__api_token: str = api_token
         self.__base_url: str = base_url
-        self.__headers["X-Token"] = self.__api_token
+
+        if api_token is not None:
+            self.__api_token: str = api_token
+            self.__headers["X-Token"] = self.__api_token
 
     @staticmethod
     def __camel_to_underscore(text: str):
         camel_pat = re.compile(r'([A-Z])')
         return camel_pat.sub(lambda x: '_' + x.group(1).lower(), text)
 
     @staticmethod
@@ -70,16 +81,23 @@
 
     def __build_data(self, **kwargs):
         data = {}
 
         for kwarg in kwargs:
             key = kwarg.replace("timestamp", "")
             key = self.__underscore_to_camel(key)
+
             value = kwargs.get(kwarg)
-            data[key] = value
+
+            if dataclasses.is_dataclass(value):
+                data[key] = value.export()
+            else:
+                data[key] = value
+
+        data = self.__json_convert(data, self.__underscore_to_camel)
 
         return data
 
     @staticmethod
     def __is_exception(response: Union[Response, ClientResponse]) -> bool:
         if isinstance(response, Response):
             status_code = response.status_code
@@ -150,19 +168,77 @@
                     data=json.dumps(data) if data is not None else None,
                     params=params
             ) as response:
                 response_data = await response.json()
                 response_data = self.__load_response(response_data)
 
                 if self.__is_exception(response):
-                    return MonoPayAPIException(**response_data)
+                    raise self.__get_exception(response)
 
                 return response_data
 
     @staticmethod
+    def _time_header():
+        def outer(func):
+            def inner(self):
+                self.__headers["X-Time"]: str = str(int(datetime.now().timestamp()))
+
+            return inner
+
+        return outer
+
+    @staticmethod
+    def _key_id_header():
+        def outer(func):
+            def inner(self):
+                self.__headers["X-Key-Id"]: str = self.__key_id
+
+            return inner
+
+        return outer
+
+    @staticmethod
+    def __generate_request_id():
+        request_id = ""
+
+        return request_id
+
+    @staticmethod
+    def _request_id_header():
+        def outer(func):
+            def inner(self):
+                self.__headers["X-Request-Id"]: str = self.__generate_request_id()
+
+            return inner
+
+        return outer
+
+    @staticmethod
+    def __create_signature(self):
+        print(self.__headers)
+        url = "https://api.monobank.ua"
+        data = (self.__headers["X-Time"] + url).encode('utf-8')
+
+        private_key = ecdsa.SigningKey.from_pem(self.__privkey, hashfunc=hashlib.sha256)
+
+        sign = private_key.sign(data, hashfunc=hashlib.sha256)
+        sign_base64 = base64.b64encode(sign)
+
+        return sign_base64
+
+    @staticmethod
+    def _sign_header():
+        def outer(func):
+            def inner(self):
+                self.__headers["X-Sign"]: str = self.__create_signature(self)
+            return inner
+
+        return outer
+
+    @staticmethod
     def _request(
             request_method: str,
             path: str
     ):
         def outer(func):
             def inner(*args, **kwargs):
                 self = args[0]
@@ -192,40 +268,80 @@
                     return sync_wrapper()
 
             return inner
 
         return outer
 
 
+class APIPaths(str, Enum):
+    # Mono Acquiring API
+    merchant_details = "merchant/details"
+    merchant_statement = "merchant/statement"
+    merchant_pubkey = "merchant/pubkey"
+
+    invoice_create = "merchant/invoice/create"
+    invoice_split = "merchant/invoice/split-payments"
+    invoice_cancel = "merchant/invoice/cancel"
+    invoice_status = "merchant/invoice/status"
+    invoice_invalidation = "merchant/invoice/remove"
+    invoice_info = "merchant/invoice/payment-info"
+    invoice_finalize = "merchant/invoice/finalize"
+
+    qr_list = "merchant/qr/list"
+    qr_details = "merchant/qr/details"
+    qr_reset_amount = "merchant/qr/reset-amount"
+
+    wallet_cards = "merchant/wallet"
+    wallet_payment = "merchant/wallet/payment"
+    wallet_delete_card = "merchant/wallet/card"
+
+    # Monobank Open API
+    currencies_list = "bank/currency"
+
+    personal_info = "personal/client-info"
+    personal_webhook = "personal/webhook"
+    personal_statement = "personal/statement/{account}/{from}/{to}"
+
+    # Monobank Corporate Open API
+    auth_registration = "personal/auth/registration"
+    auth_status = "personal/auth/registration/status"
+
+    corporate_webhook = "personal/corp/webhook"
+    corporate_info = "personal/corp/settings"
+
+    init_access = "personal/auth/request"
+    check_access = "personal/auth/request"
+
+
 # Monobank Open API
 class Public(APIMethod):
 
     @APIMethod._request("get", path=APIPaths.currencies_list)
-    def currency(self, **kwargs) -> Union[CurrencyRatesResponse, MonobankAPIException]:
+    def currency(self, **kwargs) -> Union[CurrencyList, MonobankAPIException]:
 
-        return CurrencyRatesResponse(
+        return CurrencyList(
             list=[
                 CurrencyListItem(
                     **item
                 ) for item in kwargs['response_data']
             ]
         )
 
 
 class Personal(APIMethod):
 
     @APIMethod._request("get", path=APIPaths.personal_info)
-    def info(self, **kwargs) -> Union[ClientInfoResponse, MonobankAPIException]:
+    def info(self, **kwargs) -> Union[ClientInfo, MonobankAPIException]:
         """
         Source: https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1client-info/get
 
         :return:
         """
 
-        return ClientInfoResponse(
+        return ClientInfo(
             client_id=kwargs['response_data']['client_id'],
             name=kwargs['response_data']['name'],
             web_hook_url=kwargs['response_data']['web_hook_url'],
             permissions=kwargs['response_data']['permissions'],
             accounts=[
                 Account(
                     **account
@@ -235,74 +351,61 @@
                 Jar(
                     **jar
                 ) for jar in kwargs['response_data']['jars']
             ]
         )
 
     @APIMethod._request("post", path=APIPaths.personal_webhook)
-    def set_webhook(self, web_hook_url: str) -> Union[EmptyResponse, MonobankAPIException]:
+    def set_web_hook(self, web_hook_url: str) -> Union[EmptyResponse, MonobankAPIException]:
         """
         Source: https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1webhook/post
 
         :param web_hook_url:
         :return:
         """
         return EmptyResponse()
 
     @APIMethod._request("get", path=APIPaths.personal_statement)
-    def statement(self, **kwargs) -> Union[StatementResponse, MonobankAPIException]:
+    def statement(self, **kwargs) -> Union[Statement, MonobankAPIException]:
 
-        return StatementResponse(
+        return Statement(
             list=[
                 Transaction(
                     **transaction
                 ) for transaction in kwargs['response_data']
             ]
         )
 
 
 class MonobankOpenAPIModel:
 
     __base_url = "https://api.monobank.ua"
-    __api_token = None
-    __headers = {}
-
-    def __init__(self, api_token: str, _async: bool):
-        self.__is_async = _async
-
-        self.__api_token__ = api_token
-        self.__headers["X-Token"] = self.__api_token__
-
-        self.public: Public = Public(
-            api_token=self.__api_token,
-            base_url=self.__base_url,
-            _async=self.__is_async
-        )
-
-        self.personal: Personal = Personal(
-            api_token=self.__api_token,
-            base_url=self.__base_url,
-            _async=self.__is_async
-        )
+    __is_async: bool = False
+    __api_token: str = None
 
+    def __init__(self, _async: bool, api_token: Optional[str] = None):
 
-class Corporate(APIMethod):
+        self.__is_async = _async
+        self.__api_token = api_token
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        kwargs = {
+            'base_url': self.__base_url,
+            'api_token': self.__api_token,
+            '_async': self.__is_async
+        }
 
-        self.auth: Authorization = Authorization(*args, **kwargs)
+        self.public: Public = Public(**kwargs)
 
-        self.client: Client = Client(*args, **kwargs)
+        self.personal: Personal = Personal(**kwargs)
 
-    def set_webhook(self):
-        pass
+    def set_api_token(self, api_token: str):
+        self.__api_token: str = api_token
 
-    def info(self):
-        pass
+    def get_api_token(self) -> str:
+        return self.__api_token
 
 
 class Client(APIMethod):
 
     @APIMethod._request("post", path=APIPaths.init_access)
     def init_access(self):
         pass
@@ -322,106 +425,132 @@
     def status(self):
         pass
 
 
 class MonobankCorporateOpenAPIModel:
 
     __base_url: str = "https://api.monobank.ua"
-    __api_token: str = None
     __headers: dict = {}
 
-    def __init__(self, api_token: str, _async: bool):
-        self.__is_async: bool = _async
+    __key_id: str = None
 
-        self.__api_token: str = api_token
-        self.__headers["X-Token"] = self.__api_token__
+    __priv_key: str = None
+    __pub_key: str = None
+
+    def __init__(self, _async: bool):
+        self.__is_async: bool = _async
 
         self.public: Public = Public(
-            api_token=self.__api_token,
             base_url=self.__base_url,
             _async=self.__is_async
         )
 
-        self.corporate: Corporate = Corporate(
-            api_token=self.__api_token,
+        self.auth: Authorization = Authorization(
+            base_url=self.__base_url,
+            _async=self.__is_async
+        )
+
+        self.client: Client = Client(
             base_url=self.__base_url,
             _async=self.__is_async
         )
 
+    def set_web_hook(self):
+        pass
+
+    def info(self):
+        pass
+
+    def set_key_id(self, key_id: str):
+        self.__key_id: str = key_id
+
+    def set_priv_key(self, priv_key_path: str):
+        with codecs.open(priv_key_path, 'r', 'utf-8') as f:
+            priv_key = f.read()
+            f.close()
+
+        self.__priv_key = priv_key
+
+    def set_pub_key(self, pub_key_path: str):
+        with codecs.open(pub_key_path, 'r', 'utf-8') as f:
+            pub_key = f.read()
+            f.close()
+
+        self.__pub_key = pub_key
 
 
 # MonoPay
 class Merchant(APIMethod):
 
     @APIMethod._request("get", path=APIPaths.merchant_details)
-    def details(self, **kwargs) -> Union[MerchantDetailsResponse, MonoPayAPIException]:
+    def details(self, **kwargs) -> Union[MerchantDetails, MonoPayAPIException]:
         """
         Mono Acquiring API: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1details/get
 
         :return: MerchantDetailsResponse
         """
 
-        return MerchantDetailsResponse(**kwargs["response_data"])
+        return MerchantDetails(**kwargs["response_data"])
 
     @APIMethod._request("get", path=APIPaths.merchant_statement)
     def statement(
             self,
             from_timestamp: int,
             to_timestamp: Optional[int] = None,
             **kwargs
-    ) -> Union[MerchantStatementResponse, MonoPayAPIException]:
+    ) -> Union[MerchantStatement, MonoPayAPIException]:
         """
         Mono Acquiring API: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1statement/get
 
         :param from_timestamp:
         :param to_timestamp:
         :param kwargs:
         :return:
         """
 
-        return MerchantStatementResponse(
+        return MerchantStatement(
             list=[
                 MerchantStatementItem(
                     **statement_item,
                     cancel_list=[
                         CancelListItem(
                             **cancel_item
                         ) for cancel_item in statement_item['cancel_list']
                     ] if "cancel_list" in statement_item else None
                 ) for statement_item in kwargs['response_data']['list']
             ]
         )
 
     @APIMethod._request("get", path=APIPaths.merchant_pubkey)
-    def pubkey(self, **kwargs) -> Union[MerchantPubKeyResponse, MonoPayAPIException]:
+    def pubkey(self, **kwargs) -> Union[MerchantPubKey, MonoPayAPIException]:
         """
         Mono Acquiring API Docs: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1pubkey/get
 
         :return: MerchantPubKeyResponse
         """
 
-        return MerchantPubKeyResponse(**kwargs["response_data"])
+        return MerchantPubKey(**kwargs["response_data"])
 
 
 class Invoice(APIMethod):
 
     @APIMethod._request("post", path=APIPaths.invoice_create)
     def create(
             self,
             amount: int,
             ccy: Optional[int] = None,
-            merchant_paym_info: Optional = None,
+            merchant_paym_info: Optional[MerchantPaymInfo] = None,
             redirect_url: Optional[str] = None,
             web_hook_url: Optional[str] = None,
             validity: Optional[int] = None,
             payment_type: Optional[str] = None,
             qr_id: Optional = None,
-            save_card_data: Optional = None,
+            save_card_data: Optional[SaveCardData] = None,
             **kwargs
-    ) -> Union[InvoiceCreatedResponse, MonoPayAPIException]:
+    ) -> Union[InvoiceCreated, MonoPayAPIException]:
         """
         Mono Acquiring API: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1invoice~1create/post
 
         :param amount:
         :param ccy:
         :param merchant_paym_info:
         :param redirect_url:
@@ -429,58 +558,42 @@
         :param validity:
         :param payment_type:
         :param qr_id:
         :param save_card_data:
         :return:
         """
 
-        return InvoiceCreatedResponse(**kwargs['response_data'])
-
-    @APIMethod._request("post", path=APIPaths.invoice_split)
-    def split(
-            self,
-            invoice_id: str,
-            **kwargs
-    ) -> Union[SplitInvoiceResponse, MonoPayAPIException]:
-        """
-        Mono Acquiring API:
-
-        :param invoice_id:
-        :param kwargs:
-        :return:
-        """
-
-        return SplitInvoiceResponse(**kwargs['response_data'])
+        return InvoiceCreated(**kwargs['response_data'])
 
     @APIMethod._request("post", path=APIPaths.invoice_cancel)
     def cancel(
             self,
             invoice_id: str,
             ext_ref: str = None,
             amount: int = None,
             items=None,
             **kwargs
-    ) -> Union[InvoiceCanceledResponse, MonoPayAPIException]:
+    ) -> Union[InvoiceCanceled, MonoPayAPIException]:
         """
         Mono Acquiring API: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1invoice~1cancel/post
 
         :param invoice_id:
         :param ext_ref:
         :param amount:
         :param items:
         :param kwargs:
         :return:
         """
-        return InvoiceCanceledResponse(**kwargs['response_data'])
+        return InvoiceCanceled(**kwargs['response_data'])
 
     def status(
             self,
             invoice_id: str,
             **kwargs
-    ) -> Union[InvoiceStatusResponse, MonoPayAPIException]:
+    ) -> Union[InvoiceStatus, MonoPayAPIException]:
         """
         Mono Acquiring API: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1invoice~1status?invoiceId=%7BinvoiceId%7D/get
 
         :param invoice_id:
         :param kwargs:
         :return:
         """
@@ -504,15 +617,15 @@
         return EmptyResponse()
 
     @APIMethod._request("get", path=APIPaths.invoice_info)
     async def info(
             self,
             invoice_id: str,
             **kwargs
-    ) -> Union[InvoiceInfoResponse, MonoPayAPIException]:
+    ) -> Union[InvoiceInfo, MonoPayAPIException]:
         """
         Source: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1invoice~1payment-info?invoiceId=%7BinvoiceId%7D/get
 
         :param invoice_id:
         :param kwargs:
         :return:
         """
@@ -521,51 +634,51 @@
 
     @APIMethod._request("get", path=APIPaths.invoice_finalize)
     def finalize(
             self,
             invoice_id: str,
             amount: int,
             **kwargs
-    ) -> Union[FinalizeInvoiceResponse, MonoPayAPIException]:
+    ) -> Union[FinalizeInvoice, MonoPayAPIException]:
         """
         Source: https://api.monobank.ua/docs/acquiring.html#/paths/~1api~1merchant~1invoice~1finalize/post
 
         :param invoice_id:
         :param amount:
         :param kwargs:
         :return:
         """
-        return FinalizeInvoiceResponse(
+        return FinalizeInvoice(
             **kwargs['response_data']
         )
 
 
 class Qr(APIMethod):
 
     @APIMethod._request("get", path=APIPaths.qr_list)
-    def list(self, **kwargs) -> Union[QrListResponse, MonoPayAPIException]:
-        return QrListResponse(
+    def list(self, **kwargs) -> Union[QrList, MonoPayAPIException]:
+        return QrList(
             list=[
                 QrListItem(
                     **qr
                 ) for qr in kwargs['response']['list']
             ]
         )
 
     @APIMethod._request("post", path=APIPaths.qr_details)
     def details(
             self,
             qr_id: str,
             **kwargs
-    ) -> Union[QrDetailsResponse, MonoPayAPIException]:
+    ) -> Union[QrDetails, MonoPayAPIException]:
         """
         :param qr_id:
         :return:
         """
-        return QrDetailsResponse(**kwargs['response_data'])
+        return QrDetails(**kwargs['response_data'])
 
     @APIMethod._request("post", path=APIPaths.qr_reset_amount)
     def reset_amount(
             self,
             qr_id: str,
             **kwargs
     ) -> Union[EmptyResponse, MonoPayAPIException]:
```

### Comparing `mbnk-0.1.3a0/mbnk/asyncio/mbnk.py` & `mbnk-0.2.0a1/mbnk/asyncio/mbnk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __all__ = [
     'AsyncMonoAcquiringAPI',
     'AsyncMonobankOpenAPI',
     'AsyncMonobankCorporateOpenAPI'
 ]
 
+from typing import Optional
+
 from mbnk.api import (
     MonoAcquiringAPIModel,
     MonobankOpenAPIModel,
     MonobankCorporateOpenAPIModel
 )
 
 
@@ -23,19 +25,19 @@
 
 class AsyncMonobankOpenAPI(MonobankOpenAPIModel):
     """
     Asynchronous version MonobankOpenAPI
     Source: https://api.monobank.ua/docs/
     """
 
-    def __init__(self, api_token: str):
+    def __init__(self, api_token: Optional[str] = None):
         super().__init__(api_token=api_token, _async=True)
 
 
 class AsyncMonobankCorporateOpenAPI(MonobankCorporateOpenAPIModel):
     """
     Asynchronous version MonobankCorporateOpenAPI
     Source: https://api.monobank.ua/docs/corporate.html
     """
 
-    def __init__(self, api_token: str):
-        super().__init__(api_token=api_token, _async=True)
+    def __init__(self):
+        super().__init__(_async=True)
```

### Comparing `mbnk-0.1.3a0/mbnk/exceptions.py` & `mbnk-0.2.0a1/mbnk/exceptions.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.3a0/mbnk/mbnk.py` & `mbnk-0.2.0a1/mbnk/mbnk.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 __all__ = [
     'MonoAcquiringAPI',
     'MonobankOpenAPI',
     'MonobankCorporateOpenAPI'
 ]
 
+from typing import Optional
+
 from mbnk.api import (
     MonoAcquiringAPIModel,
     MonobankOpenAPIModel,
     MonobankCorporateOpenAPIModel
 )
 
 
@@ -23,19 +25,19 @@
 
 class MonobankOpenAPI(MonobankOpenAPIModel):
     """
     Synchronous version MonobankOpenAPI
     Source: https://api.monobank.ua/docs/
     """
 
-    def __init__(self, api_token: str):
+    def __init__(self, api_token: Optional[str] = None):
         super().__init__(api_token=api_token, _async=False)
 
 
 class MonobankCorporateOpenAPI(MonobankCorporateOpenAPIModel):
     """
     Synchronous version MonobankCorporateOpenAPI
     Source: https://api.monobank.ua/docs/corporate.html
     """
 
-    def __init__(self, api_token: str):
-        super().__init__(api_token=api_token, _async=False)
+    def __init__(self):
+        super().__init__(_async=False)
```

### Comparing `mbnk-0.1.3a0/PKG-INFO` & `mbnk-0.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.1.3a0
+Version: 0.2.0a1
 Summary: Sync/Async version monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

