# Comparing `tmp/SberQR-1.0.1b1.tar.gz` & `tmp/SberQR-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SberQR-1.0.1b1.tar", last modified: Mon Sep 19 12:59:25 2022, max compression
+gzip compressed data, was "SberQR-1.0.3.tar", last modified: Thu Jul  6 10:43:05 2023, max compression
```

## Comparing `SberQR-1.0.1b1.tar` & `SberQR-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-09-19 12:59:25.434888 SberQR-1.0.1b1/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 SberQR-1.0.1b1/LICENSE
--rw-rw-rw-   0        0        0     5070 2022-09-19 12:59:25.434888 SberQR-1.0.1b1/PKG-INFO
--rw-rw-rw-   0        0        0     4271 2022-09-19 12:49:27.000000 SberQR-1.0.1b1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-19 12:59:25.425885 SberQR-1.0.1b1/SberQR/
--rw-rw-rw-   0        0        0     8105 2022-09-19 12:44:26.000000 SberQR-1.0.1b1/SberQR/AsyncSberQR.py
--rw-rw-rw-   0        0        0      441 2022-09-19 12:59:22.000000 SberQR-1.0.1b1/SberQR/__init__.py
--rw-rw-rw-   0        0        0     2727 2022-09-04 21:39:21.000000 SberQR-1.0.1b1/SberQR/api.py
--rw-rw-rw-   0        0        0       88 2022-09-05 13:25:48.000000 SberQR-1.0.1b1/SberQR/exceptions.py
--rw-rw-rw-   0        0        0      387 2022-09-19 11:50:03.000000 SberQR-1.0.1b1/SberQR/payload.py
--rw-rw-rw-   0        0        0      353 2022-09-16 13:26:26.000000 SberQR-1.0.1b1/SberQR/scope.py
--rw-rw-rw-   0        0        0      185 2022-09-05 12:36:20.000000 SberQR-1.0.1b1/SberQR/types.py
-drwxrwxrwx   0        0        0        0 2022-09-19 12:59:25.433888 SberQR-1.0.1b1/SberQR.egg-info/
--rw-rw-rw-   0        0        0     5070 2022-09-19 12:59:25.000000 SberQR-1.0.1b1/SberQR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2022-09-19 12:59:25.000000 SberQR-1.0.1b1/SberQR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-19 12:59:25.000000 SberQR-1.0.1b1/SberQR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2022-09-19 12:59:25.000000 SberQR-1.0.1b1/SberQR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-19 12:59:25.000000 SberQR-1.0.1b1/SberQR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      247 2022-09-19 12:59:25.436888 SberQR-1.0.1b1/setup.cfg
--rw-rw-rw-   0        0        0     1295 2022-09-19 12:59:22.000000 SberQR-1.0.1b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:43:05.171416 SberQR-1.0.3/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 SberQR-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7110 2023-07-06 10:43:05.171416 SberQR-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6313 2023-07-06 10:23:15.000000 SberQR-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 10:43:05.146410 SberQR-1.0.3/SberQR/
+-rw-rw-rw-   0        0        0     8243 2023-07-06 10:14:34.000000 SberQR-1.0.3/SberQR/AsyncSberQR.py
+-rw-rw-rw-   0        0        0      439 2023-07-06 10:23:15.000000 SberQR-1.0.3/SberQR/__init__.py
+-rw-rw-rw-   0        0        0     2725 2023-07-06 08:00:29.000000 SberQR-1.0.3/SberQR/api.py
+-rw-rw-rw-   0        0        0       88 2022-09-05 13:25:48.000000 SberQR-1.0.3/SberQR/exceptions.py
+-rw-rw-rw-   0        0        0      387 2022-09-19 11:50:03.000000 SberQR-1.0.3/SberQR/payload.py
+-rw-rw-rw-   0        0        0      353 2022-09-16 13:26:26.000000 SberQR-1.0.3/SberQR/scope.py
+-rw-rw-rw-   0        0        0      185 2022-09-05 12:36:20.000000 SberQR-1.0.3/SberQR/types.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:43:05.170415 SberQR-1.0.3/SberQR.egg-info/
+-rw-rw-rw-   0        0        0     7110 2023-07-06 10:43:05.000000 SberQR-1.0.3/SberQR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-07-06 10:43:05.000000 SberQR-1.0.3/SberQR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:43:05.000000 SberQR-1.0.3/SberQR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-06 10:43:05.000000 SberQR-1.0.3/SberQR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 10:43:05.000000 SberQR-1.0.3/SberQR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      247 2023-07-06 10:43:05.177418 SberQR-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-07-06 10:42:11.000000 SberQR-1.0.3/setup.py
```

### Comparing `SberQR-1.0.1b1/LICENSE` & `SberQR-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SberQR-1.0.1b1/PKG-INFO` & `SberQR-1.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SberQR
-Version: 1.0.1b1
+Version: 1.0.3
 Summary: Асинхронная библиотека для работы с SberPay QR/Плати QR.
 Home-page: https://github.com/bl4ckm45k/SberQR
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,34 +15,60 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Плати QR Сбербанк и СБП
+![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
+[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
+[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
+
+
+
+## Асинхронная библиотека для работы с SberPay QR/Плати QR.
 
 Асинхронная библиотека для работы с SberPay QR/Плати QR.
 
 Позволяет создавать динамический QR и проверять статус платежа.
 
+> Обязательно 
+
 > Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
 > платеж через СБП, иначе через ПлатиQR.
 ## Пример (async)
 
 ```python
+import os
 import asyncio
 from SberQR import AsyncSberQR
 
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
 # Если требуется передайте аргумент redis=
 # redis = aioredis.from_url("redis://localhost", decode_responses=True)
 # redis = "redis://localhost"
 # Redis используется только для временного хранения токена
-sber_qr = AsyncSberQR(member_id, id_qr, tid, client_id, client_secret,
-                      path_crt_from_pkcs12, path_key_from_pkcs12, pkcs12_password)
+sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
 positions = [{"position_name": 'Товар ра 10 рублей',
               "position_count": 1,
               "position_sum": 1000,
               "position_description": 'Какой-то товар за 10 рублей'}
              ]
 async def creation_qr():
     data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
```

### Comparing `SberQR-1.0.1b1/README.md` & `SberQR-1.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,53 @@
-# Плати QR Сбербанк и СБП
+![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
+[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
+[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
+
+
+
+## Асинхронная библиотека для работы с SberPay QR/Плати QR.
 
 Асинхронная библиотека для работы с SberPay QR/Плати QR.
 
 Позволяет создавать динамический QR и проверять статус платежа.
 
+> Обязательно 
+
 > Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
 > платеж через СБП, иначе через ПлатиQR.
 ## Пример (async)
 
 ```python
+import os
 import asyncio
 from SberQR import AsyncSberQR
 
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
 # Если требуется передайте аргумент redis=
 # redis = aioredis.from_url("redis://localhost", decode_responses=True)
 # redis = "redis://localhost"
 # Redis используется только для временного хранения токена
-sber_qr = AsyncSberQR(member_id, id_qr, tid, client_id, client_secret,
-                      path_crt_from_pkcs12, path_key_from_pkcs12, pkcs12_password)
+sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
 positions = [{"position_name": 'Товар ра 10 рублей',
               "position_count": 1,
               "position_sum": 1000,
               "position_description": 'Какой-то товар за 10 рублей'}
              ]
 async def creation_qr():
     data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
```

### Comparing `SberQR-1.0.1b1/SberQR/AsyncSberQR.py` & `SberQR-1.0.3/SberQR/AsyncSberQR.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from logging import getLogger
 from random import choices
 from string import hexdigits
 from typing import Optional, Type, Union, List, Dict
 
 import aiohttp
 import aioredis
+import certifi
 import ujson as json
 from aioredis.client import Redis
 
 from .api import make_request, Methods
 from .payload import generate_payload
 from .scope import Scope
 from .types import RegistryType, CancelType
@@ -22,14 +23,15 @@
 
 class AsyncSberQR:
 
     def __init__(self, member_id: str, id_qr: str, tid: str,
                  client_id: str, client_secret: str,
                  crt_file_path: str, key_file_path: str,
                  pkcs12_password: str,
+                 russian_crt: str,
                  redis: Union[str, Redis] = None,
                  loop: Optional[Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop]] = None,
                  connections_limit: int = None,
                  timeout: Optional[Union[int, float, aiohttp.ClientTimeout]] = None):
         """
 
         :param member_id:
@@ -37,15 +39,15 @@
         :param tid:
         :param client_id:
         :param client_secret: l
         i]
         :param crt_file_path:
         :param key_file_path:
         :param pkcs12_password:
-        :param redis_url:
+        :param redis:
         :param loop:
         :param connections_limit:
         :param timeout:
         """
 
         self._main_loop = loop
 
@@ -53,18 +55,21 @@
         self._sbp_member_id = "100000000111"
         self._id_qr = id_qr
         self._tid = tid
         self._client_id = client_id
         self._client_secret = client_secret
 
         self._currency = "643"
-        ssl_context = ssl.create_default_context()
+        ssl_context = ssl.create_default_context(cafile=certifi.where())
+
         ssl_context.load_cert_chain(certfile=crt_file_path,
                                     keyfile=key_file_path,
                                     password=pkcs12_password)
+        ssl_context.load_verify_locations(cafile=russian_crt)
+
         self._session: Optional[aiohttp.ClientSession] = None
         self._connector_class: Type[aiohttp.TCPConnector] = aiohttp.TCPConnector
         self._connector_init = dict(limit=connections_limit, ssl=ssl_context)
         if isinstance(redis, Redis):
             self._redis = redis
         else:
             self._redis = aioredis.from_url(redis, decode_responses=True) if redis is not None else None
@@ -118,15 +123,15 @@
             auth = base64.b64encode(f'{self._client_id}:{self._client_secret}'.encode('utf-8')).decode('utf-8')
             headers = {'Authorization': f'Basic {auth}',
                        'Content-Type': 'application/x-www-form-urlencoded',
                        'rquid': ''.join(choices(hexdigits, k=32))}
             data = {'grant_type': 'client_credentials', 'scope': scope.value}
             token_data = await self.request(Methods.oauth, headers, data)
             await self._redis.set(f'{self._client_id}token_{scope.value}', token_data['access_token'],
-                                  int(token_data['expires_in']) - 4)
+                                  int(token_data['expires_in']) - 10)
             return token_data['access_token']
 
     async def creation(self, description: str, order_sum: int, order_number: str, positions: Union[List, Dict]):
         """
         Создание заказа
         """
         dt = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
```

### Comparing `SberQR-1.0.1b1/SberQR/api.py` & `SberQR-1.0.3/SberQR/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     elif status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
         raise SberQrAPIError(f"{body} [{status_code}]")
     elif status_code >= HTTPStatus.INTERNAL_SERVER_ERROR:
         raise SberQrAPIError(f"{body} [{status_code}]")
 
 
 async def make_request(session, method, headers, data, **kwargs):
-    url = f'https://api.sberbank.ru:8443/prod/{method}'
+    url = f'https://mc.api.sberbank.ru/prod/{method}'
 
     if method != Methods.oauth:
         async with session.post(url, json=data, headers=headers) as response:
             try:
                 body = await response.json()
             except:
                 body = response.text
```

### Comparing `SberQR-1.0.1b1/SberQR.egg-info/PKG-INFO` & `SberQR-1.0.3/SberQR.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SberQR
-Version: 1.0.1b1
+Version: 1.0.3
 Summary: Асинхронная библиотека для работы с SberPay QR/Плати QR.
 Home-page: https://github.com/bl4ckm45k/SberQR
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,34 +15,60 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Плати QR Сбербанк и СБП
+![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
+[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
+[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
+
+
+
+## Асинхронная библиотека для работы с SberPay QR/Плати QR.
 
 Асинхронная библиотека для работы с SberPay QR/Плати QR.
 
 Позволяет создавать динамический QR и проверять статус платежа.
 
+> Обязательно 
+
 > Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
 > платеж через СБП, иначе через ПлатиQR.
 ## Пример (async)
 
 ```python
+import os
 import asyncio
 from SberQR import AsyncSberQR
 
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
 # Если требуется передайте аргумент redis=
 # redis = aioredis.from_url("redis://localhost", decode_responses=True)
 # redis = "redis://localhost"
 # Redis используется только для временного хранения токена
-sber_qr = AsyncSberQR(member_id, id_qr, tid, client_id, client_secret,
-                      path_crt_from_pkcs12, path_key_from_pkcs12, pkcs12_password)
+sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
 positions = [{"position_name": 'Товар ра 10 рублей',
               "position_count": 1,
               "position_sum": 1000,
               "position_description": 'Какой-то товар за 10 рублей'}
              ]
 async def creation_qr():
     data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
```

### Comparing `SberQR-1.0.1b1/setup.py` & `SberQR-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 
 from setuptools import setup
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
-requirements = ["aiohttp>=3.8.1", "certifi>=2022.6.15", "ujson>=5.3.0", "pytz==2022.1", "qrcode[pil]>=7.3.1",
+requirements = ["aiohttp>=3.8.4", "certifi>=2023.5.7", "ujson>=5.8.0", "pytz==2022.1", "qrcode[pil]>=7.3.1",
                 "aioredis>=2.0.1"]
 
 setup(
     name='SberQR',
-    version='1.0.1b1',
+    version='1.0.3',
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Асинхронная библиотека для работы с SberPay QR/Плати QR.',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/SberQR",
     license="MIT",
     packages=['SberQR'],
```

