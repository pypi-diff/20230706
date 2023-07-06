# Comparing `tmp/ProxyEater-1.5.1.tar.gz` & `tmp/ProxyEater-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProxyEater-1.5.1.tar", last modified: Sun Jul 31 14:09:05 2022, max compression
+gzip compressed data, was "ProxyEater-1.5.2.tar", last modified: Thu Jul  6 06:57:23 2023, max compression
```

## Comparing `ProxyEater-1.5.1.tar` & `ProxyEater-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 14:09:05.191974 ProxyEater-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11346 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-07-31 14:09:05.191974 ProxyEater-1.5.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 14:09:05.191974 ProxyEater-1.5.1/ProxyEater/
--rw-r--r--   0 runner    (1001) docker     (121)    22341 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/ProxyEater/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     9226 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/ProxyEater/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/ProxyEater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14079 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/ProxyEater/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8881 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/ProxyEater/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 14:09:05.191974 ProxyEater-1.5.1/ProxyEater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-07-31 14:09:05.000000 ProxyEater-1.5.1/ProxyEater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-07-31 14:09:05.000000 ProxyEater-1.5.1/ProxyEater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-31 14:09:05.000000 ProxyEater-1.5.1/ProxyEater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-31 14:09:05.000000 ProxyEater-1.5.1/ProxyEater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-31 14:09:05.000000 ProxyEater-1.5.1/ProxyEater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-31 14:09:05.000000 ProxyEater-1.5.1/ProxyEater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-31 14:09:05.191974 ProxyEater-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-07-31 14:09:00.000000 ProxyEater-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/ProxyEater/
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/ProxyEater/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/ProxyEater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 06:57:23.000000 ProxyEater-1.5.2/ProxyEater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:57:23.462300 ProxyEater-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 06:57:17.000000 ProxyEater-1.5.2/setup.py
```

### Comparing `ProxyEater-1.5.1/LICENSE` & `ProxyEater-1.5.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [2022] [CodeWriter21]
+   Copyright [2022-2023] [CodeWriter21]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ProxyEater-1.5.1/PKG-INFO` & `ProxyEater-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: ProxyEater
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Python Proxy Scraper for gathering fresh proxies.
 Home-page: https://github.com/MPCodeWriter21/ProxyEater
 Author: CodeWriter21
 Author-email: CodeWriter21@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-ProxyEater\[1.5.1\]
+ProxyEater\[1.5.2\]
 ===================
 
 ![version](https://img.shields.io/pypi/v/ProxyEater)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/ProxyEater)
 [![CodeFactor](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater/badge)](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater)
 
 A Python Proxy Scraper for gathering fresh proxies.
@@ -58,15 +56,15 @@
 positional arguments:
   mode              Modes: Scrape, Check
 
 options:
   -h, --help
                         show this help message and exit
   --source SOURCE, -s SOURCE
-                        The source of the proxies(default:C:\Users\Morteza\AppData\Local\Programs\
+                        The source of the proxies(default:%localappdata%\
                         Python\Python310\lib\site-packages\ProxyEater\sources.json).
   --output OUTPUT, -o OUTPUT
                         The output file.
   --file-format { text, json, csv }, -ff { text, json, csv }
                         The format of the output file(default:text).
   --format FORMAT, -f FORMAT
                         The format for saving the proxies in text
@@ -132,9 +130,7 @@
 In order to support this project you can donate some crypto of your choice 8D
 
 [Donate Addresses](https://github.com/MPCodeWriter21/ProxyEater/blob/master/DONATE.md)
 
 Or if you can't, give [this project](https://github.com/MPCodeWriter21/ProxyEater) a star on GitHub :)
 
 
-
-
```

### Comparing `ProxyEater-1.5.1/ProxyEater/Proxy.py` & `ProxyEater-1.5.2/ProxyEater/Proxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,96 @@
 # ProxyEater.Proxy.py
 # CodeWriter21
 
+from __future__ import annotations
+
 import os
 import csv  # This module is used to write proxies to a csv file.
 import json  # This module is used to parse the ProxyList to json.
 import time  # This module is used to sleep the program.
-import requests  # This module is used to send requests to the server.
 import threading  # This module is used to create threads.
-
 from enum import Enum
-from typing import Iterable as _Iterable, Union as _Union, Callable as _Callable
+from typing import (Dict as _Dict, Union as _Union, Callable as _Callable,
+                    Iterable as _Iterable, Optional as _Optional)
+
+import requests  # This module is used for sending requests to the servers.
+from requests.exceptions import InvalidProxyURL
 
 __all__ = ['Proxy', 'ProxyType', 'ProxyList', 'ProxyStatus']
 
 
 class ProxyStatus(Enum):
-    """
-    This class is used to define the status of a proxy.
-    """
+    """This class is used to define the status of a proxy."""
     UNKNOWN = 0
     ALIVE = 1
     DEAD = 2
 
+    @staticmethod
+    def from_name(name: str) -> ProxyStatus:
+        """This method is used to for getting a ProxyStatus object from its
+        name.
+
+        :param name: The name of the ProxyStatus.
+        :return: The ProxyStatus.
+        """
+        name = name.lower()
+        if name == 'unknown':
+            return ProxyStatus.UNKNOWN
+        if name == 'alive':
+            return ProxyStatus.ALIVE
+        if name == 'dead':
+            return ProxyStatus.DEAD
+        raise ValueError(f'The proxy type({name}) is not valid.')
+
 
 class ProxyType(Enum):
-    """
-    This class is used to define the type of proxy.
-    """
+    """This class is used to define the type of proxy."""
     HTTP = 0
     HTTPS = 1
     SOCKS4 = 2
     SOCKS5 = 3
 
     @staticmethod
-    def from_name(name: str) -> 'ProxyType':
-        """
-        This method is used to get the ProxyType from the name.
+    def from_name(name: str) -> ProxyType:
+        """This method is used to get the ProxyType from the name.
+
         :param name: The name of the ProxyType.
         :return: The ProxyType.
         """
         name = name.lower()
         if name == 'http':
             return ProxyType.HTTP
-        elif name == 'https':
+        if name == 'https':
             return ProxyType.HTTPS
-        elif name == 'socks4':
+        if name == 'socks4':
             return ProxyType.SOCKS4
-        elif name == 'socks5':
+        if name == 'socks5':
             return ProxyType.SOCKS5
-        else:
-            raise ValueError(f'The proxy type({name}) is not valid.')
+        raise ValueError(f'The proxy type({name}) is not valid.')
 
 
 class Proxy:
     geolocation_info: dict = {}
     status: ProxyStatus = ProxyStatus.UNKNOWN
 
     def __init__(self, ip: str, port: int, type_: ProxyType) -> None:
         self.ip: str = ip
         self.port: int = port
         if isinstance(type_, str):
             type_ = ProxyType.from_name(type_)
         self.type: ProxyType = type_
 
-    def check_status(self, timeout: int = 10, url: str = 'http://icanhazip.com/', on_success_callback: _Callable = None,
-                     on_failure_callback: _Callable = None) -> bool:
-        """
-        This method is used to check if the proxy is alive.
+    def check_status(
+        self,
+        timeout: int = 10,
+        url: str = 'http://icanhazip.com/',
+        on_success_callback: _Optional[_Callable] = None,
+        on_failure_callback: _Optional[_Callable] = None
+    ) -> bool:
+        """This method is used to check if the proxy is alive.
 
         :param timeout: The timeout of the request.
         :param url: The url to try to connect to through the proxy.
         :param on_success_callback: The callback to be called if the request succeeds.
         :param on_failure_callback: The callback to be called if the request fails.
         :return: True if the proxy is alive, False otherwise.
         """
@@ -81,97 +101,105 @@
             on_success_callback = lambda proxy, status: None
         if on_failure_callback is not None:
             if not callable(on_failure_callback):
                 raise TypeError('on_failure_callback must be a callable.')
         else:
             on_failure_callback = lambda proxy, error: None
         try:
-            if requests.get(url, proxies={'http': str(self), 'https': str(self)}, timeout=timeout).status_code == 200:
+            if requests.get(url, proxies={'http': str(self), 'https': str(self)},
+                            timeout=timeout).status_code == 200:
                 self.status = ProxyStatus.ALIVE
                 on_success_callback(self, ProxyStatus.ALIVE)
                 return True
             else:
                 self.status = ProxyStatus.DEAD
                 on_success_callback(self, ProxyStatus.DEAD)
                 return False
-        except Exception as e:
+        except Exception as ex:
             self.status = ProxyStatus.DEAD
-            on_failure_callback(self, e)
+            on_failure_callback(self, ex)
             return False
 
     @property
     def is_alive(self) -> bool:
         return self.status == ProxyStatus.ALIVE
 
-    def check_geolocation(self, fields: str = 'status,message,continent,continentCode,country,countryCode,'
-                                              'region,regionName,city,zip,lat,lon,timezone,isp,org,as,asname,'
-                                              'query', on_error_callback: _Callable = None) -> _Union[None, dict]:
-        """
-        This method is used to check the geolocation of the proxy.
+    def check_geolocation(
+        self,
+        fields: str = 'status,message,continent,continentCode,country,countryCode,'
+        'region,regionName,city,zip,lat,lon,timezone,isp,org,as,asname,'
+        'query',
+        on_error_callback: _Optional[_Callable] = None
+    ) -> _Dict:
+        """This method is used to check the geolocation of the proxy.
 
         :param fields: The fields to be returned.
         :param on_error_callback: The callback to be called if the request fails.
         """
         if on_error_callback is not None:
             if not callable(on_error_callback):
                 raise TypeError('on_error_callback must be a callable.')
         else:
             on_error_callback = lambda proxy, error: None
         try:
-            response = requests.get(url=f"http://ip-api.com/json/{self.ip}?fields={fields}")
+            response = requests.get(
+                url=f"http://ip-api.com/json/{self.ip}?fields={fields}"
+            )
             self.geolocation_info = response.json()
+            return self.geolocation_info
         except Exception as e:
             on_error_callback(self, e)
-            return None
+            return {}
 
-    def get_geolocation_info(self):
+    def get_geolocation_info(self) -> _Dict:
         if self.geolocation_info is None:
             return self.check_geolocation()
         return self.geolocation_info
 
     @staticmethod
-    def from_text(text: str, default_type: ProxyType = None) -> 'Proxy':
-        """
-        This method is used to create a Proxy from a text.
+    def from_text(text: str, default_type: _Optional[ProxyType] = None) -> 'Proxy':
+        """This method is used to create a Proxy from a text.
+
         :param text: The text to create the Proxy from.
         :param default_type: The default type of the Proxy.
         :return: The Proxy.
         """
-        if text.count(':') == 1:
+        if text.count(':') == 1:  # Proxies with no scheme; will use default_type
             ip, port = text.split(':')
             ip = ip.strip(' /')
             port = int(port)
             if default_type is None:
-                raise ValueError(f'{text}: Proxy without scheme: Default type is not specified.')
+                raise ValueError(
+                    f'`{text}`: Proxy without scheme: Default type is not specified.'
+                )
             else:
                 return Proxy(ip, port, default_type)
-        elif text.count(':') == 2:
+        elif text.count(':') == 2:  # Proxies having scheme
             scheme, ip, port = text.split(':')
             ip = ip.strip(' /')
             port = int(port)
             if scheme.lower() == 'http':
                 return Proxy(ip, port, ProxyType.HTTP)
-            elif scheme.lower() == 'https':
+            if scheme.lower() == 'https':
                 return Proxy(ip, port, ProxyType.HTTPS)
-            elif scheme.lower() == 'socks4':
+            if scheme.lower() == 'socks4':
                 return Proxy(ip, port, ProxyType.SOCKS4)
-            elif scheme.lower() == 'socks5':
+            if scheme.lower() == 'socks5':
                 return Proxy(ip, port, ProxyType.SOCKS5)
-            else:
-                raise ValueError(f'{text}: Proxy with unknown scheme: {scheme}')
+            raise ValueError(f'`{text}`: Proxy with unknown scheme: {scheme}')
         else:
-            raise ValueError(f'{text}: Proxy with invalid format.')
+            raise ValueError(f'`{text}`: Proxy with invalid format.')
 
     def __str__(self) -> str:
         return f'{self.type.name.lower()}://{self.ip}:{self.port}'
 
     def __repr__(self) -> str:
         return f"Proxy(ip='{self.ip}', port={self.port})"
 
-    def __eq__(self, other: 'Proxy') -> bool:
+    def __eq__(self, other: Proxy) -> bool:
         if not isinstance(other, Proxy):
             return False
         return self.ip == other.ip and self.port == other.port
 
     def __hash__(self) -> int:
         return hash(self.ip + str(self.port))
 
@@ -182,37 +210,39 @@
             'type': self.type.name,
             'status': self.status.name,
             'scheme': self.type.name.lower(),
             'geolocation_info': self.geolocation_info
         }
 
     def __iter__(self):
-        return iter((
-            ('ip', self.ip),
-            ('port', self.port),
-            ('type', self.type.name),
-            ('status', self.status.name),
-            ('scheme', self.type.name.lower()),
-            ('geolocation_info', self.geolocation_info)
-        ))
+        return iter(
+            (
+                ('ip', self.ip), ('port', self.port), ('type', self.type.name),
+                ('status', self.status.name), ('scheme', self.type.name.lower()),
+                ('geolocation_info', self.geolocation_info)
+            )
+        )
 
 
 class ProxyList(set):
-    def __init__(self, proxies: _Iterable[Proxy] = None):
+
+    def __init__(self, proxies: _Optional[_Iterable[Proxy]] = None):
         super().__init__()
         if proxies is not None:
             self.update(proxies)
 
     def update(self, proxies: _Iterable[Proxy]):
         temp = set()
         for proxy in set(proxies):
             if isinstance(proxy, Proxy):
                 temp.add(proxy)
             else:
-                raise TypeError("ProxyList.update() argument must be a sequence of Proxy objects.")
+                raise TypeError(
+                    "ProxyList.update() argument must be a sequence of Proxy objects."
+                )
 
         super().update(temp)
 
     def add(self, proxy: Proxy):
         if isinstance(proxy, Proxy):
             super().add(proxy)
         else:
@@ -220,122 +250,152 @@
 
     def union(self, proxies: _Iterable[Proxy]):
         temp = set()
         for proxy in set(proxies):
             if isinstance(proxy, Proxy):
                 temp.add(proxy)
             else:
-                raise TypeError("ProxyList.union() argument must be a sequence of Proxy objects.")
+                raise TypeError(
+                    "ProxyList.union() argument must be a sequence of Proxy objects."
+                )
 
         return super().union(temp)
 
-    def check_all(self, timeout: int = 10, threads_no: int = 21, url: str = 'http://icanhazip.com/',
-                  remove_dead: bool = True, on_progress_callback: _Callable = None) -> None:
-        """
-        This method is used to check the status of all proxies in the list.
+    def check_all(
+        self,
+        timeout: int = 10,
+        threads_no: int = 21,
+        url: str = 'http://icanhazip.com/',
+        remove_dead: bool = True,
+        on_progress_callback: _Optional[_Callable] = None
+    ) -> None:
+        """This method is used to check the status of all proxies in the list.
 
         :param timeout: The timeout of the requests.
         :param threads_no: The number of threads to use.
         :param url: The url to try to connect to through the proxy.
         :param remove_dead: If True, dead proxies will be removed from the list.
         :param on_progress_callback: A callback function to be called on each progress.
         """
         if on_progress_callback is not None:
             if not callable(on_progress_callback):
-                raise TypeError("ProxyList.check_all() argument on_progress_callback must be a callable.")
+                raise TypeError(
+                    "ProxyList.check_all() argument on_progress_callback must be "
+                    "a callable."
+                )
         else:
             on_progress_callback = lambda proxy_list, progress: None
 
         length = len(self)
         finished: int = 0  # The number of proxies that have been checked.
 
         def check_proxy(proxy_: Proxy):
-            """
-            This function is used for checking the status of a proxy.
+            """This function is used for checking the status of a proxy.
 
             :param proxy_: The proxy to check.
             :return:
             """
             nonlocal finished
             proxy_.check_status(timeout, url)
             if (not proxy_.is_alive) and remove_dead:
                 self.remove(proxy_)
             finished += 1
             on_progress_callback(self, finished / length * 99.99)
 
         threads = []
         for proxy in self.copy():
-            thread = threading.Thread(target=check_proxy, args=(proxy,))
+            thread = threading.Thread(target=check_proxy, args=(proxy, ))
             threads.append(thread)
             thread.start()
             while len(threads) >= threads_no:
-                for thread in threads:
+                for thread in threads.copy():
                     if not thread.is_alive():
                         threads.remove(thread)
                         break
                 time.sleep(0.1)
 
         # Wait for all threads to finish
         for thread in threads:
             thread.join()
 
         on_progress_callback(self, 100)
 
-    def to_text(self, separator: str = "\n", format_: str = '{scheme}://{ip}:{port}') -> str:
-        """
-        This method is used to convert the list to a text string.
+    def to_text(
+        self, separator: str = "\n", format_: str = '{scheme}://{ip}:{port}'
+    ) -> str:
+        """This method is used to convert the list to a text string.
 
         :param separator: The separator between proxies.
         :param format_: The format of each proxy.
         :return: The text string.
         """
         return separator.join(format_.format(**dict(proxy)) for proxy in self)
 
-    def batch_collect_geolocations(self, fields: str = 'status,message,continent,continentCode,country,countryCode,'
-                                                       'region,regionName,city,zip,lat,lon,timezone,isp,org,as,asname,'
-                                                       'query', on_progress_callback: _Callable = None,
-                                   on_error_callback: _Callable = None) -> None:
-        """
-        This method is used to collect the geolocation of all proxies in the list.
+    def batch_collect_geolocations(
+        self,
+        fields: str = 'status,message,continent,continentCode,country,countryCode,'
+        'region,regionName,city,zip,lat,lon,timezone,isp,org,as,asname,'
+        'query',
+        on_progress_callback: _Optional[_Callable] = None,
+        on_error_callback: _Optional[_Callable] = None
+    ) -> None:
+        """This method is used to collect the geolocation of all proxies in the
+        list.
 
         :param fields: The fields to be returned.
         :param on_progress_callback: A callback function to be called on each progress.
         :param on_error_callback: A callback function to be called on each error.
         """
         if on_progress_callback is not None:
             if not callable(on_progress_callback):
-                raise TypeError("ProxyList.batch_collect_geolocations() argument on_progress_callback must be a"
-                                " callable.")
+                raise TypeError(
+                    "ProxyList.batch_collect_geolocations() argument on_progress_callback must be a"
+                    " callable."
+                )
         else:
             on_progress_callback = lambda proxy_list, progress: None
         if on_error_callback is not None:
             if not callable(on_error_callback):
-                raise TypeError("ProxyList.batch_collect_geolocations() argument on_error_callback must be a callable.")
+                raise TypeError(
+                    "ProxyList.batch_collect_geolocations() argument on_error_callback "
+                    "must be a callable."
+                )
         else:
             on_error_callback = lambda proxy_list, error: None
         all_proxies = list(self)
         for start_index in range(0, len(self), 100):
-            end_index = start_index + 100 if start_index + 100 < len(self) else len(self)
+            end_index = start_index + 100 if start_index + 100 < len(self
+                                                                     ) else len(self)
             proxies = all_proxies[start_index:end_index]
             try:
-                response = requests.post(url=f"http://ip-api.com/batch?fields={fields}",
-                                         json=[proxy.ip for proxy in proxies]).json()
+                response = requests.post(
+                    url=f"http://ip-api.com/batch?fields={fields}",
+                    json=[proxy.ip for proxy in proxies]
+                ).json()
                 for index, proxy in enumerate(proxies):
                     proxy.geolocation_info = response[index]
                 on_progress_callback(self, end_index / len(self) * 100)
-            except Exception as e:
-                on_error_callback(self, Exception("Failed to collect geolocation information.", e))
-
-    def to_json(self, indent: int = 4, include_status: bool = True, include_geolocation: bool = True) -> str:
-        """
-        This method is used to convert the list to a json string.
+            except Exception as ex:
+                on_error_callback(
+                    self, Exception("Failed to collect geolocation information.", ex)
+                )
+
+    def to_json(
+        self,
+        indent: int = 4,
+        include_status: bool = True,
+        include_geolocation: bool = True
+    ) -> str:
+        """This method is used to convert the list to a json string.
 
         :param indent: The indentation of the json string.
-        :param include_status: If True, the status of the proxy will be included in the json string.
-        :param include_geolocation: If True, the geolocation of the proxy will be included in the json string.
+        :param include_status: If True, the status of the proxy will be
+                included in the json string.
+        :param include_geolocation: If True, the geolocation of the
+                proxy will be included in the json string.
         """
         if include_geolocation:
             self.batch_collect_geolocations()
         proxies = []
         for proxy in self:
             proxies.append(
                 {
@@ -347,159 +407,212 @@
             if include_status:
                 proxies[-1]['status'] = proxy.status.name
             if include_geolocation:
                 proxies[-1]['geolocation_info'] = proxy.get_geolocation_info()
 
         return json.dumps(proxies, indent=indent)
 
-    def to_text_file(self, filename: _Union[str, os.PathLike], separator: str = "\n",
-                     format_: str = '{scheme}://{ip}:{port}') -> None:
-        """
-        This method is used to write the list to a text file.
+    def to_text_file(
+        self,
+        filename: _Union[str, os.PathLike],
+        separator: str = "\n",
+        format_: str = '{scheme}://{ip}:{port}'
+    ) -> None:
+        """This method is used to write the list to a text file.
 
         :param filename: The name of the text file.
         :param separator: The separator of the text file.
         :param format_: The format of each proxy.
         """
-        with open(filename, 'w') as f:
-            f.write(self.to_text(separator, format_))
+        with open(filename, 'w', encoding='utf-8') as file:
+            file.write(self.to_text(separator, format_))
 
-    def to_json_file(self, filename: _Union[str, os.PathLike], indent: int = 4, include_status: bool = True,
-                     include_geolocation: bool = True) -> None:
-        """
-        This method is used to write the list to a json file.
+    def to_json_file(
+        self,
+        filename: _Union[str, os.PathLike],
+        indent: int = 4,
+        include_status: bool = True,
+        include_geolocation: bool = True
+    ) -> None:
+        """This method is used to write the list to a json file.
 
         :param filename: The name of the json file.
         :param indent: The indentation of the json string.
-        :param include_status: If True, the status of the proxy will be included in the json string.
-        :param include_geolocation: If True, the geolocation of the proxy will be included in the json string.
-        """
-        with open(filename, 'w') as f:
-            f.write(self.to_json(indent, include_status, include_geolocation))
-
-    def to_csv_file(self, filename: _Union[str, os.PathLike], include_status: bool = True,
-                    include_geolocation: bool = True) -> None:
-        """
-        This method is used to convert the list to a csv file.
+        :param include_status: If True, the status of the proxy will be
+                included in the json string.
+        :param include_geolocation: If True, the geolocation of the
+                proxy will be included in the json string.
+        """
+        with open(filename, 'w', encoding='utf-8') as file:
+            file.write(self.to_json(indent, include_status, include_geolocation))
+
+    def to_csv_file(
+        self,
+        filename: _Union[str, os.PathLike],
+        include_status: bool = True,
+        include_geolocation: bool = True
+    ) -> None:
+        """This method is used to convert the list to a csv file.
 
         :param filename: The name of the csv file.
-        :param include_status: If True, the status of the proxy will be included in the csv file.
-        :param include_geolocation: If True, the geolocation of the proxy will be included in the csv file.
+        :param include_status: If True, the status of the proxy will be
+                included in the csv file.
+        :param include_geolocation: If True, the geolocation of the
+                proxy will be included in the csv file.
         """
         if include_geolocation:
             self.batch_collect_geolocations()
-        with open(filename, 'w', newline='') as csvfile:
-            writer = csv.writer(csvfile)
+        with open(filename, 'w', newline='', encoding='utf-8') as csv_file:
+            writer = csv.writer(csv_file)
             if include_status and include_geolocation:
                 writer.writerow(['ip', 'port', 'type', 'status', 'geolocation_info'])
                 for proxy in self:
-                    writer.writerow([proxy.ip, proxy.port, proxy.type.name, proxy.status.name,
-                                     proxy.get_geolocation_info()])
+                    writer.writerow(
+                        [
+                            proxy.ip, proxy.port, proxy.type.name, proxy.status.name,
+                            proxy.get_geolocation_info()
+                        ]
+                    )
             elif include_status:
                 writer.writerow(['ip', 'port', 'type', 'status'])
                 for proxy in self:
-                    writer.writerow([proxy.ip, proxy.port, proxy.type.name, proxy.status.name])
+                    writer.writerow(
+                        [proxy.ip, proxy.port, proxy.type.name, proxy.status.name]
+                    )
             elif include_geolocation:
                 writer.writerow(['ip', 'port', 'type', 'geolocation_info'])
                 for proxy in self:
-                    writer.writerow([proxy.ip, proxy.port, proxy.type.name, proxy.get_geolocation_info()])
+                    writer.writerow(
+                        [
+                            proxy.ip, proxy.port, proxy.type.name,
+                            proxy.get_geolocation_info()
+                        ]
+                    )
             else:
                 writer.writerow(['ip', 'port', 'type'])
                 for proxy in self:
                     writer.writerow([proxy.ip, proxy.port, proxy.type.name])
 
     @staticmethod
-    def from_text(text: str, separator: str = "\n", default_type: ProxyType = None) -> 'ProxyList':
-        """
-        This method is used to convert a text string to a ProxyList.
+    def from_text(
+        text: str,
+        separator: str = "\n",
+        default_type: _Optional[ProxyType] = None
+    ) -> 'ProxyList':
+        """This method is used to convert a text string to a ProxyList.
 
         :param text: The text string.
         :param separator: The separator of the text string.
         :param default_type: The default type of the proxy.
         """
         proxies = ProxyList()
         for proxy in text.split(separator):
             proxies.add(Proxy.from_text(proxy, default_type))
         return proxies
 
     @staticmethod
     def from_json(json_string: str) -> 'ProxyList':
-        """
-        This method is used to convert the json string to a ProxyList
+        """This method is used to convert the json string to a ProxyList.
 
         :param json_string: The json string.
         """
         proxies = json.loads(json_string)
         proxy_list = ProxyList()
         for proxy in proxies:
             if 'ip' in proxy and 'port' in proxy and 'type' in proxy:
-                proxy_ = Proxy(ip=proxy['ip'], port=proxy['port'], type_=ProxyType.from_name(proxy['type']))
+                proxy_ = Proxy(
+                    ip=proxy['ip'],
+                    port=proxy['port'],
+                    type_=ProxyType.from_name(proxy['type'])
+                )
             else:
                 raise Exception(f"Invalid proxy format: {proxy}")
             if 'status' in proxy:
                 proxy_.status = ProxyStatus.from_name(proxy['status'])
             if 'geolocation_info' in proxy:
                 proxy_.geolocation_info = proxy['geolocation_info']
             proxy_list.add(proxy_)
 
         return proxy_list
 
     @staticmethod
-    def from_text_file(filename: _Union[str, os.PathLike], separator: str = "\n",
-                       default_type: ProxyType = None) -> 'ProxyList':
-        """
-        This method is used to convert a text file to a ProxyList.
+    def from_text_file(
+        filename: _Union[str, os.PathLike],
+        separator: str = "\n",
+        default_type: _Optional[ProxyType] = None
+    ) -> 'ProxyList':
+        """This method is used to convert a text file to a ProxyList.
 
         :param filename: The name of the text file.
         :param separator: The separator of the text file.
         :param default_type: The default type of the proxy.
         """
-        with open(filename, 'r') as f:
-            return ProxyList.from_text(f.read(), separator, default_type)
+        with open(filename, 'r', encoding='utf-8') as file:
+            return ProxyList.from_text(file.read(), separator, default_type)
 
     @staticmethod
     def from_json_file(filename: _Union[str, os.PathLike]) -> 'ProxyList':
-        """
-        This method is used to convert a json file to a ProxyList.
+        """This method is used to convert a json file to a ProxyList.
 
         :param filename: The name of the json file.
         """
-        with open(filename, 'r') as f:
-            return ProxyList.from_json(f.read())
+        with open(filename, 'r', encoding='utf-8') as file:
+            return ProxyList.from_json(file.read())
 
     @staticmethod
-    def from_csv_file(filename: _Union[str, os.PathLike], default_type: ProxyType = None) -> 'ProxyList':
-        """
-        This method is used to convert the csv file to a ProxyList.
+    def from_csv_file(
+        filename: _Union[str, os.PathLike],
+        default_type: _Optional[ProxyType] = None
+    ) -> 'ProxyList':
+        """This method is used to convert the csv file to a ProxyList.
 
         :param filename: The name of the csv file.
         :param default_type: The default type of the proxy.
         """
-        with open(filename, 'r') as f:
-            reader = csv.reader(f)
+        with open(filename, 'r', encoding='utf-8') as file:
+            reader = csv.reader(file)
             proxies = []
             for row in reader:
                 proxies.append(row)
         proxy_list = ProxyList()
         for proxy in proxies:
             if len(proxy) == [3, 4, 5]:
-                proxy_list.add(Proxy(ip=proxy[0], port=int(proxy[1]), type_=ProxyType.from_name(proxy[2])))
+                proxy_list.add(
+                    Proxy(
+                        ip=proxy[0],
+                        port=int(proxy[1]),
+                        type_=ProxyType.from_name(proxy[2])
+                    )
+                )
             elif len(proxy) == 2:
                 if default_type is None:
-                    raise Exception(f"Invalid proxy format: {proxy}. You should specify the default type.")
-                proxy_list.add(Proxy(ip=proxy[0], port=int(proxy[1]), type_=default_type))
+                    raise InvalidProxyURL(
+                        f"Invalid proxy format: {proxy}. "
+                        "You should specify the default type."
+                    )
+                proxy_list.add(
+                    Proxy(ip=proxy[0], port=int(proxy[1]), type_=default_type)
+                )
             else:
-                raise Exception(f"Invalid proxy format: {proxy}")
+                raise InvalidProxyURL(f"Invalid proxy format: {proxy}")
         return proxy_list
 
-    def filter(self, status: ProxyStatus = None, type_: _Union[ProxyType, _Iterable[ProxyType]] = None,
-               continent: str = None, country: str = None, region: str = None, city: str = None, isp: str = None,
-               org: str = None, asname: str = None) -> 'ProxyList':
-        """
-        This method is used to filter the list of proxies.
+    def filter(
+        self,
+        status: _Optional[ProxyStatus] = None,
+        type_: _Optional[_Union[ProxyType, _Iterable[ProxyType]]] = None,
+        continent: _Optional[str] = None,
+        country: _Optional[str] = None,
+        region: _Optional[str] = None,
+        city: _Optional[str] = None,
+        isp: _Optional[str] = None,
+        org: _Optional[str] = None,
+        asname: _Optional[str] = None
+    ) -> 'ProxyList':
+        """This method is used to filter the list of proxies.
 
         :param status: The status of the proxy.
         :param type_: The type of the proxy.
         :param continent: The continent of the proxy.
         :param country: The country of the proxy.
         :param region: The region of the proxy.
         :param city: The city of the proxy.
@@ -515,17 +628,19 @@
             if type_ is not None:
                 if isinstance(type_, ProxyType):
                     if proxy.type != type_:
                         continue
                 else:
                     if proxy.type not in type_:
                         continue
-            if continent is not None and proxy.get_geolocation_info()['continent'] != continent:
+            if continent is not None and proxy.get_geolocation_info(
+            )['continent'] != continent:
                 continue
-            if country is not None and proxy.get_geolocation_info()['country'] != country:
+            if country is not None and proxy.get_geolocation_info(
+            )['country'] != country:
                 continue
             if region is not None and proxy.get_geolocation_info()['region'] != region:
                 continue
             if city is not None and proxy.get_geolocation_info()['city'] != city:
                 continue
             if isp is not None and proxy.get_geolocation_info()['isp'] != isp:
                 continue
```

### Comparing `ProxyEater-1.5.1/ProxyEater/Scraper.py` & `ProxyEater-1.5.2/ProxyEater/Scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 # ProxyEater.Scraper.py
 # CodeWriter21
 
-from typing import Callable as _Callable
+from __future__ import annotations
+
+from typing import Callable as _Callable, Optional as _Optional
 
 import pandas  # This module is used to parse the html table.
 import requests  # This module is used to send requests to the server.
+from random_user_agent.user_agent import \
+    UserAgent  # This module is used for generating random user agents.
 
-from random_user_agent.user_agent import UserAgent  # This module is used to generate random user agents.
-
-from .Proxy import ProxyList, Proxy, ProxyType
+from .Proxy import Proxy, ProxyList, ProxyType
 
 useragent_generator = UserAgent()
 
 __all__ = ['Scraper']
 
 
 class Scraper:
     is_succeed: bool = False
 
-    def __init__(self, url: str, parser: dict, method: str = 'GET', name: str = None, useragent: str = None,
-                 proxy: Proxy = None, request_timeout: int = 10) -> None:
+    def __init__(
+        self,
+        url: str,
+        parser: dict,
+        method: str = 'GET',
+        name: _Optional[str] = None,
+        useragent: _Optional[str] = None,
+        proxy: _Optional[Proxy] = None,
+        request_timeout: int = 10
+    ) -> None:
         self.session: requests.Session = requests.Session()
         if useragent:
             self.session.headers.update({'User-Agent': useragent})
         else:
-            self.session.headers.update({'User-Agent': useragent_generator.get_random_user_agent()})
+            self.session.headers.update(
+                {'User-Agent': useragent_generator.get_random_user_agent()}
+            )
         self.url: str = url
         self.parser: dict = parser
         self.method: str = method
-        self.name: str = name
+        self.name: str = name or ''
         self.parser_type: str = list(self.parser.keys())[0]
         self.parser_config: dict = list(self.parser.values())[0]
-        self.default_type = ProxyType.from_name(self.parser_config.get('type', {}).get('default', 'HTTP'))
-        self.is_https_header = self.parser_config.get('type', {}).get('is_https_header', None)
-        self.is_https_value = self.parser_config.get('type', {}).get('is_https_value', 'yes')
+        self.default_type = ProxyType.from_name(
+            self.parser_config.get('type', {}).get('default', 'HTTP')
+        )
+        self.is_https_header = self.parser_config.get('type',
+                                                      {}).get('is_https_header', None)
+        self.is_https_value = self.parser_config.get('type',
+                                                     {}).get('is_https_value', 'yes')
         self.protocols = self.parser_config.get('type', {}).get('protocols', {})
         self.protocols_header = self.protocols.get('header', None)
         self.protocols_http = self.protocols.get('http', 'HTTP')
         self.protocols_https = self.protocols.get('https', 'HTTPS')
         self.protocols_socks4 = self.protocols.get('socks4', 'SOCKS4')
         self.protocols_socks5 = self.protocols.get('socks5', 'SOCKS5')
         self.pages_config = self.parser_config.get('pages', {})
@@ -46,34 +62,43 @@
         if (self.pages_end != "no-proxy") and (not isinstance(self.pages_end, int)):
             raise ValueError("The end page must be a number or 'no-proxy'.")
         if isinstance(self.pages_end, int):
             if self.pages_end < self.pages_start:
                 raise ValueError("The end page must be greater than the start page.")
         self.pages_step = self.pages_config.get('step', 1)
         self.pages_url_format_name = self.pages_config.get('format name', 'page')
-        self.proxy: Proxy = proxy
+        self.proxy: _Optional[Proxy] = proxy
         self.request_timeout: int = request_timeout
         self.proxies: ProxyList = ProxyList()
 
     def request(self, url: str) -> requests.Response:
         return self.session.request(
             method=self.method,
             url=url,
             timeout=self.request_timeout,
-            proxies=({'http': str(self.proxy), 'https': str(self.proxy)}) if self.proxy else None
+            proxies=({
+                'http': str(self.proxy),
+                'https': str(self.proxy)
+            }) if self.proxy else None
         )
 
-    def get_proxies(self, on_progress_callback: _Callable = None, on_success_callback: _Callable = None,
-                    on_failure_callback: _Callable = None) -> ProxyList:
-        """
-        This method is used to get proxies from the server.
-
-        :param on_progress_callback: This is a callback function that is called when the scraper is in progress.
-        :param on_success_callback: This is a callback function that is called when the scraper is successful.
-        :param on_failure_callback: This is a callback function that is called when the scraper is failed.
+    def get_proxies(
+        self,
+        on_progress_callback: _Optional[_Callable] = None,
+        on_success_callback: _Optional[_Callable] = None,
+        on_failure_callback: _Optional[_Callable] = None
+    ) -> ProxyList:
+        """This method is used to get proxies from the server.
+
+        :param on_progress_callback: This is a callback function that is
+                called when the scraper is in progress.
+        :param on_success_callback: This is a callback function that is
+                called when the scraper is successful.
+        :param on_failure_callback: This is a callback function that is
+                called when the scraper is failed.
         :return: A ProxyList object.
         """
         if on_progress_callback:
             if not isinstance(on_progress_callback, _Callable):
                 raise TypeError('on_progress_callback must be a callable object.')
         else:
             on_progress_callback = lambda obj, progress, page: None
@@ -84,77 +109,94 @@
             on_success_callback = lambda obj: None
         if on_failure_callback:
             if not isinstance(on_failure_callback, _Callable):
                 raise TypeError('on_failure_callback must be a callable object.')
         else:
             on_failure_callback = lambda obj, exception: None
 
-        def _get_proxies(page: int = 1) -> 'ProxyList':
+        def _get_proxies(page: int = 1) -> ProxyList:
             proxies_ = ProxyList()
             on_progress_callback(self, progress=0, page=page)
             response = self.request(self.url.format(page=page))
             on_progress_callback(self, progress=10, page=page)
             if self.parser_type == "pandas":
-                df = pandas.read_html(response.text)[self.parser_config.get('table_index', 0)]
-                for x in range(0, len(df)):
-                    on_progress_callback(self, progress=10 + (x / len(df) * 90), page=page)
+                dataframe = pandas.read_html(response.text
+                                      )[self.parser_config.get('table_index', 0)]
+                for i in range(0, len(dataframe)):
+                    on_progress_callback(
+                        self, progress=10 + (i / len(dataframe) * 90), page=page
+                    )
                     try:
                         if not self.parser_config.get('combined', None):
-                            ip = str(df.loc[df.index[x], self.parser_config.get('ip')]).strip()
-                            port = int(df.loc[df.index[x], self.parser_config.get('port')])
+                            ip = str(dataframe.loc[dataframe.index[i],
+                                            self.parser_config.get('ip')]).strip()
+                            port = int(
+                                dataframe.loc[dataframe.index[i],
+                                       self.parser_config.get('port')]
+                            )
                             if self.is_https_header:
-                                if str(df.loc[
-                                           df.index[x], self.is_https_header]).strip().lower() == self.is_https_value:
+                                if str(dataframe.loc[dataframe.index[i], self.is_https_header]
+                                       ).strip().lower() == self.is_https_value:
                                     proxies_.add(Proxy(ip, port, ProxyType.HTTPS))
                                 else:
                                     proxies_.add(Proxy(ip, port, self.default_type))
                                 continue
                             if self.protocols_header:
-                                protocol = str(df.loc[df.index[x], self.protocols_header]).strip().lower()
+                                protocol = str(
+                                    dataframe.loc[dataframe.index[i], self.protocols_header]
+                                ).strip().lower()
                                 if protocol == self.protocols_http:
                                     proxies_.add(Proxy(ip, port, ProxyType.HTTP))
                                 elif protocol == self.protocols_https:
                                     proxies_.add(Proxy(ip, port, ProxyType.HTTPS))
                                 elif protocol == self.protocols_socks4:
                                     proxies_.add(Proxy(ip, port, ProxyType.SOCKS4))
                                 elif protocol == self.protocols_socks5:
                                     proxies_.add(Proxy(ip, port, ProxyType.SOCKS5))
                                 else:
                                     proxies_.add(Proxy(ip, port, self.default_type))
                                 continue
                             proxies_.add(Proxy(ip, port, self.default_type))
                         else:
-                            combined: str = df.loc[df.index[x], self.parser_config.get('combined')]
+                            combined: str = dataframe.loc[dataframe.index[i],
+                                                   self.parser_config.get('combined')]
                             if len(combined.split(':')) == 2:
                                 ip = combined.split(':')[0].strip()
                                 port = int(combined.split(':')[1])
                                 proxies_.add(Proxy(ip, port, ProxyType.HTTP))
                     except:
                         continue
 
             if self.parser_type == "json":
                 data = response.json()[self.parser_config.get('data')]
-                for i, x in enumerate(data):
-                    on_progress_callback(self, progress=10 + (i / len(data) * 90), page=page)
-                    proxies_.add(Proxy(
-                        str(x[self.parser_config.get('ip', '')]).strip(),
-                        int(x[self.parser_config.get('port', '')]),
-                        self.default_type
-                    ))
+                for index, i in enumerate(data):
+                    on_progress_callback(
+                        self, progress=10 + (index / len(data) * 90), page=page
+                    )
+                    proxies_.add(
+                        Proxy(
+                            str(i[self.parser_config.get('ip', '')]).strip(),
+                            int(i[self.parser_config.get('port', '')]),
+                            self.default_type
+                        )
+                    )
 
             if self.parser_type == "text":
                 data = str(response.content, encoding='utf-8')
-                for i, x in enumerate(data.split('\n')):
-                    on_progress_callback(self, progress=10 + (i / len(data) * 90), page=page)
-                    if len(x.split(':')) == 2:
-                        proxies_.add(Proxy(
-                            x.split(':')[0].strip(),
-                            int(x.split(':')[1]),
-                            self.default_type
-                        ))
+                for index, i in enumerate(data.split('\n')):
+                    on_progress_callback(
+                        self, progress=10 + (index / len(data) * 90), page=page
+                    )
+                    if len(i.split(':')) == 2:
+                        proxies_.add(
+                            Proxy(
+                                i.split(':')[0].strip(), int(i.split(':')[1]),
+                                self.default_type
+                            )
+                        )
 
             on_progress_callback(self, progress=100, page=page)
 
             return proxies_
 
         try:
             if self.pages_config:
@@ -163,20 +205,22 @@
                     if self.pages_end == "no-proxy":
                         proxies = _get_proxies(page_index)
                         if proxies.count < 1:
                             break
                     elif page_index <= self.pages_end:
                         proxies = _get_proxies(page_index)
                     else:
-                        raise ValueError('The pages_end value must be "no-proxy" or a number.')
+                        raise ValueError(
+                            'The pages_end value must be "no-proxy" or a number.'
+                        )
                     page_index += self.pages_step
                     self.proxies.update(proxies)
             else:
                 self.proxies.update(_get_proxies())
 
             self.is_succeed = True
             on_success_callback(self)
-        except Exception as e:
+        except Exception as ex:
             self.is_succeed = False
-            on_failure_callback(self, e)
+            on_failure_callback(self, ex)
 
         return self.proxies
```

### Comparing `ProxyEater-1.5.1/ProxyEater/__main__.py` & `ProxyEater-1.5.2/ProxyEater/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # ProxyEater.__main__.py
 # CodeWriter21
 import sys
 import json
 import shutil
 import pathlib
+import argparse
 
 import log21
 import importlib_resources
 
-from .Proxy import Proxy, ProxyType, ProxyList
-from .Scraper import Scraper
-
 import ProxyEater
 
+from .Proxy import Proxy, ProxyList, ProxyType
+from .Scraper import Scraper
+
 path = importlib_resources.files('ProxyEater')
 
 logger = log21.get_logger("ProxyEater")
 
 
-def scrape(args):
+def scrape(args: argparse.Namespace) -> None:
+    """Scrapes different websites and collects proxies.
+
+    :param args: A Namespace containing needed arguments.
+    """
     if not args.source:
         source = path / 'sources.json'
     else:
         source = pathlib.Path(args.source)
     if not source.exists():
         logger.error(f'The source {source} does not exist.')
         return
@@ -43,51 +48,78 @@
     useragent = args.useragent
 
     proxies = ProxyList()
     # Scrape
     for config in source_data:
         progress_callback = finish_callback = error_callback = checking_callback = None
         if args.verbose:
-            logger.progress_bar = log21.ProgressBar(format_='Proxies: {count} {prefix}{bar}{suffix} {percentage}%',
-                                                    style='{', additional_variables={'count': 0})
+            logger.progress_bar = log21.ProgressBar(
+                format_='Proxies: {count} {prefix}{bar}{suffix} {percentage}%',
+                style='{',
+                additional_variables={'count': 0}
+            )
 
             def progress_callback(scraper_: Scraper, progress: float, page: int):
-                logger.info(f'{scraper_.name}: Collected: {scraper_.proxies.count}; Page: {page}, {progress:.2f}%',
-                            end='\r')
+                logger.info(
+                    f'{scraper_.name}: Collected: {scraper_.proxies.count}; Page: {page}, {progress:.2f}%',
+                    end='\r'
+                )
 
             def finish_callback(scraper_: Scraper):
-                logger.info(f'{scraper_.name}: Collected: {scraper_.proxies.count}, 100.0%')
+                logger.info(
+                    f'{scraper_.name}: Collected: {scraper_.proxies.count}, 100.0%'
+                )
                 logger.info(f'{scraper_.name}: Done.')
 
             def error_callback(scraper_: Scraper, error: Exception):
                 logger.error(f'{scraper_.name}: {error.__class__.__name__}: {error}')
 
             def checking_callback(proxy_list: ProxyList, progress: float):
                 logger.progress_bar(progress, 100, count=proxy_list.count)
 
         logger.info(f'Scraping {config.get("id")}...')
-        scraper = Scraper(config.get('url'), config.get('parser'), method=config.get('method'),
-                          name=config.get('id'), useragent=useragent, proxy=proxy, request_timeout=args.timeout)
-        proxies_ = scraper.get_proxies(on_progress_callback=progress_callback, on_success_callback=finish_callback,
-                                       on_failure_callback=error_callback)
+        scraper = Scraper(
+            config.get('url'),
+            config.get('parser'),
+            method=config.get('method'),
+            name=config.get('id'),
+            useragent=useragent,
+            proxy=proxy,
+            request_timeout=args.timeout
+        )
+        proxies_ = scraper.get_proxies(
+            on_progress_callback=progress_callback,
+            on_success_callback=finish_callback,
+            on_failure_callback=error_callback
+        )
 
         collected_proxies_count = proxies_.count
         # Filter the proxies
         logger.info('Filtering the proxies...')
         proxies_ = proxies_.filter(type_=args.proxy_types)
         if args.verbose:
-            logger.info(f'{scraper.name}: Removed {collected_proxies_count - proxies_.count} proxies of wrong type.')
+            logger.info(
+                f'{scraper.name}: Removed {collected_proxies_count - proxies_.count} '
+                'proxies of wrong type.'
+            )
         collected_proxies_count = proxies_.count
         # Check the proxies
         if collected_proxies_count > 0 and not args.no_check:
             logger.info('Checking if the proxies are alive...')
-            proxies_.check_all(timeout=args.timeout, threads_no=args.threads, on_progress_callback=checking_callback,
-                               url=args.url)
+            proxies_.check_all(
+                timeout=args.timeout,
+                threads_no=args.threads,
+                on_progress_callback=checking_callback,
+                url=args.url
+            )
             if args.verbose:
-                logger.info(f'{scraper.name}: Removed {collected_proxies_count - proxies_.count} dead proxies.')
+                logger.info(
+                    f'{scraper.name}: Removed '
+                    f'{collected_proxies_count - proxies_.count} dead proxies.'
+                )
 
         proxies.update(proxies_)
         logger.info(f'Scraped {len(proxies)} proxies.')
 
         if proxies.count > 0:
             if args.include_geolocation:
                 on_progress_callback = on_error_callback = None
@@ -95,28 +127,37 @@
                     logger.progress_bar = log21.ProgressBar()
 
                     def on_progress_callback(proxy_list: ProxyList, progress: float):
                         logger.progress_bar(progress, 100)
 
                     def on_error_callback(proxy_list: ProxyList, error: Exception):
                         logger.error(f'{error.__class__.__name__}: {error}')
+
                 logger.info('Getting the geolocation info of the proxies...')
-                proxies.batch_collect_geolocations(on_progress_callback=on_progress_callback,
-                                                   on_error_callback=on_error_callback)
+                proxies.batch_collect_geolocations(
+                    on_progress_callback=on_progress_callback,
+                    on_error_callback=on_error_callback
+                )
             if args.verbose:
                 logger.info(f'Writing {proxies.count} proxies to {args.output}...')
             # Write to file
             if args.file_format == 'text':
                 proxies.to_text_file(args.output, '\n', format_=args.format)
             elif args.file_format == 'json':
-                proxies.to_json_file(args.output, include_status=args.include_status,
-                                     include_geolocation=args.include_geolocation)
+                proxies.to_json_file(
+                    args.output,
+                    include_status=args.include_status,
+                    include_geolocation=args.include_geolocation
+                )
             elif args.file_format == 'csv':
-                proxies.to_csv_file(args.output, include_status=args.include_status,
-                                    include_geolocation=args.include_geolocation)
+                proxies.to_csv_file(
+                    args.output,
+                    include_status=args.include_status,
+                    include_geolocation=args.include_geolocation
+                )
     if proxies.count > 0:
         logger.info(f'Wrote {proxies.count} proxies to {args.output}.')
 
 
 def check(args):
     # Validate the source path
     if not args.source:
@@ -143,29 +184,38 @@
 
     if len(args.proxy_types) < 4:
         loaded_proxies_count = proxies.count
         # Filter the proxies
         logger.info('Filtering the proxies...')
         proxies = proxies.filter(type_=args.proxy_types)
         if args.verbose:
-            logger.info(f'Removed {loaded_proxies_count - proxies.count} proxies of wrong type.')
-
-    logger.progress_bar = log21.ProgressBar(format_='Proxies: {count} {prefix}{bar}{suffix} {percentage}%', style='{',
-                                            additional_variables={'count': 0})
+            logger.info(
+                f'Removed {loaded_proxies_count - proxies.count} proxies of wrong type.'
+            )
+
+    logger.progress_bar = log21.ProgressBar(
+        format_='Proxies: {count} {prefix}{bar}{suffix} {percentage}%',
+        style='{',
+        additional_variables={'count': 0}
+    )
 
     def checking_callback(proxy_list: ProxyList, progress: float):
         logger.progress_bar(progress, 100, count=proxy_list.count)
 
     # Check the proxies
     count = proxies.count
     if args.verbose:
         logger.info('Checking if the proxies are alive...')
         logger.info('Number of proxies:', proxies.count)
-    proxies.check_all(timeout=args.timeout, threads_no=args.threads, on_progress_callback=checking_callback,
-                      url=args.url)
+    proxies.check_all(
+        timeout=args.timeout,
+        threads_no=args.threads,
+        on_progress_callback=checking_callback,
+        url=args.url
+    )
     if args.verbose:
         logger.info(f'Removed {count - proxies.count} dead proxies.')
     logger.info(f'Alive proxies: {proxies.count}')
 
     if proxies.count > 0:
         if args.include_geolocation:
             on_progress_callback = on_error_callback = None
@@ -173,73 +223,156 @@
                 logger.progress_bar = log21.ProgressBar()
 
                 def on_progress_callback(proxy_list: ProxyList, progress: float):
                     logger.progress_bar(progress, 100)
 
                 def on_error_callback(proxy_list: ProxyList, error: Exception):
                     logger.error(f'{error.__class__.__name__}: {error}')
+
             logger.info('Getting the geolocation info of the proxies...')
-            proxies.batch_collect_geolocations(on_progress_callback=on_progress_callback,
-                                               on_error_callback=on_error_callback)
+            proxies.batch_collect_geolocations(
+                on_progress_callback=on_progress_callback,
+                on_error_callback=on_error_callback
+            )
         # Write to file
         if args.file_format == 'text':
             proxies.to_text_file(args.output, '\n', format_=args.format)
         elif args.file_format == 'json':
-            proxies.to_json_file(args.output, include_status=args.include_status,
-                                 include_geolocation=args.include_geolocation)
+            proxies.to_json_file(
+                args.output,
+                include_status=args.include_status,
+                include_geolocation=args.include_geolocation
+            )
         elif args.file_format == 'csv':
-            proxies.to_csv_file(args.output, include_status=args.include_status,
-                                include_geolocation=args.include_geolocation)
+            proxies.to_csv_file(
+                args.output,
+                include_status=args.include_status,
+                include_geolocation=args.include_geolocation
+            )
         logger.info(f'Wrote {proxies.count} proxies to {args.output}.')
 
 
 def main():
     try:
         parser = log21.ColorizingArgumentParser()
         parser.add_argument('mode', help='Modes: Scrape, Check')
-        parser.add_argument('--source', '-s', help=f'The source of the proxies(default:{path / "sources.json"}).')
+        parser.add_argument(
+            '--source',
+            '-s',
+            help=f'The source of the proxies(default:{path / "sources.json"}).'
+        )
         parser.add_argument('--output', '-o', help=f'The output file.')
-        parser.add_argument('--file-format', '-ff', help=f'The format of the output file(default:text).',
-                            default='text',
-                            choices=['text', 'json', 'csv'])
-        parser.add_argument('--format', '-f', help='The format for saving the proxies in text file(default:'
-                                                   '"{scheme}://{ip}:{port}").',
-                            default='{scheme}://{ip}:{port}')
-        parser.add_argument('--proxy-type', '-type', help=f'The type of the proxies(default:all).', default='')
-        parser.add_argument('--include-status', '-is', help=f'Include the status of the proxies in the output file.',
-                            action='store_true')
-        parser.add_argument('--threads', '-t', help=f'The number of threads to use for scraping(default:25).', type=int,
-                            default=25)
-        parser.add_argument('--timeout', '-to', help=f'The timeout of the requests(default:15).', default=15, type=int)
-        parser.add_argument('--url', '-u', help='The url to use for checking the proxies'
-                                                '(default:http://icanhazip.com).', default='http://icanhazip.com')
-        parser.add_argument('--verbose', '-v', help=f'The verbose of the program(default:False).', action='store_true')
-        parser.add_argument('--quiet', '-q', help=f'The quiet of the program(default:False).', action='store_true')
-        parser.add_argument('--version', '-V', help=f'The version of the program.', action='version',
-                            version='%(prog)s ' + ProxyEater.__version__)
+        parser.add_argument(
+            '--file-format',
+            '-ff',
+            help='The format of the output file(default:text).',
+            default='text',
+            choices=['text', 'json', 'csv']
+        )
+        parser.add_argument(
+            '--format',
+            '-f',
+            help='The format for saving the proxies in text file(default:'
+            '"{scheme}://{ip}:{port}").',
+            default='{scheme}://{ip}:{port}'
+        )
+        parser.add_argument(
+            '--proxy-type',
+            '-type',
+            help='The type of the proxies(default:all).',
+            default=''
+        )
+        parser.add_argument(
+            '--include-status',
+            '-is',
+            help='Include the status of the proxies in the output file.',
+            action='store_true'
+        )
+        parser.add_argument(
+            '--threads',
+            '-t',
+            help='The number of threads to use for scraping(default:25).',
+            type=int,
+            default=25
+        )
+        parser.add_argument(
+            '--timeout',
+            '-to',
+            help='The timeout of the requests(default:15).',
+            default=15,
+            type=int
+        )
+        parser.add_argument(
+            '--url',
+            '-u',
+            help='The url to use for checking the proxies'
+            '(default:http://icanhazip.com).',
+            default='http://icanhazip.com'
+        )
+        parser.add_argument(
+            '--verbose',
+            '-v',
+            help='The verbose of the program(default:False).',
+            action='store_true'
+        )
+        parser.add_argument(
+            '--quiet',
+            '-q',
+            help='The quiet of the program(default:False).',
+            action='store_true'
+        )
+        parser.add_argument(
+            '--version',
+            '-V',
+            help='The version of the program.',
+            action='version',
+            version='%(prog)s ' + ProxyEater.__version__
+        )
         scrap_arguments = parser.add_argument_group('Scrape', 'Scrape mode arguments')
-        scrap_arguments.add_argument('--proxy', '-p', help=f'The proxy to use for scraping.')
-        scrap_arguments.add_argument('--useragent', '-ua', help=f'The useragent of the requests(default:random).')
-        scrap_arguments.add_argument('--include-geolocation', '-ig',
-                                     help=f'Include the geolocation info of the proxies in the output file.',
-                                     action='store_true')
-        scrap_arguments.add_argument('--no-check', '-nc',
-                                     help=f'Use this option to skip the checking of the proxies after ',
-                                     action='store_true')
+        scrap_arguments.add_argument(
+            '--proxy', '-p', help='The proxy to use for scraping.'
+        )
+        scrap_arguments.add_argument(
+            '--useragent',
+            '-ua',
+            help='The useragent of the requests(default:random).'
+        )
+        scrap_arguments.add_argument(
+            '--include-geolocation',
+            '-ig',
+            help='Include the geolocation info of the proxies in the output file.',
+            action='store_true'
+        )
+        scrap_arguments.add_argument(
+            '--no-check',
+            '-nc',
+            help='Use this option to skip the checking of the proxies after ',
+            action='store_true'
+        )
         check_arguments = parser.add_argument_group('Check', 'Check mode arguments')
-        check_arguments.add_argument('--source-format', '-sf', help=f'The format of the source file(default:text).',
-                                     default='text', choices=['text', 'json', 'csv'])
-        check_arguments.add_argument('--default-type', '-dt', help=f'The default type of the proxies - '
-                                                                   f'Use this if you are providing proxies without '
-                                                                   f'scheme(default:http).',
-                                     default='http', choices=['http', 'https', 'socks4', 'socks5'])
+        check_arguments.add_argument(
+            '--source-format',
+            '-sf',
+            help='The format of the source file(default:text).',
+            default='text',
+            choices=['text', 'json', 'csv']
+        )
+        check_arguments.add_argument(
+            '--default-type',
+            '-dt',
+            help='The default type of the proxies - '
+            'Use this if you are providing proxies without '
+            'scheme(default:http).',
+            default='http',
+            choices=['http', 'https', 'socks4', 'socks5']
+        )
         args = parser.parse_args()
 
         if args.verbose and args.quiet:
-            parser.error(f'The verbose and quiet are both set.')
+            parser.error('The verbose and quiet are both set.')
             return
 
         logger.setLevel(log21.ERROR if args.quiet else log21.INFO)
 
         args.timeout = int(args.timeout)
         if args.timeout < 0.1:
             parser.error(f'The timeout({args.timeout}) is not valid.')
@@ -272,18 +405,20 @@
         # Parse the proxy type
         if args.proxy_type:
             proxy_types = [x.strip() for x in args.proxy_type.split(',')]
         if not proxy_types:
             proxy_types = ['http', 'https', 'socks4', 'socks5']
         try:
             proxy_types = [ProxyType.from_name(x) for x in proxy_types]
-        except ValueError as e:
-            logger.error(e)
+        except ValueError as ex:
+            logger.error(ex)
             return
-        logger.info(f'Using proxy types: {[proxy_type.name for proxy_type in proxy_types]}')
+        logger.info(
+            f'Using proxy types: {[proxy_type.name for proxy_type in proxy_types]}'
+        )
         args.proxy_types = proxy_types
 
         args.mode = args.mode.lower()
         if args.mode == 'scrape':
             scrape(args)
         elif args.mode == 'check':
             check(args)
```

### Comparing `ProxyEater-1.5.1/ProxyEater/sources.json` & `ProxyEater-1.5.2/ProxyEater/sources.json`

 * *Files identical despite different names*

### Comparing `ProxyEater-1.5.1/ProxyEater.egg-info/PKG-INFO` & `ProxyEater-1.5.2/ProxyEater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: ProxyEater
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Python Proxy Scraper for gathering fresh proxies.
 Home-page: https://github.com/MPCodeWriter21/ProxyEater
 Author: CodeWriter21
 Author-email: CodeWriter21@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-ProxyEater\[1.5.1\]
+ProxyEater\[1.5.2\]
 ===================
 
 ![version](https://img.shields.io/pypi/v/ProxyEater)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/ProxyEater)
 [![CodeFactor](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater/badge)](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater)
 
 A Python Proxy Scraper for gathering fresh proxies.
@@ -58,15 +56,15 @@
 positional arguments:
   mode              Modes: Scrape, Check
 
 options:
   -h, --help
                         show this help message and exit
   --source SOURCE, -s SOURCE
-                        The source of the proxies(default:C:\Users\Morteza\AppData\Local\Programs\
+                        The source of the proxies(default:%localappdata%\
                         Python\Python310\lib\site-packages\ProxyEater\sources.json).
   --output OUTPUT, -o OUTPUT
                         The output file.
   --file-format { text, json, csv }, -ff { text, json, csv }
                         The format of the output file(default:text).
   --format FORMAT, -f FORMAT
                         The format for saving the proxies in text
@@ -132,9 +130,7 @@
 In order to support this project you can donate some crypto of your choice 8D
 
 [Donate Addresses](https://github.com/MPCodeWriter21/ProxyEater/blob/master/DONATE.md)
 
 Or if you can't, give [this project](https://github.com/MPCodeWriter21/ProxyEater) a star on GitHub :)
 
 
-
-
```

### Comparing `ProxyEater-1.5.1/README.md` & `ProxyEater-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ProxyEater\[1.5.1\]
+ProxyEater\[1.5.2\]
 ===================
 
 ![version](https://img.shields.io/pypi/v/ProxyEater)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/ProxyEater)
 [![CodeFactor](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater/badge)](https://www.codefactor.io/repository/github/mpcodewriter21/proxyeater)
 
 A Python Proxy Scraper for gathering fresh proxies.
@@ -45,15 +45,15 @@
 positional arguments:
   mode              Modes: Scrape, Check
 
 options:
   -h, --help
                         show this help message and exit
   --source SOURCE, -s SOURCE
-                        The source of the proxies(default:C:\Users\Morteza\AppData\Local\Programs\
+                        The source of the proxies(default:%localappdata%\
                         Python\Python310\lib\site-packages\ProxyEater\sources.json).
   --output OUTPUT, -o OUTPUT
                         The output file.
   --file-format { text, json, csv }, -ff { text, json, csv }
                         The format of the output file(default:text).
   --format FORMAT, -f FORMAT
                         The format for saving the proxies in text
```

### Comparing `ProxyEater-1.5.1/setup.py` & `ProxyEater-1.5.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-with open('README.md', 'r') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ProxyEater',
-    version='1.5.1',
+    version='1.5.2',
     author='CodeWriter21',
     author_email='CodeWriter21@gmail.com',
     description='A Python Proxy Scraper for gathering fresh proxies.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MPCodeWriter21/ProxyEater',
     packages=find_packages(),
```

