# Comparing `tmp/pyrainbird-2.0.1.tar.gz` & `tmp/pyrainbird-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrainbird-2.0.1.tar", last modified: Thu Apr  6 01:20:42 2023, max compression
+gzip compressed data, was "pyrainbird-2.1.0.tar", last modified: Thu Jul  6 06:06:08 2023, max compression
```

## Comparing `pyrainbird-2.0.1.tar` & `pyrainbird-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:20:42.051878 pyrainbird-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-06 01:20:42.051878 pyrainbird-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:20:42.051878 pyrainbird-2.0.1/pyrainbird/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/rainbird.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:20:42.051878 pyrainbird-2.0.1/pyrainbird/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/resources/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/resources/sipcommands.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/pyrainbird/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:20:42.051878 pyrainbird-2.0.1/pyrainbird.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-06 01:20:42.000000 pyrainbird-2.0.1/pyrainbird.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-06 01:20:42.000000 pyrainbird-2.0.1/pyrainbird.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 01:20:42.000000 pyrainbird-2.0.1/pyrainbird.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-06 01:20:42.000000 pyrainbird-2.0.1/pyrainbird.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 01:20:42.000000 pyrainbird-2.0.1/pyrainbird.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-06 01:20:42.051878 pyrainbird-2.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:20:42.051878 pyrainbird-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    43569 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-06 01:20:29.000000 pyrainbird-2.0.1/tests/test_rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.453235 pyrainbird-2.1.0/pyrainbird/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.453235 pyrainbird-2.1.0/pyrainbird/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/resources/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/resources/sipcommands.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.453235 pyrainbird-2.1.0/pyrainbird.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/tests/test_rainbird.py
```

### Comparing `pyrainbird-2.0.1/LICENSE` & `pyrainbird-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/PKG-INFO` & `pyrainbird-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 2.0.1
+Version: 2.1.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Description-Content-Type: text/markdown
```

### Comparing `pyrainbird-2.0.1/README.md` & `pyrainbird-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/pyrainbird/async_client.py` & `pyrainbird-2.1.0/pyrainbird/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 and querying the device.
 """
 
 import datetime
 import logging
 from collections.abc import Callable
 from http import HTTPStatus
-from typing import Any, Optional, TypeVar
+from typing import Any, TypeVar, Union
 
 import aiohttp
 from aiohttp.client_exceptions import ClientError, ClientResponseError
+from aiohttp_retry import RetryClient, RetryOptions, JitterRetry
+
 
 from . import encryption, rainbird
 from .data import (
     AvailableStations,
     ControllerFirmwareVersion,
     ControllerState,
     ModelAndVersion,
@@ -62,36 +64,56 @@
     "Accept": "*/*",
     "Connection": "keep-alive",
     "Content-Type": "application/octet-stream",
 }
 DATA = "data"
 CLOUD_API_URL = "http://rdz-rbcloud.rainbird.com/phone-api"
 
+# In general, these devices can handle only one in flight request at a time
+# otherwise return a 503. The caller is expected to follow that, however ESP
+# ME devices also seem to return 503s more regularly than other devices so we
+# include retry behavior for them. We only retry the specific device busy error.
+DEVICE_BUSY_RETRY = JitterRetry(
+    attempts=3,
+    statuses=[HTTPStatus.SERVICE_UNAVAILABLE.value],
+    retry_all_server_errors=False,
+)
+
 
 class AsyncRainbirdClient:
     """An asyncio rainbird client.
 
     This is used by the controller and not expected to be used directly.
     """
 
     def __init__(
         self,
         websession: aiohttp.ClientSession,
         host: str,
-        password: Optional[str],
+        password: Union[str, None],
     ) -> None:
         self._websession = websession
+        self._host = host
         if host.startswith("/") or host.startswith("http://"):
             self._url = host
         else:
             self._url = f"http://{host}/stick"
+        self._password = password
         self._coder = encryption.PayloadCoder(password, _LOGGER)
 
+    def with_retry_options(self, retry_options: RetryOptions) -> "AsyncRainbirdClient":
+        """Create a new AsyncRainbirdClient with retry options."""
+        return AsyncRainbirdClient(
+            RetryClient(client_session=self._websession, retry_options=retry_options),
+            self._host,
+            self._password,
+        )
+
     async def request(
-        self, method: str, params: dict[str, Any] = None
+        self, method: str, params: Union[dict[str, Any], None] = None
     ) -> dict[str, Any]:
         """Send a request for any command."""
         payload = self._coder.encode_command(method, params or {})
         try:
             resp = await self._websession.request(
                 "post", self._url, data=payload, headers=HEAD
             )
@@ -114,15 +136,15 @@
         return self._coder.decode_command(content)
 
 
 def CreateController(
     websession: aiohttp.ClientSession, host: str, password: str
 ) -> "AsyncRainbirdController":
     """Create an AsyncRainbirdController."""
-    local_client = AsyncRainbirdClient(websession, host, password)
+    local_client = (AsyncRainbirdClient(websession, host, password),)
     cloud_client = AsyncRainbirdClient(websession, CLOUD_API_URL, None)
     return AsyncRainbirdController(local_client, cloud_client)
 
 
 class AsyncRainbirdController:
     """Rainbird controller that uses asyncio."""
 
@@ -131,25 +153,33 @@
         local_client: AsyncRainbirdClient,
         cloud_client: AsyncRainbirdClient = None,
     ) -> None:
         """Initialize AsyncRainbirdController."""
         self._local_client = local_client
         self._cloud_client = cloud_client
         self._cache: dict[str, Any] = {}
+        self._model: ModelAndVersion | None = None
 
     async def get_model_and_version(self) -> ModelAndVersion:
         """Return the model and version."""
-        return await self._cacheable_command(
+        response = await self._cacheable_command(
             lambda response: ModelAndVersion(
                 response["modelID"],
                 response["protocolRevisionMajor"],
                 response["protocolRevisionMinor"],
             ),
             "ModelAndVersionRequest",
         )
+        if self._model is None:
+            self._model = response
+            if self._model.model_info.retries:
+                self._local_client = self._local_client.with_retry_options(
+                    DEVICE_BUSY_RETRY
+                )
+        return response
 
     async def get_available_stations(self) -> AvailableStations:
         """Get the available stations."""
         mask = (
             "%%0%dX"
             % RAINBIRD_COMMANDS["AvailableStationsResponse"]["setStations"][LENGTH]
         )
```

### Comparing `pyrainbird-2.0.1/pyrainbird/const.py` & `pyrainbird-2.1.0/pyrainbird/const.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/pyrainbird/data.py` & `pyrainbird-2.1.0/pyrainbird/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 @dataclass
 class CommandSupport:
     """Command support response from the API."""
 
     support: int
     """Return if the command is supported."""
 
-
     echo: int
     """Return the input command."""
 
     def __str__(self):
         return "command support: %02X, echo: %s" % (self.support, self.echo)
 
 
@@ -64,14 +63,17 @@
 
     max_programs: int
     """The maximum number of programs supported by the device."""
 
     max_run_times: int
     """The maximum number of run times supported by the device."""
 
+    retries: bool = False
+    """If device busy errors should be retried"""
+
 
 @dataclass
 class ModelAndVersion:
     """Model and version response from the API."""
 
     model: int
     """The device model number hex code."""
```

### Comparing `pyrainbird-2.0.1/pyrainbird/encryption.py` & `pyrainbird-2.1.0/pyrainbird/encryption.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/pyrainbird/rainbird.py` & `pyrainbird-2.1.0/pyrainbird/rainbird.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/pyrainbird/resources/__init__.py` & `pyrainbird-2.1.0/pyrainbird/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/pyrainbird/resources/models.yaml` & `pyrainbird-2.1.0/pyrainbird/resources/models.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 - device_id: "0007"
   code: ESP_ME
   name: ESP-Me
   supports_water_budget: true
   max_programs: 4
   max_run_times: 6
+  retries: true
 
 - device_id: "0006"
   code: ST8X_WF
   name: ST8x-WiFi
   supports_water_budget: false
   max_programs: 0
   max_run_times: 6
@@ -36,21 +37,23 @@
 
 - device_id: "0009"
   code: ESP_ME3
   name: ESP-ME3
   supports_water_budget: true
   max_programs: 4
   max_run_times: 6
+  retries: true
 
 - device_id: "0010"
   code: MOCK_ESP_ME2
   name: ESP=Me2
   supports_water_budget: true
   max_programs: 4
   max_run_times: 6
+  retries: true
 
 - device_id: "000a"
   code: ESP_TM2v2
   name: ESP-TM2
   supports_water_budget: true
   max_programs: 3
   max_run_times: 4
@@ -71,14 +74,15 @@
 
 - device_id: "0107"
   code: ESP_MEv2
   name: ESP-Me
   supports_water_budget: true
   max_programs: 4
   max_run_times: 6
+  retries: true
 
 - device_id: "0103"
   code: ESP_RZXe2
   name: ESP-RZXe2
   supports_water_budget: false
   max_programs: 8
   max_run_times: 6
```

### Comparing `pyrainbird-2.0.1/pyrainbird/resources/sipcommands.yaml` & `pyrainbird-2.1.0/pyrainbird/resources/sipcommands.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/pyrainbird/timeline.py` & `pyrainbird-2.1.0/pyrainbird/timeline.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/pyrainbird.egg-info/PKG-INFO` & `pyrainbird-2.1.0/pyrainbird.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 2.0.1
+Version: 2.1.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Description-Content-Type: text/markdown
```

### Comparing `pyrainbird-2.0.1/pyrainbird.egg-info/SOURCES.txt` & `pyrainbird-2.1.0/pyrainbird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/setup.cfg` & `pyrainbird-2.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrainbird
-version = 2.0.1
+version = 2.1.0
 description = Rain Bird Controller
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/pyrainbird
 author = J.J.Barrancos
 author_email = jordy@fusion-ict.nl
 license = MIT
@@ -17,14 +17,15 @@
 install_requires = 
 	pycryptodome>=3.16.0
 	requests>=2.22.0
 	PyYAML>=5.4
 	pydantic>=1.10.4
 	python-dateutil>=2.8.2
 	ical>=4.2.9
+	aiohttp_retry>=2.8.3
 install_package_data = True
 package_dir = 
 	= .
 
 [options.packages.find]
 where = .
 exclude =
```

### Comparing `pyrainbird-2.0.1/tests/test_async_client.py` & `pyrainbird-2.1.0/tests/test_async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,26 +129,90 @@
     assert result.model_name == "ESP-TM2"
     model_info = result.model_info
     assert model_info.code == "ESP_TM2v2"
     assert model_info.name == "ESP-TM2"
     assert model_info.supports_water_budget
     assert model_info.max_programs == 3
     assert model_info.max_run_times == 4
+    assert not model_info.retries
 
 
 async def test_get_available_stations(
     rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
     api_response: Callable[[...], Awaitable[None]],
 ) -> None:
     controller = await rainbird_controller()
     api_response("83", pageNumber=1, setStations=0x7F000000)
     stations = await controller.get_available_stations()
     assert stations.active_set == {1, 2, 3, 4, 5, 6, 7}
 
 
+async def test_device_busy_retries(
+    rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
+    rainbird_client: Callable[[], Awaitable[AsyncRainbirdClient]],
+    api_response: Callable[[...], Awaitable[None]],
+    response: ResponseResult,
+) -> None:
+    """Test a basic request failure handling with retries."""
+    controller = await rainbird_controller()
+    api_response("82", modelID=0x09, protocolRevisionMajor=1, protocolRevisionMinor=3)
+    result = await controller.get_model_and_version()
+    assert result.model_code == "ESP_ME3"
+    assert result.model_info.retries
+
+    # Make two attempts then succeed
+    response(aiohttp.web.Response(status=503))
+    response(aiohttp.web.Response(status=503))
+    api_response("83", pageNumber=1, setStations=0x7F000000)
+
+    stations = await controller.get_available_stations()
+    assert stations.active_set == {1, 2, 3, 4, 5, 6, 7}
+
+
+async def test_non_retryable_errors(
+    rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
+    rainbird_client: Callable[[], Awaitable[AsyncRainbirdClient]],
+    api_response: Callable[[...], Awaitable[None]],
+    response: ResponseResult,
+) -> None:
+    """Test a basic request failure handling with retries."""
+    controller = await rainbird_controller()
+    api_response("82", modelID=0x09, protocolRevisionMajor=1, protocolRevisionMinor=3)
+    result = await controller.get_model_and_version()
+    assert result.model_code == "ESP_ME3"
+    assert result.model_info.retries
+
+    # Other types of errors are not retried
+    response(aiohttp.web.Response(status=403))
+    with pytest.raises(RainbirdAuthException):
+        await controller.get_available_stations()
+
+
+
+async def test_device_busy_retries_not_enabled(
+    rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
+    rainbird_client: Callable[[], Awaitable[AsyncRainbirdClient]],
+    api_response: Callable[[...], Awaitable[None]],
+    response: ResponseResult,
+) -> None:
+    """Test a basic request failure handling for device without retries."""
+    controller = await rainbird_controller()
+    api_response("82", modelID=0x0A, protocolRevisionMajor=1, protocolRevisionMinor=3)
+    result = await controller.get_model_and_version()
+    assert result == ModelAndVersion(0x0A, 1, 3)
+    assert result.model_code == "ESP_TM2v2"
+    assert result.model_name == "ESP-TM2"
+    assert not result.model_info.retries
+
+    response(aiohttp.web.Response(status=503))
+
+    with pytest.raises(RainbirdDeviceBusyException):
+        await controller.get_available_stations()
+
+
 async def test_get_serial_number(
     rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
     api_response: Callable[[...], Awaitable[None]],
 ) -> None:
     controller = await rainbird_controller()
     api_response("85", serialNumber=0x12635436566)
     assert await controller.get_serial_number() == 0x12635436566
```

### Comparing `pyrainbird-2.0.1/tests/test_data.py` & `pyrainbird-2.1.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.0.1/tests/test_rainbird.py` & `pyrainbird-2.1.0/tests/test_rainbird.py`

 * *Files identical despite different names*

