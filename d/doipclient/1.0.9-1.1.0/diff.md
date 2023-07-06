# Comparing `tmp/doipclient-1.0.9.tar.gz` & `tmp/doipclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doipclient-1.0.9.tar", last modified: Tue Jul  4 21:32:24 2023, max compression
+gzip compressed data, was "doipclient-1.1.0.tar", last modified: Thu Jul  6 04:59:10 2023, max compression
```

## Comparing `doipclient-1.0.9.tar` & `doipclient-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.449567 doipclient-1.0.9/
--rw-rw-rw-   0        0        0     1090 2023-06-30 04:57:22.000000 doipclient-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     4555 2023-07-04 21:32:24.449069 doipclient-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3947 2023-06-30 04:57:22.000000 doipclient-1.0.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.444067 doipclient-1.0.9/doipclient/
--rw-rw-rw-   0        0        0       32 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/__init__.py
--rw-rw-rw-   0        0        0    33511 2023-07-04 21:25:05.000000 doipclient-1.0.9/doipclient/client.py
--rw-rw-rw-   0        0        0     1707 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/connectors.py
--rw-rw-rw-   0        0        0      598 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/constants.py
--rw-rw-rw-   0        0        0    33278 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/messages.py
-drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.447069 doipclient-1.0.9/doipclient.egg-info/
--rw-rw-rw-   0        0        0     4555 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2023-06-30 04:57:22.000000 doipclient-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 21:32:24.449567 doipclient-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-07-04 21:30:26.000000 doipclient-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.448570 doipclient-1.0.9/tests/
--rw-rw-rw-   0        0        0        0 2023-06-30 04:57:22.000000 doipclient-1.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0    23458 2023-07-04 21:28:31.000000 doipclient-1.0.9/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:59:10.179101 doipclient-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-30 04:57:22.000000 doipclient-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4555 2023-07-06 04:59:10.178601 doipclient-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3947 2023-06-30 04:57:22.000000 doipclient-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 04:59:10.174102 doipclient-1.1.0/doipclient/
+-rw-rw-rw-   0        0        0       32 2023-06-30 04:57:22.000000 doipclient-1.1.0/doipclient/__init__.py
+-rw-rw-rw-   0        0        0    36520 2023-07-06 04:57:54.000000 doipclient-1.1.0/doipclient/client.py
+-rw-rw-rw-   0        0        0     1707 2023-06-30 04:57:22.000000 doipclient-1.1.0/doipclient/connectors.py
+-rw-rw-rw-   0        0        0      598 2023-06-30 04:57:22.000000 doipclient-1.1.0/doipclient/constants.py
+-rw-rw-rw-   0        0        0    33278 2023-06-30 04:57:22.000000 doipclient-1.1.0/doipclient/messages.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:59:10.177101 doipclient-1.1.0/doipclient.egg-info/
+-rw-rw-rw-   0        0        0     4555 2023-07-06 04:59:10.000000 doipclient-1.1.0/doipclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-06 04:59:10.000000 doipclient-1.1.0/doipclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 04:59:10.000000 doipclient-1.1.0/doipclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-06 04:59:10.000000 doipclient-1.1.0/doipclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2023-06-30 04:57:22.000000 doipclient-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 04:59:10.179101 doipclient-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-06 04:55:37.000000 doipclient-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:59:10.178101 doipclient-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-30 04:57:22.000000 doipclient-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    24737 2023-07-06 04:56:06.000000 doipclient-1.1.0/tests/test_client.py
```

### Comparing `doipclient-1.0.9/LICENSE` & `doipclient-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doipclient-1.0.9/PKG-INFO` & `doipclient-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doipclient
-Version: 1.0.9
+Version: 1.1.0
 Summary: A Diagnostic over IP (DoIP) client implementing ISO-13400-2.
 Home-page: https://github.com/jacobschaer/python-doipclient
 Author: Jacob Schaer
 Keywords: uds,14229,iso-14229,diagnostic,automotive,13400,iso-13400,doip
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `doipclient-1.0.9/README.rst` & `doipclient-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `doipclient-1.0.9/doipclient/client.py` & `doipclient-1.1.0/doipclient/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import socket
 import struct
 import time
 import ssl
 from enum import IntEnum
 from typing import Union
 from .constants import (
+    A_DOIP_CTRL,
     TCP_DATA_UNSECURED,
     UDP_DISCOVERY,
     A_PROCESSING_TIME,
     LINK_LOCAL_MULTICAST_ADDRESS,
 )
 from .messages import *
 
@@ -112,19 +113,20 @@
     This is a basic DoIP client which was designed primarily for use with the python-udsoncan package for UDS communication
     with ECU's over automotive ethernet. Certain parts of the specification would require threaded operation to
     maintain the time-based state described by the ISO document. However, in practice these are rarely important,
     particularly for use with UDS - especially with scripts that tend to go through instructions as fast as possible.
 
     :param ecu_ip_address: This is the IP address of the target ECU. This should be a string representing an IPv4
         address like "192.168.1.1" or an IPv6 address like "2001:db8::". Like the logical_address, if you don't know the
-        value for your ECU, utilize the await_vehicle_announcement() method.
+        value for your ECU, utilize the get_entity() or await_vehicle_announcement() method.
     :type ecu_ip_address: str
     :param ecu_logical_address: The logical address of the target ECU. This should be an integer. According to the
         specification, the correct range is 0x0001 to 0x0DFF ("VM specific"). If you don't know the logical address,
-        use the await_vehicle_announcement() method and power cycle the ECU - it should identify itself on bootup.
+        either use the get_entity() method OR the await_vehicle_announcement() method and power
+        cycle the ECU - it should identify itself on bootup.
     :type ecu_logical_address: int
     :param tcp_port: The destination TCP port for DoIP data communication. By default this is 13400 for unsecure and
         3496 when using TLS.
     :type tcp_port: int, optional
     :param activation_type: The activation type to use on initial connection. Most ECU's require an activation request
         before they'll respond, and typically the default activation type will do. The type can be changed later using
         request_activation() method. Use `None` to disable activation at startup.
@@ -201,41 +203,18 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
 
-    @classmethod
-    def await_vehicle_announcement(
-        cls, udp_port=UDP_DISCOVERY, timeout=None, ipv6=False, source_interface=None
+    @staticmethod
+    def _create_udp_socket(
+        ipv6=False, udp_port=UDP_DISCOVERY, timeout=None, source_interface=None
     ):
-        """Receive Vehicle Announcement Message
-
-        When an ECU first turns on, it's supposed to broadcast a Vehicle Announcement Message over UDP 3 times
-        to assist DoIP clients in determining ECU IP's and Logical Addresses. Will use an IPv4 socket by default,
-        though this can be overridden with the `ipv6` parameter.
-
-        :param udp_port: The UDP port to listen on. Per the spec this should be 13400, but some VM's use a custom
-            one.
-        :type udp_port: int, optional
-        :param timeout: Maximum amount of time to wait for message
-        :type timeout: float, optional
-        :param ipv6: Bool forcing IPV6 socket instead of IPV4 socket
-        :type ipv6: bool, optional
-        :return: IP Address of ECU and VehicleAnnouncementMessage object
-        :rtype: tuple
-        :param source_interface: Interface name (like "eth0") to bind to for use with IPv6. Defaults to None which
-            will use the default interface (which may not be the one connected to the ECU). Does nothing for IPv4,
-            which will bind to all interfaces uses INADDR_ANY.
-        :type source_interface: str, optional
-        :raises TimeoutError: If vehicle announcement not received in time
-        """
-        start_time = time.time()
-
         if ipv6:
             sock = socket.socket(socket.AF_INET6, socket.SOCK_DGRAM)
 
             # IPv6 version always uses link-local scope multicast address (FF02 16 ::1)
             sock.bind((LINK_LOCAL_MULTICAST_ADDRESS, udp_port))
 
             if source_interface is None:
@@ -260,16 +239,71 @@
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
             sock.bind(("", udp_port))
 
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         if timeout is not None:
             sock.settimeout(timeout)
 
+        return sock
+
+    @staticmethod
+    def _pack_doip(protocol_version, payload_type, payload_data):
+        data_bytes = struct.pack(
+            "!BBHL",
+            protocol_version,
+            0xFF ^ protocol_version,
+            payload_type,
+            len(payload_data),
+        )
+        data_bytes += payload_data
+
+        return data_bytes
+
+    @classmethod
+    def await_vehicle_announcement(
+        cls,
+        udp_port=UDP_DISCOVERY,
+        timeout=None,
+        ipv6=False,
+        source_interface=None,
+        sock=None,
+    ):
+        """Receive Vehicle Announcement Message
+
+        When an ECU first turns on, it's supposed to broadcast a Vehicle Announcement Message over UDP 3 times
+        to assist DoIP clients in determining ECU IP's and Logical Addresses. Will use an IPv4 socket by default,
+        though this can be overridden with the `ipv6` parameter.
+
+        :param udp_port: The UDP port to listen on. Per the spec this should be 13400, but some VM's use a custom
+            one.
+        :type udp_port: int, optional
+        :param timeout: Maximum amount of time to wait for message
+        :type timeout: float, optional
+        :param ipv6: Bool forcing IPV6 socket instead of IPV4 socket
+        :type ipv6: bool, optional
+        :param source_interface: Interface name (like "eth0") to bind to for use with IPv6. Defaults to None which
+            will use the default interface (which may not be the one connected to the ECU). Does nothing for IPv4,
+            which will bind to all interfaces uses INADDR_ANY.
+        :type source_interface: str, optional
+        :return: IP Address of ECU and VehicleAnnouncementMessage object
+        :rtype: tuple
+        :raises TimeoutError: If vehicle announcement not received in time
+        """
+        start_time = time.time()
+
         parser = Parser()
 
+        if not sock:
+            sock = cls._create_udp_socket(
+                ipv6=ipv6,
+                udp_port=udp_port,
+                timeout=timeout,
+                source_interface=source_interface,
+            )
+
         while True:
             remaining = None
             if timeout:
                 duration = time.time() - start_time
                 if duration >= timeout:
                     raise TimeoutError(
                         "Timed out waiting for Vehicle Announcement broadcast"
@@ -286,14 +320,62 @@
             # "Only one DoIP message shall be transmitted by any DoIP entity per datagram"
             # So, reset the parser after each UDP read
             parser.reset()
             result = parser.read_message(data)
             if result and type(result) == VehicleIdentificationResponse:
                 return addr, result
 
+    @classmethod
+    def get_entity(
+        cls, ecu_ip_address="255.255.255.255", protocol_version=0x02, eid=None, vin=None
+    ):
+        """Sends a VehicleIdentificationRequest and awaits a VehicleIdentificationResponse from the ECU,
+        either with a specified VIN, EIN, or nothing. Equivalent to the request_vehicle_identification() method
+        but can be called without instantiation.
+
+        :param ecu_ip_address: This is the IP address of the target ECU for unicast. Defaults to broadcast if
+        the address is not known.
+        :type ecu_ip_address: str, optional
+        :param protocol_version: The DoIP protocol version to use for communication. Represents the version of the ISO 13400
+            specification to follow. 0x02 (2012) is probably correct for most ECU's at the time of writing, though technically
+            this implementation is against 0x03 (2019).
+        :type protocol_version: int, optional
+        :param eid: EID of the Vehicle
+        :type eid: bytes, optional
+        :param vin: VIN of the Vehicle
+        :type vin: str, optional
+        :return: The vehicle identification response message
+        :rtype: VehicleIdentificationResponse
+        """
+
+        # UDP_TEST_EQUIPMENT_REQUEST is dynamically assigned using udp_port=0
+        sock = cls._create_udp_socket(udp_port=0, timeout=A_DOIP_CTRL)
+
+        if eid:
+            message = VehicleIdentificationRequestWithEID(eid)
+        elif vin:
+            message = VehicleIdentificationRequestWithVIN(vin)
+        else:
+            message = VehicleIdentificationRequest()
+
+        payload_data = message.pack()
+        payload_type = payload_message_to_type[type(message)]
+
+        data_bytes = cls._pack_doip(protocol_version, payload_type, payload_data)
+        logger.debug(
+            "Sending DoIP Vehicle Identification Request: Type: 0x{:X}, Payload Size: {}, Payload: {}".format(
+                payload_type,
+                len(payload_data),
+                " ".join(f"{byte:02X}" for byte in payload_data),
+            )
+        )
+        sock.sendto(data_bytes, (ecu_ip_address, UDP_DISCOVERY))
+
+        return cls.await_vehicle_announcement(timeout=A_DOIP_CTRL, sock=sock)
+
     def empty_rxqueue(self):
         """Implemented for compatibility with udsoncan library. Nothing useful to be done yet"""
         pass
 
     def empty_txqueue(self):
         """Implemented for compatibility with udsoncan library. Nothing useful to be done yet"""
         pass
@@ -410,22 +492,15 @@
         :param disable_retry: Disables retry regardless of auto_reconnect_tcp flag. This is used by activation
             requests during connect/reconnect.
         :type disable_retry: bool, optional
         """
 
         retry = self._auto_reconnect_tcp and not disable_retry
 
-        data_bytes = struct.pack(
-            "!BBHL",
-            self._protocol_version,
-            0xFF ^ self._protocol_version,
-            payload_type,
-            len(payload_data),
-        )
-        data_bytes += payload_data
+        data_bytes = self._pack_doip(self._protocol_version, payload_type, payload_data)
         logger.debug(
             "Sending DoIP Message: Type: 0x{:X}, Payload Size: {}, Payload: {}".format(
                 payload_type,
                 len(payload_data),
                 " ".join(f"{byte:02X}" for byte in payload_data),
             )
         )
@@ -525,17 +600,16 @@
                 logger.warning(
                     "Received unexpected DoIP message type {}. Ignoring".format(
                         type(result)
                     )
                 )
 
     def request_vehicle_identification(self, eid=None, vin=None):
-        """Requests a VehicleIdentificationResponse from the ECU, either with a specified VIN, EIN,
+        """Sends a VehicleIdentificationRequest and awaits a VehicleIdentificationResponse from the ECU, either with a specified VIN, EIN,
         or nothing.
-
         :param eid: EID of the Vehicle
         :type eid: bytes, optional
         :param vin: VIN of the Vehicle
         :type vin: str, optional
         :return: The vehicle identification response message
         :rtype: VehicleIdentificationResponse
         """
```

### Comparing `doipclient-1.0.9/doipclient/connectors.py` & `doipclient-1.1.0/doipclient/connectors.py`

 * *Files identical despite different names*

### Comparing `doipclient-1.0.9/doipclient/constants.py` & `doipclient-1.1.0/doipclient/constants.py`

 * *Files identical despite different names*

### Comparing `doipclient-1.0.9/doipclient/messages.py` & `doipclient-1.1.0/doipclient/messages.py`

 * *Files identical despite different names*

### Comparing `doipclient-1.0.9/doipclient.egg-info/PKG-INFO` & `doipclient-1.1.0/doipclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doipclient
-Version: 1.0.9
+Version: 1.1.0
 Summary: A Diagnostic over IP (DoIP) client implementing ISO-13400-2.
 Home-page: https://github.com/jacobschaer/python-doipclient
 Author: Jacob Schaer
 Keywords: uds,14229,iso-14229,diagnostic,automotive,13400,iso-13400,doip
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `doipclient-1.0.9/setup.py` & `doipclient-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="doipclient",
-    version="1.0.9",
+    version="1.1.0",
     description="A Diagnostic over IP (DoIP) client implementing ISO-13400-2.",
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author="Jacob Schaer",
     url="https://github.com/jacobschaer/python-doipclient",
     packages=setuptools.find_packages(),
     keywords=[
```

### Comparing `doipclient-1.0.9/tests/test_client.py` & `doipclient-1.1.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,24 +523,56 @@
 def test_request_vehicle_identification_with_ein(mock_socket):
     sut = DoIPClient(test_ip, test_logical_address)
     mock_socket.rx_queue.append(vehicle_identification_response)
     result = sut.request_vehicle_identification(eid=b"1" * 6)
     assert mock_socket.tx_queue[-1] == vehicle_identification_request_with_ein
     assert result.vin == "1" * 17
     assert result.logical_address == 0x1234
+
+
+def test_request_vehicle_identification_with_vin(mock_socket):
+    sut = DoIPClient(test_ip, test_logical_address)
+    mock_socket.rx_queue.append(vehicle_identification_response)
+    result = sut.request_vehicle_identification(vin="1" * 17)
+    assert mock_socket.tx_queue[-1] == vehicle_identification_request_with_vin
+    assert result.vin == "1" * 17
+    assert result.logical_address == 0x1234
     assert result.eid == b"1" * 6
     assert result.gid == b"2" * 6
     assert result.further_action_required == 0x00
     assert result.vin_sync_status == 0x00
 
 
-def test_request_vehicle_identification_with_vin(mock_socket):
-    sut = DoIPClient(test_ip, test_logical_address)
+def test_get_entity(mock_socket):
     mock_socket.rx_queue.append(vehicle_identification_response)
-    result = sut.request_vehicle_identification(vin="1" * 17)
+    _, result = DoIPClient.get_entity()
+    assert mock_socket.tx_queue[-1] == vehicle_identification_request
+    assert result.vin == "1" * 17
+    assert result.logical_address == 0x1234
+    assert result.eid == b"1" * 6
+    assert result.gid == b"2" * 6
+    assert result.further_action_required == 0x00
+    assert result.vin_sync_status == 0x00
+
+
+def test_get_entity_with_ein(mock_socket):
+    mock_socket.rx_queue.append(vehicle_identification_response)
+    _, result = DoIPClient.get_entity(eid=b"1" * 6)
+    assert mock_socket.tx_queue[-1] == vehicle_identification_request_with_ein
+    assert result.vin == "1" * 17
+    assert result.logical_address == 0x1234
+    assert result.eid == b"1" * 6
+    assert result.gid == b"2" * 6
+    assert result.further_action_required == 0x00
+    assert result.vin_sync_status == 0x00
+
+
+def test_get_entity_with_vin(mock_socket):
+    mock_socket.rx_queue.append(vehicle_identification_response)
+    _, result = DoIPClient.get_entity(vin="1" * 17)
     assert mock_socket.tx_queue[-1] == vehicle_identification_request_with_vin
     assert result.vin == "1" * 17
     assert result.logical_address == 0x1234
     assert result.eid == b"1" * 6
     assert result.gid == b"2" * 6
     assert result.further_action_required == 0x00
     assert result.vin_sync_status == 0x00
```

