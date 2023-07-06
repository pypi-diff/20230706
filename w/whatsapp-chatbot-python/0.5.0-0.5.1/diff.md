# Comparing `tmp/whatsapp-chatbot-python-0.5.0.tar.gz` & `tmp/whatsapp-chatbot-python-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.5.0.tar", last modified: Tue Jul  4 19:54:37 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.5.1.tar", last modified: Thu Jul  6 11:53:38 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.5.0.tar` & `whatsapp-chatbot-python-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.481515 whatsapp-chatbot-python-0.5.0/
--rw-rw-rw-   0        0        0    18829 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.0/LICENSE
--rw-rw-rw-   0        0        0    15378 2023-07-04 19:54:37.480823 whatsapp-chatbot-python-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    14404 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 19:54:37.481515 whatsapp-chatbot-python-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1355 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.468943 whatsapp-chatbot-python-0.5.0/tests/
--rw-rw-rw-   0        0        0     1416 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.0/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.471803 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      270 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-06-30 12:14:11.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     4091 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.479820 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     4513 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     2022 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-06-28 14:02:48.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/router.py
--rw-rw-rw-   0        0        0     2643 2023-07-04 19:52:35.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/state.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:54:37.475811 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0    15378 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-04 19:54:37.000000 whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.687980 whatsapp-chatbot-python-0.5.1/
+-rw-rw-rw-   0        0        0    18829 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    15842 2023-07-06 11:53:38.687980 whatsapp-chatbot-python-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14404 2023-07-06 09:38:10.000000 whatsapp-chatbot-python-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 11:53:38.687980 whatsapp-chatbot-python-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-07-06 11:51:48.000000 whatsapp-chatbot-python-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.675948 whatsapp-chatbot-python-0.5.1/tests/
+-rw-rw-rw-   0        0        0     1459 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.678957 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      270 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     4091 2023-07-06 09:38:10.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.686977 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     4513 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     2022 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/router.py
+-rw-rw-rw-   0        0        0     2643 2023-07-06 09:38:10.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/state.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.682967 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0    15842 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.5.0/LICENSE` & `whatsapp-chatbot-python-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.0/PKG-INFO` & `whatsapp-chatbot-python-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.0
+Version: 0.5.1
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
```

### Comparing `whatsapp-chatbot-python-0.5.0/README.md` & `whatsapp-chatbot-python-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.0/setup.py` & `whatsapp-chatbot-python-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.5.0",
+    version="0.5.1",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -17,21 +17,31 @@
     url="https://github.com/green-api/whatsapp-chatbot-python",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: Other/Proprietary License",
+        "Natural Language :: English",
+        "Natural Language :: Russian",
         "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Communications",
+        "Topic :: Communications :: Chat",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
-    install_requires=["whatsapp-api-client-python==0.0.38"],
-    python_requires=">=3.8"
+    install_requires=["whatsapp-api-client-python==0.0.39"],
+    python_requires=">=3.7"
 )
```

### Comparing `whatsapp-chatbot-python-0.5.0/tests/test_manager.py` & `whatsapp-chatbot-python-0.5.1/tests/test_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
-from unittest.mock import patch
+from unittest.mock import MagicMock, patch
 
 from whatsapp_chatbot_python import GreenAPIBot, Notification
 
-event_example = {
+event_example: dict = {
     "typeWebhook": "incomingMessageReceived",
     "messageData": {
         "typeMessage": "textMessage",
         "textMessageData": {
             "textMessage": "Hello"
         }
     }
@@ -41,15 +41,15 @@
             pass
 
         bot.router.message.add_handler(handler)
 
         self.assertEqual(len(bot.router.message.handlers), 2)
 
     @patch("whatsapp_chatbot_python.bot.Bot._update_settings")
-    def create_bot(self, mock__update_settings):
+    def create_bot(self, mock__update_settings: MagicMock) -> GreenAPIBot:
         mock__update_settings.return_value = None
 
         return GreenAPIBot("", "")
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from typing import NoReturn, Optional
+
 from whatsapp_api_client_python.API import GreenApi
 
 from .manager.router import Router
 
 
 class Bot:
     def __init__(self, id_instance: str, api_token_instance: str):
         self.api = GreenAPI(id_instance, api_token_instance)
 
         self._update_settings()
 
         self.router = Router(self.api)
 
-    def run_forever(self):
+    def run_forever(self) -> Optional[NoReturn]:
         while True:
             try:
                 response = self.api.receiving.receiveNotification()
                 if response.error:
                     raise GreenAPIError(response.error)
 
                 if not response.data:
@@ -24,15 +26,15 @@
 
                 self.router.route_event(response["body"])
 
                 self.api.receiving.deleteNotification(response["receiptId"])
             except KeyboardInterrupt:
                 break
 
-    def _update_settings(self):
+    def _update_settings(self) -> Optional[NoReturn]:
         settings = self.api.account.getSettings()
         if settings.error:
             raise GreenAPIError(settings.error)
 
         response = settings.data
 
         incoming_webhook = response["incomingWebhook"]
@@ -46,20 +48,20 @@
             self.api.account.setSettings({
                 "incomingWebhook": "yes",
                 "outgoingMessageWebhook": "yes",
                 "outgoingAPIMessageWebhook": "yes"
             })
 
 
-class GreenAPIBot(Bot):
+class GreenAPI(GreenApi):
     pass
 
 
-class GreenAPI(GreenApi):
+class GreenAPIBot(Bot):
     pass
 
 
 class GreenAPIError(Exception):
     pass
 
 
-__all__ = ["Bot", "GreenAPIBot", "GreenAPI", "GreenAPIError"]
+__all__ = ["Bot", "GreenAPI", "GreenAPIBot", "GreenAPIError"]
```

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/filters.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,8 +141,8 @@
         if response:
             self.handler(notification)
 
             return True
         return False
 
 
-__all__ = ["Notification", "HandlerType", "AbstractHandler", "Handler"]
+__all__ = ["AbstractHandler", "Handler", "HandlerType", "Notification"]
```

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List, TYPE_CHECKING
 
-from .handler import HandlerType, AbstractHandler, Handler
+from .handler import AbstractHandler, Handler, HandlerType
 from .state import AbstractStateManager, StateManager
 
 if TYPE_CHECKING:
     from .router import Router
 
 
 class AbstractObserver(ABC):
@@ -64,8 +64,8 @@
         message_type = filters.get("type_message")
         if message_type not in message_types:
             filters["type_message"] = message_types
 
         self.router.message.add_handler(handler, **filters)
 
 
-__all__ = ["AbstractObserver", "Observer", "ButtonObserver"]
+__all__ = ["AbstractObserver", "ButtonObserver", "Observer"]
```

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, TYPE_CHECKING
 
-from .observer import AbstractObserver, Observer, ButtonObserver
+from .observer import AbstractObserver, ButtonObserver, Observer
 
 if TYPE_CHECKING:
     from ..bot import GreenAPI
 
 
 class Router:
     def __init__(self, api: "GreenAPI"):
```

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python/manager/state.py` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/state.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.0
+Version: 0.5.1
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
```

### Comparing `whatsapp-chatbot-python-0.5.0/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

