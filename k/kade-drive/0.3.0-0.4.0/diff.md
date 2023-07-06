# Comparing `tmp/kade_drive-0.3.0.tar.gz` & `tmp/kade_drive-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kade_drive-0.3.0.tar", max compression
+gzip compressed data, was "kade_drive-0.4.0.tar", max compression
```

## Comparing `kade_drive-0.3.0.tar` & `kade_drive-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.3.0/LICENSE
--rw-r--r--   0        0        0      391 2023-07-05 05:42:42.391327 kade_drive-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-04 16:17:23.029053 kade_drive-0.3.0/kade_drive/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-05 18:42:18.719455 kade_drive-0.3.0/kade_drive/cli.py
--rw-r--r--   0        0        0     6860 2023-07-05 19:47:23.095393 kade_drive-0.3.0/kade_drive/client.py
--rw-r--r--   0        0        0        1 2023-07-04 16:17:23.029053 kade_drive-0.3.0/kade_drive/core/__init__.py
--rw-r--r--   0        0        0     9628 2023-07-05 19:50:49.320361 kade_drive-0.3.0/kade_drive/core/crawling.py
--rw-r--r--   0        0        0    19005 2023-07-05 20:17:40.992780 kade_drive-0.3.0/kade_drive/core/network.py
--rw-r--r--   0        0        0     3994 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/core/node.py
--rw-r--r--   0        0        0     8137 2023-07-05 20:14:26.342405 kade_drive-0.3.0/kade_drive/core/protocol.py
--rw-r--r--   0        0        0     8834 2023-07-05 18:42:18.720455 kade_drive-0.3.0/kade_drive/core/routing.py
--rw-r--r--   0        0        0     9643 2023-07-05 20:13:35.887049 kade_drive-0.3.0/kade_drive/core/storage.py
--rw-r--r--   0        0        0     1340 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/core/utils.py
--rw-r--r--   0        0        0      209 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/main_recv.py
--rw-r--r--   0        0        0      248 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/main_send.py
--rw-r--r--   0        0        0        0 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/message_system/__init__.py
--rw-r--r--   0        0        0     7085 2023-07-05 20:59:37.300407 kade_drive-0.3.0/kade_drive/message_system/message_system.py
--rw-r--r--   0        0        0     2366 2023-07-05 18:42:18.720455 kade_drive-0.3.0/kade_drive/server.py
--rw-r--r--   0        0        0      733 2023-07-05 18:29:56.160697 kade_drive-0.3.0/kade_drive/test_store_file.py
--rw-r--r--   0        0        0       25 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/__init__.py
--rw-r--r--   0        0        0     1698 2023-07-05 18:29:45.621586 kade_drive-0.3.0/kade_drive/tests/conftest.py
--rw-r--r--   0        0        0     3100 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/data_to_split.txt
--rw-r--r--   0        0        0     1785 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_node.py
--rw-r--r--   0        0        0     4520 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_routing.py
--rw-r--r--   0        0        0        1 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_server.py
--rw-r--r--   0        0        0      841 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_splitdata.py
--rw-r--r--   0        0        0     1458 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_storage.py
--rw-r--r--   0        0        0      717 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_utils.py
--rw-r--r--   0        0        0      508 2023-07-05 21:04:14.088945 kade_drive-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 kade_drive-0.3.0/setup.py
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 kade_drive-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.4.0/LICENSE
+-rw-r--r--   0        0        0      391 2023-07-05 21:17:07.160141 kade_drive-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/cli.py
+-rw-r--r--   0        0        0     6968 2023-07-05 21:19:40.817571 kade_drive-0.4.0/kade_drive/client.py
+-rw-r--r--   0        0        0        1 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/core/__init__.py
+-rw-r--r--   0        0        0     9628 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/core/crawling.py
+-rw-r--r--   0        0        0    19005 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/core/network.py
+-rw-r--r--   0        0        0     3994 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/core/node.py
+-rw-r--r--   0        0        0     8137 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/core/protocol.py
+-rw-r--r--   0        0        0     8834 2023-07-05 21:17:07.161141 kade_drive-0.4.0/kade_drive/core/routing.py
+-rw-r--r--   0        0        0     9643 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/core/storage.py
+-rw-r--r--   0        0        0     1340 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/core/utils.py
+-rw-r--r--   0        0        0      209 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/main_recv.py
+-rw-r--r--   0        0        0      248 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/main_send.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/message_system/__init__.py
+-rw-r--r--   0        0        0     7085 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/message_system/message_system.py
+-rw-r--r--   0        0        0     2839 2023-07-05 21:19:40.817571 kade_drive-0.4.0/kade_drive/server.py
+-rw-r--r--   0        0        0      733 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/test_store_file.py
+-rw-r--r--   0        0        0       25 2023-07-05 21:17:07.162141 kade_drive-0.4.0/kade_drive/tests/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/conftest.py
+-rw-r--r--   0        0        0     3100 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/data_to_split.txt
+-rw-r--r--   0        0        0     1785 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/test_node.py
+-rw-r--r--   0        0        0     4520 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/test_routing.py
+-rw-r--r--   0        0        0        1 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/test_server.py
+-rw-r--r--   0        0        0      841 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/test_splitdata.py
+-rw-r--r--   0        0        0     1458 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/test_storage.py
+-rw-r--r--   0        0        0      717 2023-07-05 21:17:07.163141 kade_drive-0.4.0/kade_drive/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2023-07-05 21:20:35.451080 kade_drive-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 kade_drive-0.4.0/setup.py
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 kade_drive-0.4.0/PKG-INFO
```

### Comparing `kade_drive-0.3.0/LICENSE` & `kade_drive-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/cli.py` & `kade_drive-0.4.0/kade_drive/cli.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/client.py` & `kade_drive-0.4.0/kade_drive/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 import rpyc
 from time import sleep
 from rpyc.core.protocol import PingError
 from message_system.message_system import Message_System
 
 import logging
 
-logging.basicConfig(level=logging.DEBUG,
-                    format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
-logger = logging.getLogger(__name__)
-logger.info("TESTTTTTT")
+# logger.info("TESTTTTTT")
 # rpyc.core.protocol.DEFAULT_CONFIG['allow_pickle'] = True
-
+try:
+    logger = logging.getLogger(__name__)
+except:
+    pass
 
 class ClientSession:
     """
     Class to handle connection to the distributed file system
     It is necessary to run ensure_connection or broadcast method before
     accessing to the other functionality
     """
 
-    def __init__(self, bootstrap_nodes: list[tuple[str, int]]) -> None:
+    def __init__(self, bootstrap_nodes: list[tuple[str, int]], log_level=logging.INFO) -> None:
+        logging.basicConfig(level=log_level,
+                            format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
+        logger = logging.getLogger(__name__)
         self.connection: rpyc.Connection | None = None
         self.bootstrap_nodes: list[tuple[str, int]] = bootstrap_nodes
 
     def connect(self, time_to_reconnect=5, use_broadcast_if_needed: bool = False, update_boostrap_nodes: bool = True,  attempts_to_reconnect=2):
         self.connection, self.bootstrap_nodes = self._ensure_connection(
             self.bootstrap_nodes, self.connection, time_to_reconnect, use_broadcast_if_needed, update_boostrap_nodes, attempts_to_reconnect)
         return self.connection is not None
```

### Comparing `kade_drive-0.3.0/kade_drive/core/crawling.py` & `kade_drive-0.4.0/kade_drive/core/crawling.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/core/network.py` & `kade_drive-0.4.0/kade_drive/core/network.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/core/node.py` & `kade_drive-0.4.0/kade_drive/core/node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/core/protocol.py` & `kade_drive-0.4.0/kade_drive/core/protocol.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/core/routing.py` & `kade_drive-0.4.0/kade_drive/core/routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/core/storage.py` & `kade_drive-0.4.0/kade_drive/core/storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/core/utils.py` & `kade_drive-0.4.0/kade_drive/core/utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/message_system/message_system.py` & `kade_drive-0.4.0/kade_drive/message_system/message_system.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/server.py` & `kade_drive-0.4.0/kade_drive/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typer import Typer, Argument, Option
-from typing import Optional
+from typing import Match, Optional
 import socket
 from core.storage import PersistentStorage
 from core.network import Server
 import threading
 import time
 import sys
 from message_system.message_system import Message_System
@@ -14,20 +14,19 @@
 file_handler = logging.FileHandler('log_file.log')
 
 # Set the logging format
 formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
 file_handler.setFormatter(formatter)
 
 # Add the file handler to the logger
-logging.basicConfig(level=logging.DEBUG, 
-                    format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
-logging.getLogger("SERVER/8086").setLevel(logging.CRITICAL)
+# logging.basicConfig(level=logging.INFO,
+#                     format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
+# logging.getLogger("SERVER/8086").setLevel(logging.CRITICAL)
 # Create a logger instance
 logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
 
 
 def start_server(host_ip=None):
     # host_ip = socket.gethostbynahost_ipme(socket.gethostname())
     broadcast = None
     logger.debug(host_ip)
     bootstrap_nodes = None
@@ -71,14 +70,29 @@
     logger.info(f'Server started at {host_ip}')
 
 
 app = Typer()
 
 
 @app.command()
-def _start(host_ip=Option(default=None)):
+def _start(host_ip=Option(default=None), log_level=Option(default='INFO')):
+
+    if log_level == 'INFO':
+        log_level = logging.INFO
+    if log_level == 'DEBUG':
+        log_level = logging.DEBUG
+    if log_level == 'WARNING':
+        log_level = logging.WARNING
+
+    logging.basicConfig(level=log_level,
+                        format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
+
+    logging.getLogger("SERVER/8086").setLevel(logging.CRITICAL)
+    # Create a logger instance
+    logger = logging.getLogger(__name__)
+
     logger.debug(host_ip)
     start_server(host_ip)
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `kade_drive-0.3.0/kade_drive/test_store_file.py` & `kade_drive-0.4.0/kade_drive/test_store_file.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/tests/conftest.py` & `kade_drive-0.4.0/kade_drive/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/tests/data_to_split.txt` & `kade_drive-0.4.0/kade_drive/tests/data_to_split.txt`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/tests/test_node.py` & `kade_drive-0.4.0/kade_drive/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/tests/test_routing.py` & `kade_drive-0.4.0/kade_drive/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/tests/test_splitdata.py` & `kade_drive-0.4.0/kade_drive/tests/test_splitdata.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/tests/test_storage.py` & `kade_drive-0.4.0/kade_drive/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/kade_drive/tests/test_utils.py` & `kade_drive-0.4.0/kade_drive/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.3.0/setup.py` & `kade_drive-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces==0.11.0', 'rpyc==5.3.1', 'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'kade-drive',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'distributed file system based on kademlia dht',
     'long_description': 'Distributed file system based on <https://github.com/bmuller/kademlia>\n\n\n## Basic Usage\n\n- Clone the repo and run poetry install\n- Run server.py in one pc or several pc in a local network\n- Run cli.py in any pc of the network and start playing with the system\n\n## Installation\n\n- pip install kade-drive\n  \n### Tests\n\nTo run tests make shure that there is at least one server in the network.\n',
     'author': 'DanielUH2019',
     'author_email': 'danielcardenascabrera2016@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kade_drive-0.3.0/PKG-INFO` & `kade_drive-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kade-drive
-Version: 0.3.0
+Version: 0.4.0
 Summary: distributed file system based on kademlia dht
 License: MIT
 Author: DanielUH2019
 Author-email: danielcardenascabrera2016@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

